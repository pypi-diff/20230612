# Comparing `tmp/datarobot-3.1.1.tar.gz` & `tmp/datarobot-3.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarobot-3.1.1.tar", last modified: Mon May 15 19:50:05 2023, max compression
+gzip compressed data, was "datarobot-3.2.0b0.tar", last modified: Mon Jun 12 17:35:34 2023, max compression
```

## Comparing `datarobot-3.1.1.tar` & `datarobot-3.2.0b0.tar`

### file list

```diff
@@ -1,197 +1,153 @@
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.067422 datarobot-3.1.1/
--rw-r--r--   0 andrew.levan   (504) staff       (20)   161611 2023-05-15 19:45:56.000000 datarobot-3.1.1/CHANGES.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7555 2023-03-10 16:03:09.000000 datarobot-3.1.1/LICENSE.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)      421 2023-03-10 16:03:09.000000 datarobot-3.1.1/MANIFEST.in
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3283 2023-05-15 19:50:05.067684 datarobot-3.1.1/PKG-INFO
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8441 2023-05-15 19:45:52.000000 datarobot-3.1.1/README.md
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5603 2023-05-15 19:45:52.000000 datarobot-3.1.1/common_setup.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.987268 datarobot-3.1.1/datarobot/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2140 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      687 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/_compat.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      306 2023-05-15 19:45:56.000000 datarobot-3.1.1/datarobot/_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16695 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/client.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    22697 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/enums.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7993 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/errors.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.994033 datarobot-3.1.1/datarobot/helpers/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    22432 2023-05-09 15:22:07.000000 datarobot-3.1.1/datarobot/helpers/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13002 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/helpers/binary_data_utils.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1127 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/helpers/deployment_monitoring.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1156 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/helpers/eligibility_result.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14350 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/helpers/feature_discovery.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8696 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/helpers/image_utils.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    94333 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/helpers/partitioning_methods.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.995403 datarobot-3.1.1/datarobot/mixins/
--rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/mixins/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1134 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/mixins/browser_mixin.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1112 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/mixins/update_attributes_mixin.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.037797 datarobot-3.1.1/datarobot/models/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3943 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    12809 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/accuracy.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9166 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/advanced_tuning.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23993 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/anomaly_assessment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2794 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/api_object.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14645 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/automated_documentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    81984 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/batch_prediction_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10455 2023-05-11 14:05:22.000000 datarobot-3.1.1/datarobot/models/blueprint.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23822 2023-05-11 14:05:22.000000 datarobot-3.1.1/datarobot/models/calendar_file.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13301 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/change_request.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3978 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/cluster.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7233 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/cluster_insight.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11139 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/compliance_doc_template.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4180 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/confusion_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6953 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/connector.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11955 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/credential.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    24027 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11963 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_model_test.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    40995 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/custom_model_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15409 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_task.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21195 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/custom_task_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2315 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/custom_task_version_dependency_build.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8969 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/data_drift.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17613 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/data_engine_query_generator.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16402 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/data_source.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    13812 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/data_store.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    55708 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    30524 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/datetime_trend_plots.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    83580 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/deployment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6583 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/driver.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9411 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/execution_environment.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11344 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/execution_environment_version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5374 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_baseline_validation.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.041171 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      355 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6403 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4915 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4523 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5208 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4509 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6789 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    53938 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/feature.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.043055 datarobot-3.1.1/datarobot/models/feature_association_matrix/
--rw-r--r--   0 andrew.levan   (504) staff       (20)      237 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2600 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6177 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4753 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16677 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/feature_effect.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10333 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/feature_fit.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17463 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/featurelist.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7336 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/imported_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21264 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2370 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/lift_chart.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5468 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/missing_report.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)   268103 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7215 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/modeljob.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14320 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/pairwise_statistics.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5438 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/pareto_front.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8726 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/payoff_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7403 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/predict_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10203 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/prediction_dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    33200 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/prediction_explanations.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2426 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/prediction_server.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15940 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/predictions.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2655 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/prime_file.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)   209294 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/project.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    55518 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/project_options.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8774 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/rating_table.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4337 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/recommended_model.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    19064 2023-03-13 20:20:37.000000 datarobot-3.1.1/datarobot/models/relationships_configuration.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2831 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/residuals.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4524 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/restore_discarded_features.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8203 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/roc_curve.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2927 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/ruleset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    19381 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/secondary_dataset.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14217 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/segmentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10058 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/service_stats.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4070 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/shap_impact.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7057 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/shap_matrix.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2645 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/shap_matrix_job.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4214 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/sharing.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1431 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/trafarets.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    28260 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/training_predictions.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.044445 datarobot-3.1.1/datarobot/models/user_blueprints/
--rw-r--r--   0 andrew.levan   (504) staff       (20)       49 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/user_blueprints/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    69622 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/user_blueprints/models.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     8758 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/user_blueprints/trafarets.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2668 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/models/validators.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.046784 datarobot-3.1.1/datarobot/models/visualai/
--rw-r--r--   0 andrew.levan   (504) staff       (20)       89 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/visualai/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    18528 2023-05-11 14:04:17.000000 datarobot-3.1.1/datarobot/models/visualai/augmentation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7729 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/visualai/images.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10592 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/models/visualai/insights.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4936 2023-05-11 14:05:28.000000 datarobot-3.1.1/datarobot/models/word_cloud.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/py.typed
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17131 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/rest.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.050697 datarobot-3.1.1/datarobot/utils/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    15333 2023-05-15 19:45:52.000000 datarobot-3.1.1/datarobot/utils/__init__.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2997 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/deprecation.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)      495 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/logger.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1200 2023-04-18 15:18:29.000000 datarobot-3.1.1/datarobot/utils/pagination.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1461 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/retry.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1282 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/source.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4109 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/sourcedata.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4061 2023-03-10 16:03:09.000000 datarobot-3.1.1/datarobot/utils/waiters.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:04.989196 datarobot-3.1.1/datarobot.egg-info/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3283 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/PKG-INFO
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6326 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)        1 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1077 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/requires.txt
--rw-r--r--   0 andrew.levan   (504) staff       (20)       10 2023-05-15 19:50:04.000000 datarobot-3.1.1/datarobot.egg-info/top_level.txt
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.052773 datarobot-3.1.1/docs/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6404 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/Makefile
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.053098 datarobot-3.1.1/docs/autodoc/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    17499 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/autodoc/api_reference.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10245 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/conf.py
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.053461 datarobot-3.1.1/docs/examples/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1958 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/examples/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      415 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/getting_started.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      961 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)        2 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/predicted.csv
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.053779 datarobot-3.1.1/docs/reference/
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.054859 datarobot-3.1.1/docs/reference/admin/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3474 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/admin/credentials.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      415 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/admin/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3645 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/admin/sharing.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.056262 datarobot-3.1.1/docs/reference/data/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7711 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/database_connectivity.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9959 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/dataset.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    22218 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/feature_discovery.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      612 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/data/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      391 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/index.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.057403 datarobot-3.1.1/docs/reference/mlops/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    29303 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/mlops/custom_model.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    23173 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/mlops/deployment.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      427 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/mlops/index.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.059850 datarobot-3.1.1/docs/reference/modeling/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4396 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/blueprint.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      570 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/index.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.061731 datarobot-3.1.1/docs/reference/modeling/insights/
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5077 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/automated_documentation.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     4033 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/external_testset.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      536 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10234 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/prediction_explanations.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     2277 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/insights/rating_table.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     5305 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/job.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    21949 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/model.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3448 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/model_recommendation.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3385 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/prime.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    16205 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/project.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.065381 datarobot-3.1.1/docs/reference/modeling/spec/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    11364 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/binary_data.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7430 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/custom_task.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10036 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/datetime_partition.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      620 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6625 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/monotonic_constraints.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     6204 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/segmented_modeling.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    36391 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/time_series.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    10392 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/unsupervised_anomaly.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     7376 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/unsupervised_clustering.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)    14760 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/modeling/spec/visualai.rst
-drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-05-15 19:50:05.066848 datarobot-3.1.1/docs/reference/predictions/
--rw-r--r--   0 andrew.levan   (504) staff       (20)    39016 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/predictions/batch_predictions.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1180 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/predictions/index.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)     9015 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/reference/predictions/predict_job.rst
--rw-r--r--   0 andrew.levan   (504) staff       (20)      319 2023-05-15 19:45:52.000000 datarobot-3.1.1/docs/version.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     3386 2023-05-15 19:45:52.000000 datarobot-3.1.1/pyproject.toml
--rw-r--r--   0 andrew.levan   (504) staff       (20)      123 2023-05-15 19:50:05.068334 datarobot-3.1.1/setup.cfg
--rw-r--r--   0 andrew.levan   (504) staff       (20)      965 2023-03-10 16:03:09.000000 datarobot-3.1.1/setup.py
--rw-r--r--   0 andrew.levan   (504) staff       (20)     1208 2023-05-15 19:45:52.000000 datarobot-3.1.1/setup_major.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.803885 datarobot-3.2.0b0/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   173551 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/CHANGES.rst
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7555 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/LICENSE.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      421 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/MANIFEST.in
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3389 2023-06-12 17:35:34.804173 datarobot-3.2.0b0/PKG-INFO
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8911 2023-05-24 20:04:06.000000 datarobot-3.2.0b0/README.md
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5678 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/common_setup.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.683410 datarobot-3.2.0b0/datarobot/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2257 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      687 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/_compat.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      313 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    18879 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/client.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3126 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/context.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    25285 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/enums.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8680 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/errors.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.690327 datarobot-3.2.0b0/datarobot/helpers/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    22432 2023-06-01 15:04:06.000000 datarobot-3.2.0b0/datarobot/helpers/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13002 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/helpers/binary_data_utils.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1156 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/helpers/eligibility_result.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14350 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/helpers/feature_discovery.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8696 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/helpers/image_utils.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   101561 2023-05-22 13:04:57.000000 datarobot-3.2.0b0/datarobot/helpers/partitioning_methods.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.692712 datarobot-3.2.0b0/datarobot/mixins/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-06-01 15:04:06.000000 datarobot-3.2.0b0/datarobot/mixins/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1134 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/mixins/browser_mixin.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1112 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/mixins/update_attributes_mixin.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.760349 datarobot-3.2.0b0/datarobot/models/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4012 2023-06-01 15:10:47.000000 datarobot-3.2.0b0/datarobot/models/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9166 2023-05-24 18:13:09.000000 datarobot-3.2.0b0/datarobot/models/advanced_tuning.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    27075 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/anomaly_assessment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2925 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/api_object.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8859 2023-05-22 13:04:57.000000 datarobot-3.2.0b0/datarobot/models/application.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15447 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/automated_documentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    23047 2023-05-23 15:25:49.000000 datarobot-3.2.0b0/datarobot/models/batch_monitoring_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    83098 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/batch_prediction_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11096 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/blueprint.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    23822 2023-05-11 14:05:22.000000 datarobot-3.2.0b0/datarobot/models/calendar_file.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13301 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/change_request.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3978 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/cluster.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7233 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/cluster_insight.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12910 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/compliance_doc_template.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4887 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/confusion_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6953 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/connector.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11955 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/models/credential.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    32642 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/custom_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11963 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/custom_model_test.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    59153 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/custom_model_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15411 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/models/custom_task.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    21102 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/custom_task_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2315 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/custom_task_version_dependency_build.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17613 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/data_engine_query_generator.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16402 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/data_source.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13812 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/data_store.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    58123 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/models/dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    30524 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/datetime_trend_plots.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.768900 datarobot-3.2.0b0/datarobot/models/deployment/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      387 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/deployment/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12535 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/accuracy.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5688 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/deployment/bias_and_fairness.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    12650 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/data_drift.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    93319 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/deployment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1131 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/mixins.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10065 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/service_stats.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3450 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/deployment/sharing.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6583 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/driver.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     9411 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/execution_environment.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    11344 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/execution_environment_version.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5374 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/external_baseline_validation.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.776507 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      355 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6403 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4915 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4523 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5208 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4521 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6789 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    53938 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/feature.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.780766 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      237 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2600 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6177 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4753 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    16683 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/feature_effect.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17463 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/featurelist.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7336 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/imported_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    21038 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2370 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/lift_chart.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5468 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/missing_report.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   256455 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7215 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/modeljob.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14320 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/pairwise_statistics.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5438 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/pareto_front.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8726 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/payoff_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7403 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/predict_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10218 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/prediction_dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    34744 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/prediction_explanations.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2426 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/prediction_server.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15940 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/predictions.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2655 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/prime_file.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)   215251 2023-05-31 16:21:11.000000 datarobot-3.2.0b0/datarobot/models/project.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    55519 2023-05-22 13:04:57.000000 datarobot-3.2.0b0/datarobot/models/project_options.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8774 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/rating_table.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4337 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/recommended_model.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    19064 2023-03-13 20:20:37.000000 datarobot-3.2.0b0/datarobot/models/relationships_configuration.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2831 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/residuals.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4524 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/restore_discarded_features.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7730 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/roc_curve.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2927 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/ruleset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    19381 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/secondary_dataset.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    14217 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/segmentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4070 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/shap_impact.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     7057 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/shap_matrix.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2645 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/shap_matrix_job.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     6340 2023-05-22 13:05:29.000000 datarobot-3.2.0b0/datarobot/models/sharing.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1431 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/trafarets.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    28260 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/training_predictions.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1822 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/types.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.784473 datarobot-3.2.0b0/datarobot/models/use_cases/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      262 2023-06-01 15:04:06.000000 datarobot-3.2.0b0/datarobot/models/use_cases/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    24565 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/use_cases/use_case.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8680 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/datarobot/models/use_cases/utils.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.789528 datarobot-3.2.0b0/datarobot/models/user_blueprints/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)       49 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/user_blueprints/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    69649 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/user_blueprints/models.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     8758 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/user_blueprints/trafarets.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2668 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/models/validators.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.794571 datarobot-3.2.0b0/datarobot/models/visualai/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      226 2023-06-01 15:04:09.000000 datarobot-3.2.0b0/datarobot/models/visualai/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    18528 2023-05-11 14:04:17.000000 datarobot-3.2.0b0/datarobot/models/visualai/augmentation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    10521 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/visualai/images.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    13615 2023-05-15 20:05:42.000000 datarobot-3.2.0b0/datarobot/models/visualai/insights.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4936 2023-05-11 14:05:28.000000 datarobot-3.2.0b0/datarobot/models/word_cloud.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        0 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/py.typed
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    17330 2023-06-12 17:23:01.000000 datarobot-3.2.0b0/datarobot/rest.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.802841 datarobot-3.2.0b0/datarobot/utils/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)    15590 2023-06-01 15:11:07.000000 datarobot-3.2.0b0/datarobot/utils/__init__.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     2997 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/deprecation.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      495 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/logger.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1200 2023-04-18 15:18:29.000000 datarobot-3.2.0b0/datarobot/utils/pagination.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1461 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/retry.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1282 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/source.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4109 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/sourcedata.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     4061 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/datarobot/utils/waiters.py
+drwxr-xr-x   0 andrew.levan   (504) staff       (20)        0 2023-06-12 17:35:34.685978 datarobot-3.2.0b0/datarobot.egg-info/
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3389 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     5016 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)        1 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1080 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/requires.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)       10 2023-06-12 17:35:34.000000 datarobot-3.2.0b0/datarobot.egg-info/top_level.txt
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     3066 2023-06-07 13:50:47.000000 datarobot-3.2.0b0/pyproject.toml
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      123 2023-06-12 17:35:34.805137 datarobot-3.2.0b0/setup.cfg
+-rw-r--r--   0 andrew.levan   (504) staff       (20)      965 2023-03-10 16:03:09.000000 datarobot-3.2.0b0/setup.py
+-rw-r--r--   0 andrew.levan   (504) staff       (20)     1225 2023-06-12 17:34:54.000000 datarobot-3.2.0b0/setup_major.py
```

### Comparing `datarobot-3.1.1/CHANGES.rst` & `datarobot-3.2.0b0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,163 @@
 #########
 Changelog
 #########
+3.2.0b0
+========
+
+New Features
+************
+- Added :meth:`DatetimePartitioning.datetime_partitioning_log_retrieve <datarobot.DatetimePartitioning.datetime_partitioning_log_retrieve>` to download the datetime partitioning log.
+- Added method :meth:`DatetimePartitioning.datetime_partitioning_log_list <datarobot.DatetimePartitioning.datetime_partitioning_log_list>` to list the datetime partitioning log.
+- Added :meth:`DatetimePartitioning.get_input_data <datarobot.DatetimePartitioning.get_input_data>` to retrieve the input data used to create an optimized datetime partitioning.
+- Added :class:`DatetimePartitioningId <datarobot.helpers.partitioning_methods.DatetimePartitioningId>`, which can be passed as a `partitioning_method` to :meth:`Project.analyze_and_model <datarobot.models.Project.analyze_and_model>`.
+- Added the ability to share deployments. See :ref:`deployment sharing <deployment_sharing>` for more information on sharing deployments.
+
+- Added new methods get_bias_and_fairness_settings and update_bias_and_fairness_settings to retrieve or update bias and fairness settings.
+   :meth:`Deployment.get_bias_and_fairness_settings<datarobot.models.Deployment.get_bias_and_fairness_settings>`
+   :meth:`Deployment.update_bias_and_fairness_settings<datarobot.models.Deployment.update_bias_and_fairness_settings>`
+
+- Added a new class :class:`UseCase <datarobot.UseCase>` for interacting with the DataRobot Use Cases API.
+- Added a new class :class:`Application <datarobot.Application>` for retrieving DataRobot Applications available to the user.
+- Added a new class :class:`SharingRole <datarobot.models.sharing.SharingRole>` to hold user or organization access rights.
+- Added a new class :class:`BatchMonitoringJob <datarobot.models.BatchMonitoringJob>` for interacting with batch monitoring jobs.
+- Added a new class :class:`BatchMonitoringJobDefinition <datarobot.models.BatchMonitoringJobDefinition>` for interacting with batch monitoring jobs definitions.
+- Added a new methods for handling monitoring job definitions: list, get, create, update, delete, run_on_schedule and run_once
+  :meth:`BatchMonitoringJobDefinition.list <datarobot.models.BatchMonitoringJobDefinition.list>`
+  :meth:`BatchMonitoringJobDefinition.get <datarobot.models.BatchMonitoringJobDefinition.get>`
+  :meth:`BatchMonitoringJobDefinition.create <datarobot.models.BatchMonitoringJobDefinition.create>`
+  :meth:`BatchMonitoringJobDefinition.update <datarobot.models.BatchMonitoringJobDefinition.update>`
+  :meth:`BatchMonitoringJobDefinition.delete <datarobot.models.BatchMonitoringJobDefinition.delete>`
+  :meth:`BatchMonitoringJobDefinition.run_on_schedule <datarobot.models.BatchMonitoringJobDefinition.run_on_schedule>`
+  :meth:`BatchMonitoringJobDefinition.run_once <datarobot.models.BatchMonitoringJobDefinition.run_once>`
+- Added a new method to retrieve a monitoring job
+  :meth:`BatchMonitoringJob.get <datarobot.models.BatchMonitoringJob.get>`
+- Added the ability to filter return objects by a Use Case ID passed to the following methods:
+  :meth:`Dataset.list <datarobot.models.Dataset.list>`
+  :meth:`Project.list <datarobot.models.Project.list>`
+- Added the ability to automatically add a newly created dataset or project to a Use Case by passing a UseCase, list of UseCase objects, UseCase ID or list of UseCase IDs using the keyword argument `use_cases` to the following methods:
+  :meth:`Dataset.create_from_file <datarobot.models.Dataset.create_from_file>`
+  :meth:`Dataset.create_from_in_memory_data <datarobot.models.Dataset.create_from_in_memory_data>`
+  :meth:`Dataset.create_from_url <datarobot.models.Dataset.create_from_url>`
+  :meth:`Dataset.create_from_data_source <datarobot.models.Dataset.create_from_data_source>`
+  :meth:`Dataset.create_from_query_generator <datarobot.models.Dataset.create_from_query_generator>`
+  :meth:`Dataset.create_project <datarobot.models.Dataset.create_project>`
+  :meth:`Project.create <datarobot.models.Project.create>`
+  :meth:`Project.create_from_data_source <datarobot.models.Project.create_from_data_source>`
+  :meth:`Project.create_from_dataset <datarobot.models.Project.create_from_dataset>`
+  :meth:`Project.create_segmented_project_from_clustering_model <datarobot.models.Project.create_segmented_project_from_clustering_model>`
+  :meth:`Project.start <datarobot.models.Project.start>`
+- Added the ability to set a default :class:`UseCase <datarobot.UseCase>` for requests. It can be set in several ways.
+
+  - If the user configures the client via `Client(...)`, then invoke `Client(..., default_use_case = <id>)`.
+  - If the user configures the client via dr.config.yaml, then add the property `default_use_case: <id>`.
+  - If the user configures the client via env vars, then set the env var ``DATAROBOT_DEFAULT_USE_CASE``.
+  - The default use case can also be set programmatically as a context manager via `with UseCase.get(<id>):`.
+
+- Added method meth:`Deployment.get_predictions_over_time <datarobot.models.Deployment.get_predictions_over_time>` to retrieve deployment predictions over time data.
+- Added a new class :class:`FairnessScoresOverTime <datarobot.models.deployment.bias_and_fairness.FairnessScoresOverTime>` to retrieve fairness over time information.
+- Added a new method :meth:`Deployment.get_fairness_scores_over_time <datarobot.models.Deployment.get_fairness_scores_over_time>` to retrieve fairness scores over time of a deployment.
+- Added a new `use_gpu` parameter to the method :meth:`Project.analyze_and_model<datarobot.models.Project.analyze_and_model>` to set whether the project should allow usage of GPU
+- Added a new `use_gpu` parameter to the class :class:`Project <datarobot.models.Project>` with information whether project allows usage of GPU
+- Added a new class :class:`TrainingData <datarobot.models.custom_model_version.TrainingData>` for retrieving TrainingData assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+- Added a new class :class:`HoldoutData <datarobot.models.custom_model_version.HoldoutData>` for retrieving HoldoutData assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+- Added the ability to retrieve the model and blueprint json using the following methods:
+  :meth:`Model.get_model_blueprint_json <datarobot.models.Model.get_model_blueprint_json>`
+  :meth:`Blueprint.get_json <datarobot.models.Blueprint.get_json>`
+
+
+Enhancements
+************
+- Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
+  to clarify that a selected parameter cannot be used when a project has not proceeded to the
+  correct stage prior to calling this method.
+
+- Extended :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>` by two parameters
+  to filter for a target value range in regression projects.
+
+- Added text explanations data to :meth:`PredictionExplanations <datarobot.PredictionExplanations>` and made sure it is returned in both :py:meth:`datarobot.PredictionExplanations.get_all_as_dataframe`  and :py:meth:`datarobot.PredictionExplanations.get_rows` method.
+
+- Added two new parameters to :meth:`Project.upload_dataset_from_catalog <datarobot.models.Project.upload_dataset_from_catalog>`:
+    - `credential_id`
+    - `credential_data`
+
+- Implemented training and holdout data assignment for Custom Model Version creation APIs:
+    - :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>`
+    - :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_from_previous>`
+
+    The parameters added to both APIs are:
+        - `training_dataset_id`
+        - `partition_column`
+        - `holdout_dataset_id`
+        - `keep_training_holdout_data`
+        - `max_wait`
+
+- Extended :meth:`CustomInferenceModel.update <datarobot.CustomInferenceModel.create>` and :meth:`CustomInferenceModel.update <datarobot.CustomInferenceModel.update>`
+  with `is_training_data_for_versions_permanently_enabled` parameter.
+
+
+Bugfixes
+********
+- Fixed incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
+- Fixed a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
+- Fixed an issue where failed authentication when invoking `datarobot.client.Client()` raises a misleading error about client-server compatibility.
+
+API Changes
+***********
+- Added parameter ``unsupervised_type`` to the class :class:`DatetimePartitioning <datarobot.DatetimePartitioning>`.
+
+Deprecation Summary
+*******************
+- ``Model.get_feature_fit_metadata`` has been removed.
+  Use :meth:`Model.get_feature_effect_metadata <datarobot.models.Model.get_feature_effect_metadata>` instead.
+- ``DatetimeModel.get_feature_fit_metadata`` has been removed.
+  Use :meth:`DatetimeModel.get_feature_effect_metadata <datarobot.models.DatetimeModel.get_feature_effect_metadata>` instead.
+- ``Model.request_feature_fit`` has been removed.
+  Use :meth:`Model.request_feature_effect <datarobot.models.Model.request_feature_effect>` instead.
+- ``DatetimeModel.request_feature_fit`` has been removed.
+  Use :meth:`DatetimeModel.request_feature_effect <datarobot.models.DatetimeModel.request_feature_effect>` instead.
+- ``Model.get_feature_fit`` has been removed.
+  Use :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>` instead.
+- ``DatetimeModel.get_feature_fit`` has been removed.
+  Use :meth:`DatetimeModel.get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` instead.
+- ``Model.get_or_request_feature_fit`` has been removed.
+  Use :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>` instead.
+- ``DatetimeModel.get_or_request_feature_fit`` has been removed.
+  Use :meth:`DatetimeModel.get_or_request_feature_effect <datarobot.models.DatetimeModel.get_or_request_feature_effect>` instead.
+
+Configuration Changes
+*********************
+- Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
+
+Documentation Changes
+*********************
+- Fixed in-line documentation of `DataRobotClientConfig`.
+- Fixed documentation around client configuration from environment variables or config file.
+
+Experimental changes
+*********************
+- Added experimental support for data matching:
+
+  - :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`
+  - :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>`
+
+- Added new method :meth:`DataMatchingQuery.get_result <datarobot._experimental.models.data_matching.DataMatchingQuery.get_result>` for returning data matching query results as pandas dataframes to :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>` .
+- Changed behavior for returning results in the :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. Instead of saving the results as a file, a pandas dataframe will be returned in the following methods:
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data>`
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_model>`
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_featurelist>`
+
+- Added experimental support for model lineage: :class:`ModelLineage <datarobot._experimental.models.model_lineage.ModelLineage>`
+
+- Changed behavior for methods that search for the closest data points in :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. If the index is missing, instead of throwing the error, methods try to create the index and then query it. This is enabled by default, but if this is not the intended behavior it can be changed by passing `False` to the new `build_index` parameter added to the methods:
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data>`
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_model>`
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_featurelist>`
+- Added a new class :class:`Notebook <datarobot._experimental.models.notebooks.Notebook>` for retrieving DataRobot Notebooks available to the user.
+
 
 3.1.1
 =====
 
 Configuration Changes
 *********************
 - Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
@@ -65,19 +218,14 @@
 - ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead.
 
 Configuration Changes
 *********************
 
 Experimental changes
 *********************
-- Added :meth:`DatetimePartitioning.datetime_partitioning_log_retrieve <datarobot._experimental.helpers.partitioning_methods.DatetimePartitioning.datetime_partitioning_log_retrieve>` to download the datetime partitioning log.
-
-- Added :meth:`DatetimePartitioning.get_input_data <datarobot._experimental.helpers.partitioning_methods.DatetimePartitioning.get_input_data>` to retrieve the input data used to create an optimized datetime partitioning.
-
-- Added :class:`DatetimePartitioningId <datarobot._experimental.helpers.partitioning_methods.DatetimePartitioningId>`, which can be passed as a `partitioning_method` to :meth:`Project.analyze_and_model <datarobot.models.Project.analyze_and_model>`.
 
 Documentation Changes
 *********************
 - Update the documentation to suggest that setting `use_backtest_start_end_format` of :py:meth:`DatetimePartitioning.to_specification <datarobot.DatetimePartitioning.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 - Update the documentation to suggest setting `use_start_end_format` of :py:meth:`Backtest.to_specification <datarobot.helpers.partitioning_methods.Backtest.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
@@ -469,17 +617,17 @@
 - Fix a bug in :meth:`datarobot.models.BatchPredictionJobDefinition.create` where `schedule` was not optional for all cases
 
 API Changes
 ***********
 
 - User can include ICE plots data in the response when requesting Feature Effects/Feature Fit. Extended methods are
     - :meth:`Model.get_feature_effect <datarobot.models.Model.get_feature_effect>`,
-    - :meth:`Model.get_feature_fit <datarobot.models.Model.get_feature_fit>`,
+    - ``Model.get_feature_fit <datarobot.models.Model.get_feature_fit>``,
     - :meth:`DatetimeModel.get_feature_effect <datarobot.models.DatetimeModel.get_feature_effect>` and
-    - :meth:`DatetimeModel.get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>`.
+    - ``DatetimeModel.get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>``.
 
 Deprecation Summary
 *******************
 
 - `attrs` library is removed from library dependencies
 - ``ImageAugmentationSample.compute`` was marked as deprecated and will be removed in v2.30. You
   can get the same information with newly introduced method ``ImageAugmentationList.compute_samples``
@@ -1143,15 +1291,15 @@
 - A description can now be added or updated for a project.
   :meth:`Project.set_project_description <datarobot.models.Project.set_project_description>`.
 
 - Added new parameters `read_timeout` and `max_wait` to method :meth:`Dataset.create_from_file<datarobot.models.Dataset.create_from_file>`.
   Values larger than the default can be specified for both to avoid timeouts when uploading large files.
 
 
-- Added new parameter `metric` to :class:`datarobot.models.TargetDrift`, :class:`datarobot.models.FeatureDrift`,
+- Added new parameter `metric` to :class:`datarobot.models.deployment.TargetDrift`, :class:`datarobot.models.deployment.FeatureDrift`,
   :meth:`Deployment.get_target_drift<datarobot.models.Deployment.get_target_drift>`
   and :meth:`Deployment.get_feature_drift<datarobot.models.Deployment.get_feature_drift>`.
 
 - Added new parameter `timeout` to :meth:`BatchPredictionJob.download <datarobot.models.BatchPredictionJob.download>` to indicate
   how many seconds to wait for the download to start (in case the job doesn't start processing immediately).
   Set to ``-1`` to disable.
   This parameter can also be sent as `download_timeout` to :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`
@@ -1293,16 +1441,16 @@
     :class:`ExternalScores<datarobot.ExternalScores>`, :class:`ExternalLiftChart<datarobot.ExternalLiftChart>`, :class:`ExternalRocCurve<datarobot.ExternalRocCurve>`.
 
 - Users can create payoff matrices for generating profit curves for binary classification projects
   using :meth:`PayoffMatrix.create <datarobot.models.PayoffMatrix.create>`.
 
 - Deployment Improvements:
 
-  - :class:`datarobot.models.TargetDrift` can be used to retrieve target drift information.
-  - :class:`datarobot.models.FeatureDrift` can be used to retrieve feature drift information.
+  - :class:`datarobot.models.deployment.TargetDrift` can be used to retrieve target drift information.
+  - :class:`datarobot.models.deployment.FeatureDrift` can be used to retrieve feature drift information.
   - :meth:`Deployment.submit_actuals<datarobot.models.Deployment.submit_actuals>` will submit actuals in batches if the total number of actuals exceeds the limit of one single request.
   - ``Deployment.create_from_custom_model_image`` can be used to create a deployment from a custom model image.
   - Deployments now support predictions data collection that enables prediction requests and results to be saved in Predictions Data Storage. See
     :meth:`Deployment.get_predictions_data_collection_settings<datarobot.models.Deployment.get_predictions_data_collection_settings>`
     and :meth:`Deployment.update_predictions_data_collection_settings<datarobot.models.Deployment.update_predictions_data_collection_settings>` for usage.
```

### Comparing `datarobot-3.1.1/LICENSE.txt` & `datarobot-3.2.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/PKG-INFO` & `datarobot-3.2.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.1.1
+Version: 3.2.0b0
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
@@ -12,14 +12,16 @@
 Project-URL: Changelog, https://datarobot-public-api-client.readthedocs-hosted.com/page/CHANGES.html
 Project-URL: Bug Reporting, https://community.datarobot.com/t5/forums/postpage/board-id/datarobot-api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: examples
```

### Comparing `datarobot-3.1.1/README.md` & `datarobot-3.2.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,83 +4,100 @@
 [DataRobot](!http://datarobot.com) platform API.
 
 This README is primarily intended for those developing the client. There is
 also documentation intended for users of the client contained in the `docs`
 directory of this repository. You can view the public documentation at
 [https://datarobot-public-api-client.readthedocs-hosted.com](https://datarobot-public-api-client.readthedocs-hosted.com).
 
+## Topics
+
+* Development:
+  * [Getting Started](#getting-started)
+  * [Guidelines](#guidelines)
+  * [Setup datarobot sdk locally](#installation)
+  * [Running tests](#running-tests)
+  * [Linting](#linting)
+* Setup topics:
+  * [Common DataRobot Client setup](#datarobot-client-setup)
+    * [Setup with cfg file](#setup-with-cfg-file)
+    * [Setup explicitly in code](#setup-explicitly-in-code)
+    * [Setup with environment variables](#setup-with-environment-variables)
+* Building the documentation
+
 ## Getting Started
 
 You need to have
 
     - Git
     - Docker
     - Python >= 3.7
     - DataRobot account
     - pip
 
 We recommend using a virtualenv to keep dependencies from conflicting with
 projects you may have on your machine.
 
+## Guidelines
+
+Our full list of suggestions and guidelines for code being added to this repository can be found [here](GUIDELINES.md).
+
 ## Installation
 
 ```console
 git clone git@github.com:datarobot/public_api_client.git
 cd public_api_client
 # mkvirtualenv ...
 make req  # upgrades pip, setuptools, installs dev requirements
 ```
 
 Note: This may have to be run as `root` or with `--user` flag if you are not
 using python virtual environment.
 
 ## Build the documentation
 
+Docker env:
+
+```console
+make clean test-docs
+```
+
+Local virtual env:
+
+| WARNING: currently the documentation commands below needs py3.11 env in order to work (there seem to be an issue with type hinting) |
+| --- |
+
 > Be sure to install pandoc before building documentation. Available via `apt-get` and `brew`
 
 DataRobot has extensive documentation, which you can build locally for your
 own reference. Before running the following build commands, please make sure that your
 [public_api_client configuration](https://datarobot-public-api-client.readthedocs-hosted.com/en/v2.22.1/setup/getting_started.html#use-a-configuration-file)
 is present and valid or you have set the
 [correct environment variables](https://datarobot-public-api-client.readthedocs-hosted.com/en/v2.22.1/setup/getting_started.html#set-credentials-using-environment-variables).
 Otherwise building the docs will take a lot of time.
 
 ```console
-cd docs
+cd sdk_docs
 make clean html
 ```
 
 The documentation will then be built in a subdirectory, and can be viewed with
 your web browser.
 
 Alternatively, see <https://datarobot.atlassian.net/wiki/spaces/AIAPI/pages/28967932/Release+Tracker>
 for pre-built documentation for the current cloud release and all enterprise
 releases, as well as guidance on which version of the API goes with which
 enterprise release.
 
 To build a PDF of the docs for release:
 
 ```console
-cd docs
+cd sdk_docs
 make clean xelatexpdf
 ```
 
-## Topics
-
-* Setup topics:
-  * [Common DataRobot Client setup](#datarobot-client-setup)
-    * [Setup with cfg file](#setup-with-cfg-file)
-    * [Setup explicitly in code](#setup-explicitly-in-code)
-    * [Setup with environment variables](#setup-with-environment-variables)
-* Building the documentation
-* Development:
-  * [Setup datarobot sdk locally](#installation)
-  * [Running tests](#running-tests)
-  * [Linting](#linting)
-
 ### DataRobot Client Setup
 
 There are three different ways to set up the client to authenticate with the
 server: through a config file, through environment variables, or explicitly in
 the code.
 
 You must specify an endpoint and an API token.  You can manage your API tokens in the DataRobot
@@ -165,19 +182,19 @@
 
 ## Linting
 
 You can use the following ``make`` commands to run linting (isort, black, mypy, flake8, pylint) against this repo:
 
 * ``make black-quick``: This runs black against only the files you've changed compared to master.
 * ``make black``: This runs [black](https://pypi.org/project/black/) against all files in the repo.
-* ``make isort``: This runs [isort](https://pypi.org/project/isort/) against all files in the repo.
-* ``make flake``: This runs [flake8](https://pypi.org/project/flake8/) against all files in the repo.
-* ``make pylint``: This runs [pylint](https://pypi.org/project/pylint/) against the repo.'s `datarobot` and `tests` directories
-* ``make mypy``: This runs [mypy](https://pypi.org/project/mypy/) against a subset of the python files - see [pyproject.toml](pyproject.toml) for more information.
-* ``make lint``: This runs all the linters against the repo: check-isort, mypy, check-black, flake, pylint
+* ``make check-isort``: This runs [isort](https://pypi.org/project/isort/) checks against all files in the repo.
+* ``make flake``: This runs [flake8](https://pypi.org/project/flake8/) checks against all files in the repo.
+* ``make pylint``: This runs [pylint](https://pypi.org/project/pylint/) checks against the repo.'s `datarobot` and `tests` directories
+* ``make mypy``: This runs [mypy](https://pypi.org/project/mypy/) checks against a subset of the python files - see [pyproject.toml](pyproject.toml) for more information.
+* ``make lint``: This runs all the linters checks against the repo: check-isort, mypy, check-black, flake, pylint
 
 ## Type Annotations
 
 As you contribute to the repo, consider adding type annotations. See [DSX-2322](https://datarobot.atlassian.net/browse/DSX-2322) for more information, but:
 
 1. Prefer `from __future__ import annotations` (PEP 563) to postpone annotation evaluation, rather than explicit string literals.
 2. If you have updated an entire file, please remove it from `[tool.mypy.overrides]` in `pyproject.toml`.
```

### Comparing `datarobot-3.1.1/common_setup.py` & `datarobot-3.2.0b0/common_setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 
 DEFAULT_CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 
@@ -129,23 +131,20 @@
 ] + images_require
 
 dev_require = (
     tests_require
     + lint_require
     + images_require
     + [
-        "Sphinx==1.8.3",
-        "sphinx_rtd_theme==0.1.9",
-        "nbsphinx>=0.2.9,<1",
-        "mistune==0.8.4",
-        "nbconvert==5.3.1",
-        "numpydoc>=0.6.0",
+        "Sphinx==4.3.2",
+        "sphinx_rtd_theme==1.0.0",
+        "nbsphinx==0.8.9",
+        "numpydoc==1.4.0",
         "jupyter_contrib_nbextensions",
-        "tornado<6.0",
-        "jsonschema<=4.3.1",
+        "sphinx-autodoc-typehints==1.17.1",
     ]
 )
 
 example_require = [
     "jupyter<=5.0",
     "fredapi==0.4.0",
     "matplotlib>=2.1.0",
@@ -178,19 +177,20 @@
     python_requires=">=3.7",
     long_description=None,
     classifiers=None,
     install_requires=[
         "pandas>=0.15",
         "numpy",
         "pyyaml>=3.11",
-        "requests>=2.21",
+        "requests>=2.28.1",
         "requests_toolbelt>=0.6",
         "trafaret>=0.7,<2.2,!=1.1.0",
-        "urllib3>=1.23",
+        "urllib3>=1.23,<2.0.0",
         "typing-extensions>=4.3.0,<5",
+        "mypy-extensions>=0.4.0,<2",
     ],
     extras_require={
         "dev": dev_require,
         "examples": example_require,
         "release": release_require,
         "lint": lint_require,
         "images": images_require,
```

### Comparing `datarobot-3.1.1/datarobot/__init__.py` & `datarobot-3.2.0b0/datarobot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # flake8: noqa
 
 from ._version import __version__
 from .client import Client
+from .context import Context
 from .enums import (
     AUTOPILOT_MODE,
     NETWORK_EGRESS_POLICY,
     QUEUE_STATUS,
     SCORING_TYPE,
     SNAPSHOT_POLICY,
     TARGET_TYPE,
     VERBOSITY_LEVEL,
 )
 from .errors import AppPlatformError
 from .helpers import *
 from .models import (
+    Application,
     AutomatedDocument,
+    BatchMonitoringJob,
+    BatchMonitoringJobDefinition,
     BatchPredictionJob,
     BatchPredictionJobDefinition,
     BlenderModel,
     Blueprint,
     BlueprintChart,
     BlueprintTaskDocument,
     CalendarFile,
@@ -92,9 +96,10 @@
     SegmentInfo,
     ShapImpact,
     ShapMatrix,
     ShapMatrixJob,
     SharingAccess,
     TrainingPredictions,
     TrainingPredictionsJob,
+    UseCase,
     UserBlueprint,
 )
```

### Comparing `datarobot-3.1.1/datarobot/_compat.py` & `datarobot-3.2.0b0/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/client.py` & `datarobot-3.2.0b0/datarobot/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -19,14 +19,15 @@
 from typing import Optional, Tuple, TYPE_CHECKING, Union
 import warnings
 
 from urllib3 import Retry
 import yaml
 
 from ._version import __expected_server_version__, __version__
+from .context import Context, DefaultUseCase
 from .errors import ClientError
 from .rest import DataRobotClientConfig, RESTClientObject
 
 if TYPE_CHECKING:
     from requests import Response
 
 logger = logging.getLogger(__package__)
@@ -43,23 +44,29 @@
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
-) -> RESTClientObject:
-    """Return a new `RESTClientObject` with optional configuration.
-    Missing configuration will be read from environment variables or a config
-    file.
+    default_use_case: Optional[str] = None,
+) -> Tuple[RESTClientObject, Optional[str]]:
+    """Return a new `RESTClientObject` and default_use_case id with optional configuration.
+    The client will be configured in one of the following ways, in order of priority.
+
+      1. From call args iff ``token`` and ``endpoint`` kwargs are specified;
+      2. From a YAML file at the path specified in the ``config_path`` kwarg;
+      3. From a YAML file at the path specified in the env var ``DATAROBOT_CONFIG_FILE``;
+      4. From env vars, iff ``DATAROBOT_ENDPOINT`` and ``DATAROBOT_API_TOKEN`` are specified;
+      5. From a YAML file at the path `$HOME/.config/datarobot/drconfig.yaml`.
 
     .. note::
-        This function is intended for use with the ``client_configuration``
-        context manager only. Use of the global context will eventually
-        be deprecated.
+        This function is intended for use with the ``Client`` function and the
+        ``client_configuration`` context manager only. Use of the global context will
+        be deprecated in v4.0.
 
     Parameters
     ----------
     token : str, optional
         API token
     endpoint : str, optional
         Base url of API
@@ -78,25 +85,28 @@
         Could be set to path with certificates of trusted certification authorities
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools
+    default_use_case: str, optional
+        The entity ID of the default Use Case to use with any requests made by this Client instance.
     """
     env_config = _get_config_file_from_env()
     if token and endpoint:
         drconfig = DataRobotClientConfig(
             endpoint=endpoint,
             token=token,
             connect_timeout=connect_timeout,
             user_agent_suffix=user_agent_suffix,
             ssl_verify=ssl_verify,
             max_retries=max_retries,
             token_type=token_type,
+            default_use_case=default_use_case,
         )
     elif config_path:
         if not _file_exists(config_path):
             raise ValueError(f"Invalid config path - no file at {config_path}")
         drconfig = _config_from_file(config_path)
     elif env_config:
         if not _file_exists(env_config):
@@ -115,31 +125,43 @@
     if not drconfig.max_retries:
         drconfig.max_retries = Retry(backoff_factor=0.1, respect_retry_after_header=True)
 
     client = RESTClientObject.from_config(drconfig)
     if not _is_compatible_client(client):
         raise ValueError("The client is not compatible with the server version")
 
-    return client
+    return client, drconfig.default_use_case
 
 
 def Client(
     token: Optional[str] = None,
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
+    default_use_case: Optional[str] = None,
 ) -> RESTClientObject:
     """
-    Configures the global API client for the Python SDK with optional
-    configuration. Missing configuration will be read from env
-    or config file.
+    Configures the global API client for the Python SDK. The client will be configured in one of
+    the following ways, in order of priority.
+
+      1. From call args iff ``token`` and ``endpoint`` kwargs are specified;
+      2. From a YAML file at the path specified in the ``config_path`` kwarg;
+      3. From a YAML file at the path specified in the env var ``DATAROBOT_CONFIG_FILE``;
+      4. From env vars, iff ``DATAROBOT_ENDPOINT`` and ``DATAROBOT_API_TOKEN`` are specified;
+      5. From a YAML file at the path `$HOME/.config/datarobot/drconfig.yaml`.
+
+    .. note::
+        All client configuration must be done via a single method; there is no fall back to
+        lower priority methods.
+
+    This can also have the side effect of setting a default Use Case for client API requests.
 
     Parameters
     ----------
     token : str, optional
         API token
     endpoint : str, optional
         Base url of API
@@ -158,31 +180,34 @@
         Could be set to path with certificates of trusted certification authorities.
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools.
-
+    default_use_case: str, optional
+        The entity ID of the default Use Case to use with any requests made by the client.
     Returns
     -------
         The ``RESTClientObject`` instance created.
     """
-    new_client = _create_client(
+    new_client, default_use_case = _create_client(
         token,
         endpoint,
         config_path,
         connect_timeout,
         user_agent_suffix,
         ssl_verify,
         max_retries,
         token_type,
+        default_use_case,
     )
 
     set_client(new_client)
+    Context.use_case = default_use_case
 
     return new_client
 
 
 def _is_compatible_client(client: RESTClientObject) -> bool:
     """
     Check that this client version is not ahead of the DataRobot version that
@@ -191,18 +216,26 @@
     Parameters
     ----------
     client : RESTClientObject
 
     Returns
     -------
     bool : True if client is compatible with server, False otherwise.
+
+    Raises
+    ------
+    ClientError
+        If the client is unable to authenticate with the DataRobot API.
+
     """
     try:
         server_response = client.get("version/")
     except ClientError as cerr:
+        # TODO Prefer to do further error handling via BaseException.add_note but that
+        # is only available in Python 3.11+
         if cerr.status_code == 401:
             w_msg_tmpl = (
                 'Unable to authenticate to the server - are you sure the provided token of "{}" '
                 'and endpoint of "{}" are correct? '.format(client.token, client.endpoint)
             )
         else:
             w_msg_tmpl = (
@@ -212,16 +245,17 @@
                 "incompatible with this version of the DataRobot client package. "
             )
         w_msg_tmpl += (
             "Note that if you access the DataRobot webapp at "
             "`https://app.datarobot.com`, then the correct endpoint to specify would "
             "be `https://app.datarobot.com/api/v2`."
         )
-        warnings.warn(w_msg_tmpl.format(client.endpoint))
-        return False
+        raise ClientError(
+            w_msg_tmpl.format(client.endpoint), status_code=cerr.status_code
+        ) from cerr
 
     if not _is_compatible_version(server_response):
         return False
 
     _ensure_protocol_match(client, server_response)
     return True
 
@@ -322,14 +356,18 @@
 
 
 def _get_client_version() -> str:
     return __version__
 
 
 def get_client() -> RESTClientObject:
+    """
+    Returns the global HTTP client for the Python SDK, instantiating it
+    if necessary.
+    """
     return _context_client.get(_global_client) or Client()
 
 
 class staticproperty(property):
     def __get__(self, instance, owner):
         return self.fget()
 
@@ -372,50 +410,50 @@
 
 
 _file_exists = os.path.isfile
 
 
 def _config_from_env() -> DataRobotClientConfig:
     """
-    Create and return a DataRobotClientConfig from environment variables.
-
-    There are two ways this can be used:
-    1. Use the environment variable DATAROBOT_CONFIG_FILE to specify the path to a yaml config
-       file specifying the configuration to use
-    2. Use both the environment variables DATAROBOT_ENDPOINT and DATAROBOT_API_TOKEN to specify
-       the connection parameters. Note that this method only allows for configuration of endpoint,
-       token and user_agent_suffix; any more advanced configuration must be done through a yaml
-       file
+    Create and return a DataRobotClientConfig from environment variables. This method only allows
+    for configuration of endpoint, token, user_agent_suffix, max retries, and a default use case.
+    More advanced configuration must be done through a yaml file.
 
     Returns
     -------
     config : DataRobotClientConfig
 
     Raises
     ------
     ValueError
         If either of DATAROBOT_ENDPOINT or DATAROBOT_API_TOKEN is not specified as an environment
         variable
     IOError
         If the config file that DATAROBOT_CONFIG_FILE points to does not exist
     """
-    endpoint = os.environ.get("DATAROBOT_ENDPOINT")
-    token = os.environ.get("DATAROBOT_API_TOKEN")
-    user_agent_suffix = os.environ.get("DATAROBOT_USER_AGENT_SUFFIX")
+    endpoint: Optional[str] = os.environ.get("DATAROBOT_ENDPOINT")
+    token: Optional[str] = os.environ.get("DATAROBOT_API_TOKEN")
+    user_agent_suffix: Optional[str] = os.environ.get("DATAROBOT_USER_AGENT_SUFFIX")
     max_retries: Optional[Union[str, int]] = os.environ.get("DATAROBOT_MAX_RETRIES")
     if max_retries is not None:
         max_retries = int(max_retries)
+    use_case_id: Optional[str] = os.environ.get("DATAROBOT_DEFAULT_USE_CASE")
+
     if endpoint is None or token is None:
         e_msg = (
             "Incomplete DataRobot configuration specified in environment variables; both "
             "DATAROBOT_ENDPOINT and DATAROBOT_API_TOKEN must be specified"
         )
         raise ValueError(e_msg)
     return DataRobotClientConfig(
-        endpoint=endpoint, token=token, user_agent_suffix=user_agent_suffix, max_retries=max_retries
+        endpoint=endpoint,
+        token=token,
+        user_agent_suffix=user_agent_suffix,
+        max_retries=max_retries,
+        default_use_case=use_case_id,
     )
 
 
 def _config_from_file(config_path: str) -> DataRobotClientConfig:
     """
     Create and return a DataRobotClientConfig from a config path. The file must be
     a yaml formatted file
@@ -443,15 +481,15 @@
     per thread.
 
     DataRobot does not recommend nesting these contexts.
 
     Parameters
     ----------
         args : Parameters passed to ``datarobot.client.Client()``
-        kwargs : Keyword arguments passed to ``datarobot.Client()``
+        kwargs : Keyword arguments passed to ``datarobot.client.Client()``
 
     Examples
     --------
 
     .. code-block:: python
 
         from datarobot.client import client_configuration
@@ -470,14 +508,18 @@
 
         with client_configuration(config_path="/path/to/a/drconfig.yaml"):
             # Interact with DataRobot using a different configuration.
             Project.list()
     """
 
     contextvars_token: contextvars.Token[RESTClientObject] = None
+    previous_use_case: DefaultUseCase = None
     try:
-        client = _create_client(*args, **kwargs)
+        client, default_use_case = _create_client(*args, **kwargs)
         contextvars_token = _context_client.set(client)
+        previous_use_case = Context.get_use_case(raw=True)
+        Context.use_case = default_use_case
         yield
     finally:
         if contextvars_token is not None:
             _context_client.reset(contextvars_token)
+        Context.use_case = previous_use_case
```

### Comparing `datarobot-3.1.1/datarobot/enums.py` & `datarobot-3.2.0b0/datarobot/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,42 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+from __future__ import annotations
+
+from enum import Enum, EnumMeta
+from typing import Optional
+
+
+# A decorator to add an ALL attribute to (str, Enum) classes.
+def use_all(enum_instance):
+    setattr(enum_instance, "ALL", list(map(lambda c: c, enum_instance)))
+    return enum_instance
+
+
+class StrEnum(EnumMeta):
+    """
+    Enum that permits comparison of strings.
+    Ref: https://stackoverflow.com/questions/63335753/how-to-check-if-string-exists-in-enum-of-strings
+    """
+
+    def __contains__(cls: type, member: object) -> bool:
+        try:
+            cls(member)  # pylint: disable=no-value-for-parameter
+        except ValueError:
+            return False
+        return True
 
 
 def enum(*vals, **enums):
     """
     Enum without third party libs and compatible with py2 and py3 versions.
     """
     enums.update(dict(zip(vals, vals)))
@@ -76,14 +100,17 @@
     QUICK="quick",
     COMPREHENSIVE="comprehensive",
 )
 
 PROJECT_STAGE = enum(
     AIM="aim", EDA="eda", EDA2="eda2", FASTEDA="fasteda", EMPTY="empty", MODELING="modeling"
 )
+PRE_EDA2_STAGES = [PROJECT_STAGE.EDA, PROJECT_STAGE.AIM, PROJECT_STAGE.FASTEDA, PROJECT_STAGE.EMPTY]
+POST_EDA2_STAGES = [PROJECT_STAGE.EDA2, PROJECT_STAGE.MODELING]
+
 
 ASYNC_PROCESS_STATUS = enum(
     ABORTED="ABORTED",
     COMPLETED="COMPLETED",
     ERROR="ERROR",
     INITIALIZED="INITIALIZED",
     RUNNING="RUNNING",
@@ -99,19 +126,19 @@
     REGRESSION = "Regression"
     UNSTRUCTURED = "Unstructured"
     ANOMALY = "Anomaly"
     ALL = [BINARY, MULTICLASS, MULTILABEL, REGRESSION, UNSTRUCTURED, ANOMALY]
 
 
 JOB_TYPE = enum(
+    BATCH_MONITORING="batchMonitoring",
     BATCH_PREDICTIONS="batchPredictions",
     BATCH_PREDICTION_JOB_DEFINITIONS="batchPredictionJobDefinitions",
     FEATURE_IMPACT="featureImpact",
     FEATURE_EFFECTS="featureEffects",
-    FEATURE_FIT="featureFit",
     MODEL="model",
     MODEL_EXPORT="modelExport",
     PREDICT="predict",
     TRAINING_PREDICTIONS="trainingPredictions",
     PRIME_MODEL="primeModel",
     PRIME_RULESETS="primeRulesets",
     PRIME_VALIDATION="primeDownloadValidation",
@@ -162,26 +189,27 @@
 TS_BLENDER_METHOD = enum(
     AVERAGE="AVG",
     MEDIAN="MED",
     FORECAST_DISTANCE_ENET="FORECAST_DISTANCE_ENET",
     FORECAST_DISTANCE_AVG="FORECAST_DISTANCE_AVG",
 )
 
-CHART_DATA_SOURCE = enum(
-    CROSSVALIDATION="crossValidation",
-    HOLDOUT="holdout",
-    VALIDATION="validation",
-)
 
-DATA_SUBSET = enum(
-    ALL="all",
-    VALIDATION_AND_HOLDOUT="validationAndHoldout",
-    HOLDOUT="holdout",
-    ALL_BACKTESTS="allBacktests",
-)
+class CHART_DATA_SOURCE(str, Enum):
+    CROSSVALIDATION = "crossValidation"
+    HOLDOUT = "holdout"
+    VALIDATION = "validation"
+
+
+class DATA_SUBSET(str, Enum):
+    ALL = "all"
+    VALIDATION_AND_HOLDOUT = "validationAndHoldout"
+    HOLDOUT = "holdout"
+    ALL_BACKTESTS = "allBacktests"
+
 
 FEATURE_TYPE = enum(NUMERIC="numeric", CATEGORICAL="categorical", DATETIME="datetime")
 
 DEFAULT_MAX_WAIT = 600
 
 # default time out values in seconds for waiting response from client
 DEFAULT_TIMEOUT = enum(
@@ -293,22 +321,29 @@
     MULTISERIES_VALUE="multiseriesValue",
     ROW_COUNT="rowCount",
     VALIDATION_SCORE="validationScore",
     BACKTESTING_SCORE="backtestingScore",
     HOLDOUT_SCORE="holdoutScore",
 )
 
-SHARING_ROLE = enum(
-    OWNER="OWNER",
-    READ_WRITE="READ_WRITE",
-    USER="USER",
-    EDITOR="EDITOR",
-    READ_ONLY="READ_ONLY",
-    CONSUMER="CONSUMER",
-)
+
+class SHARING_ROLE(str, Enum):
+    OWNER = ("OWNER",)
+    READ_WRITE = ("READ_WRITE",)
+    USER = ("USER",)
+    EDITOR = ("EDITOR",)
+    READ_ONLY = ("READ_ONLY",)
+    CONSUMER = ("CONSUMER",)
+    NO_ROLE = "NO_ROLE"
+
+
+class SHARING_RECIPIENT_TYPE(str, Enum):
+    USER = "user"
+    ORGANIZATION = "organization"
+
 
 MODEL_REPLACEMENT_REASON = enum(
     ACCURACY="ACCURACY",
     DATA_DRIFT="DATA_DRIFT",
     ERRORS="ERRORS",
     SCHEDULED_REFRESH="SCHEDULED_REFRESH",
     SCORING_SPEED="SCORING_SPEED",
@@ -333,14 +368,23 @@
     SPEARMAN = "spearman"
     PEARSON = "pearson"
     TAU = "tau"
 
     ALL = [MUTUAL_INFO, CRAMER, SPEARMAN, PEARSON, TAU]
 
 
+class BUCKET_SIZE:
+    PT1H = "PT1H"
+    P1D = "P1D"
+    P7D = "P7D"
+    P1M = "P1M"
+
+    ALL = [PT1H, P1D, P7D, P1M]
+
+
 class SERVICE_STAT_METRIC:  # pylint: disable=missing-class-docstring
     TOTAL_PREDICTIONS = "totalPredictions"
     TOTAL_REQUESTS = "totalRequests"
     SLOW_REQUESTS = "slowRequests"
     EXECUTION_TIME = "executionTime"
     RESPONSE_TIME = "responseTime"
     USER_ERROR_RATE = "userErrorRate"
@@ -512,22 +556,21 @@
 
     NONE = "NONE"
     PUBLIC = "PUBLIC"
 
     ALL = [NONE, PUBLIC]
 
 
-class SOURCE_TYPE:
+@use_all
+class SOURCE_TYPE(str, Enum):
     """Enum of backtest source types"""
 
     TRAINING = "training"
     VALIDATION = "validation"
 
-    ALL = [TRAINING, VALIDATION]
-
 
 class DATETIME_TREND_PLOTS_STATUS:
     COMPLETED = "completed"
     NOT_COMPLETED = "notCompleted"
     IN_PROGRESS = "inProgress"
     ERRORED = "errored"
     NOT_SUPPORTED = "notSupported"
@@ -827,7 +870,68 @@
             UNSUPERVISED_MODE,
             USE_SUPERVISED_FEATURE_REDUCTION,
             USE_TIME_SERIES,
             VALIDATION_DURATION,
             WINDOW_BASIS_UNIT,
         ]
     )
+
+
+class Locales(str, Enum):
+    EN_US = "EN_US"
+    FR_FR = "FR_FR"
+    JA_JP = "JA_JP"
+    KO_KR = "KO_KR"
+    PT_BR = "PT_BR"
+
+
+class DocumentType(str, Enum):
+    AUTOPILOT_SUMMARY = "AUTOPILOT_SUMMARY"
+    MODEL_COMPLIANCE = "MODEL_COMPLIANCE"
+    DEPLOYMENT_REPORT = "DEPLOYMENT_REPORT"
+
+
+class ComplianceDocType(str, Enum):
+    DATAROBOT = "datarobot"
+    USER = "user"
+    CUSTOM = "custom"
+
+
+class ComplianceDocTemplateType(str, Enum):
+    NORMAL = "normal"
+    TIME_SERIES = "time_series"
+
+
+class UseCaseEntityType(str, Enum, metaclass=StrEnum):
+    PROJECT = "project"
+    DATASET = "dataset"
+    NOTEBOOK = "notebook"
+    APPLICATION = "application"
+    RECIPE = "recipe"
+
+
+class UseCaseAPIPathEntityType(str, Enum):
+    PROJECT = "projects"
+    DATASET = "datasets"
+    APPLICATION = "applications"
+    RECIPE = "recipes"
+
+
+UseCaseReferenceEntityMap: dict[Optional[UseCaseEntityType], UseCaseAPIPathEntityType] = {
+    UseCaseEntityType.PROJECT: UseCaseAPIPathEntityType.PROJECT,
+    UseCaseEntityType.DATASET: UseCaseAPIPathEntityType.DATASET,
+    UseCaseEntityType.APPLICATION: UseCaseAPIPathEntityType.APPLICATION,
+    UseCaseEntityType.RECIPE: UseCaseAPIPathEntityType.RECIPE,
+}
+
+
+class ApplicationPermissions(str, Enum):
+    CAN_DELETE = "CAN_DELETE"
+    CAN_SHARE = "CAN_SHARE"
+    CAN_UPDATE = "CAN_UPDATE"
+    CAN_VIEW = "CAN_VIEW"
+
+
+class CredentialTypes(str, Enum):
+    BASIC = "basic"
+    OAUTH = "oauth"
+    S3 = "s3"
```

### Comparing `datarobot-3.1.1/datarobot/errors.py` & `datarobot-3.2.0b0/datarobot/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,14 +135,34 @@
 
 class DuplicateFeaturesError(Exception):
     """
     Raised when trying to create featurelist with duplicating features
     """
 
 
+class TrainingDataAssignmentError(Exception):
+    """
+    Raised when the training data assignment for a custom model version fails
+    """
+
+    def __init__(
+        self, custom_model_id: str, custom_model_version_id: str, error_message: str
+    ) -> None:
+        self.custom_model_id = custom_model_id
+        self.custom_model_version_id = custom_model_version_id
+        self.error_message = error_message
+        self.message = (
+            f"Training data assignment failed for: "
+            f"model ID: {custom_model_id}; "
+            f"version ID: {custom_model_version_id}; "
+            f"Error message: {error_message}"
+        )
+        super().__init__(self.message)
+
+
 class DataRobotDeprecationWarning(DeprecationWarning):
     """
     Raised when using deprecated functions or using functions in a deprecated way
 
     See Also
     --------
     PlatformDeprecationWarning
```

### Comparing `datarobot-3.1.1/datarobot/helpers/__init__.py` & `datarobot-3.2.0b0/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/helpers/binary_data_utils.py` & `datarobot-3.2.0b0/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/helpers/deployment_monitoring.py` & `datarobot-3.2.0b0/datarobot/models/deployment/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import pytz
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 
-class DeploymentQueryBuilderMixin:  # pylint: disable=missing-class-docstring
+class MonitoringDataQueryBuilderMixin:  # pylint: disable=missing-class-docstring
     @staticmethod
     def _build_query_params(  # pylint: disable=missing-function-docstring
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         **kwargs: Any,
     ) -> Dict[str, Any]:
         def timezone_aware(dt: datetime) -> datetime:
```

### Comparing `datarobot-3.1.1/datarobot/helpers/eligibility_result.py` & `datarobot-3.2.0b0/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/helpers/feature_discovery.py` & `datarobot-3.2.0b0/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/helpers/image_utils.py` & `datarobot-3.2.0b0/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/helpers/partitioning_methods.py` & `datarobot-3.2.0b0/datarobot/helpers/partitioning_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 import abc
 from datetime import datetime
-from typing import Any, cast, Dict, List, Optional, TYPE_CHECKING
+from typing import Any, cast, Dict, List, NoReturn, Optional, TYPE_CHECKING
 
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.client import get_client, staticproperty
 from datarobot.enums import (
     CV_METHOD,
     DEFAULT_MAX_WAIT,
     DIFFERENCING_METHOD,
     PERIODICITY_MAX_TIME_STEP,
     SERIES_AGGREGATION_TYPE,
     TIME_UNITS,
     TREAT_AS_EXPONENTIAL,
+    UnsupervisedTypeEnum,
 )
 from datarobot.errors import InvalidUsageError, UpdateAttributesError
 from datarobot.mixins.update_attributes_mixin import UpdateAttributesMixin
 from datarobot.utils import (
     deprecated,
     deprecation_warning,
     from_api,
@@ -47,14 +48,15 @@
     "GroupCV",
     "UserCV",
     "RandomTVH",
     "UserTVH",
     "StratifiedTVH",
     "GroupTVH",
     "DatetimePartitioning",
+    "DatetimePartitioningId",
     "DatetimePartitioningSpecification",
     "BacktestSpecification",
     "FeatureSettings",
     "Periodicity",
 )
 
 if TYPE_CHECKING:
@@ -1091,14 +1093,18 @@
     model_splits: int, optional
         (New in version v2.21) Sets the cap on the number of jobs per model used when
         building models to control number of jobs in the queue. Higher number of model splits
         will allow for less downsampling leading to the use of more post-processed data.
     allow_partial_history_time_series_predictions: bool, optional
         (New in version v2.24) Whether to allow time series models to make predictions using
         partial historical data.
+    unsupervised_type: str, optional
+        (New in version v3.2) The unsupervised project type, only valid if ``unsupervised_mode`` is
+        True. Use values from ``datarobot.enums.UnsupervisedTypeEnum`` enum.
+        If not specified then the project defaults to 'anomaly' when ``unsupervised_mode`` is True.
     """
 
     _converter = t.Dict(
         {
             t.Key("datetime_partition_column"): String(),
             t.Key("autopilot_data_selection_method", optional=True): String(),
             t.Key("validation_duration", optional=True): String(),
@@ -1145,14 +1151,17 @@
                 SERIES_AGGREGATION_TYPE.AVERAGE, SERIES_AGGREGATION_TYPE.TOTAL
             ),
             t.Key("cross_series_group_by_columns", optional=True): t.List(String()),
             t.Key("calendar_id", optional=True): String(),
             t.Key("unsupervised_mode", optional=True): t.Bool(),
             t.Key("model_splits", optional=True): Int(),
             t.Key("allow_partial_history_time_series_predictions", optional=True): t.Bool,
+            t.Key("unsupervised_type", optional=True): t.Enum(
+                UnsupervisedTypeEnum.ANOMALY, UnsupervisedTypeEnum.CLUSTERING
+            ),
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         datetime_partition_column: str,
         autopilot_data_selection_method: Optional[str] = None,
@@ -1180,14 +1189,15 @@
         aggregation_type: Optional[str] = None,
         cross_series_group_by_columns: Optional[List[str]] = None,
         calendar_id: Optional[str] = None,
         holdout_end_date=None,
         unsupervised_mode: bool = False,
         model_splits: Optional[int] = None,
         allow_partial_history_time_series_predictions: bool = False,
+        unsupervised_type: Optional[str] = None,
     ) -> None:
         self.datetime_partition_column = datetime_partition_column
         self.autopilot_data_selection_method = autopilot_data_selection_method
         self.validation_duration = validation_duration
         self.holdout_start_date = holdout_start_date
         self.holdout_duration = holdout_duration
         self.holdout_end_date = holdout_end_date
@@ -1213,14 +1223,15 @@
         self.cross_series_group_by_columns = cross_series_group_by_columns
         self.calendar_id = calendar_id
         self.unsupervised_mode = unsupervised_mode
         self.model_splits = model_splits
         self.allow_partial_history_time_series_predictions = (
             allow_partial_history_time_series_predictions
         )
+        self.unsupervised_type = unsupervised_type
 
     def collect_payload(self) -> Dict[str, Any]:
         if self.holdout_start_date and not isinstance(self.holdout_start_date, datetime):
             raise ValueError("expected holdout_start_date to be a datetime.datetime")
         if self.holdout_end_date and not isinstance(self.holdout_end_date, datetime):
             raise ValueError("expected holdout_end_date to be a datetime.datetime")
         if self.holdout_duration and self.holdout_end_date:
@@ -1265,14 +1276,16 @@
             "model_splits": self.model_splits,
             "allow_partial_history_time_series_predictions": (
                 self.allow_partial_history_time_series_predictions
             ),
         }
         if self.unsupervised_mode:
             payload["unsupervised_mode"] = self.unsupervised_mode
+            if self.unsupervised_type:
+                payload["unsupervised_type"] = self.unsupervised_type
         if not self.disable_holdout:
             payload["holdout_start_date"] = self.holdout_start_date
             if self.holdout_duration:
                 payload["holdout_duration"] = self.holdout_duration
             elif self.holdout_end_date:
                 payload["holdout_end_date"] = self.holdout_end_date
 
@@ -1517,14 +1530,18 @@
         building models to control number of jobs in the queue. Higher number of model splits
         will allow for less downsampling leading to the use of more post-processed data.
     allow_partial_history_time_series_predictions: bool, optional
         (New in version v2.24) Whether to allow time series models to make predictions using
         partial historical data.
     unsupervised_mode: bool, optional
         (New in version v3.1) Whether the date/time partitioning is for an unsupervised project
+    unsupervised_type: str, optional
+        (New in version v3.2) The unsupervised project type, only valid if ``unsupervised_mode`` is
+        True. Use values from ``datarobot.enums.UnsupervisedTypeEnum`` enum.
+        If not specified then the project defaults to 'anomaly' when ``unsupervised_mode`` is True.
     """
 
     _client = staticproperty(get_client)
     _converter = t.Dict(
         {
             t.Key("project_id"): String(),
             t.Key("datetime_partitioning_id", optional=True): t.Or(String(), t.Null),
@@ -1591,14 +1608,17 @@
             ),
             t.Key("cross_series_group_by_columns", optional=True): t.List(String()),
             t.Key("calendar_id", optional=True): String(),
             t.Key("calendar_name", optional=True): String(),
             t.Key("model_splits", optional=True): Int(),
             t.Key("allow_partial_history_time_series_predictions", optional=True): t.Bool,
             t.Key("unsupervised_mode", optional=True): t.Bool,
+            t.Key("unsupervised_type", optional=True): t.Enum(
+                UnsupervisedTypeEnum.ANOMALY, UnsupervisedTypeEnum.CLUSTERING
+            ),
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         project_id=None,
         datetime_partitioning_id=None,
@@ -1645,14 +1665,15 @@
         aggregation_type=None,
         cross_series_group_by_columns=None,
         calendar_id=None,
         calendar_name=None,
         model_splits=None,
         allow_partial_history_time_series_predictions=False,
         unsupervised_mode=False,
+        unsupervised_type=None,
     ):
         self.project_id = project_id
         self.datetime_partitioning_id = datetime_partitioning_id
         self.datetime_partition_column = datetime_partition_column
         self.date_format = date_format
         self.autopilot_data_selection_method = autopilot_data_selection_method
         self.validation_duration = validation_duration
@@ -1697,14 +1718,15 @@
         self.calendar_id = calendar_id
         self.calendar_name = calendar_name
         self.model_splits = model_splits
         self.allow_partial_history_time_series_predictions = (
             allow_partial_history_time_series_predictions
         )
         self.unsupervised_mode = unsupervised_mode
+        self.unsupervised_type = unsupervised_type
 
     @classmethod
     def from_server_data(cls, data):  # pylint: disable=missing-function-docstring
         converted_data = cls._converter.check(from_api(data))
         converted_data["backtests"] = [
             Backtest(**backtest_data) for backtest_data in converted_data["backtests"]
         ]
@@ -2012,14 +2034,15 @@
             "calendar_id": self.calendar_id,
             "model_splits": self.model_splits,
             "disable_holdout": self.disable_holdout,
             "allow_partial_history_time_series_predictions": (
                 self.allow_partial_history_time_series_predictions
             ),
             "unsupervised_mode": self.unsupervised_mode,
+            "unsupervised_type": self.unsupervised_type,
         }
         if use_holdout_start_end_format:
             init_data["holdout_end_date"] = self.holdout_end_date
         else:
             init_data["holdout_duration"] = self.holdout_duration
 
         return DatetimePartitioningSpecification(**init_data)
@@ -2051,10 +2074,161 @@
             "end_date": {
                 "available_training": self.available_training_end_date,
                 "primary_training": self.primary_training_end_date,
                 "gap": self.gap_end_date,
                 "holdout": self.holdout_end_date,
             },
         }
-        display_df = pd.DataFrame.from_dict(display_dict)
-        final_df = display_df.append([bt.to_dataframe() for bt in self.backtests])
+        display_df_list = [pd.DataFrame.from_dict(display_dict)]
+        display_df_list.extend([bt.to_dataframe() for bt in self.backtests])
+        final_df = pd.concat(display_df_list)
         return final_df
+
+    @classmethod
+    def datetime_partitioning_log_retrieve(
+        cls, project_id: str, datetime_partitioning_id: str
+    ) -> Any:
+        """Retrieve the datetime partitioning log content for an optimized datetime partitioning.
+
+        The datetime partitioning log provides details about the partitioning process for an OTV
+        or time series project.
+
+        Parameters
+        ----------
+        project_id : str
+            The project ID of the project associated with the datetime partitioning.
+        datetime_partitioning_id : str
+            id of the optimized datetime partitioning
+        """
+        url = (
+            f"projects/{project_id}/optimizedDatetimePartitionings/{datetime_partitioning_id}/"
+            "datetimePartitioningLog/file/"
+        )
+        response = cls._client.get(url)
+        return response.text
+
+    @classmethod
+    def datetime_partitioning_log_list(
+        cls,
+        project_id: str,
+        datetime_partitioning_id: str,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> Any:
+        """Retrieve the datetime partitioning log content and log length for an optimized
+        datetime partitioning.
+
+        The Datetime Partitioning Log provides details about the partitioning process for an OTV
+        or Time Series project.
+
+        Parameters
+        ----------
+        project_id : str
+            project id of the project associated with the datetime partitioning.
+        datetime_partitioning_id : str
+            id of the optimized datetime partitioning
+        offset : int or None
+            optional, defaults is 0, this many results will be skipped.
+        limit : int or None
+            optional, defaults to 100, at most this many results are returned. To specify
+            no limit, use 0. The default may change without notice.
+        """
+        url = (
+            f"projects/{project_id}/optimizedDatetimePartitionings/{datetime_partitioning_id}/"
+            "datetimePartitioningLog/"
+        )
+        response = cls._client.get(url, params=dict(offset=offset, limit=limit))
+        return response.json()
+
+    @classmethod
+    def get_input_data(
+        cls, project_id: str, datetime_partitioning_id: str
+    ) -> DatetimePartitioningSpecification:
+        """Retrieve the input used to create an optimized DatetimePartitioning from a project for
+        the specified datetime_partitioning_id. A datetime_partitioning_id is created by using the
+        :meth:`generate_optimized<datarobot.DatetimePartitioning.generate_optimized>` function.
+
+        Parameters
+        ----------
+        project_id : str
+            The ID of the project to retrieve partitioning for.
+        datetime_partitioning_id : ObjectId
+            The ObjectId associated with the project to retrieve from Mongo.
+
+        Returns
+        -------
+        DatetimePartitioningInput : The input to optimized datetime partitioning.
+        """
+        url = "projects/{}/optimizedDatetimePartitionings/{}/datetimePartitioningInput/".format(
+            project_id, datetime_partitioning_id
+        )
+        response = cls._client.get(url)
+        return DatetimePartitioningSpecification.from_server_data(
+            # type: ignore[no-untyped-call, no-any-return]
+            response.json()
+        )
+
+
+class DatetimePartitioningId(PartitioningMethod):
+    """Defines a DatetimePartitioningId used for datetime partitioning.
+
+    This class only includes the datetime_partitioning_id that identifies a previously
+    optimized datetime partitioning and the project_id for the associated project.
+
+    This is the specification that should be passed to :meth:`Project.analyze_and_model
+    <datarobot.models.Project.analyze_and_model>` via the ``partitioning_method`` parameter. To see
+    the full partitioning use :meth:`DatetimePartitioning.get_optimized
+    <datarobot.DatetimePartitioning.get_optimized>`.
+
+    Attributes
+    ----------
+    datetime_partitioning_id : str
+        The ID of the datetime partitioning to use.
+    project_id : str
+        The ID of the project that the datetime partitioning is associated with.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("datetime_partitioning_id"): String(),
+            t.Key("project_id"): String(),
+        }
+    ).ignore_extra("*")
+
+    def __init__(self, datetime_partitioning_id: str, project_id: str):
+        self.datetime_partitioning_id = datetime_partitioning_id
+        self.project_id = project_id
+
+    def _keys_with_defaults(self) -> List[str]:
+        """These keys have default values in the API so they will always be present when starting
+        a project. Make sure these values are set if they are present in the datetime
+        partitioning input."""
+        return [
+            "unsupervised_mode",
+            "treat_as_exponential",
+            "autopilot_data_selection_method",
+            "use_supervised_feature_reduction",
+            "use_time_series",
+            "disable_holdout",
+            "model_splits",
+        ]
+
+    def collect_payload(self) -> Dict[str, Any]:
+        payload = {
+            "datetime_partitioning_id": self.datetime_partitioning_id,
+            "cv_method": CV_METHOD.DATETIME,
+        }
+        datetime_partitioning_input = DatetimePartitioning.get_input_data(
+            self.project_id, self.datetime_partitioning_id
+        )
+        input_payload = datetime_partitioning_input.collect_payload()
+        for key in self._keys_with_defaults():
+            if key in input_payload and input_payload[key] is not None:
+                payload[key] = input_payload[key]
+
+        return payload
+
+    def prep_payload(self, project_id: str, max_wait: int = DEFAULT_MAX_WAIT) -> None:
+        pass
+
+    def update(self, **kwargs: Any) -> NoReturn:
+        raise InvalidUsageError
```

### Comparing `datarobot-3.1.1/datarobot/mixins/browser_mixin.py` & `datarobot-3.2.0b0/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/mixins/update_attributes_mixin.py` & `datarobot-3.2.0b0/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/__init__.py` & `datarobot-3.2.0b0/datarobot/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # because the unused imports are on purpose
 
-from .accuracy import Accuracy, AccuracyOverTime
+from .application import Application
 from .automated_documentation import AutomatedDocument
+from .batch_monitoring_job import BatchMonitoringJob, BatchMonitoringJobDefinition
 from .batch_prediction_job import BatchPredictionJob, BatchPredictionJobDefinition
 from .blueprint import Blueprint, BlueprintChart, BlueprintTaskDocument, ModelBlueprintChart
 from .calendar_file import CalendarFile
 from .change_request import ChangeRequest, ChangeRequestReview
 from .cluster import Cluster
 from .cluster_insight import ClusterInsight
 from .compliance_doc_template import ComplianceDocTemplate
@@ -17,15 +18,14 @@
 from .custom_model_version import (
     CustomModelVersion,
     CustomModelVersionConversion,
     CustomModelVersionDependencyBuild,
 )
 from .custom_task import CustomTask
 from .custom_task_version import CustomTaskVersion
-from .data_drift import FeatureDrift, TargetDrift
 from .data_engine_query_generator import DataEngineQueryGenerator
 from .data_source import DataSource, DataSourceParameters
 from .data_store import DataStore
 from .dataset import Dataset, DatasetDetails
 from .deployment import Deployment
 from .driver import DataDriver
 from .execution_environment import ExecutionEnvironment
@@ -57,20 +57,14 @@
 from .feature_effect import (
     FeatureEffectMetadata,
     FeatureEffectMetadataDatetime,
     FeatureEffectMetadataDatetimePerBacktest,
     FeatureEffects,
     FeatureEffectsMulticlass,
 )
-from .feature_fit import (
-    FeatureFit,
-    FeatureFitMetadata,
-    FeatureFitMetadataDatetime,
-    FeatureFitMetadataDatetimePerBacktest,
-)
 from .featurelist import DatasetFeaturelist, Featurelist, ModelingFeaturelist
 from .imported_model import ImportedModel
 from .job import FeatureImpactJob, Job, TrainingPredictionsJob
 from .model import (
     BlenderModel,
     ClusteringModel,
     CombinedModel,
@@ -102,14 +96,22 @@
 from .project import Project
 from .rating_table import RatingTable
 from .recommended_model import ModelRecommendation
 from .relationships_configuration import RelationshipsConfiguration
 from .ruleset import Ruleset
 from .secondary_dataset import SecondaryDatasetConfigurations
 from .segmentation import SegmentationTask, SegmentInfo
-from .service_stats import ServiceStats, ServiceStatsOverTime
 from .shap_impact import ShapImpact
 from .shap_matrix import ShapMatrix
 from .shap_matrix_job import ShapMatrixJob
 from .sharing import SharingAccess
 from .training_predictions import TrainingPredictions
+from .types import (
+    AnomalyAssessmentDataPoint,
+    AnomalyAssessmentPreviewBin,
+    AnomalyAssessmentRecordMetadata,
+    RegionExplanationsData,
+    RocCurveEstimatedMetric,
+    ShapleyFeatureContribution,
+)
+from .use_cases.use_case import UseCase
 from .user_blueprints import UserBlueprint
```

### Comparing `datarobot-3.1.1/datarobot/models/accuracy.py` & `datarobot-3.2.0b0/datarobot/models/deployment/accuracy.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 from typing import Dict, List, Optional, TYPE_CHECKING
 
 import dateutil
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
+from datarobot.enums import ACCURACY_METRIC
 from datarobot.models.api_object import APIObject
-
-from ..enums import ACCURACY_METRIC
-from ..helpers.deployment_monitoring import DeploymentQueryBuilderMixin
-from ..utils import from_api
+from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
+from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
         end: datetime
@@ -42,46 +41,38 @@
 
     class Bucket(TypedDict):
         period: Period
         value: int
         sample_size: int
 
 
-class Accuracy(APIObject, DeploymentQueryBuilderMixin):
+class Accuracy(APIObject, MonitoringDataQueryBuilderMixin):
     """Deployment accuracy information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metrics
     period : dict
         the time period used to retrieve accuracy metrics
     metrics : dict
         the accuracy metrics
     """
 
     _path = "deployments/{}/accuracy/"
-    _period = t.Dict(
-        {
-            t.Key("start"): String >> dateutil.parser.parse,
-            t.Key("end"): String >> dateutil.parser.parse,
-        }
-    )
-    _metric = t.Dict(
-        {
-            t.Key("value", optional=True): t.Or(t.Float, t.Null),
-            t.Key("baseline_value", optional=True): t.Or(t.Float, t.Null),
-            t.Key("percent_change", optional=True): t.Or(t.Float, t.Null),
-        }
-    ).allow_extra("*")
     _converter = t.Dict(
         {
-            t.Key("period"): _period,
-            t.Key("metrics"): t.Mapping(t.Enum(*ACCURACY_METRIC.ALL), _metric),
-            t.Key("model_id"): t.Or(String(), t.Null),
+            t.Key("period"): t.Dict(
+                {
+                    t.Key("start"): String >> dateutil.parser.parse,
+                    t.Key("end"): String >> dateutil.parser.parse,
+                }
+            ),
+            t.Key("model_id"): t.String(),
+            t.Key("metrics"): t.Dict().allow_extra("*"),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
         period: Optional[Period] = None,
         metrics: Optional[Dict[str, Metric]] = None,
@@ -146,15 +137,15 @@
         """
 
         path = cls._path.format(deployment_id)
         params = cls._build_query_params(
             start_time=start_time,
             end_time=end_time,
             model_id=model_id,
-            target_classes=target_classes,
+            target_class=target_classes,
         )
         data = cls._client.get(path, params=params).json()
 
         # we don't want to convert keys of the metrics object
         metrics = data.pop("metrics")
         for metric, value in metrics.items():
             metrics[metric] = from_api(value, keep_null_keys=True)
@@ -193,15 +184,15 @@
         -------
         percent_changes: Dict
         """
 
         return {name: value.get("percent_change") for name, value in self.metrics.items()}
 
 
-class AccuracyOverTime(APIObject, DeploymentQueryBuilderMixin):
+class AccuracyOverTime(APIObject, MonitoringDataQueryBuilderMixin):
     """Deployment accuracy over time information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metric
     metric : str
@@ -217,23 +208,21 @@
     _path = "deployments/{}/accuracyOverTime/"
     _period = t.Dict(
         {
             t.Key("start"): String >> dateutil.parser.parse,
             t.Key("end"): String >> dateutil.parser.parse,
         }
     )
-
     _bucket = t.Dict(
         {
             t.Key("period"): t.Or(_period, t.Null),
             t.Key("value"): t.Or(t.Float, t.Null),
             t.Key("sample_size"): t.Or(Int, t.Null),
         }
     ).allow_extra("*")
-
     _converter = t.Dict(
         {
             t.Key("buckets"): t.List(_bucket),
             t.Key("summary"): _bucket,
             t.Key("baseline"): _bucket,
             t.Key("metric"): String(),
             t.Key("model_id"): t.Or(String(), t.Null),
@@ -317,15 +306,15 @@
         path = cls._path.format(deployment_id)
         params = cls._build_query_params(
             start_time=start_time,
             end_time=end_time,
             model_id=model_id,
             metric=metric,
             bucket_size=bucket_size,
-            target_classes=target_classes,
+            target_class=target_classes,
         )
         data = cls._client.get(path, params=params).json()
         case_converted = from_api(data, keep_null_keys=True)
         return cls.from_data(case_converted)
 
     @classmethod
     def get_as_dataframe(
```

### Comparing `datarobot-3.1.1/datarobot/models/advanced_tuning.py` & `datarobot-3.2.0b0/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/anomaly_assessment.py` & `datarobot-3.2.0b0/datarobot/models/anomaly_assessment.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,64 +5,73 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+from __future__ import annotations
+
 from operator import itemgetter
+from typing import Any, cast, Dict, Iterable, List, Optional, Union
 
 import trafaret as t
+from typing_extensions import Literal, Unpack
 
 from datarobot._compat import Int, String
+from datarobot.enums import AnomalyAssessmentStatus, DATA_SUBSET, SOURCE_TYPE
 from datarobot.models.api_object import APIObject
-
-from ..enums import AnomalyAssessmentStatus, SOURCE_TYPE
-from ..utils import from_api
-from ..utils.pagination import unpaginate
-from ..utils.waiters import wait_for_async_resolution
+from datarobot.models.types import (
+    AnomalyAssessmentDataPoint,
+    AnomalyAssessmentPreviewBin,
+    AnomalyAssessmentRecordMetadata,
+    RegionExplanationsData,
+)
+from datarobot.utils import from_api
+from datarobot.utils.pagination import unpaginate
+from datarobot.utils.waiters import wait_for_async_resolution
 
 DEFAULT_BATCH_SIZE = 1000
 
 RecordMetadataTrafaret = t.Dict(
     {
         t.Key("record_id"): String,
         t.Key("project_id"): String,
         t.Key("model_id"): String,
         t.Key("backtest"): t.Or(String(), Int),
-        t.Key("source"): t.Enum(*SOURCE_TYPE.ALL),
+        t.Key("source"): t.Enum(*SOURCE_TYPE.ALL),  # type: ignore[attr-defined]
         t.Key("series_id"): t.Or(String(), t.Null),
     }
 )
 
 
 class BaseAPIObject(APIObject):  # pylint: disable=missing-class-docstring
-    def __init__(self, **record_kwargs):
-        self.record_id = record_kwargs["record_id"]
-        self.project_id = record_kwargs["project_id"]
-        self.model_id = record_kwargs["model_id"]
-        self.backtest = record_kwargs["backtest"]
-        self.source = record_kwargs["source"]
-        self.series_id = record_kwargs["series_id"]
+    def __init__(self, **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata]) -> None:
+        self.record_id: str = record_kwargs["record_id"]
+        self.project_id: str = record_kwargs["project_id"]
+        self.model_id: str = record_kwargs["model_id"]
+        self.backtest: Union[str, int] = record_kwargs["backtest"]
+        self.source: Union[
+            Literal[SOURCE_TYPE.TRAINING], Literal[SOURCE_TYPE.VALIDATION]
+        ] = record_kwargs["source"]
+        self.series_id: Optional[str] = record_kwargs["series_id"]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
-            "{}(project_id={}, model_id={}, series_id={}, " "backtest={}, source={}, record_id={})"
-        ).format(
-            self.__class__.__name__,
-            self.project_id,
-            self.model_id,
-            self.series_id,
-            self.backtest,
-            self.source,
-            self.record_id,
+            f"{self.__class__.__name__}(project_id={self.project_id}, model_id={self.model_id}, "
+            f"series_id={self.series_id}, backtest={self.backtest}, source={self.source}, "
+            f"record_id={self.record_id})"
         )
 
     @classmethod
-    def from_server_data(cls, data, keep_attrs=None):
+    def from_server_data(
+        cls,
+        data: Union[Dict[str, Any], List[Dict[str, Any]]],
+        keep_attrs: Optional[Iterable[str]] = None,
+    ) -> "BaseAPIObject":
         """
         Instantiate an object of this class using the data directly from the server,
         meaning that the keys may have the wrong camel casing
 
         Parameters
         ----------
         data : dict
@@ -72,14 +81,27 @@
             List of the dotted namespace notations for attributes to keep within the
             object structure even if their values are None
         """
         case_converted = from_api(data, keep_attrs=keep_attrs, keep_null_keys=True)
         return cls.from_data(case_converted)
 
 
+PARAMS_TYPE = Dict[
+    str,
+    Union[
+        int,
+        str,
+        Literal[DATA_SUBSET.HOLDOUT],
+        Literal[SOURCE_TYPE.TRAINING],
+        Literal[SOURCE_TYPE.VALIDATION],
+        None,
+    ],
+]
+
+
 class AnomalyAssessmentRecord(BaseAPIObject):
     """Object which keeps metadata about anomaly assessment insight for the particular
     subset, backtest and series and the links to proceed to get the anomaly assessment data.
 
     .. versionadded:: v2.25
 
     Attributes
@@ -160,46 +182,48 @@
         )
         .merge(RecordMetadataTrafaret)
         .ignore_extra("*")
     )
 
     def __init__(
         self,
-        status,
-        status_details,
-        start_date,
-        end_date,
-        prediction_threshold,
-        preview_location,
-        delete_location,
-        latest_explanations_location,
-        **record_kwargs,
-    ):
+        status: AnomalyAssessmentStatus,
+        status_details: str,
+        start_date: Optional[str],
+        end_date: Optional[str],
+        prediction_threshold: Optional[float],
+        preview_location: Optional[str],
+        delete_location: str,
+        latest_explanations_location: Optional[str],
+        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
+    ) -> None:
         self.status = status
         self.status_details = status_details
         self.start_date = start_date
         self.end_date = end_date
         self.prediction_threshold = prediction_threshold
         self.preview_location = preview_location
         self.delete_location = delete_location
         self.latest_explanations_location = latest_explanations_location
         super().__init__(**record_kwargs)
 
     @classmethod
     def list(
         cls,
-        project_id,
-        model_id,
-        backtest=None,
-        source=None,
-        series_id=None,
-        limit=100,
-        offset=0,
-        with_data_only=False,
-    ):
+        project_id: str,
+        model_id: str,
+        backtest: Optional[Union[int, Literal[DATA_SUBSET.HOLDOUT]]] = None,
+        source: Optional[
+            Union[Literal[SOURCE_TYPE.TRAINING], Literal[SOURCE_TYPE.VALIDATION]]
+        ] = None,
+        series_id: Optional[str] = None,
+        limit: Optional[int] = 100,
+        offset: Optional[int] = 0,
+        with_data_only: Optional[bool] = False,
+    ) -> List["AnomalyAssessmentRecord"]:
         """Retrieve the list of the anomaly assessment records for the project and model.
         Output can be filtered and limited.
 
         Parameters
         ----------
         project_id: str
             The ID of the project record belongs to.
@@ -220,40 +244,51 @@
             no data or not supported will be omitted.
 
         Returns
         -------
         AnomalyAssessmentRecord
             The anomaly assessment record.
         """
-        params = {"limit": limit, "offset": offset}
+        params: PARAMS_TYPE = {"limit": limit, "offset": offset}
         if model_id:
             params["modelId"] = model_id
         if backtest:
             params["backtest"] = backtest
         if source:
             params["source"] = source
         if series_id:
             params["series_id"] = series_id
         url = cls._path.format(project_id=project_id)
         if limit == 0:  # unlimited results
             params["limit"] = DEFAULT_BATCH_SIZE
-            records = [
-                cls.from_server_data(entry) for entry in unpaginate(url, params, cls._client)
-            ]
+            records = cast(
+                List["AnomalyAssessmentRecord"],
+                [cls.from_server_data(entry) for entry in unpaginate(url, params, cls._client)],
+            )
         else:
             r_data = cls._client.get(url, params=params).json()
-            records = [cls.from_server_data(item) for item in r_data["data"]]
+            records = cast(
+                List["AnomalyAssessmentRecord"],
+                [cls.from_server_data(item) for item in r_data["data"]],
+            )
         if with_data_only:
             records = [
                 record for record in records if record.status == AnomalyAssessmentStatus.COMPLETED
             ]
         return records
 
     @classmethod
-    def compute(cls, project_id, model_id, backtest, source, series_id=None):
+    def compute(
+        cls,
+        project_id: str,
+        model_id: int,
+        backtest: Optional[Union[int, Literal[DATA_SUBSET.HOLDOUT]]],
+        source: Union[Literal[SOURCE_TYPE.TRAINING], Literal[SOURCE_TYPE.VALIDATION]],
+        series_id: Optional[str] = None,
+    ) -> "AnomalyAssessmentRecord":
         """Request anomaly assessment insight computation on the specified subset.
 
         Parameters
         ----------
         project_id: str
             The ID of the project to compute insight for.
         model_id: str
@@ -266,49 +301,63 @@
             The series id to compute insight for. Required for multiseries projects.
 
         Returns
         -------
         AnomalyAssessmentRecord
             The anomaly assessment record.
         """
-        payload = {"backtest": backtest, "source": source}
+        payload: Dict[str, Union[int, Literal[DATA_SUBSET.HOLDOUT], str, None]] = {
+            "backtest": backtest,
+            "source": source,
+        }
         if series_id:
             payload["series_id"] = series_id
         url = cls._create_path.format(project_id=project_id, model_id=model_id)
         response = cls._client.post(url, data=payload)
         finished_url = wait_for_async_resolution(cls._client, response.headers["Location"])
         r_data = cls._client.get(finished_url).json()
         # it ll be always one record
-        return cls.from_server_data(r_data["data"][0])
+        return cast("AnomalyAssessmentRecord", cls.from_server_data(r_data["data"][0]))
 
-    def delete(self):
+    def delete(self) -> None:
         """Delete anomaly assessment record with preview and explanations."""
         self._client.delete(self.delete_location)
 
-    def get_predictions_preview(self):
+    def get_predictions_preview(self) -> AnomalyAssessmentPredictionsPreview:
         """Retrieve aggregated predictions statistics for the anomaly assessment record.
 
         Returns
         -------
         AnomalyAssessmentPredictionsPreview
         """
         data = self._client.get(self.preview_location).json()
-        return AnomalyAssessmentPredictionsPreview.from_server_data(data)
+        return cast(
+            AnomalyAssessmentPredictionsPreview,
+            AnomalyAssessmentPredictionsPreview.from_server_data(data),
+        )
 
-    def get_latest_explanations(self):
+    def get_latest_explanations(self) -> AnomalyAssessmentExplanations:
         """Retrieve latest predictions along with shap explanations for the most anomalous records.
 
         Returns
         -------
         AnomalyAssessmentExplanations
         """
         data = self._client.get(self.latest_explanations_location).json()
-        return AnomalyAssessmentExplanations.from_server_data(data)
+        return cast(
+            AnomalyAssessmentExplanations,
+            AnomalyAssessmentExplanations.from_server_data(data),
+        )
 
-    def get_explanations(self, start_date=None, end_date=None, points_count=None):
+    def get_explanations(
+        self,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        points_count: Optional[int] = None,
+    ) -> AnomalyAssessmentExplanations:
         """Retrieve predictions along with shap explanations for the most anomalous records
         in the specified date range/for defined number of points.
         Two out of three parameters: start_date, end_date or points_count must be specified.
 
         Parameters
         ----------
         start_date: str, optional
@@ -328,15 +377,17 @@
             self.project_id,
             self.record_id,
             start_date=start_date,
             end_date=end_date,
             points_count=points_count,
         )
 
-    def get_explanations_data_in_regions(self, regions, prediction_threshold=0.0):
+    def get_explanations_data_in_regions(
+        self, regions: List[AnomalyAssessmentPreviewBin], prediction_threshold: float = 0.0
+    ) -> RegionExplanationsData:
         """Get predictions along with explanations for the specified regions, sorted by
         predictions in descending order.
 
         Parameters
         ----------
         regions: list of preview_bins
             For each region explanations will be retrieved and merged.
@@ -344,26 +395,29 @@
             If specified, only points with score greater or equal to the threshold will be returned.
 
         Returns
         -------
         dict in a form of {'explanations': explanations, 'shap_base_value': shap_base_value}
 
         """
-        explanations = []
-        shap_base_value = None
+        explanations: List[AnomalyAssessmentDataPoint] = []
+        shap_base_value: Optional[float] = None
         for region in regions:
             response = self.get_explanations(
                 start_date=region["start_date"], end_date=region["end_date"]
             )
             shap_base_value = response.shap_base_value
             for item in response.data:
                 if item["prediction"] >= prediction_threshold:
                     explanations.append(item)
         explanations = list(sorted(explanations, key=itemgetter("prediction"), reverse=True))
-        return {"explanations": explanations, "shap_base_value": shap_base_value}
+        return cast(
+            RegionExplanationsData,
+            {"explanations": explanations, "shap_base_value": shap_base_value},
+        )
 
 
 class AnomalyAssessmentPredictionsPreview(BaseAPIObject):
     """Aggregated predictions over time for the corresponding anomaly assessment record.
     Intended to find the bins with highest anomaly scores.
 
     .. versionadded:: v2.25
@@ -440,22 +494,28 @@
                 t.Key("preview_bins"): t.List(PreviewBinTrafaret),
             }
         )
         .merge(RecordMetadataTrafaret)
         .ignore_extra("*")
     )
 
-    def __init__(self, start_date, end_date, preview_bins, **record_kwargs):
+    def __init__(
+        self,
+        start_date: str,
+        end_date: str,
+        preview_bins: List[AnomalyAssessmentPreviewBin],
+        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
+    ) -> None:
         self.preview_bins = preview_bins
         self.start_date = start_date
         self.end_date = end_date
         super().__init__(**record_kwargs)
 
     @classmethod
-    def get(cls, project_id, record_id):
+    def get(cls, project_id: str, record_id: str) -> "AnomalyAssessmentPredictionsPreview":
         """Retrieve aggregated predictions over time.
 
         Parameters
         ----------
         project_id: str
             The ID of the project.
         record_id: str
@@ -464,17 +524,19 @@
         Returns
         -------
         AnomalyAssessmentPredictionsPreview
 
         """
         url = cls._path.format(project_id=project_id, record_id=record_id)
         r_data = cls._client.get(url).json()
-        return cls.from_server_data(r_data)
+        return cast("AnomalyAssessmentPredictionsPreview", cls.from_server_data(r_data))
 
-    def find_anomalous_regions(self, max_prediction_threshold=0.0):
+    def find_anomalous_regions(
+        self, max_prediction_threshold: float = 0.0
+    ) -> List[AnomalyAssessmentPreviewBin]:
         """Sort preview bins by max_predicted value and select those with max predicted value
          greater or equal to max prediction threshold.
          Sort the result by max predicted value in descending order.
 
         Parameters
         ----------
         max_prediction_threshold: float, optional
@@ -484,15 +546,17 @@
         -------
         preview_bins: list of preview_bin
             Filtered and sorted preview bins
 
         """
         no_empty_bins = [bin for bin in self.preview_bins if bin["frequency"]]
         filtered_bins = [
-            bin for bin in no_empty_bins if bin["max_predicted"] >= max_prediction_threshold
+            bin
+            for bin in no_empty_bins
+            if cast(float, bin["max_predicted"]) >= max_prediction_threshold
         ]
         sorted_bins = list(sorted(filtered_bins, key=itemgetter("max_predicted"), reverse=True))
         return sorted_bins
 
 
 class AnomalyAssessmentExplanations(BaseAPIObject):
     """Object which keeps predictions along with shap explanations for the most anomalous records
@@ -586,24 +650,39 @@
                 t.Key("end_date"): t.Or(String(), t.Null),
             }
         )
         .merge(RecordMetadataTrafaret)
         .ignore_extra("*")
     )
 
-    def __init__(self, shap_base_value, data, start_date, end_date, count, **record_kwargs):
+    def __init__(
+        self,
+        shap_base_value: float,
+        data: List[AnomalyAssessmentDataPoint],
+        start_date: Optional[str],
+        end_date: Optional[str],
+        count: int,
+        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
+    ) -> None:
         self.shap_base_value = shap_base_value
         self.data = data
         self.count = count
         self.start_date = start_date
         self.end_date = end_date
         super().__init__(**record_kwargs)
 
     @classmethod
-    def get(cls, project_id, record_id, start_date=None, end_date=None, points_count=None):
+    def get(
+        cls,
+        project_id: str,
+        record_id: str,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        points_count: Optional[int] = None,
+    ) -> "AnomalyAssessmentExplanations":
         """Retrieve predictions along with shap explanations for the most anomalous records
         in the specified date range/for defined number of points.
         Two out of three parameters: start_date, end_date or points_count must be specified.
 
         Parameters
         ----------
         project_id: str
@@ -621,18 +700,18 @@
 
 
         Returns
         -------
         AnomalyAssessmentExplanations
 
         """
-        params = {}
+        params: Dict[str, Union[str, int]] = {}
         if start_date:
             params["startDate"] = start_date
         if end_date:
             params["endDate"] = end_date
         if points_count:
             params["pointsCount"] = points_count
 
         url = cls._path.format(project_id=project_id, record_id=record_id)
         r_data = cls._client.get(url, params=params).json()
-        return cls.from_server_data(r_data)
+        return cast("AnomalyAssessmentExplanations", cls.from_server_data(r_data))
```

### Comparing `datarobot-3.1.1/datarobot/models/api_object.py` & `datarobot-3.2.0b0/datarobot/models/api_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,16 +41,21 @@
             Correctly snake_cased keys and their values.
         """
         checked = cls._converter.check(data)
         safe_data = cls._filter_data(checked)
         return cls(**safe_data)
 
     @classmethod
-    def from_location(cls: Type[T], path: str, keep_attrs: Optional[List[str]] = None) -> T:
-        server_data = cls._server_data(path)
+    def from_location(
+        cls: Type[T],
+        path: str,
+        keep_attrs: Optional[List[str]] = None,
+        params: Optional[Dict] = None,
+    ) -> T:
+        server_data = cls._server_data(path, params=params)
         return cls.from_server_data(server_data, keep_attrs=keep_attrs)
 
     @classmethod
     def from_server_data(
         cls: Type[T],
         data: ServerDataType,
         keep_attrs: Optional[Iterable[str]] = None,
@@ -77,9 +82,9 @@
         return {key: value for key, value in data.items() if key in fields}
 
     @classmethod
     def _safe_data(cls, data, do_recursive=False):
         return cls._filter_data(cls._converter.check(from_api(data, do_recursive=do_recursive)))
 
     @classmethod
-    def _server_data(cls, path: str) -> ServerDataType:
-        return cls._client.get(path).json()
+    def _server_data(cls, path: str, params: Optional[Dict] = None) -> ServerDataType:
+        return cls._client.get(path, params=params).json()
```

### Comparing `datarobot-3.1.1/datarobot/models/automated_documentation.py` & `datarobot-3.2.0b0/datarobot/models/automated_documentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,34 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from requests.models import Response
+from __future__ import annotations
+
+from datetime import datetime
+from typing import cast, List, Optional, Tuple
+
+from requests import Response
 import trafaret as t
+from typing_extensions import TypedDict
 
 from datarobot._compat import String
+from datarobot.enums import DEFAULT_MAX_WAIT, DocumentType, Locales
 from datarobot.models.api_object import APIObject
 from datarobot.utils import camelize, from_api, get_id_from_location, parse_time
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
-from ..enums import DEFAULT_MAX_WAIT
+
+class DocumentOption(TypedDict):
+    document_type: DocumentType
+    locale: Locales
 
 
 class AutomatedDocument(APIObject):
     """
     An :ref:`automated documentation <automated_documentation_overview>` object.
 
     .. versionadded:: v2.24
@@ -70,34 +80,34 @@
             t.Key("document_type"): String(),
             t.Key("template_id", optional=True): t.Or(String(), t.Null()),
         }
     ).allow_extra("*")
 
     def __init__(
         self,
-        entity_id=None,
-        document_type=None,
-        output_format=None,
-        locale=None,
-        template_id=None,
-        id=None,
-        filepath=None,
-        created_at=None,
-    ):
+        entity_id: Optional[str] = None,
+        document_type: Optional[str] = None,
+        output_format: Optional[str] = None,
+        locale: Optional[str] = None,
+        template_id: Optional[str] = None,
+        id: Optional[str] = None,
+        filepath: Optional[str] = None,
+        created_at: Optional[datetime] = None,
+    ) -> None:
         self.entity_id = entity_id
         self.document_type = document_type
         self.output_format = output_format
         self.locale = locale
         self.template_id = template_id
         self.id = id
         self.filepath = filepath
         self.created_at = created_at
 
     @classmethod
-    def list_available_document_types(cls):
+    def list_available_document_types(cls) -> List[DocumentOption]:
         """
         Get a list of all available document types and locales.
 
         Returns
         -------
         List of dicts
 
@@ -109,33 +119,33 @@
 
             dr.Client(token=my_token, endpoint=endpoint)
             doc_types = dr.AutomatedDocument.list_available_document_types()
 
         """
 
         response = cls._client.get("automatedDocumentOptions/")
-        return from_api(response.json())
+        return cast(List[DocumentOption], from_api(response.json()))
 
     @property
-    def is_model_compliance_initialized(self):
+    def is_model_compliance_initialized(self) -> Tuple[bool, str]:
         """Check if model compliance documentation pre-processing is initialized.
         Model compliance documentation pre-processing must be initialized before
         generating documentation for a custom model.
 
         Returns
         -------
         Tuple of (boolean, string)
             - `boolean` flag is whether model compliance documentation pre-processing is initialized
             - `string` value is the initialization status
         """
         return self._model_compliance_initialization_status(
             f"{self._model_compliance_initialization_path}{self.entity_id}/"
         )
 
-    def initialize_model_compliance(self):
+    def initialize_model_compliance(self) -> Tuple[bool, str]:
         """Initialize model compliance documentation pre-processing.
         Must be called before generating documentation for a custom model.
 
         Returns
         -------
         Tuple of (boolean, string)
             - `boolean` flag is whether model compliance documentation pre-processing is initialized
@@ -170,15 +180,15 @@
         """Request generation of an automated document.
 
         Required attributes to request document generation: ``document_type``, ``entity_id``,
         and ``output_format``.
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
 
         Examples
         --------
         .. code-block:: python
 
             import datarobot as dr
 
@@ -208,24 +218,24 @@
 
         response = self._client.post(self._path, data=payload)
         location = wait_for_async_resolution(
             self._client, response.headers["Location"], max_wait=max_wait
         )
         self.id = get_id_from_location(location)
 
-        return response
+        return cast(Response, response)
 
-    def download(self):
+    def download(self) -> Response:
         """
         Download a generated Automated Document.
         Document ID is required to download a file.
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
 
         Examples
         --------
 
         Generating and downloading the generated document:
 
         .. code-block:: python
@@ -277,27 +287,27 @@
                 "Document ID not provided. Assign it to AutomatedDocument object `id` attribute."
             )
         response = self._client.get(f"{self._path}{self.id}/", stream=True)
 
         if not self.filepath:
             self.filepath = response.headers["Content-Disposition"].split("=")[-1]
 
-        with open(self.filepath, mode="wb") as f:
+        with open(cast(str, self.filepath), mode="wb") as f:
             for chunk in response.iter_content(chunk_size=1024 * 1024):
                 f.write(chunk)
 
-        return response
+        return cast(Response, response)
 
-    def delete(self):
+    def delete(self) -> Response:
         """
         Delete a document using its ID.
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
 
         Examples
         --------
 
         .. code-block:: python
 
             import datarobot as dr
@@ -313,26 +323,26 @@
         """
         if not self.id:
             raise AttributeError(
                 "Provide Document ID to delete a document."
                 "Assign it to AutomatedDocument object `id` attribute or pass to class constructor."
             )
 
-        return self._client.delete(f"{self._path}{self.id}/")
+        return cast(Response, self._client.delete(f"{self._path}{self.id}/"))
 
     @classmethod
     def list_generated_documents(
         cls,
-        document_types=None,
-        entity_ids=None,
-        output_formats=None,
-        locales=None,
-        offset=None,
-        limit=None,
-    ):
+        document_types: Optional[List[str]] = None,
+        entity_ids: Optional[List[str]] = None,
+        output_formats: Optional[List[str]] = None,
+        locales: Optional[List[str]] = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> List["AutomatedDocument"]:
         """
         Get information about all previously generated documents available for your account. The
         information includes document ID and type, ID of the entity it was generated for, time of
         creation, and other information.
 
         Parameters
         ----------
@@ -430,15 +440,15 @@
             return [
                 cls.from_server_data(item) for item in unpaginate(cls._path, params, cls._client)
             ]
 
         items = cls._client.get(cls._path, params=params).json()["data"]
         return [cls.from_server_data(item) for item in items]
 
-    def _model_compliance_initialization_status(self, location):
+    def _model_compliance_initialization_status(self, location: str) -> Tuple[bool, str]:
         response = self._client.get(location)
         data = response.json()
         return data["initialized"], data["status"]
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         attrs = ", ".join(item[0] + "=" + str(item[1]) for item in self.__dict__.items())
         return f"{self.__class__.__name__}({attrs})"
```

### Comparing `datarobot-3.1.1/datarobot/models/batch_prediction_job.py` & `datarobot-3.2.0b0/datarobot/models/batch_prediction_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 
 import csv
 import datetime
 import io
 import os
 import threading
 import time
-from typing import cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
+from typing import Any, cast, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 
 import pandas as pd
 import requests
 import trafaret as t
 
 from datarobot import errors
 from datarobot._compat import Int, String
 from datarobot.models.credential import Credential
 from datarobot.models.dataset import Dataset
 from datarobot.models.job import AbstractSpecificJob
 from datarobot.models.prediction_explanations import PredictionExplanationsMode
 from datarobot.models.project import Project
-from datarobot.utils import get_id_from_response, pagination, recognize_sourcedata, to_api
+from datarobot.utils import get_id_from_response, pagination
+from datarobot.utils import recognize_sourcedata as orig_recognize_sourcedata
+from datarobot.utils import to_api
 
 from ..enums import AVAILABLE_STATEMENT_TYPES, DEFAULT_TIMEOUT, JOB_TYPE, QUEUE_STATUS
 from ..utils import logger, parse_time
 from .api_object import APIObject
 
 LOG = logger.get_logger(__name__)
 
@@ -100,14 +102,31 @@
         day_of_week: List[Union[int, str]]
         month: List[Union[int, str]]
         hour: List[Union[int, str]]
         minute: List[Union[int, str]]
         day_of_month: List[Union[int, str]]
 
 
+def recognize_sourcedata(sourcedata: Any, default_fname: str) -> Dict[str, Any]:
+    """Override the default recognize_sourcedata with one that converts
+    DataFrame to io.BytesIO"""
+    if not isinstance(sourcedata, pd.DataFrame):
+        return orig_recognize_sourcedata(sourcedata, default_fname)
+    # The original recognize_sourcedata will encode dataframes into StringIO
+    # To pass this to requests.put, we need BytesIO - otherwise, requests will
+    # try to encode it using latin-1 encoding (the default HTTP encoding),
+    # which will crash when a charater not contained in latin-1 is used
+    #
+    # https://github.com/python/cpython/blob/b9797417315cc2d1700cb2d427685016d3380711/Lib/http/client.py#L1046
+    buf = io.BytesIO()
+    sourcedata.to_csv(buf, encoding="utf-8", index=False, quoting=csv.QUOTE_ALL)
+    buf.seek(0)
+    return {"filelike": buf, "fname": default_fname}
+
+
 class BatchPredictionJob(AbstractSpecificJob):
     """
     A Batch Prediction Job is used to score large data sets on
     prediction servers using the Batch Prediction API.
 
     Attributes
     ----------
@@ -1564,16 +1583,17 @@
         return batch_job
 
     def download(self, fileobj, timeout: int = 120, read_timeout: int = 660) -> None:
         """Downloads the CSV result of a prediction job
 
         Attributes
         ----------
-        fileobj: file-like object
-            Write CSV data to this file-like object
+        fileobj: A file-like object where the CSV prediction results will be
+            written to. Examples include an in-memory buffer
+            (e.g., io.BytesIO) or a file on disk (opened for binary writing).
 
         timeout : int (optional, default 120)
             .. versionadded:: 2.22
 
             Seconds to wait for the download to become available.
 
             The download will not be available before the job has started processing.
```

### Comparing `datarobot-3.1.1/datarobot/models/blueprint.py` & `datarobot-3.2.0b0/datarobot/models/blueprint.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,20 @@
         name: str
         url: str
 
     class ReferenceType(TypedDict):
         name: str
         url: Optional[str]
 
+    BlueprintInput = List[str]
+    BlueprintTask = List[str]
+    BlueprintTaskType = str
+    BlueprintStage = Tuple[BlueprintInput, BlueprintTask, BlueprintTaskType]
+    BlueprintJson = Dict[str, BlueprintStage]
+
 
 class BlueprintTaskDocument(APIObject):
     """Document describing a task from a blueprint.
 
     Attributes
     ----------
     title : str
@@ -287,14 +293,26 @@
         -------
         blueprint : Blueprint
             The queried blueprint.
         """
         url = f"projects/{project_id}/blueprints/{blueprint_id}/"
         return cls.from_location(url)
 
+    def get_json(self) -> BlueprintJson:
+        """Get the blueprint json representation used by this model.
+
+        Returns
+        -------
+        BlueprintJson
+            Json representation of the blueprint stages.
+        """
+        url = f"projects/{self.project_id}/blueprints/{self.id}/json/"
+        response_json = self._client.get(url).json()
+        return cast("BlueprintJson", response_json.get("blueprint"))
+
     def get_chart(self) -> BlueprintChart:
         """Retrieve a chart.
 
         Returns
         -------
         BlueprintChart
             The current blueprint chart.
```

### Comparing `datarobot-3.1.1/datarobot/models/calendar_file.py` & `datarobot-3.2.0b0/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/change_request.py` & `datarobot-3.2.0b0/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/cluster.py` & `datarobot-3.2.0b0/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/cluster_insight.py` & `datarobot-3.2.0b0/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/compliance_doc_template.py` & `datarobot-3.2.0b0/datarobot/models/compliance_doc_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+from __future__ import annotations
+
 from functools import partial
 import json
+from typing import cast, Dict, List, Optional, Union
 
 import trafaret as t
+from typing_extensions import TypedDict
 
 from datarobot._compat import String
+from datarobot.enums import ComplianceDocTemplateType, ComplianceDocType
 from datarobot.models.api_object import APIObject
 
 # Make sure validator stays insync with main repo
 OptKey = partial(t.Key, optional=True)
 TitleString = String(max_length=500)
 SectionDict = t.Forward()
 SectionDict.provide(
@@ -70,22 +75,62 @@
         t.Dict(
             {"type": t.Atom("table_of_contents"), "title": TitleString, OptKey("locked"): t.Bool}
         ),
     )
 )
 
 
-def make_url(root, template_id):
+class Instructions(TypedDict):
+    owner: str
+    user: str
+
+
+class Section(TypedDict):
+    title: str
+    type: ComplianceDocType
+    locked: bool
+
+
+class DataRobotSection(Section):
+    content_id: str
+    sections: Optional[List["Section"]]
+    description: Optional[str]
+    instructions: Optional[Instructions]
+
+
+class UserSection(Section):
+    regular_test: str
+    highlighted_test: str
+    sections: Optional[List["Section"]]
+    description: Optional[str]
+    instructions: Optional[Instructions]
+
+
+class CustomSection(Section):
+    regular_test: str
+    highlighted_test: str
+    sections: Optional[List["Section"]]
+    description: Optional[str]
+    instructions: Optional[Instructions]
+
+
+class TableOfContentsSection(Section):
+    """
+    Table of Contents Sections only have the base fields available to all Section classes
+    """
+
+
+def make_url(root: str, template_id: str) -> str:
     return f"{root}{template_id}/"
 
 
-def load_sections_from_path(path):
+def load_sections_from_path(path: str) -> List[Section]:
     with open(path) as f:  # pylint: disable=unspecified-encoding
         sections = json.loads(f.read())
-        return sections
+        return cast(List[Section], sections)
 
 
 class ComplianceDocTemplate(APIObject):
     """A :ref:`compliance documentation template <automated_documentation_overview>`. Templates
     are used to customize contents of :class:`AutomatedDocument
     <datarobot.models.automated_documentation.AutomatedDocument>`.
 
@@ -147,27 +192,37 @@
             t.Key("creator_username"): String(),
             OptKey("org_id"): t.Or(String(), t.Null),
             t.Key("name"): String(),
             OptKey("sections"): t.Or(t.List(SectionDict), t.Null),
         }
     ).allow_extra("*")
 
-    def __init__(self, id, creator_id, creator_username, name, org_id=None, sections=None):
+    def __init__(
+        self,
+        id: str,
+        creator_id: str,
+        creator_username: str,
+        name: str,
+        org_id: Optional[str] = None,
+        sections: Optional[List[Section]] = None,
+    ):
         self.id = id
         self.creator_id = creator_id
         self.creator_username = creator_username
         self.org_id = org_id
         self.name = name
         self.sections = sections
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"ComplianceDocTemplate({self.name!r})"
 
     @classmethod
-    def get_default(cls, template_type=None):
+    def get_default(
+        cls, template_type: Optional[ComplianceDocTemplateType] = None
+    ) -> "ComplianceDocTemplate":
         """Get a default DataRobot template. This template is used for generating
         compliance documentation when no template is specified.
 
 
         Parameters
         ----------
         template_type : str or None
@@ -177,24 +232,24 @@
         -------
         template : ComplianceDocTemplate
             the default template object with ``sections`` attribute populated with default sections.
         """
         query_params = {"type": template_type} if template_type else None
         response = cls._client.get("complianceDocTemplates/default/", params=query_params)
         return cls(
-            id=None,
-            creator_id=None,
-            creator_username=None,
+            id=cast(str, None),
+            creator_id=cast(str, None),
+            creator_username=cast(str, None),
             org_id=None,
             name="default",
             sections=response.json()["sections"],
         )
 
     @classmethod
-    def create_from_json_file(cls, name, path):
+    def create_from_json_file(cls, name: str, path: str) -> "ComplianceDocTemplate":
         """Create a template with the specified name and sections in a JSON file.
 
         This is useful when working with sections in a JSON file. Example:
 
         .. code-block:: python
 
             default_template = ComplianceDocTemplate.get_default()
@@ -219,15 +274,15 @@
         """
         resp = cls._client.post(
             cls._root_path, data={"name": name, "sections": load_sections_from_path(path)}
         )
         return cls.from_location(resp.headers["Location"])
 
     @classmethod
-    def create(cls, name, sections):
+    def create(cls, name: str, sections: List[Section]) -> "ComplianceDocTemplate":
         """Create a template with the specified name and sections.
 
         Parameters
         ----------
         name : str
             the name of the template. Must be unique for your user.
         sections : list
@@ -238,15 +293,15 @@
         template : ComplianceDocTemplate
             the created template
         """
         resp = cls._client.post(cls._root_path, data={"name": name, "sections": sections})
         return cls.from_location(resp.headers["Location"])
 
     @classmethod
-    def get(cls, template_id):
+    def get(cls, template_id: str) -> "ComplianceDocTemplate":
         """Retrieve a specific template.
 
         Parameters
         ----------
         template_id :  str
             the id of the template to retrieve
 
@@ -254,15 +309,20 @@
         -------
         template : ComplianceDocTemplate
             the retrieved template
         """
         return cls.from_location(make_url(cls._root_path, template_id))
 
     @classmethod
-    def list(cls, name_part=None, limit=None, offset=None):
+    def list(
+        cls,
+        name_part: Optional[str] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> List["ComplianceDocTemplate"]:
         """Get a paginated list of compliance documentation template objects.
 
         Parameters
         ----------
         name_part : str or None
             Return only the templates with names matching specified string. The matching is
             case-insensitive.
@@ -276,50 +336,52 @@
         -------
         templates : list of ComplianceDocTemplate
             the list of template objects
         """
         r_data = cls._client.get(
             cls._root_path, params={"limit": limit, "offset": offset, "namePart": name_part}
         ).json()
-        return [cls.from_server_data(item) for item in r_data["data"]]
+        return cast(
+            List["ComplianceDocTemplate"], [cls.from_server_data(item) for item in r_data["data"]]
+        )
 
-    def sections_to_json_file(self, path, indent=2):
+    def sections_to_json_file(self, path: str, indent: int = 2) -> None:
         """Save sections of the template to a json file at the specified path
 
         Parameters
         ----------
         path : str
             the path to save the file to
         indent : int
             indentation to use in the json file.
         """
         with open(path, "w") as f:  # pylint: disable=unspecified-encoding
             f.write(json.dumps(self.sections, indent=indent))
 
-    def update(self, name=None, sections=None):
+    def update(self, name: Optional[str] = None, sections: Optional[List[Section]] = None) -> None:
         """Update the name or sections of an existing doc template.
 
         Note that default or non-existent templates can not be updated.
 
         Parameters
         ----------
         name : str, optional
             the new name for the template
         sections : list of dicts
             list of sections
         """
-        payload = {}
+        payload: Dict[str, Union[str, List[Section]]] = {}
         if name is not None:
             payload["name"] = name
         if sections is not None:
             payload["sections"] = sections
 
         self._client.patch(make_url(self._root_path, self.id), data=payload)
 
         if name is not None:
             self.name = name
         if sections is not None:
             self.sections = sections
 
-    def delete(self):
+    def delete(self) -> None:
         """Delete the compliance documentation template."""
         self._client.delete(make_url(self._root_path, self.id))
```

### Comparing `datarobot-3.1.1/datarobot/models/confusion_chart.py` & `datarobot-3.2.0b0/datarobot/models/confusion_chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+from typing import List
+
 import trafaret as t
+from typing_extensions import TypedDict
 
 from datarobot._compat import Int, String
+from datarobot.enums import CHART_DATA_SOURCE
 from datarobot.models.api_object import APIObject
 
 _PercentageFloat = t.Float(gte=0, lte=1)  # 0.0 <= x <= 1.0
 
 _ClassPercentage = t.Dict(
     {t.Key("other_class_name"): String, t.Key("percentage"): _PercentageFloat}
 ).ignore_extra("*")
@@ -43,14 +47,37 @@
         # NxN confusion matrix
         t.Key("confusion_matrix"): t.List(t.List(Int)),
         t.Key("class_metrics"): t.List(_ClassMetrics),
     }
 ).ignore_extra("*")
 
 
+class ClassPercentage(TypedDict):
+    other_class_name: str
+    percentage: float
+
+
+class ClassMetric(TypedDict):
+    class_name: str
+    actual_count: int
+    predicted_count: int
+    f1: float
+    recall: float
+    precision: float
+    confusion_matrix_one_vs_all: List[List[int]]
+    was_actual_percentages: List[ClassPercentage]
+    was_predicted_percentages: List[ClassPercentage]
+
+
+class ConfusionChartRawData(TypedDict):
+    class_metrics: List[ClassMetric]
+    confusion_matrix: List[List[int]]
+    classes: List[str]
+
+
 class ConfusionChart(APIObject):
     """ Confusion Chart data for model.
 
     Notes
     -----
     ``ClassMetrics`` is a dict containing the following:
 
@@ -101,17 +128,19 @@
             t.Key("source"): String,
             t.Key("source_model_id"): String,
         }
     ).ignore_extra("*")
 
     _converter = ConfusionChartWrapper
 
-    def __init__(self, source, data, source_model_id):
+    def __init__(
+        self, source: CHART_DATA_SOURCE, data: ConfusionChartRawData, source_model_id: str
+    ):
         self.source = source
         self.raw_data = data
         self.class_metrics = data["class_metrics"]
         self.confusion_matrix = data["confusion_matrix"]
         self.classes = data["classes"]
         self.source_model_id = source_model_id
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"ConfusionChart({self.source})"
```

### Comparing `datarobot-3.1.1/datarobot/models/connector.py` & `datarobot-3.2.0b0/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/credential.py` & `datarobot-3.2.0b0/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/custom_model.py` & `datarobot-3.2.0b0/datarobot/models/custom_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,35 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+from __future__ import annotations
+
+from typing import Any, cast, Dict, List, Optional, Type, TypeVar
+
 import trafaret as t
 
 from datarobot._compat import Int, String
-from datarobot.enums import CUSTOM_MODEL_TARGET_TYPE, DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
+from datarobot.enums import (
+    CUSTOM_MODEL_TARGET_TYPE,
+    DEFAULT_MAX_WAIT,
+    NETWORK_EGRESS_POLICY,
+    TARGET_TYPE,
+)
 from datarobot.errors import ClientError
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model_version import CustomModelVersion
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
+T_CustomModelBase = TypeVar("T_CustomModelBase", bound="_CustomModelBase")
+
 
 class _CustomModelBase(APIObject):  # pylint: disable=missing-class-docstring
     _path = "customModels/"
 
     _converter = t.Dict(
         {
             t.Key("id"): String(),
@@ -37,34 +48,34 @@
             t.Key("created_by"): String(),
             t.Key("updated") >> "updated_at": String(),
             t.Key("created") >> "created_at": String(),
             t.Key("target_type", optional=True, default=None): String(),
         }
     ).ignore_extra("*")
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.name or self.id!r})"
 
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
-        id,
-        name,
-        description,
-        supports_binary_classification,
-        supports_regression,
-        latest_version,
-        deployments_count,
-        created_by,
-        updated_at,
-        created_at,
-        target_type,
-    ):
+        id: str,
+        name: str,
+        description: str,
+        supports_binary_classification: bool,
+        supports_regression: bool,
+        latest_version: CustomModelVersion,
+        deployments_count: int,
+        created_by: str,
+        updated_at: str,
+        created_at: str,
+        target_type: str,
+    ) -> None:
         self.id = id
         self.name = name
         self.description = description
 
         self.target_type = target_type
         if supports_binary_classification and supports_regression:
             raise ValueError("Model should support only 1 target type")
@@ -84,56 +95,168 @@
                 )
             elif target_type != CUSTOM_MODEL_TARGET_TYPE.REGRESSION and supports_regression:
                 raise ValueError(
                     "Cannot specify both target_type {} and "
                     "supports_regression.".format(target_type)
                 )
 
-        self.latest_version = CustomModelVersion(**latest_version) if latest_version else None
+        self.latest_version = CustomModelVersion(**latest_version) if latest_version else None  # type: ignore[arg-type]
         self.deployments_count = deployments_count
         self.created_by = created_by
         self.updated_at = updated_at
         self.created_at = created_at
 
     @classmethod
-    def _check_model_type(cls, data):
-        return data["customModelType"] == cls._model_type
+    def _check_model_type(cls, data: Dict[str, Any]) -> bool:
+        return cast(bool, data["customModelType"] == cls._model_type)  # type: ignore[attr-defined]
 
     @classmethod
-    def list(cls, is_deployed=None, order_by=None, search_for=None):
+    def list(  # pylint: disable=missing-function-docstring
+        cls: Type[T_CustomModelBase],
+        is_deployed: Optional[bool] = None,
+        order_by: Optional[str] = None,
+        search_for: Optional[str] = None,
+    ) -> List[T_CustomModelBase]:
+        """List instances of _CustomModelBase.
+
+        .. versionadded:: v2.21
+
+        Parameters
+        ----------
+        is_deployed: bool, optional
+            Flag for filtering custom inference models.
+            If set to `True`, only deployed custom inference models are returned.
+            If set to `False`, only not deployed custom inference models are returned.
+        search_for: str, optional
+            String for filtering custom inference models - only custom.
+            inference models that contain the string in name or description will
+            be returned.
+            If not specified, all custom models will be returned.
+        order_by: str, optional
+            Property to sort custom inference models by.
+            Supported properties are "created" and "updated".
+            Prefix the attribute name with a dash to sort in descending order,
+            e.g. order_by='-created'.
+            By default, the order_by parameter is None which will result in
+            custom models being returned in order of creation time descending
+
+        Returns
+        -------
+        List[T_CustomModelBase]
+            A list of instances of _CustomModelBase.
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
+        """
         payload = {
-            "custom_model_type": cls._model_type,
+            "custom_model_type": cls._model_type,  # type: ignore[attr-defined]
             "is_deployed": is_deployed,
             "order_by": order_by,
             "search_for": search_for,
         }
         data = unpaginate(cls._path, payload, cls._client)
         return [cls.from_server_data(item) for item in data]
 
     @classmethod
-    def get(cls, custom_model_id):
+    def get(cls: Type[T_CustomModelBase], custom_model_id: str) -> T_CustomModelBase:
+        """Get custom inference model by id.
+
+        .. versionadded:: v2.21
+
+        Parameters
+        ----------
+        custom_model_id: str
+            ID of the _CustomModelBase.
+
+        Returns
+        -------
+        T_CustomModelBase
+            Retrieved instance of _CustomModelBase
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
+        """
         path = f"{cls._path}{custom_model_id}/"
         data = cls._client.get(path).json()
         if not cls._check_model_type(data):
-            raise Exception(f"Requested model is not a {cls._model_type} model")
+            raise Exception(f"Requested model is not a {cls._model_type} model")  # type: ignore[attr-defined]
         return cls.from_server_data(data)
 
-    def download_latest_version(self, file_path):
+    def download_latest_version(self, file_path: str) -> None:
+        """Download the latest custom inference model version.
+
+        .. versionadded:: v2.21
+
+        Parameters
+        ----------
+        file_path: str
+            Path to create a file with custom model version content.
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
+        """
         path = f"{self._path}{self.id}/download/"
 
         response = self._client.get(path)
         with open(file_path, "wb") as f:
             f.write(response.content)
 
     @classmethod
     def create(
-        cls, name, target_type, description=None, **kwargs
-    ):  # pylint: disable=missing-function-docstring
+        cls: Type[T_CustomModelBase],
+        name: str,
+        target_type: TARGET_TYPE,
+        description: Optional[str] = None,
+        **kwargs: Any,
+    ) -> T_CustomModelBase:
+        """Create a custom inference model.
+
+        .. versionadded:: v2.21
+
+        Parameters
+        ----------
+        name: str
+            The name of the custom inference model.
+        target_type: datarobot.TARGET_TYPE
+            The target type of the custom inference model.
+            Values: [`datarobot.TARGET_TYPE.BINARY`, `datarobot.TARGET_TYPE.REGRESSION`,
+            `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`,
+            `datarobot.TARGET_TYPE.ANOMALY`]
+        description: str, optional
+            The description of the custom inference model.
+
+        Returns
+        -------
+        CustomModelVersion
+            Created instance of _CustomModelBase.
+
+        Raises
+        ------
+            datarobot.errors.ClientError
+                If the server responded with 4xx status.
+            datarobot.errors.ServerError
+                If the server responded with 5xx status.
+        """
         payload = dict(
-            custom_model_type=cls._model_type, name=name, description=description, **kwargs
+            custom_model_type=cls._model_type,  # type: ignore[attr-defined]
+            name=name,
+            description=description,
+            **kwargs,
         )
         if target_type in CUSTOM_MODEL_TARGET_TYPE.ALL:
             payload["target_type"] = target_type
 
         # this will be removed when these params are fully deprecated
         if target_type == CUSTOM_MODEL_TARGET_TYPE.BINARY:
             payload["supports_binary_classification"] = True
@@ -148,107 +271,172 @@
             )
 
         response = cls._client.post(cls._path, data=payload)
         return cls.from_server_data(response.json())
 
     @classmethod
     def copy_custom_model(
-        cls,
-        custom_model_id,
-    ):
+        cls: Type[T_CustomModelBase],
+        custom_model_id: str,
+    ) -> T_CustomModelBase:
+        """Create a custom inference model by copying existing one.
+
+        .. versionadded:: v2.21
+
+        Parameters
+        ----------
+        custom_model_id: str
+            id of the custom inference model to copy
+
+        Returns
+        -------
+        T_CustomModelBase
+            Created a custom inference model.
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
+        """
         path = f"{cls._path}fromCustomModel/"
         response = cls._client.post(path, data={"custom_model_id": custom_model_id})
         return cls.from_server_data(response.json())
 
-    def update(self, name=None, description=None, **kwargs):
+    def update(
+        self, name: Optional[str] = None, description: Optional[str] = None, **kwargs: Any
+    ) -> None:
+        """Update custom inference model properties.
+
+        .. versionadded:: v2.21
+
+        Parameters
+        ----------
+        name: str, optional
+            New custom model name.
+        description: str, optional
+            New custom model description.
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
+        """
         payload = dict(name=name, description=description, **kwargs)
         url = f"{self._path}{self.id}/"
         response = self._client.patch(url, data=payload)
 
         data = response.json()
-        self._set_values(**self._safe_data(data, do_recursive=True))
+        self._set_values(**self._safe_data(data, do_recursive=True))  # type: ignore[no-untyped-call]
+
+    def refresh(self) -> None:
+        """Update custom inference model with the latest data from server.
+
+        .. versionadded:: v2.21
 
-    def refresh(self):
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
+        """
         url = self._path.format(self.id)
         path = f"{url}{self.id}/"
 
         response = self._client.get(path)
 
         data = response.json()
-        self._set_values(**self._safe_data(data, do_recursive=True))
+        self._set_values(**self._safe_data(data, do_recursive=True))  # type: ignore[no-untyped-call]
 
-    def delete(self):
+    def delete(self) -> None:
+        """Delete custom inference model.
+
+        .. versionadded:: v2.21
+
+        Raises
+        ------
+        datarobot.errors.ClientError
+            If the server responded with 4xx status.
+        datarobot.errors.ServerError
+            If the server responded with 5xx status.
+        """
         url = f"{self._path}{self.id}/"
         self._client.delete(url)
 
 
 class CustomInferenceModel(_CustomModelBase):
     """A custom inference model.
 
     .. versionadded:: v2.21
 
     Attributes
     ----------
     id: str
-        id of the custom model
+        The ID of the custom model.
     name: str
-        name of the custom model
+        The name of the custom model.
     language: str
-        programming language of the custom model.
-        Can be "python", "r", "java" or "other"
+        The programming language of the custom inference model.
+        Can be "python", "r", "java" or "other".
     description: str
-        description of the custom model
+        The description of the custom inference model.
     target_type: datarobot.TARGET_TYPE
-        target type of the custom inference model.
+        Target type of the custom inference model.
         Values: [`datarobot.TARGET_TYPE.BINARY`, `datarobot.TARGET_TYPE.REGRESSION`,
         `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`,
         `datarobot.TARGET_TYPE.ANOMALY`]
     target_name: str, optional
-        Target feature name;
-        it is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED`
-        or `datarobot.TARGET_TYPE.ANOMALY` target type
+        Target feature name.
+        It is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED`
+        or `datarobot.TARGET_TYPE.ANOMALY` target type.
     latest_version: datarobot.CustomModelVersion or None
-        latest version of the custom model if the model has a latest version
+        The latest version of the custom model if the model has a latest version.
     deployments_count: int
-        number of a deployments of the custom models
+        Number of a deployments of the custom models.
     target_name: str
-        custom model target name
+        The custom model target name.
     positive_class_label: str
-        for binary classification projects, a label of a positive class
+        For binary classification projects, a label of a positive class.
     negative_class_label: str
-        for binary classification projects, a label of a negative class
+        For binary classification projects, a label of a negative class.
     prediction_threshold: float
-        for binary classification projects, a threshold used for predictions
+        For binary classification projects, a threshold used for predictions.
     training_data_assignment_in_progress: bool
-        flag describing if training data assignment is in progress
+        Flag describing if training data assignment is in progress.
     training_dataset_id: str, optional
-        id of a dataset assigned to the custom model
+        The ID of a dataset assigned to the custom model.
     training_dataset_version_id: str, optional
-        id of a dataset version assigned to the custom model
+        The ID of a dataset version assigned to the custom model.
     training_data_file_name: str, optional
-        name of assigned training data file
+        The name of assigned training data file.
     training_data_partition_column: str, optional
-        name of a partition column in a training dataset assigned to the custom model
+        The name of a partition column in a training dataset assigned to the custom model.
     created_by: str
-        username of a user who user who created the custom model
+        The username of a user who user who created the custom model.
     updated_at: str
         ISO-8601 formatted timestamp of when the custom model was updated
     created_at: str
         ISO-8601 formatted timestamp of when the custom model was created
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
         Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
-        If exceeded, the custom-model will be killed by k8s
+        If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
         A fixed number of replicas that will be deployed in the cluster
+    is_training_data_for_versions_permanently_enabled: bool, optional
+        Whether training data assignment on the version level is permanently enabled for the model.
     """
 
-    _model_type = "inference"
+    _model_type: str = "inference"
     _converter = (
         _CustomModelBase._converter
         + {
             t.Key("language"): String(allow_blank=True),
             t.Key("target_name", optional=True): String(),
             t.Key("training_dataset_id", optional=True): String(),
             t.Key("training_dataset_version_id", optional=True): String(),
@@ -258,35 +446,39 @@
             t.Key("class_labels", optional=True): t.List(String()),
             t.Key("prediction_threshold", optional=True): t.Float(),
             t.Key("training_data_file_name", optional=True): String(),
             t.Key("training_data_partition_column", optional=True): String(),
             t.Key("network_egress_policy", optional=True): t.Enum(*NETWORK_EGRESS_POLICY.ALL),
             t.Key("maximum_memory", optional=True): Int(),
             t.Key("replicas", optional=True): Int(),
+            t.Key(
+                "is_training_data_for_versions_permanently_enabled", optional=True, default=False
+            ): t.Bool(),
         }
     ).allow_extra("*")
 
-    def _set_values(  # pylint: disable=arguments-renamed
+    def _set_values(  # type: ignore[override] # pylint: disable=arguments-renamed
         self,
-        language,
-        training_data_assignment_in_progress,
-        target_name=None,
-        positive_class_label=None,
-        negative_class_label=None,
-        prediction_threshold=None,
-        class_labels=None,
-        training_dataset_id=None,
-        training_dataset_version_id=None,
-        training_data_file_name=None,
-        training_data_partition_column=None,
-        network_egress_policy=None,
-        maximum_memory=None,
-        replicas=None,
-        **custom_model_kwargs,
-    ):
+        language: str,
+        training_data_assignment_in_progress: bool,
+        is_training_data_for_versions_permanently_enabled: bool,
+        target_name: Optional[str] = None,
+        positive_class_label: Optional[str] = None,
+        negative_class_label: Optional[str] = None,
+        prediction_threshold: Optional[float] = None,
+        class_labels: Optional[List[str]] = None,
+        training_dataset_id: Optional[str] = None,
+        training_dataset_version_id: Optional[str] = None,
+        training_data_file_name: Optional[str] = None,
+        training_data_partition_column: Optional[str] = None,
+        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
+        maximum_memory: Optional[int] = None,
+        replicas: Optional[int] = None,
+        **custom_model_kwargs: Any,
+    ) -> None:
         super()._set_values(**custom_model_kwargs)
 
         self.language = language
         self.target_name = target_name
         self.training_dataset_id = training_dataset_id
         self.training_dataset_version_id = training_dataset_version_id
         self.training_data_assignment_in_progress = training_data_assignment_in_progress
@@ -295,173 +487,180 @@
         self.class_labels = class_labels
         self.prediction_threshold = prediction_threshold
         self.training_data_file_name = training_data_file_name
         self.training_data_partition_column = training_data_partition_column
         self.network_egress_policy = network_egress_policy
         self.maximum_memory = maximum_memory
         self.replicas = replicas
+        self.is_training_data_for_versions_permanently_enabled = (
+            is_training_data_for_versions_permanently_enabled
+        )
 
     @classmethod
-    def list(  # pylint: disable=arguments-renamed
+    def list(  # type: ignore[override] # pylint: disable=arguments-renamed
         cls,
-        is_deployed=None,
-        search_for=None,
-        order_by=None,
-    ):
+        is_deployed: Optional[bool] = None,
+        search_for: Optional[str] = None,
+        order_by: Optional[str] = None,
+    ) -> List[CustomInferenceModel]:
         """List custom inference models available to the user.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         is_deployed: bool, optional
-            flag for filtering custom inference models.
+            Flag for filtering custom inference models.
             If set to `True`, only deployed custom inference models are returned.
-            If set to `False`, only not deployed custom inference models are returned
+            If set to `False`, only not deployed custom inference models are returned.
         search_for: str, optional
-            string for filtering custom inference models - only custom
+            String for filtering custom inference models - only custom
             inference models that contain the string in name or description will
             be returned.
             If not specified, all custom models will be returned
         order_by: str, optional
-            property to sort custom inference models by.
+            Property to sort custom inference models by.
             Supported properties are "created" and "updated".
             Prefix the attribute name with a dash to sort in descending order,
             e.g. order_by='-created'.
             By default, the order_by parameter is None which will result in
-            custom models being returned in order of creation time descending
+            custom models being returned in order of creation time descending.
 
         Returns
         -------
         List[CustomInferenceModel]
-            a list of custom inference models.
+            A list of custom inference models.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status
         """
         return super().list(is_deployed, order_by, search_for)
 
     @classmethod
-    def get(cls, custom_model_id):
+    def get(cls, custom_model_id: str) -> CustomInferenceModel:
         """Get custom inference model by id.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            id of the custom inference model
+            The ID of the custom inference model.
 
         Returns
         -------
         CustomInferenceModel
-            retrieved custom inference model
+            Retrieved custom inference model.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            The ID the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            The ID the server responded with 5xx status.
         """
         return super().get(custom_model_id)
 
     # We must leave this method here in order for the docs to properly be generated
     # pylint: disable-next=useless-super-delegation
-    def download_latest_version(self, file_path):
+    def download_latest_version(self, file_path: str) -> None:
         """Download the latest custom inference model version.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         file_path: str
-            path to create a file with custom model version content
+            Path to create a file with custom model version content.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
         super().download_latest_version(file_path)
 
     @classmethod
-    def create(  # pylint: disable=arguments-differ,arguments-renamed
+    def create(  # type: ignore[override] # pylint: disable=arguments-differ,arguments-renamed
         cls,
-        name,
-        target_type,
-        target_name=None,
-        language=None,
-        description=None,
-        positive_class_label=None,
-        negative_class_label=None,
-        prediction_threshold=None,
-        class_labels=None,
-        class_labels_file=None,
-        network_egress_policy=None,
-        maximum_memory=None,
-        replicas=None,
-    ):
+        name: str,
+        target_type: TARGET_TYPE,
+        target_name: Optional[str] = None,
+        language: Optional[str] = None,
+        description: Optional[str] = None,
+        positive_class_label: Optional[str] = None,
+        negative_class_label: Optional[str] = None,
+        prediction_threshold: Optional[float] = None,
+        class_labels: Optional[List[str]] = None,
+        class_labels_file: Optional[str] = None,
+        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
+        maximum_memory: Optional[int] = None,
+        replicas: Optional[int] = None,
+        is_training_data_for_versions_permanently_enabled: Optional[bool] = None,
+    ) -> CustomInferenceModel:
         """Create a custom inference model.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         name: str
-            name of the custom inference model
+            Name of the custom inference model.
         target_type: datarobot.TARGET_TYPE
-            target type of the custom inference model.
+            Target type of the custom inference model.
             Values: [`datarobot.TARGET_TYPE.BINARY`, `datarobot.TARGET_TYPE.REGRESSION`,
             `datarobot.TARGET_TYPE.MULTICLASS`, `datarobot.TARGET_TYPE.UNSTRUCTURED`]
         target_name: str, optional
-            Target feature name;
-            it is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED` target type
+            Target feature name.
+            It is optional(ignored if provided) for `datarobot.TARGET_TYPE.UNSTRUCTURED` target type.
         language: str, optional
-            programming language of the custom learning model
+            Programming language of the custom learning model.
         description: str, optional
-            description of the custom learning model
+            Description of the custom learning model.
         positive_class_label: str, optional
-            custom inference model positive class label for binary classification
+            Custom inference model positive class label for binary classification.
         negative_class_label: str, optional
-            custom inference model negative class label for binary classification
+            Custom inference model negative class label for binary classification.
         prediction_threshold: float, optional
-            custom inference model prediction threshold
+            Custom inference model prediction threshold.
         class_labels: List[str], optional
-            custom inference model class labels for multiclass classification
-            Cannot be used with class_labels_file
+            Custom inference model class labels for multiclass classification.
+            Cannot be used with class_labels_file.
         class_labels_file: str, optional
-            path to file containing newline separated class labels for multiclass classification.
-            Cannot be used with class_labels
+            Path to file containing newline separated class labels for multiclass classification.
+            Cannot be used with class_labels.
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
+            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
-            If exceeded, the custom-model will be killed by k8s
+            If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
-            A fixed number of replicas that will be deployed in the cluster
+            A fixed number of replicas that will be deployed in the cluster.
+        is_training_data_for_versions_permanently_enabled: bool, optional
+            Permanently enable training data assignment on the version level for the current model,
+            instead of training data assignment on the model level.
 
         Returns
         -------
         CustomInferenceModel
-            created a custom inference model
+            Created a custom inference model.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         if target_type in CUSTOM_MODEL_TARGET_TYPE.REQUIRES_TARGET_NAME and target_name is None:
             raise ValueError(
                 f"target_name is required for custom models with target type {target_type}"
             )
         if class_labels and class_labels_file:
             raise ValueError("class_labels and class_labels_file cannot be used together")
@@ -478,89 +677,94 @@
             positive_class_label=positive_class_label,
             negative_class_label=negative_class_label,
             prediction_threshold=prediction_threshold,
             class_labels=class_labels,
             network_egress_policy=network_egress_policy,
             maximum_memory=maximum_memory,
             replicas=replicas,
+            is_training_data_for_versions_permanently_enabled=is_training_data_for_versions_permanently_enabled,
         )
 
     @classmethod
     def copy_custom_model(
         cls,
-        custom_model_id,
-    ):
+        custom_model_id: str,
+    ) -> CustomInferenceModel:
         """Create a custom inference model by copying existing one.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            id of the custom inference model to copy
+            The ID of the custom inference model to copy.
 
         Returns
         -------
         CustomInferenceModel
-            created a custom inference model
+            Created a custom inference model.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         return super().copy_custom_model(custom_model_id)
 
-    def update(  # pylint: disable=arguments-differ,arguments-renamed
+    def update(  # type: ignore[override] # pylint: disable=arguments-differ,arguments-renamed
         self,
-        name=None,
-        language=None,
-        description=None,
-        target_name=None,
-        positive_class_label=None,
-        negative_class_label=None,
-        prediction_threshold=None,
-        class_labels=None,
-        class_labels_file=None,
-    ):
+        name: Optional[str] = None,
+        language: Optional[str] = None,
+        description: Optional[str] = None,
+        target_name: Optional[str] = None,
+        positive_class_label: Optional[str] = None,
+        negative_class_label: Optional[str] = None,
+        prediction_threshold: Optional[float] = None,
+        class_labels: Optional[List[str]] = None,
+        class_labels_file: Optional[str] = None,
+        is_training_data_for_versions_permanently_enabled: Optional[bool] = None,
+    ) -> None:
         """Update custom inference model properties.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         name: str, optional
-            new custom inference model name
+            New custom inference model name.
         language: str, optional
-            new custom inference model programming language
+            New custom inference model programming language.
         description: str, optional
-            new custom inference model description
+            New custom inference model description.
         target_name: str, optional
-            new custom inference model target name
+            New custom inference model target name.
         positive_class_label: str, optional
-            new custom inference model positive class label
+            New custom inference model positive class label.
         negative_class_label: str, optional
-            new custom inference model negative class label
+            New custom inference model negative class label.
         prediction_threshold: float, optional
-            new custom inference model prediction threshold
+            New custom inference model prediction threshold.
         class_labels: List[str], optional
             custom inference model class labels for multiclass classification
             Cannot be used with class_labels_file
         class_labels_file: str, optional
-            path to file containing newline separated class labels for multiclass classification.
+            Path to file containing newline separated class labels for multiclass classification.
             Cannot be used with class_labels
+        is_training_data_for_versions_permanently_enabled: bool, optional
+            Permanently enable training data assignment on the version level for the current model,
+            instead of training data assignment on the model level.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
         if class_labels and class_labels_file:
             raise ValueError("class_labels and class_labels_file cannot be used together")
         if class_labels_file:
             with open(class_labels_file) as f:  # pylint: disable=unspecified-encoding
                 class_labels = [label for label in f.read().split("\n") if label]
 
@@ -569,70 +773,76 @@
             description,
             language=language,
             target_name=target_name,
             positive_class_label=positive_class_label,
             negative_class_label=negative_class_label,
             prediction_threshold=prediction_threshold,
             class_labels=class_labels,
+            is_training_data_for_versions_permanently_enabled=is_training_data_for_versions_permanently_enabled,
         )
 
     # We must leave this method here in order for the docs to properly be generated
     # pylint: disable-next=useless-super-delegation
-    def refresh(self):
+    def refresh(self) -> None:
         """Update custom inference model with the latest data from server.
 
         .. versionadded:: v2.21
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         super().refresh()
 
     # We must leave this method here in order for the docs to properly be generated
     # pylint: disable-next=useless-super-delegation
-    def delete(self):
+    def delete(self) -> None:
         """Delete custom inference model.
 
         .. versionadded:: v2.21
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         super().delete()
 
-    def assign_training_data(self, dataset_id, partition_column=None, max_wait=DEFAULT_MAX_WAIT):
+    def assign_training_data(
+        self,
+        dataset_id: str,
+        partition_column: Optional[str] = None,
+        max_wait: int = DEFAULT_MAX_WAIT,
+    ) -> None:
         """Assign training data to the custom inference model.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         dataset_id: str
-            the id of the training dataset to be assigned
+            The id of the training dataset to be assigned.
         partition_column: str, optional
-            name of a partition column in the training dataset
+            Name of a partition column in the training dataset.
         max_wait: int, optional
-            max time to wait for a training data assignment.
+            Max time to wait for a training data assignment.
             If set to None - method will return without waiting.
-            Defaults to 10 min
+            Defaults to 10 min.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status
         """
         payload = {"dataset_id": dataset_id, "partition_column": partition_column}
 
         path = f"{self._path}{self.id}/trainingData/"
 
         response = self._client.patch(path, data=payload)
```

### Comparing `datarobot-3.1.1/datarobot/models/custom_model_test.py` & `datarobot-3.2.0b0/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/custom_model_version.py` & `datarobot-3.2.0b0/datarobot/models/custom_model_version.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,26 +5,31 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+from __future__ import annotations
+
 import contextlib
 import copy
 import json
 import os
+import time
+from typing import Any, cast, Dict, Iterable, List, Mapping, Optional, Tuple, Union
 
+from requests import Response
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
-from datarobot.errors import InvalidUsageError
-from datarobot.models.api_object import APIObject
+from datarobot.errors import InvalidUsageError, TrainingDataAssignmentError
+from datarobot.models.api_object import APIObject, ServerDataType
 from datarobot.models.job import filter_feature_impact_result
 from datarobot.models.validators import custom_model_feature_impact_trafaret
 from datarobot.utils import camelize
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution, wait_for_custom_resolution
 
 
@@ -36,56 +41,151 @@
     Attributes
     ----------
     field_name: str
         The required field names.  Required field names are defined by the
         environment's required_metadata_keys. This value will be added as an
         environment vairable when running custom models.
     value: str
-        the value for the required field.
+        The value for the required field.
     """
 
     _converter = t.Dict({t.Key("field_name"): String(), t.Key("value"): String()})
 
     schema = _converter
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "{}(field_name={!r}, value={!r})".format(
             self.__class__.__name__,
             self.field_name,
             self.value,
         )
 
-    def _set_values(self, field_name, value):
+    def _set_values(self, field_name: str, value: str) -> None:
         self.field_name = field_name
         self.value = value
 
-    def to_dict(self):
-        return self._converter.check({"field_name": self.field_name, "value": self.value})
+    def to_dict(self) -> Dict[str, str]:
+        return cast(
+            Dict[str, str],
+            self._converter.check({"field_name": self.field_name, "value": self.value}),
+        )
+
+
+class TrainingData(APIObject):
+    """Training data assigned to a DataRobot custom model version.
+
+    .. versionadded:: v3.2
+
+    Attributes
+    ----------
+    dataset_id: str
+        The ID of the dataset.
+    dataset_version_id: str
+        The ID of the dataset version.
+    dataset_name: str
+        The name of the dataset.
+    assignment_in_progress: bool
+        The status of the assignment in progress.
+    assignment_error: dict
+        The assignment error message.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("dataset_id", optional=True): t.Or(String(), t.Null()),
+            t.Key("dataset_version_id", optional=True): t.Or(String(), t.Null()),
+            t.Key("dataset_name", optional=True): t.Or(String(), t.Null()),
+            t.Key("assignment_in_progress", optional=True): t.Bool(),
+            t.Key("assignment_error", optional=True): t.Dict(
+                {
+                    t.Key("message"): t.Or(String(), t.Null()),
+                }
+            )
+            | t.Null,
+        }
+    ).ignore_extra("*")
+
+    schema = _converter
+
+    def __init__(
+        self,
+        dataset_id: Optional[str] = None,
+        dataset_version_id: Optional[str] = None,
+        dataset_name: Optional[str] = None,
+        assignment_in_progress: Optional[str] = None,
+        assignment_error: Optional[Dict[str, str]] = None,
+    ) -> None:
+        self.dataset_id = dataset_id
+        self.dataset_version_id = dataset_version_id
+        self.dataset_name = dataset_name
+        self.assignment_in_progress = assignment_in_progress
+        self.assignment_error = assignment_error
+
+
+class HoldoutData(APIObject):
+    """Holdout data assigned to a DataRobot custom model version.
+
+    .. versionadded:: v3.2
+
+    Attributes
+    ----------
+    dataset_id: str
+        The ID of the dataset.
+    dataset_version_id: str
+        The ID of the dataset version.
+    dataset_name: str
+        The name of the dataset.
+    partition_column: str
+        The name of the partitions column.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("dataset_id", optional=True): t.Or(String(), t.Null()),
+            t.Key("dataset_version_id", optional=True): t.Or(String(), t.Null()),
+            t.Key("dataset_name", optional=True): t.Or(String(), t.Null()),
+            t.Key("partition_column", optional=True): t.Or(String(), t.Null()),
+        }
+    ).ignore_extra("*")
+
+    schema = _converter
+
+    def __init__(
+        self,
+        dataset_id: Optional[str] = None,
+        dataset_version_id: Optional[str] = None,
+        dataset_name: Optional[str] = None,
+        partition_column: Optional[str] = None,
+    ) -> None:
+        self.dataset_id = dataset_id
+        self.dataset_version_id = dataset_version_id
+        self.dataset_name = dataset_name
+        self.partition_column = partition_column
 
 
 class CustomModelFileItem(APIObject):
     """A file item attached to a DataRobot custom model version.
 
     .. versionadded:: v2.21
 
     Attributes
     ----------
     id: str
-        id of the file item
+        The ID of the file item.
     file_name: str
-        name of the file item
+        The name of the file item.
     file_path: str
-        path of the file item
+        The path of the file item.
     file_source: str
-        source of the file item
+        The source of the file item.
     created_at: str, optional
-        ISO-8601 formatted timestamp of when the version was created
+        ISO-8601 formatted timestamp of when the version was created.
     """
 
     _converter = t.Dict(
         {
             t.Key("id"): String(),
             t.Key("file_name"): String(),
             t.Key("file_path"): String(),
@@ -94,20 +194,20 @@
         }
     ).ignore_extra("*")
 
     schema = _converter
 
     def __init__(
         self,
-        id,
-        file_name,
-        file_path,
-        file_source,
-        created_at=None,
-    ):
+        id: str,
+        file_name: str,
+        file_path: str,
+        file_source: str,
+        created_at: Optional[str] = None,
+    ) -> None:
         self.id = id
         self.file_name = file_name
         self.file_path = file_path
         self.file_source = file_source
         self.created_at = created_at
 
 
@@ -115,23 +215,23 @@
     """Metadata about a DataRobot custom model version's dependency build
 
     .. versionadded:: v2.22
 
     Attributes
     ----------
     custom_model_id: str
-        id of the custom model
+        The ID of the custom model.
     custom_model_version_id: str
-        id of the custom model version
+        The ID of the custom model version.
     build_status: str
-        the status of the custom model version's dependency build
+        The status of the custom model version's dependency build.
     started_at: str
-        ISO-8601 formatted timestamp of when the build was started
+        ISO-8601 formatted timestamp of when the build was started.
     completed_at: str, optional
-        ISO-8601 formatted timestamp of when the build has completed
+        ISO-8601 formatted timestamp of when the build has completed.
     """
 
     _path = "customModels/{}/versions/{}/dependencyBuild/"
     _log_path = "customModels/{}/versions/{}/dependencyBuildLog/"
 
     _converter = t.Dict(
         {
@@ -141,91 +241,100 @@
             t.Key("build_start") >> "started_at": String(),
             t.Key("build_end", optional=True) >> "completed_at": String(allow_blank=True),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "{}(model={!r}, version={!r}, status={!r})".format(
             self.__class__.__name__,
             self.custom_model_id,
             self.custom_model_version_id,
             self.build_status,
         )
 
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
-        custom_model_id,
-        custom_model_version_id,
-        build_status,
-        started_at,
-        completed_at=None,
-    ):
+        custom_model_id: str,
+        custom_model_version_id: str,
+        build_status: str,
+        started_at: str,
+        completed_at: Optional[str] = None,
+    ) -> None:
         self.custom_model_id = custom_model_id
         self.custom_model_version_id = custom_model_version_id
         self.build_status = build_status
         self.started_at = started_at
         self.completed_at = completed_at
 
     @classmethod
-    def _update_server_data(cls, server_data, custom_model_id, custom_model_version_id):
+    def _update_server_data(
+        cls, server_data: Dict[str, Any], custom_model_id: str, custom_model_version_id: str
+    ) -> Dict[str, Any]:
         updated_data = copy.copy(server_data)
         updated_data.update(
             {"customModelId": custom_model_id, "customModelVersionId": custom_model_version_id}
         )
         return updated_data
 
     @classmethod
-    def get_build_info(cls, custom_model_id, custom_model_version_id):
+    def get_build_info(
+        cls, custom_model_id: str, custom_model_version_id: str
+    ) -> CustomModelVersionDependencyBuild:
         """Retrieve information about a custom model version's dependency build
 
         .. versionadded:: v2.22
 
         Parameters
         ----------
         custom_model_id: str
-            the id of the custom model
+            The ID of the custom model.
         custom_model_version_id: str
-            the id of the custom model version
+            The ID of the custom model version.
 
         Returns
         -------
         CustomModelVersionDependencyBuild
-            the dependency build information
+            The dependency build information.
         """
         url = cls._path.format(custom_model_id, custom_model_version_id)
         response = cls._client.get(url)
         server_data = response.json()
         updated_data = cls._update_server_data(
             server_data, custom_model_id, custom_model_version_id
         )
         return cls.from_server_data(updated_data)
 
     @classmethod
-    def start_build(cls, custom_model_id, custom_model_version_id, max_wait=DEFAULT_MAX_WAIT):
+    def start_build(
+        cls,
+        custom_model_id: str,
+        custom_model_version_id: str,
+        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
+    ) -> Optional[CustomModelVersionDependencyBuild]:
         """Start the dependency build for a custom model version  dependency build
 
         .. versionadded:: v2.22
 
         Parameters
         ----------
         custom_model_id: str
-            the id of the custom model
+            The ID of the custom model
         custom_model_version_id: str
-            the id of the custom model version
+            the ID of the custom model version
         max_wait: int, optional
-            max time to wait for a build completion.
+            Max time to wait for a build completion.
             If set to None - method will return without waiting.
         """
 
-        def build_complete(response):
+        def build_complete(response: Response) -> Optional[CustomModelVersionDependencyBuild]:
             data = response.json()
             if data["buildStatus"] in ["success", "failed"]:
                 updated_data = cls._update_server_data(
                     data, custom_model_id, custom_model_version_id
                 )
                 return cls.from_server_data(updated_data)
             return None
@@ -236,191 +345,205 @@
         if max_wait is None:
             server_data = response.json()
             updated_data = cls._update_server_data(
                 server_data, custom_model_id, custom_model_version_id
             )
             return cls.from_server_data(updated_data)
         else:
-            return wait_for_custom_resolution(cls._client, url, build_complete, max_wait)
+            return cast(
+                Optional[CustomModelVersionDependencyBuild],
+                wait_for_custom_resolution(cls._client, url, build_complete, max_wait),
+            )
 
-    def get_log(self):
+    def get_log(self) -> str:
         """Get log of a custom model version dependency build.
 
         .. versionadded:: v2.22
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         url = self._log_path.format(self.custom_model_id, self.custom_model_version_id)
-        return self._client.get(url).text
+        return cast(str, self._client.get(url).text)
 
-    def cancel(self):
+    def cancel(self) -> None:
         """Cancel custom model version dependency build that is in progress.
 
         .. versionadded:: v2.22
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         url = self._path.format(self.custom_model_id, self.custom_model_version_id)
         self._client.delete(url)
 
-    def refresh(self):
+    def refresh(self) -> None:
         """Update custom model version dependency build with the latest data from server.
 
         .. versionadded:: v2.22
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         url = self._path.format(self.custom_model_id, self.custom_model_version_id)
 
         response = self._client.get(url)
 
         data = response.json()
         updated_data = self._update_server_data(
             data, self.custom_model_id, self.custom_model_version_id
         )
-        self._set_values(**self._safe_data(updated_data, do_recursive=True))
+        self._set_values(**self._safe_data(updated_data, do_recursive=True))  # type: ignore[no-untyped-call]
 
 
 class CustomDependencyConstraint(APIObject):
     """Metadata about a constraint on a dependency of a custom model version
 
     .. versionadded:: v2.22
 
     Attributes
     ----------
     constraint_type: str
-        How the dependency should be constrained by version (<, <=, ==, >=, >)
+        How the dependency should be constrained by version (<, <=, ==, >=, >).
     version: str
-        The version to use in the dependency's constraint
+        The version to use in the dependency's constraint.
     """
 
     _converter = t.Dict(
         {t.Key("constraint_type"): String(), t.Key("version"): String()}
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "{}(constraint_type={!r}, version={!r})".format(
             self.__class__.__name__,
             self.constraint_type,
             self.version,
         )
 
-    def _set_values(self, constraint_type, version):
+    def _set_values(self, constraint_type: str, version: str) -> None:
         self.constraint_type = constraint_type
         self.version = version
 
 
 class CustomDependency(APIObject):
     """Metadata about an individual dependency of a custom model version
 
     .. versionadded:: v2.22
 
     Attributes
     ----------
     package_name: str
-        The dependency's package name
+        The dependency's package name.
     constraints: List[CustomDependencyConstraint]
-        Version constraints to apply on the dependency
+        Version constraints to apply on the dependency.
     line: str
-        The original line from the requirements file
+        The original line from the requirements file.
     line_number: int
-        The line number the requirement was on in the requirements file
+        The line number the requirement was on in the requirements file.
     """
 
     _converter = t.Dict(
         {
             t.Key("package_name"): String(),
             t.Key("constraints"): t.List(CustomDependencyConstraint.schema),
             t.Key("line"): String(),
             t.Key("line_number"): Int(gt=0),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "{}(package_name={!r}, constraints={!r})".format(
             self.__class__.__name__,
             self.package_name,
             self.constraints,
         )
 
-    def _set_values(self, package_name, constraints, line, line_number):
+    def _set_values(  # pylint: disable=missing-function-docstring
+        self,
+        package_name: str,
+        constraints: List[CustomDependencyConstraint],
+        line: str,
+        line_number: int,
+    ) -> None:
         self.package_name = package_name
-        self.constraints = [CustomDependencyConstraint(**c) for c in constraints]
+        # TODO: maybe CustomDependencyConstraint should be implemented as TypedDict
+        self.constraints = [CustomDependencyConstraint(**c) for c in constraints]  # type: ignore[arg-type]
         self.line = line
         self.line_number = line_number
 
 
 class CustomModelVersion(APIObject):
     """A version of a DataRobot custom model.
 
     .. versionadded:: v2.21
 
     Attributes
     ----------
     id: str
-        id of the custom model version
+        The ID of the custom model version.
     custom_model_id: str
-        id of the custom model
+        The ID of the custom model.
     version_minor: int
-        a minor version number of custom model version
+        A minor version number of the custom model version.
     version_major: int
-        a major version number of custom model version
+        A major version number of the custom model version.
     is_frozen: bool
-        a flag if the custom model version is frozen
+        A flag if the custom model version is frozen.
     items: List[CustomModelFileItem]
-        a list of file items attached to the custom model version
+        A list of file items attached to the custom model version.
     base_environment_id: str
-        id of the environment to use with the model
+        The ID of the environment to use with the model.
     base_environment_version_id: str
-        id of the environment version to use with the model
+        The ID of the environment version to use with the model.
     label: str, optional
-        short human readable string to label the version
+        A short human readable string to label the version.
     description: str, optional
-        custom model version description
+        The custom model version description.
     created_at: str, optional
-        ISO-8601 formatted timestamp of when the version was created
+        ISO-8601 formatted timestamp of when the version was created.
     dependencies: List[CustomDependency]
-        the parsed dependencies of the custom model version if the
-        version has a valid requirements.txt file
+        The parsed dependencies of the custom model version if the
+        version has a valid requirements.txt file.
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
+        Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
-        If exceeded, the custom-model will be killed by k8s
+        If exceeded, the custom-model will be killed by k8s.
     replicas: int, optional
-        A fixed number of replicas that will be deployed in the cluster
+        A fixed number of replicas that will be deployed in the cluster.
     required_metadata_values: List[RequiredMetadataValue]
         Additional parameters required by the execution environment. The required keys are
         defined by the fieldNames in the base environment's requiredMetadataKeys.
+    training_data: TrainingData, optional
+        The information about the training data assigned to the model version.
+    holdout_data: HoldoutData, optional
+        The information about the holdout data assigned to the model version.
     """
 
     _path = "customModels/{}/versions/"
 
     _converter = t.Dict(
         {
             t.Key("id"): String(),
@@ -439,224 +562,392 @@
             ),
             t.Key("created", optional=True) >> "created_at": String(),
             t.Key("dependencies", optional=True): t.List(CustomDependency.schema),
             t.Key("network_egress_policy", optional=True): t.Enum(*NETWORK_EGRESS_POLICY.ALL),
             t.Key("maximum_memory", optional=True): Int(),
             t.Key("replicas", optional=True): Int(),
             t.Key("required_metadata_values", optional=True): t.List(RequiredMetadataValue.schema),
+            t.Key("training_data", optional=True): t.Or(TrainingData.schema, t.Null()),
+            t.Key("holdout_data", optional=True): t.Or(HoldoutData.schema, t.Null()),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.label or self.id!r})"
 
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
-        id,
-        custom_model_id,
-        version_minor,
-        version_major,
-        is_frozen,
-        items,
-        base_environment_id=None,
-        base_environment_version_id=None,
-        label=None,
-        description=None,
-        created_at=None,
-        dependencies=None,
-        network_egress_policy=None,
-        maximum_memory=None,
-        replicas=None,
-        required_metadata_values=None,
-    ):
+        id: str,
+        custom_model_id: str,
+        version_minor: int,
+        version_major: int,
+        is_frozen: bool,
+        items: List[CustomModelFileItem],
+        base_environment_id: Optional[str] = None,
+        base_environment_version_id: Optional[str] = None,
+        label: Optional[str] = None,
+        description: Optional[str] = None,
+        created_at: Optional[str] = None,
+        dependencies: Optional[List[CustomDependency]] = None,
+        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
+        maximum_memory: Optional[int] = None,
+        replicas: Optional[int] = None,
+        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
+        training_data: Optional[Mapping[str, Any]] = None,
+        holdout_data: Optional[Mapping[str, Any]] = None,
+    ) -> None:
         self.id = id
         self.custom_model_id = custom_model_id
         self.version_minor = version_minor
         self.version_major = version_major
         self.is_frozen = is_frozen
-        self.items = [CustomModelFileItem(**item) for item in items]
+        self.items = [CustomModelFileItem(**item) for item in items]  # type: ignore[arg-type]
         self.base_environment_id = base_environment_id
         self.base_environment_version_id = base_environment_version_id
         self.label = label
         self.description = description
         self.created_at = created_at
-        self.dependencies = [CustomDependency(**dep) for dep in dependencies or []]
+        self.dependencies = [CustomDependency(**dep) for dep in dependencies or []]  # type: ignore[arg-type]
         self.network_egress_policy = network_egress_policy
         self.maximum_memory = maximum_memory
         self.replicas = replicas
         self.required_metadata_values = (
-            [RequiredMetadataValue.from_server_data(val) for val in required_metadata_values]
+            [RequiredMetadataValue.from_server_data(val) for val in required_metadata_values]  # type: ignore[arg-type]
             if required_metadata_values
             else None
         )
+        self.training_data = TrainingData(**training_data) if training_data else None
+        self.holdout_data = HoldoutData(**holdout_data) if holdout_data else None
 
     @classmethod
-    def from_server_data(cls, data, keep_attrs=None):
+    def from_server_data(
+        cls, data: ServerDataType, keep_attrs: Optional[Iterable[str]] = None
+    ) -> CustomModelVersion:
         initial = super().from_server_data(data, keep_attrs)
         # from_server_data will make the keys in requiredMetadata lowercase,
         # which is not OK. we need to preserve case
-        initial.required_metadata = data.get("requiredMetadata")
+        initial.required_metadata = data.get("requiredMetadata")  # type: ignore[union-attr]
         return initial
 
     @classmethod
     def create_clean(
         cls,
-        custom_model_id,
-        base_environment_id,
-        is_major_update=True,
-        folder_path=None,
-        files=None,
-        network_egress_policy=None,
-        maximum_memory=None,
-        replicas=None,
-        required_metadata_values=None,
-    ):
+        custom_model_id: str,
+        base_environment_id: str,
+        is_major_update: bool = True,
+        folder_path: Optional[str] = None,
+        files: Optional[List[Tuple[str, str]]] = None,
+        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
+        maximum_memory: Optional[int] = None,
+        replicas: Optional[int] = None,
+        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
+        training_dataset_id: Optional[str] = None,
+        partition_column: Optional[str] = None,
+        holdout_dataset_id: Optional[str] = None,
+        keep_training_holdout_data: Optional[bool] = None,
+        max_wait: int = DEFAULT_MAX_WAIT,
+    ) -> CustomModelVersion:
         """Create a custom model version without files from previous versions.
 
+           Create a version with training or holdout data:
+           If training/holdout data related parameters are provided,
+           the training data is assigned asynchronously.
+           In this case:
+           * if max_wait is not None, the function returns once the job is finished.
+           * if max_wait is None, the function returns immediately. Progress can be polled by the user (see examples).
+
+           If training data assignment fails, new version is still created,
+           but it is not allowed to create a model package for the model version and to deploy it.
+           To check for training data assignment error, check version.training_data.assignment_error["message"].
+
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            the id of the custom model
+            The ID of the custom model.
         base_environment_id: str
-            the id of the base environment to use with the custom model version
+            The ID of the base environment to use with the custom model version.
         is_major_update: bool
-            the flag defining if a custom model version
-            will be a minor or a major version.
+            The flag defining if a custom model version will be a minor or a major version.
             Default to `True`
         folder_path: str, optional
-            the path to a folder containing files to be uploaded.
-            Each file in the folder is uploaded under path relative
-            to a folder path
+            The path to a folder containing files to be uploaded.
+            Each file in the folder is uploaded under path relative to a folder path.
         files: list, optional
-            the list of tuples, where values in each tuple are the local filesystem path and
+            The list of tuples, where values in each tuple are the local filesystem path and
             the path the file should be placed in the model.
-            if list is of strings, then basenames will be used for tuples
+            If the list is of strings, then basenames will be used for tuples.
             Example:
             [("/home/user/Documents/myModel/file1.txt", "file1.txt"),
             ("/home/user/Documents/myModel/folder/file2.txt", "folder/file2.txt")]
             or
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
+            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
-            If exceeded, the custom-model will be killed by k8s
+            If exceeded, the custom-model will be killed by k8s.
         replicas: int, optional
-            A fixed number of replicas that will be deployed in the cluster
+            A fixed number of replicas that will be deployed in the cluster.
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
             defined by the fieldNames in the base environment's requiredMetadataKeys.
+        training_dataset_id: str, optional
+            The ID of the training dataset to assign to the custom model.
+        partition_column: str, optional
+            Name of a partition column in a training dataset assigned to the custom model.
+            Can only be assigned for structured models.
+        holdout_dataset_id: str, optional
+            The ID of the holdout dataset to assign to the custom model.
+            Can only be assigned for unstructured models.
+        keep_training_holdout_data: bool, optional
+            If the version should inherit training and holdout data from the previous version.
+            Defaults to True.
+            This field is only applicable if the model has training data for versions enabled,
+            otherwise the field value will be ignored.
+        max_wait: int, optional
+            Max time to wait for training data assignment.
+            If set to None - method will return without waiting.
+            Defaults to 10 minutes.
 
         Returns
         -------
         CustomModelVersion
-            created custom model version
+            Created custom model version.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
+        datarobot.errors.InvalidUsageError
+            If wrong parameters are provided.
+        datarobot.errors.TrainingDataAssignmentError
+            If training data assignment fails.
+
+        Examples
+        --------
+        Create a version with blocking (default max_wait=600) training data assignment:
+
+        .. code-block:: python
+
+            import datarobot as dr
+            from datarobot.errors import TrainingDataAssignmentError
+
+            dr.Client(token=my_token, endpoint=endpoint)
+
+            try:
+                version = dr.CustomModelVersion.create_from_previous(
+                    custom_model_id="6444482e5583f6ee2e572265",
+                    base_environment_id="642209acc563893014a41e24",
+                    training_dataset_id="6421f2149a4f9b1bec6ad6dd",
+                )
+            except TrainingDataAssignmentError as e:
+                print(e)
+
+        Create a version with non-blocking training data assignment:
+
+        .. code-block:: python
+
+            import datarobot as dr
+
+            dr.Client(token=my_token, endpoint=endpoint)
+
+            version = dr.CustomModelVersion.create_from_previous(
+                custom_model_id="6444482e5583f6ee2e572265",
+                base_environment_id="642209acc563893014a41e24",
+                training_dataset_id="6421f2149a4f9b1bec6ad6dd",
+                max_wait=None,
+            )
+
+            while version.training_data.assignment_in_progress:
+                time.sleep(10)
+                version.refresh()
+            if version.training_data.assignment_error:
+                print(version.training_data.assignment_error["message"])
         """
-        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):
-            files = [(filename, os.path.basename(filename)) for filename in files]
+        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):  # type: ignore[unreachable]
+            files = [(filename, os.path.basename(filename)) for filename in files]  # type: ignore[unreachable]
         return cls._create(
             "post",
             custom_model_id,
             is_major_update,
             base_environment_id,
             folder_path,
             files,
+            extra_upload_data=None,
             network_egress_policy=network_egress_policy,
             maximum_memory=maximum_memory,
             replicas=replicas,
             required_metadata_values=required_metadata_values,
+            training_dataset_id=training_dataset_id,
+            partition_column=partition_column,
+            holdout_dataset_id=holdout_dataset_id,
+            keep_training_holdout_data=keep_training_holdout_data,
+            max_wait=max_wait,
         )
 
     @classmethod
     def create_from_previous(
         cls,
-        custom_model_id,
-        base_environment_id,
-        is_major_update=True,
-        folder_path=None,
-        files=None,
-        files_to_delete=None,
-        network_egress_policy=None,
-        maximum_memory=None,
-        replicas=None,
-        required_metadata_values=None,
-    ):
+        custom_model_id: str,
+        base_environment_id: str,
+        is_major_update: bool = True,
+        folder_path: Optional[str] = None,
+        files: Optional[List[Tuple[str, str]]] = None,
+        files_to_delete: Optional[List[str]] = None,
+        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
+        maximum_memory: Optional[int] = None,
+        replicas: Optional[int] = None,
+        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
+        training_dataset_id: Optional[str] = None,
+        partition_column: Optional[str] = None,
+        holdout_dataset_id: Optional[str] = None,
+        keep_training_holdout_data: Optional[bool] = None,
+        max_wait: int = DEFAULT_MAX_WAIT,
+    ) -> CustomModelVersion:
         """Create a custom model version containing files from a previous version.
 
+           Create a version with training/holdout data:
+           If training/holdout data related parameters are provided,
+           the training data is assigned asynchronously.
+           In this case:
+           * if max_wait is not None, function returns once job is finished.
+           * if max_wait is None, function returns immediately, progress can be polled by the user, see examples.
+
+           If training data assignment fails, new version is still created,
+           but it is not allowed to create a model package for the model version and to deploy it.
+           To check for training data assignment error, check version.training_data.assignment_error["message"].
+
+
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            the id of the custom model
+            The ID of the custom model.
         base_environment_id: str
-            the id of the base environment to use with the custom model version
+            The ID of the base environment to use with the custom model version.
         is_major_update: bool, optional
-            the flag defining if a custom model version
-            will be a minor or a major version.
-            Default to `True`
+            The flag defining if a custom model version will be a minor or a major version.
+            Defaults to `True`.
         folder_path: str, optional
-            the path to a folder containing files to be uploaded.
-            Each file in the folder is uploaded under path relative
-            to a folder path
+            The path to a folder containing files to be uploaded.
+            Each file in the folder is uploaded under path relative to a folder path.
         files: list, optional
-            the list of tuples, where values in each tuple are the local filesystem path and
+            The list of tuples, where values in each tuple are the local filesystem path and
             the path the file should be placed in the model.
-            if list is of strings, then basenames will be used for tuples
+            If list is of strings, then basenames will be used for tuples
             Example:
             [("/home/user/Documents/myModel/file1.txt", "file1.txt"),
             ("/home/user/Documents/myModel/folder/file2.txt", "folder/file2.txt")]
             or
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         files_to_delete: list, optional
-            the list of a file items ids to be deleted
+            The list of a file items ids to be deleted.
             Example: ["5ea95f7a4024030aba48e4f9", "5ea6b5da402403181895cc51"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
             Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
             defined by the fieldNames in the base environment's requiredMetadataKeys.
+        training_dataset_id: str, optional
+            The ID of the training dataset to assign to the custom model.
+        partition_column: str, optional
+            Name of a partition column in a training dataset assigned to the custom model.
+            Can only be assigned for structured models.
+        holdout_dataset_id: str, optional
+            The ID of the holdout dataset to assign to the custom model.
+            Can only be assigned for unstructured models.
+        keep_training_holdout_data: bool, optional
+            If the version should inherit training and holdout data from the previous version.
+            Defaults to True.
+            This field is only applicable if the model has training data for versions enabled,
+            otherwise the field value will be ignored.
+        max_wait: int, optional
+            Max time to wait for training data assignment.
+            If set to None - method will return without waiting.
+            Defaults to 10 minutes.
 
         Returns
         -------
         CustomModelVersion
             created custom model version
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
+        datarobot.errors.InvalidUsageError
+            If wrong parameters are provided.
+        datarobot.errors.TrainingDataAssignmentError
+            If training data assignment fails.
+
+        Examples
+        --------
+        Create a version with blocking (default max_wait=600) training data assignment:
+
+        .. code-block:: python
+
+            import datarobot as dr
+            from datarobot.errors import TrainingDataAssignmentError
+
+            dr.Client(token=my_token, endpoint=endpoint)
+
+            try:
+                version = dr.CustomModelVersion.create_from_previous(
+                    custom_model_id="6444482e5583f6ee2e572265",
+                    base_environment_id="642209acc563893014a41e24",
+                    training_dataset_id="6421f2149a4f9b1bec6ad6dd",
+                )
+            except TrainingDataAssignmentError as e:
+                print(e)
+
+        Create a version with non-blocking training data assignment:
+
+        .. code-block:: python
+
+            import datarobot as dr
+
+            dr.Client(token=my_token, endpoint=endpoint)
+
+            version = dr.CustomModelVersion.create_from_previous(
+                custom_model_id="6444482e5583f6ee2e572265",
+                base_environment_id="642209acc563893014a41e24",
+                training_dataset_id="6421f2149a4f9b1bec6ad6dd",
+                max_wait=None,
+            )
+
+            while version.training_data.assignment_in_progress:
+                time.sleep(10)
+                version.refresh()
+            if version.training_data.assignment_error:
+                print(version.training_data.assignment_error["message"])
+
         """
-        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):
-            files = [(filename, os.path.basename(filename)) for filename in files]
+        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):  # type: ignore[unreachable]
+            files = [(filename, os.path.basename(filename)) for filename in files]  # type: ignore[unreachable]
         if files_to_delete:
             upload_data = [("filesToDelete", file_id) for file_id in files_to_delete]
         else:
             upload_data = None
         return cls._create(
             "patch",
             custom_model_id,
@@ -665,55 +956,106 @@
             folder_path,
             files,
             upload_data,
             network_egress_policy,
             maximum_memory,
             replicas,
             required_metadata_values=required_metadata_values,
+            training_dataset_id=training_dataset_id,
+            partition_column=partition_column,
+            holdout_dataset_id=holdout_dataset_id,
+            keep_training_holdout_data=keep_training_holdout_data,
+            max_wait=max_wait,
         )
 
     @classmethod
-    def _create(  # pylint: disable=missing-function-docstring
+    def _create(
         cls,
-        method,
-        custom_model_id,
-        is_major_update,
-        base_environment_id,
-        folder_path=None,
-        files=None,
-        extra_upload_data=None,
-        network_egress_policy=None,
-        maximum_memory=None,
-        replicas=None,
-        required_metadata_values=None,
-    ):
+        method: str,
+        custom_model_id: str,
+        is_major_update: bool,
+        base_environment_id: str,
+        folder_path: Optional[str],
+        files: Optional[List[Tuple[str, str]]],
+        extra_upload_data: Optional[List[Tuple[str, Any]]],
+        network_egress_policy: Optional[NETWORK_EGRESS_POLICY],
+        maximum_memory: Optional[int],
+        replicas: Optional[int],
+        required_metadata_values: Optional[List[RequiredMetadataValue]],
+        training_dataset_id: Optional[str],
+        partition_column: Optional[str],
+        holdout_dataset_id: Optional[str],
+        keep_training_holdout_data: Optional[bool],
+        max_wait: Optional[int],
+    ) -> CustomModelVersion:
+        # TODO: pass model object
+        """Create a custom model version"""
+
+        def _wait_for_training_data_assignment(version: CustomModelVersion) -> None:
+            # This check is needed to make sure user explicitly passes new training data.
+            # Checking only for `version.training_data.assignment_in_progress` is not enough as it is not known
+            # whether this training data is new or copied from the previous version.
+            # TODO: replace `not holdout_dataset_id` with `not model.is_unstructured_model_kind`
+            #  once `model` entity is introduced in the API
+            if training_dataset_id and max_wait and not holdout_dataset_id:
+                start_time = time.time()
+                while time.time() < start_time + max_wait:
+                    version.refresh()
+                    if (
+                        not version.training_data
+                        or not version.training_data.assignment_in_progress
+                    ):
+                        break
+                    time.sleep(5)
+
+                if version.training_data and version.training_data.assignment_error:
+                    raise TrainingDataAssignmentError(
+                        version.custom_model_id,
+                        version.id,
+                        version.training_data.assignment_error["message"],
+                    )
+
         url = cls._path.format(custom_model_id)
 
         with contextlib.ExitStack() as stack:
-            upload_data = [
+            # TODO: add training data params checks depending on structured/unstructured model kind.
+            if not training_dataset_id and (holdout_dataset_id or partition_column):
+                raise InvalidUsageError(
+                    "It is not allowed to provide holdout data or partition column without training data."
+                )
+
+            if holdout_dataset_id and partition_column:
+                raise InvalidUsageError(
+                    "It is not allowed to provide holdout_dataset_id and partition_column at the same time. "
+                    "For regular(structured) models you can provide training_dataset_id and partition_column. "
+                    "For unstructured models you can provide training_dataset_id and holdout_dataset_id."
+                )
+
+            if keep_training_holdout_data and (training_dataset_id or holdout_dataset_id):
+                raise InvalidUsageError(
+                    "It is not allowed to keep existing training/holdout data and to provide a new ones."
+                )
+
+            upload_data: List[Tuple[str, Any]] = [
                 ("isMajorUpdate", str(is_major_update)),
                 ("baseEnvironmentId", base_environment_id),
             ]
 
             if folder_path:
                 for root_path, _, file_paths in os.walk(folder_path):
                     for path in file_paths:
                         file_path = os.path.join(root_path, path)
-                        file = stack.enter_context(
-                            open(file_path, "rb")  # pylint: disable=consider-using-with
-                        )
+                        file = stack.enter_context(open(file_path, "rb"))
 
                         upload_data.append(("file", (os.path.basename(file_path), file)))
                         upload_data.append(("filePath", os.path.relpath(file_path, folder_path)))
 
             if files:
                 for file_path, upload_file_path in files:
-                    file = stack.enter_context(
-                        open(file_path, "rb")  # pylint: disable=consider-using-with
-                    )
+                    file = stack.enter_context(open(file_path, "rb"))
 
                     upload_data.append(("file", (os.path.basename(upload_file_path), file)))
                     upload_data.append(("filePath", upload_file_path))
 
             if extra_upload_data:
                 upload_data += extra_upload_data
 
@@ -735,162 +1077,191 @@
                                 {camelize(k): v for k, v in val.to_dict().items()}
                                 for val in required_metadata_values
                             ]
                         ),
                     )
                 )
 
+            if training_dataset_id:
+                keep_training_holdout_data = False
+
+                td_payload = {
+                    "datasetId": training_dataset_id,
+                }
+                upload_data.append(("trainingData", json.dumps(td_payload)))
+
+                # If holdout data is not provided don't include it in the payload with None values.
+                # There should be more checks added in the API.
+                hd_payload = {}
+                if holdout_dataset_id:
+                    hd_payload["datasetId"] = holdout_dataset_id
+                if partition_column:
+                    hd_payload["partitionColumn"] = partition_column
+
+                if len(hd_payload):
+                    upload_data.append(("holdoutData", json.dumps(hd_payload)))
+            if keep_training_holdout_data is not None:
+                upload_data.append(("keepTrainingHoldoutData", str(keep_training_holdout_data)))
+
             encoder = MultipartEncoder(fields=upload_data)
             headers = {"Content-Type": encoder.content_type}
             response = cls._client.request(method, url, data=encoder, headers=headers)
-            return cls.from_server_data(response.json())
+            new_version = cls.from_server_data(response.json())
+
+            _wait_for_training_data_assignment(new_version)
+
+        return new_version
 
     @classmethod
-    def list(cls, custom_model_id):
+    def list(cls, custom_model_id: str) -> List[CustomModelVersion]:
         """List custom model versions.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            the id of the custom model
+            The ID of the custom model.
 
         Returns
         -------
         List[CustomModelVersion]
-            a list of custom model versions
+            A list of custom model versions.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         url = cls._path.format(custom_model_id)
         data = unpaginate(url, None, cls._client)
         return [cls.from_server_data(item) for item in data]
 
     @classmethod
-    def get(cls, custom_model_id, custom_model_version_id):
+    def get(cls, custom_model_id: str, custom_model_version_id: str) -> CustomModelVersion:
         """Get custom model version by id.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            the id of the custom model
+            The ID of the custom model.
         custom_model_version_id: str
-            the id of the custom model version to retrieve
+            The id of the custom model version to retrieve.
 
         Returns
         -------
         CustomModelVersion
-            retrieved custom model version
+            Retrieved custom model version.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
         url = cls._path.format(custom_model_id)
         path = f"{url}{custom_model_version_id}/"
         return cls.from_location(path)
 
-    def download(self, file_path):
+    def download(self, file_path: str) -> None:
         """Download custom model version.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         file_path: str
-            path to create a file with custom model version content
+            Path to create a file with custom model version content.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/download/"
 
         response = self._client.get(path)
         with open(file_path, "wb") as f:
             f.write(response.content)
 
-    def update(self, description=None, required_metadata_values=None):
+    def update(
+        self,
+        description: Optional[str] = None,
+        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
+    ) -> None:
         """Update custom model version properties.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
-        description: str
-            new custom model version description
-        required_metadata_values: List[RequiredMetadataValue]
+        description: str, optional
+            New custom model version description.
+        required_metadata_values: List[RequiredMetadataValue], optional
             Additional parameters required by the execution environment. The required keys are
             defined by the fieldNames in the base environment's requiredMetadataKeys.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
-        payload = {}
+        payload: Dict[str, Any] = {}
         if description:
             payload.update({"description": description})
 
         if required_metadata_values is not None:
             payload.update(
                 {"requiredMetadataValues": [val.to_dict() for val in required_metadata_values]}
             )
 
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/"
 
         response = self._client.patch(path, data=payload)
 
         data = response.json()
-        self._set_values(**self._safe_data(data, do_recursive=True))
+        self._set_values(**self._safe_data(data, do_recursive=True))  # type: ignore[no-untyped-call]
         # _safe_data will make the keys in requiredMetadata lowercase,
         # which is not OK. we need to preserve case
         self.required_metadata = data.get(  # pylint: disable=attribute-defined-outside-init
             "requiredMetadata"
         )
 
-    def refresh(self):
+    def refresh(self) -> None:
         """Update custom model version with the latest data from server.
 
         .. versionadded:: v2.21
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status
+            If the server responded with 5xx status.
         """
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/"
 
         response = self._client.get(path)
 
         data = response.json()
-        self._set_values(**self._safe_data(data, do_recursive=True))
+        self._set_values(**self._safe_data(data, do_recursive=True))  # type: ignore[no-untyped-call]
 
-    def get_feature_impact(self, with_metadata=False):
+    def get_feature_impact(self, with_metadata: bool = False) -> List[Dict[str, Any]]:
         """Get custom model feature impact.
 
         .. versionadded:: v2.23
 
         Parameters
         ----------
         with_metadata : bool
@@ -901,33 +1272,34 @@
         feature_impacts : list of dict
            The feature impact data. Each item is a dict with the keys 'featureName',
            'impactNormalized', and 'impactUnnormalized', and 'redundantWith'.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/featureImpact/"
         data = self._client.get(path).json()
         data = custom_model_feature_impact_trafaret.check(data)
-        return filter_feature_impact_result(data, with_metadata=with_metadata)
+        ret = filter_feature_impact_result(data, with_metadata=with_metadata)  # type: ignore[no-untyped-call]
+        return ret  # type: ignore[no-any-return]
 
-    def calculate_feature_impact(self, max_wait=DEFAULT_MAX_WAIT):
+    def calculate_feature_impact(self, max_wait: int = DEFAULT_MAX_WAIT) -> None:
         """Calculate custom model feature impact.
 
         .. versionadded:: v2.23
 
         Parameters
         ----------
         max_wait: int, optional
-            max time to wait for feature impact calculation.
+            Max time to wait for feature impact calculation.
             If set to None - method will return without waiting.
             Defaults to 10 min
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status
@@ -946,21 +1318,21 @@
     """A conversion of a DataRobot custom model version.
 
     .. versionadded:: v2.27
 
     Attributes
     ----------
     id: str
-        ID of the custom model version conversion.
+        The ID of the custom model version conversion.
     custom_model_version_id: str
-        ID of the custom model version.
+        The ID of the custom model version.
     created: str
         ISO-8601 timestamp of when the custom model conversion created.
     main_program_item_id: str or None
-        ID of the main program item.
+        The ID of the main program item.
     log_message: str or None
         The conversion output log message.
     generated_metadata: dict or None
         The dict contains two items: 'outputDataset' & 'outputColumns'.
     conversion_succeeded: bool
         Whether the conversion succeeded or not.
     conversion_in_progress: bool
@@ -990,117 +1362,121 @@
             t.Key("conversion_in_progress", optional=True): t.Bool() | t.Null(),
             t.Key("should_stop", optional=True): t.Bool(),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: Any) -> None:
         self._set_values(**kwargs)
         self.custom_model_id = None
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.id!r})"
 
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
-        id,
-        custom_model_version_id,
-        created,
-        main_program_item_id=None,
-        log_message=None,
-        generated_metadata=None,
-        conversion_succeeded=None,
-        conversion_in_progress=None,
-        should_stop=None,
-    ):
+        id: str,
+        custom_model_version_id: str,
+        created: str,
+        main_program_item_id: Optional[str] = None,
+        log_message: Optional[str] = None,
+        generated_metadata: Optional[Dict[str, Union[List[str], List[List[str]]]]] = None,
+        conversion_succeeded: Optional[bool] = None,
+        conversion_in_progress: Optional[bool] = None,
+        should_stop: Optional[bool] = None,
+    ) -> None:
         self.id = id
         self.custom_model_version_id = custom_model_version_id
         self.created = created
         self.main_program_item_id = main_program_item_id
         self.log_message = log_message
         self.generated_metadata = generated_metadata
         self.conversion_succeeded = conversion_succeeded
         self.conversion_in_progress = conversion_in_progress
         self.should_stop = should_stop
 
     @classmethod
     def run_conversion(
         cls,
-        custom_model_id,
-        custom_model_version_id,
-        main_program_item_id,
-        max_wait=None,
-    ):
+        custom_model_id: str,
+        custom_model_version_id: str,
+        main_program_item_id: str,
+        max_wait: Optional[int] = None,
+    ) -> str:
         """Initiate a new custom model version conversion.
 
         Parameters
         ----------
         custom_model_id : str
             The associated custom model ID.
         custom_model_version_id : str
             The associated custom model version ID.
         main_program_item_id : str
             The selected main program item ID. This should be one of the SAS items in the
             associated custom model version.
         max_wait: int or None
-            Max wait time in seconds. If None, than don't wait.
+            Max wait time in seconds. If None, then don't wait.
 
         Returns
         -------
         conversion_id : str
             The ID of the newly created conversion entity.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx statuscustom model conversion
+            If the server responded with 5xx status.
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         payload = {"mainProgramItemId": main_program_item_id}
         response = cls._client.post(base_conversion_url, json=payload)
         if max_wait is not None:
             wait_for_async_resolution(cls._client, response.headers["Location"], max_wait)
-        return response.json()["conversionId"]
+        return cast(str, response.json()["conversionId"])
 
     @classmethod
-    def stop_conversion(cls, custom_model_id, custom_model_version_id, conversion_id):
+    def stop_conversion(
+        cls, custom_model_id: str, custom_model_version_id: str, conversion_id: str
+    ) -> Response:
         """
         Stop a conversion that is in progress.
 
         Parameters
         ----------
         custom_model_id : str
-            ID of the associated custom model.
+            The ID of the associated custom model.
         custom_model_version_id : str
-            ID of the associated custom model version.
+            The ID of the associated custom model version.
         conversion_id :
-            ID of a conversion that is in-progress.
+            THe ID of a conversion that is in-progress.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
 
         conversion = cls.get(custom_model_id, custom_model_version_id, conversion_id)
         if not conversion.conversion_in_progress:
             raise InvalidUsageError("You may only stop a conversion that is in progress.")
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         conversion_entity_url = "{}{}/".format(base_conversion_url, conversion_id)
-        return cls._client.delete(conversion_entity_url)
+        return cast(Response, cls._client.delete(conversion_entity_url))
 
     @classmethod
-    def get(cls, custom_model_id, custom_model_version_id, conversion_id):
+    def get(
+        cls, custom_model_id: str, custom_model_version_id: str, conversion_id: str
+    ) -> CustomModelVersionConversion:
         """Get custom model version conversion by id.
 
         .. versionadded:: v2.27
 
         Parameters
         ----------
         custom_model_id: str
@@ -1114,25 +1490,27 @@
         -------
         CustomModelVersionConversion
             Retrieved custom model version conversion.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         conversion_entity_url = "{}{}/".format(base_conversion_url, conversion_id)
         return cls.from_location(conversion_entity_url)
 
     @classmethod
-    def get_latest(cls, custom_model_id, custom_model_version_id):
+    def get_latest(
+        cls, custom_model_id: str, custom_model_version_id: str
+    ) -> Optional[CustomModelVersionConversion]:
         """Get latest custom model version conversion for a given custom model version.
 
         .. versionadded:: v2.27
 
         Parameters
         ----------
         custom_model_id: str
@@ -1144,25 +1522,27 @@
         -------
         CustomModelVersionConversion or None
             Retrieved latest conversion for a given custom model version.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         data = unpaginate(base_conversion_url, {"isLatest": True}, cls._client)
         return cls.from_server_data(next(data))
 
     @classmethod
-    def list(cls, custom_model_id, custom_model_version_id):
+    def list(
+        cls, custom_model_id: str, custom_model_version_id: str
+    ) -> List[CustomModelVersionConversion]:
         """Get custom model version conversions list per custom model version.
 
         .. versionadded:: v2.27
 
         Parameters
         ----------
         custom_model_id: str
@@ -1174,15 +1554,15 @@
         -------
         List[CustomModelVersionConversion]
             Retrieved conversions for a given custom model version.
 
         Raises
         ------
         datarobot.errors.ClientError
-            if the server responded with 4xx status.
+            If the server responded with 4xx status.
         datarobot.errors.ServerError
-            if the server responded with 5xx status.
+            If the server responded with 5xx status.
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         data = unpaginate(base_conversion_url, None, cls._client)
         return [cls.from_server_data(item) for item in data]
```

### Comparing `datarobot-3.1.1/datarobot/models/custom_task.py` & `datarobot-3.2.0b0/datarobot/models/custom_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
         - `datarobot.enums.CUSTOM_TASK_TARGET_TYPE.ANOMALY`
         - `datarobot.enums.CUSTOM_TASK_TARGET_TYPE.TRANSFORM`
     latest_version: datarobot.CustomTaskVersion or None
         latest version of the custom task if the task has a latest version. If the
         latest version is None, the custom task is not ready for use in user blueprints.
         You must create its first CustomTaskVersion before you can use the CustomTask
     created_by: str
-        username of a user who user who created the custom task
+        The username of the user who created the custom task.
     updated_at: str
-        ISO-8601 formatted timestamp of when the custom task was updated
+        An ISO-8601 formatted timestamp of when the custom task was updated.
     created_at: str
         ISO-8601 formatted timestamp of when the custom task was created
     calibrate_predictions: bool
         whether anomaly predictions should be calibrated to be between 0 and 1 by DR.
         only applies to custom estimators with target type
         `datarobot.enums.CUSTOM_TASK_TARGET_TYPE.ANOMALY`
     """
```

### Comparing `datarobot-3.1.1/datarobot/models/custom_task_version.py` & `datarobot-3.2.0b0/datarobot/models/custom_task_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,17 +357,15 @@
         cls._verify_folder_path(folder_path)
 
         with contextlib.ExitStack() as stack:
             if folder_path:
                 for dir_name, _, file_names in os.walk(folder_path):
                     for file_name in file_names:
                         file_path = os.path.join(dir_name, file_name)
-                        file = stack.enter_context(
-                            open(file_path, "rb")  # pylint: disable=consider-using-with
-                        )
+                        file = stack.enter_context(open(file_path, "rb"))
 
                         upload_data.append(("file", (os.path.basename(file_path), file)))
                         upload_data.append(("filePath", os.path.relpath(file_path, folder_path)))
 
             encoder = MultipartEncoder(fields=upload_data)
             headers = {"Content-Type": encoder.content_type}
             response = cls._client.request(method, url, data=encoder, headers=headers)
```

### Comparing `datarobot-3.1.1/datarobot/models/custom_task_version_dependency_build.py` & `datarobot-3.2.0b0/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/data_drift.py` & `datarobot-3.2.0b0/datarobot/models/deployment/data_drift.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,28 +8,56 @@
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, TYPE_CHECKING
 
 import dateutil
 import trafaret as t
 
 from datarobot._compat import Int, String
+from datarobot.enums import BUCKET_SIZE, DATA_DRIFT_METRIC
 from datarobot.models.api_object import APIObject
+from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
+from datarobot.utils import from_api
 
-from ..enums import DATA_DRIFT_METRIC
-from ..helpers.deployment_monitoring import DeploymentQueryBuilderMixin
-from ..utils import from_api
+if TYPE_CHECKING:
+    from mypy_extensions import TypedDict
 
+    class Period(TypedDict, total=False):
+        start: datetime
+        end: datetime
+
+    class Percentile(TypedDict, total=False):
+        percent: float
+        value: float
+
+    class MeanProbability(TypedDict, total=False):
+        class_name: str
+        value: float
+
+    class ClassDistribution(TypedDict, total=False):
+        class_name: str
+        count: int
+        percent: float
+
+    class PredictionsOverTimeBucket(TypedDict, total=False):
+        period: Period
+        model_id: str
+        row_count: Optional[int]
+        mean_predicted_value: Optional[int]
+        percentiles: List[Percentile]
+        mean_probabilities: List[MeanProbability]
+        class_distribution: List[ClassDistribution]
 
-class TargetDrift(APIObject, DeploymentQueryBuilderMixin):
+
+class TargetDrift(APIObject, MonitoringDataQueryBuilderMixin):
     """Deployment target drift information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve target drift metric
     period : dict
@@ -145,15 +173,15 @@
         if metric:
             params["metric"] = metric
         data = cls._client.get(path, params=params).json()
         data = from_api(data, keep_null_keys=True)
         return cls.from_data(data)
 
 
-class FeatureDrift(APIObject, DeploymentQueryBuilderMixin):
+class FeatureDrift(APIObject, MonitoringDataQueryBuilderMixin):
     """Deployment feature drift information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve feature drift metric
     period : dict
@@ -290,7 +318,93 @@
         while response_json["next"] is not None:
             response_json = cls._client.get(response_json["next"]).json()
             response_json = from_api(response_json, keep_null_keys=True)
             for item in response_json["data"]:
                 data.append(_from_data_item(item))
 
         return data
+
+
+class PredictionsOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+    """Deployment predictions over time information.
+
+    Attributes
+    ----------
+    baselines : List
+        target baseline for each model queried
+    buckets : List
+        predictions over time bucket for each model and bucket queried
+    """
+
+    _path = "deployments/{}/predictionsOverTime/"
+    _period = t.Dict(
+        {
+            t.Key("start"): String >> dateutil.parser.parse,
+            t.Key("end"): String >> dateutil.parser.parse,
+        }
+    )
+    _converter = t.Dict(
+        {
+            t.Key("baselines"): t.List(t.Dict().allow_extra("*")),
+            t.Key("buckets"): t.List(t.Dict({"period": _period}).allow_extra("*")),
+        }
+    )
+
+    def __init__(
+        self,
+        baselines: Optional[List[PredictionsOverTimeBucket]] = None,
+        buckets: Optional[List[PredictionsOverTimeBucket]] = None,
+    ):
+        self.baselines = baselines or []
+        self.buckets = buckets or []
+
+    @classmethod
+    def get(
+        cls,
+        deployment_id: str,
+        model_ids: Optional[List[str]] = None,
+        start_time: Optional[datetime] = None,
+        end_time: Optional[datetime] = None,
+        bucket_size: Optional[BUCKET_SIZE] = None,
+        target_classes: Optional[List[str]] = None,
+        include_percentiles: Optional[bool] = False,
+    ) -> PredictionsOverTime:
+        """Retrieve information for deployment's prediction response over a certain time period.
+
+        .. versionadded:: v3.2
+
+        Parameters
+        ----------
+        deployment_id : str
+            the id of the deployment
+        model_ids : list[str]
+            ID of models to retrieve prediction stats
+        start_time : datetime
+            start of the time period
+        end_time : datetime
+            end of the time period
+        bucket_size : BUCKET_SIZE
+            time duration of each bucket
+        target_classes : list[str]
+            class names of target, only for deployments with multiclass target
+        include_percentiles : bool
+            if the returned data includes percentiles,
+            only for a deployment with a binary and regression target
+
+        Returns
+        -------
+        predictions_over_time : PredictionsOverTime
+            the queried predictions over time information
+        """
+
+        path = cls._path.format(deployment_id)
+        params = cls._build_query_params(
+            start_time=start_time,
+            end_time=end_time,
+            model_ids=model_ids,
+            bucket_size=bucket_size,
+            target_class=target_classes,
+            include_percentiles=include_percentiles,
+        )
+        data = cls._client.get(path, params=params).json()
+        case_converted = from_api(data, keep_null_keys=True)
+        return cls.from_data(case_converted)
```

### Comparing `datarobot-3.1.1/datarobot/models/data_engine_query_generator.py` & `datarobot-3.2.0b0/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/data_source.py` & `datarobot-3.2.0b0/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/data_store.py` & `datarobot-3.2.0b0/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/dataset.py` & `datarobot-3.2.0b0/datarobot/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -26,14 +26,15 @@
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject
 from datarobot.models.credential import CredentialDataSchema
 from datarobot.models.feature import DatasetFeature
 from datarobot.models.featurelist import DatasetFeaturelist
 from datarobot.models.project import Project
 from datarobot.models.sharing import SharingAccess
+from datarobot.models.use_cases.utils import add_to_use_case, resolve_use_cases, UseCaseLike
 from datarobot.utils import assert_single_parameter, dataframe_to_buffer
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
 from datarobot.utils.sourcedata import list_of_records_to_buffer
 from datarobot.utils.waiters import wait_for_async_resolution
 
 from ..enums import DEFAULT_MAX_WAIT, DEFAULT_TIMEOUT
@@ -199,14 +200,15 @@
             return cls.create_from_file(file_path=cast(str, source))
         elif source_type == LocalSourceType.DATA_FRAME:
             return cls.create_from_in_memory_data(data_frame=source)
         elif source_type == LocalSourceType.FILELIKE:
             return cls.create_from_file(filelike=cast(IOBase, source))
 
     @classmethod
+    @add_to_use_case(allow_multiple=True)
     def create_from_file(
         cls: Type[TDataset],
         file_path: Optional[str] = None,
         filelike: Optional[IOBase] = None,
         categories: Optional[List[str]] = None,
         read_timeout: int = DEFAULT_TIMEOUT.UPLOAD,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -230,14 +232,17 @@
             An array of strings describing the intended use of the dataset. The
             current supported options are "TRAINING" and "PREDICTION".
         read_timeout: int, optional
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful
+        use_cases: list[UseCase] | UseCase | list[string] | string, optional
+            A list of UseCase objects, UseCase object,
+            list of Use Case ids or a single Use Case id to add this new Dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             A fully armed and operational Dataset
         """
         assert_single_parameter(("filelike", "file_path"), file_path, filelike)
@@ -268,14 +273,15 @@
         )
         dataset = cls.from_location(new_dataset_location)
         if categories:
             dataset.modify(categories=categories)
         return dataset
 
     @classmethod
+    @add_to_use_case(allow_multiple=True)
     def create_from_in_memory_data(
         cls: Type[TDataset],
         data_frame: Optional[pd.DataFrame] = None,
         records: Optional[List[Dict[str, Any]]] = None,
         categories: Optional[List[str]] = None,
         read_timeout: int = DEFAULT_TIMEOUT.UPLOAD,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -301,14 +307,17 @@
         read_timeout: int, optional
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful
         fname: string, optional
             The file name, "data.csv" by default
+        use_cases: list[UseCase] | UseCase | list[string] | string, optional
+            A list of UseCase objects, UseCase object,
+            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data.
 
         Raises
@@ -329,14 +338,15 @@
             filelike=buff,
             categories=categories,
             read_timeout=read_timeout,
             max_wait=max_wait,
         )
 
     @classmethod
+    @add_to_use_case(allow_multiple=True)
     def create_from_url(
         cls: Type[TDataset],
         url: str,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
         categories: Optional[List[str]] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -363,14 +373,17 @@
             available. Specifying this parameter to false and `doSnapshot` to true will result in
             an error.
         categories: list[string], optional
             An array of strings describing the intended use of the dataset. The
             current supported options are "TRAINING" and "PREDICTION".
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful.
+        use_cases: list[UseCase] | UseCase | list[string] | string, optional
+            A list of UseCase objects, UseCase object,
+            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data
         """
         base_data = {
@@ -385,14 +398,15 @@
 
         new_dataset_location = wait_for_async_resolution(
             cls._client, response.headers["Location"], max_wait
         )
         return cls.from_location(new_dataset_location)
 
     @classmethod
+    @add_to_use_case(allow_multiple=True)
     def create_from_data_source(
         cls: Type[TDataset],
         data_source_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
@@ -441,15 +455,17 @@
             If unset, uses the server default: False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         max_wait: int, optional
             Time in seconds after which project creation is considered unsuccessful.
-
+        use_cases: list[UseCase] | UseCase | list[string] | string, optional
+            A list of UseCase objects, UseCase object,
+            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data
         """
         base_data = {
@@ -473,14 +489,15 @@
 
         new_dataset_location = wait_for_async_resolution(
             cls._client, response.headers["Location"], max_wait
         )
         return cls.from_location(new_dataset_location)
 
     @classmethod
+    @add_to_use_case(allow_multiple=True)
     def create_from_query_generator(
         cls: Type[TDataset],
         generator_id: str,
         dataset_id: Optional[str] = None,
         dataset_version_id: Optional[str] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TDataset:
@@ -499,14 +516,17 @@
         dataset_id: str, optional
             The id of the dataset to apply the query to.
         dataset_version_id: str, optional
             The id of the dataset version to apply the query to. If not specified the
             latest version associated with dataset_id (if specified) is used.
         max_wait : int
             optional, the maximum number of seconds to wait before giving up.
+        use_cases: list[UseCase] | UseCase | list[string] | string, optional
+            A list of UseCase objects, UseCase object,
+            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the query generator
         """
         url = "dataEngineWorkspaceStates/fromDataEngineQueryGenerator/"
@@ -581,14 +601,15 @@
 
     @classmethod
     def list(
         cls: Type[TDataset],
         category: Optional[str] = None,
         filter_failed: Optional[bool] = None,
         order_by: Optional[str] = None,
+        use_cases: Optional[UseCaseLike] = None,
     ) -> List[TDataset]:
         """
         List all datasets a user can view.
 
 
         Parameters
         ----------
@@ -604,30 +625,41 @@
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
 
+        use_cases: Union[UseCase, List[UseCase], str, List[str]], optional
+            Filter available datasets by a specific Use Case or Cases. Accepts either the entity or the ID.
+
         Returns
         -------
         list[Dataset]
             a list of datasets the user can view
 
         """
-        return list(cls.iterate(category=category, order_by=order_by, filter_failed=filter_failed))
+        return list(
+            cls.iterate(
+                category=category,
+                order_by=order_by,
+                filter_failed=filter_failed,
+                use_cases=use_cases,
+            )
+        )
 
     @classmethod
     def iterate(
         cls: Type[TDataset],
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         category: Optional[str] = None,
         order_by: Optional[str] = None,
         filter_failed: Optional[bool] = None,
+        use_cases: Optional[UseCaseLike] = None,
     ) -> Generator[TDataset, None, None]:
         """
         Get an iterator for the requested datasets a user can view.
         This lazily retrieves results. It does not get the next page from the server until the
         current page is exhausted.
 
         Parameters
@@ -651,27 +683,31 @@
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
 
+        use_cases: Union[UseCase, List[UseCase], str, List[str]], optional
+            Filter available datasets by a specific Use Case or Cases. Accepts either the entity or the ID.
+
         Yields
         ------
         Dataset
             An iterator of the datasets the user can view
 
         """
         all_params = {
             "offset": offset,
             "limit": limit,
             "category": category,
             "order_by": order_by,
             "filter_failed": filter_failed,
         }
+        all_params = resolve_use_cases(use_cases=use_cases, params=all_params)
         params = _remove_empty_params(all_params)
         _update_filter_failed(params)
 
         for dataset_json in unpaginate(cls._path, params, cls._client):
             yield cls.from_server_data(dataset_json)
 
     def update(self) -> None:
@@ -957,14 +993,15 @@
         Returns
         -------
         locations: list[ProjectLocation]
         """
         url = f"{self._path}{self.id}/projects/"
         return [ProjectLocation(**kwargs) for kwargs in unpaginate(url, None, self._client)]
 
+    @add_to_use_case(allow_multiple=True)
     def create_project(
         self,
         project_name: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         credential_id: Optional[str] = None,
         use_kerberos: Optional[bool] = None,
@@ -988,14 +1025,17 @@
             The ID of the set of credentials to use instead of user and password.
         use_kerberos: bool, optional
             Server default is False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
+        use_cases: list[UseCase] | UseCase | list[string] | string, optional
+            A list of UseCase objects, UseCase object,
+            list of Use Case ids or a single Use Case id to add this new Dataset to. Must be a kwarg.
 
         Returns
         -------
         Project
         """
         return Project.create_from_dataset(
             self.id,
```

### Comparing `datarobot-3.1.1/datarobot/models/datetime_trend_plots.py` & `datarobot-3.2.0b0/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/deployment.py` & `datarobot-3.2.0b0/datarobot/models/deployment/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,40 @@
 
 import dateutil
 import pandas as pd
 import pytz
 import trafaret as t
 
 from datarobot._compat import String
-from datarobot.enums import ACCURACY_METRIC, DEFAULT_MAX_WAIT, FileLocationType, LocalSourceType
+from datarobot.enums import (
+    ACCURACY_METRIC,
+    BUCKET_SIZE,
+    DEFAULT_MAX_WAIT,
+    FileLocationType,
+    LocalSourceType,
+)
 from datarobot.errors import InvalidUsageError
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject, ServerDataDictType
 from datarobot.models.batch_prediction_job import BatchPredictionJob
 from datarobot.models.custom_model_version import CustomModelVersion
+from datarobot.models.deployment.accuracy import Accuracy, AccuracyOverTime
+from datarobot.models.deployment.bias_and_fairness import FairnessScoresOverTime
+from datarobot.models.deployment.data_drift import FeatureDrift, PredictionsOverTime, TargetDrift
+from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
+from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
+from datarobot.models.deployment.sharing import (
+    DeploymentGrantSharedRoleWithId,
+    DeploymentGrantSharedRoleWithUsername,
+    DeploymentSharedRole,
+)
 from datarobot.utils import deprecated, from_api, get_id_from_location
+from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
-
-from ..helpers.deployment_monitoring import DeploymentQueryBuilderMixin
-from ..utils.pagination import unpaginate
-from ..utils.waiters import wait_for_async_resolution
-from .accuracy import Accuracy, AccuracyOverTime
-from .data_drift import FeatureDrift, TargetDrift
-from .service_stats import ServiceStats, ServiceStatsOverTime
+from datarobot.utils.waiters import wait_for_async_resolution
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.batch_prediction_job import IntakeSettings
 
     class FeatureDict(TypedDict):
@@ -100,25 +111,42 @@
 
     class ChallengerModelsSettings(Settings):
         pass
 
     class PredictionIntervalsSettings(Settings):
         percentiles: list[int]
 
+    class BiasAndFairnessSettings(TypedDict):
+        protected_features: List[str]
+        preferable_target_value: bool
+        fairness_metric_set: str
+        fairness_threshold: float
+
     class Actual(TypedDict):
         association_id: str
         actual_value: Union[str, int, float]
         was_acted_on: Optional[bool]
         timestamp: Union[datetime, str]
 
 
 TDeployment = TypeVar("TDeployment", bound="Deployment")
 
 
-class Deployment(APIObject, DeploymentQueryBuilderMixin, BrowserMixin):
+def _check(trafaret: t, value: Any, default_to_null: bool = True) -> Any:
+    if default_to_null and value is None:
+        return None
+
+    # Allow users to pass a single value even if a list of values is expected.
+    if isinstance(trafaret, t.List) and not isinstance(value, list):
+        value = [value]
+
+    return trafaret.check(value)
+
+
+class Deployment(APIObject, MonitoringDataQueryBuilderMixin, BrowserMixin):
     """A deployment created from a DataRobot model.
 
     Attributes
     ----------
     id : str
         the id of the deployment
     label : str
@@ -1166,14 +1194,78 @@
         payload["segment_analysis"]["enabled"] = segment_analysis_enabled
         if segment_analysis_attributes:
             payload["segment_analysis"]["attributes"] = segment_analysis_attributes
         url = f"{self._path}{self.id}/settings/"
         response = self._client.patch(url, data=payload)
         wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
 
+    def get_bias_and_fairness_settings(self) -> Optional[BiasAndFairnessSettings]:
+        """Retrieve bias and fairness settings of this deployment.
+
+        ..versionadded:: v3.2.0
+
+        Returns
+        -------
+        settings : dict in the following format:
+            protected_features : List[str]
+                A list of features to mark as protected.
+            preferable_target_value : bool
+                A target value that should be treated as a positive outcome for the prediction.
+            fairness_metric_set : str
+                Can be one of <datarobot.enums.FairnessMetricsSet>.
+                A set of fairness metrics to use for calculating fairness.
+            fairness_threshold : float
+                Threshold value of the fairness metric. Cannot be less than 0 or greater than 1.
+        """
+        url = f"{self._path}/{self.id}/settings/"
+        response = cast(ServerDataDictType, from_api(self._client.get(url).json()))
+        return cast("BiasAndFairnessSettings", response.get("bias_and_fairness"))
+
+    def update_bias_and_fairness_settings(
+        self,
+        protected_features: List[str],
+        fairness_metric_set: str,
+        fairness_threshold: float,
+        preferable_target_value: Union[bool, int, str],
+        max_wait: int = DEFAULT_MAX_WAIT,
+    ) -> None:
+        """Update bias and fairness settings of this deployment.
+
+        ..versionadded:: v3.2.0
+
+        Updating challenger models setting is an asynchronous process, which means some preparatory
+        work may be performed after the initial request is completed. This function will not return
+        until all preparatory work is fully finished.
+
+        Parameters
+        ----------
+        protected_features : List[str]
+            A list of features to mark as protected.
+        preferable_target_value : bool
+            A target value that should be treated as a positive outcome for the prediction.
+        fairness_metric_set : str
+             Can be one of <datarobot.enums.FairnessMetricsSet>.
+             The fairness metric used to calculate the fairness scores.
+        fairness_threshold : float
+            Threshold value of the fairness metric. Cannot be less than 0 or greater than 1.
+        max_wait : int, optional
+            seconds to wait for successful resolution
+        """
+        url = f"{self._path}/{self.id}/settings/"
+        payload = {
+            "biasAndFairness": {
+                "protectedFeatures": protected_features,
+                "fairnessMetricsSet": fairness_metric_set,
+                "fairnessThreshold": fairness_threshold,
+                "preferableTargetValue": preferable_target_value,
+            }
+        }
+        response = self._client.patch(url, json=payload)
+        wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
+
     def get_drift_tracking_settings(self) -> DriftTrackingSettings:
         """Retrieve drift tracking settings of this deployment.
 
         .. versionadded:: v2.17
 
         Returns
         -------
@@ -1500,15 +1592,15 @@
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         execution_time_quantile: Optional[float] = None,
         response_time_quantile: Optional[float] = None,
         slow_requests_threshold: Optional[float] = None,
     ) -> ServiceStats:
-        """Retrieve value of service stat metrics over a certain time period.
+        """Retrieves values of many service stat metrics aggregated over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         model_id : str, optional
             the id of the model
@@ -1548,15 +1640,15 @@
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[str] = None,
         quantile: Optional[float] = None,
         threshold: Optional[int] = None,
     ) -> ServiceStatsOverTime:
-        """Retrieve information about how a service stat metric changes over a certain time period.
+        """Retrieves values of a single service stat metric over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         metric : SERVICE_STAT_METRIC, optional
             the service stat metric to retrieve
@@ -1661,24 +1753,84 @@
         if not self.id:
             raise ValueError("Deployment ID is required to get feature drift.")
 
         return FeatureDrift.list(
             self.id, model_id=model_id, start_time=start_time, end_time=end_time, metric=metric
         )
 
+    def get_predictions_over_time(
+        self,
+        model_ids: Optional[List[str]] = None,
+        start_time: Optional[datetime] = None,
+        end_time: Optional[datetime] = None,
+        bucket_size: Optional[BUCKET_SIZE] = None,
+        target_classes: Optional[List[str]] = None,
+        include_percentiles: Optional[bool] = False,
+    ) -> PredictionsOverTime:
+        """Retrieve stats of deployment's prediction response over a certain time period.
+
+        .. versionadded:: v3.2
+
+        Parameters
+        ----------
+        model_ids : list[str]
+            ID of models to retrieve prediction stats
+        start_time : datetime
+            start of the time period
+        end_time : datetime
+            end of the time period
+        bucket_size : BUCKET_SIZE
+            time duration of each bucket
+        target_classes : list[str]
+            class names of target, only for deployments with multiclass target
+        include_percentiles : bool
+            if the returned data includes percentiles,
+            only for a deployment with a binary and regression target
+
+        Returns
+        -------
+        predictions_over_time : PredictionsOverTime
+            the queried predictions over time information
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from datarobot import Deployment
+            deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
+            predictions_over_time = deployment.get_predictions_over_time()
+            predictions_over_time.buckets[0]['mean_predicted_value']
+            >>>0.3772
+            predictions_over_time.buckets[0]['row_count']
+            >>>2000
+        """
+
+        if not self.id:
+            raise ValueError("Deployment ID is required to get predictions over time.")
+
+        return PredictionsOverTime.get(
+            self.id,
+            model_ids=model_ids,
+            start_time=start_time,
+            end_time=end_time,
+            bucket_size=bucket_size,
+            target_classes=target_classes,
+            include_percentiles=include_percentiles,
+        )
+
     def get_accuracy(
         self,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         start: Optional[datetime] = None,
         end: Optional[datetime] = None,
         target_classes: Optional[List[str]] = None,
     ) -> Accuracy:
-        """Retrieve values of accuracy metrics over a certain time period.
+        """Retrieves values of many accuracy metrics aggregated over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         model_id : str
             the id of the model
@@ -1715,15 +1867,15 @@
         metric: Optional[ACCURACY_METRIC] = None,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[str] = None,
         target_classes: Optional[List[str]] = None,
     ) -> AccuracyOverTime:
-        """Retrieve information about how an accuracy metric changes over a certain time period.
+        """Retrieves values of a single accuracy metric over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         metric : ACCURACY_METRIC
             the accuracy metric to retrieve
@@ -1753,14 +1905,59 @@
             model_id=model_id,
             start_time=start_time,
             end_time=end_time,
             bucket_size=bucket_size,
             target_classes=target_classes,
         )
 
+    def get_fairness_scores_over_time(
+        self,
+        start_time: Optional[datetime] = None,
+        end_time: Optional[datetime] = None,
+        bucket_size: Optional[BUCKET_SIZE] = None,
+        model_id: Optional[str] = None,
+        protected_feature: Optional[str] = None,
+        fairness_metric: Optional[str] = None,
+    ) -> FairnessScoresOverTime:
+        """Retrieves values of a single fairness score over a time period.
+
+        .. versionadded:: v3.2
+
+        Parameters
+        ----------
+        model_id : str
+            the id of the model
+        start_time : datetime
+            start of the time period
+        end_time : datetime
+            end of the time period
+        bucket_size : str
+            time duration of a bucket, in ISO 8601 time duration format
+        protected_feature : str
+            name of protected feature
+        fairness_metric : str
+            A consolidation of the fairness metrics by the use case.
+
+        Returns
+        -------
+        fairness_scores_over_time : FairnessScoresOverTime
+            the queried fairness score over time information
+        """
+        if not self.id:
+            raise ValueError("Deployment ID is required to get fairness score.")
+        return FairnessScoresOverTime.get(
+            self.id,
+            start_time=start_time,
+            end_time=end_time,
+            model_id=model_id,
+            bucket_size=bucket_size,
+            fairness_metric=fairness_metric,
+            protected_feature=protected_feature,
+        )
+
     def update_secondary_dataset_config(
         self,
         secondary_dataset_config_id: str,
         credential_ids: Optional[List[str]] = None,
     ) -> str:
         """Update the secondary dataset config used by Feature discovery model for a
         given deployment.
@@ -2024,24 +2221,87 @@
             payload["start"] = timezone_aware(start_time).isoformat()
         if end_time:
             payload["end"] = timezone_aware(end_time).isoformat()
         url = f"{self._path}{self.id}/monitoringDataDeletions/"
         response = self._client.post(url, data=payload)
         wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
 
+    def list_shared_roles(
+        self,
+        id: Optional[str] = None,
+        name: Optional[str] = None,
+        share_recipient_type: Optional[str] = None,
+        limit: int = 100,
+        offset: int = 0,
+    ) -> List[DeploymentSharedRole]:
+        """
+        Get a list of users, groups and organizations that have an access to this user blueprint
 
-def _check(trafaret: t, value: Any, default_to_null: bool = True) -> Any:
-    if default_to_null and value is None:
-        return None
+        Parameters
+        ----------
+        id: str, Optional
+            Only return the access control information for a organization, group or user with this
+            ID.
+        name: string, Optional
+            Only return the access control information for a organization, group or user with this
+            name.
+        share_recipient_type: enum('user', 'group', 'organization'), Optional
+            Only returns results with the given recipient type.
+        limit: int (Default=0)
+            At most this many results are returned.
+        offset: int (Default=0)
+            This many results will be skipped.
 
-    # Allow users to pass a single value even if a list of values is expected.
-    if isinstance(trafaret, t.List) and not isinstance(value, list):
-        value = [value]
+        Returns
+        -------
+        list(DeploymentSharedRole)
+        """
+        path = f"{self._path}{self.id}/sharedRoles/"
+        params = dict(
+            name=name,
+            id=id,
+            share_recipient_type=share_recipient_type,
+            limit=limit,
+            offset=offset,
+        )
 
-    return trafaret.check(value)
+        if limit == 0:
+            data = list(unpaginate(path, params, self._client))
+        else:
+            data = self._client.get(path, params=params).json()["data"]
+
+        return [DeploymentSharedRole.from_server_data(role) for role in data]
+
+    def update_shared_roles(
+        self,
+        roles: List[Union[DeploymentGrantSharedRoleWithId, DeploymentGrantSharedRoleWithUsername]],
+    ) -> None:
+        """
+        Share a deployment with a user, group, or organization
+
+        Parameters
+        ----------
+        roles: list(or(GrantAccessControlWithUsernameValidator, GrantAccessControlWithIdValidator))
+            Array of GrantAccessControl objects, up to maximum 100 objects.
+
+        """
+        path = f"{self._path}{self.id}/sharedRoles/"
+        roles_json = []
+        for role in roles:
+            if not isinstance(
+                role,
+                (dict, DeploymentGrantSharedRoleWithUsername, DeploymentGrantSharedRoleWithId),
+            ):
+                raise TypeError(
+                    "'roles' must be a list of one of: dict, "
+                    "DeploymentGrantSharedRoleWithUsername, DeploymentGrantSharedRoleWithId"
+                )
+            roles_json.append(role if isinstance(role, dict) else role.to_dict())
+
+        self._client.patch(path, data=dict(operation="updateRoles", roles=roles_json))
 
 
 class DeploymentListFilters:  # pylint: disable=missing-class-docstring
     def __init__(
         self,
         role: Optional[str] = None,
         service_health: Optional[List[str]] = None,
```

### Comparing `datarobot-3.1.1/datarobot/models/driver.py` & `datarobot-3.2.0b0/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/execution_environment.py` & `datarobot-3.2.0b0/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/execution_environment_version.py` & `datarobot-3.2.0b0/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/external_baseline_validation.py` & `datarobot-3.2.0b0/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from datarobot.models.roc_curve import RocCurveThresholdMixin, RocPointsTrafaret
 from datarobot.utils.pagination import unpaginate
 
 from ..api_object import APIObject
 from .external_scores import DEFAULT_BATCH_SIZE
 
 if TYPE_CHECKING:
-    from datarobot.models.roc_curve import EstimatedMetric
+    from datarobot.models.types import RocCurveEstimatedMetric
 
 
 class ExternalRocCurve(APIObject, RocCurveThresholdMixin):
     """ROC curve data for the model and prediction dataset with target or actual value column in
     unsupervised case.
 
     .. versionadded:: v2.21
@@ -48,15 +48,15 @@
     _path = "projects/{project_id}/models/{model_id}/datasetRocCurves/"
 
     _converter = t.Dict({t.Key("dataset_id"): String}).merge(RocPointsTrafaret).ignore_extra("*")
 
     def __init__(
         self,
         dataset_id: str,
-        roc_points: List[EstimatedMetric],
+        roc_points: List[RocCurveEstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
     ) -> None:
         self.dataset_id = dataset_id
         self.roc_points = roc_points
         self.negative_class_predictions = negative_class_predictions
         self.positive_class_predictions = positive_class_predictions
```

### Comparing `datarobot-3.1.1/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot-3.2.0b0/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/feature.py` & `datarobot-3.2.0b0/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot-3.2.0b0/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/feature_effect.py` & `datarobot-3.2.0b0/datarobot/models/feature_effect.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class FeatureEffectMetadata(APIObject):
     """Feature Effect Metadata for model, contains status and available model sources.
 
     Notes
     -----
 
-    `source` is expected parameter to retrieve Feature Fit. One of provided sources
+    `source` is expected parameter to retrieve Feature Effect. One of provided sources
     shall be used.
 
     """
 
     _converter = t.Dict({t.Key("status"): String, t.Key("sources"): t.List(String)}).ignore_extra(
         "*"
     )
@@ -48,15 +48,15 @@
     Notes
     -----
     ``feature effect metadata per backtest`` contains:
         * ``status`` : string.
         * ``backtest_index`` : string.
         * ``sources`` : list(string).
 
-    `source` is expected parameter to retrieve Feature Fit. One of provided sources
+    `source` is expected parameter to retrieve Feature Effect. One of provided sources
     shall be used.
 
     `backtest_index` is expected parameter to submit compute request and retrieve Feature Effect.
     One of provided backtest indexes shall be used.
 
     Attributes
     ----------
```

### Comparing `datarobot-3.1.1/datarobot/models/featurelist.py` & `datarobot-3.2.0b0/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/imported_model.py` & `datarobot-3.2.0b0/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/job.py` & `datarobot-3.2.0b0/datarobot/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Optional, Tuple, Type, TypeVar
 
 import trafaret as t
 
 from datarobot._compat import Int, String
-from datarobot.models.feature_fit import FeatureFit
 from datarobot.models.shap_impact import ShapImpact
 from datarobot.models.validators import feature_impact_trafaret, single_feature_impact_trafaret
 from datarobot.utils.waiters import wait_for_async_resolution
 
 from .. import errors
 from ..client import get_client, staticproperty
 from ..enums import DEFAULT_MAX_WAIT, JOB_TYPE, PREDICTION_PREFIX, QUEUE_STATUS
@@ -143,15 +142,15 @@
     def get_result(self, params=None):
         """
         Parameters
         ----------
         params : dict or None
             Query parameters to be added to request to get results.
 
-        For featureEffects and featureFit, source param is required to define source,
+        For featureEffects, source param is required to define source,
         otherwise the default is `training`
 
         Returns
         -------
         result : object
             Return type depends on the job type:
                 - for model jobs, a Model is returned
@@ -161,15 +160,14 @@
                 - for primeRulesets jobs, a list of Rulesets
                 - for primeModel jobs, a PrimeModel
                 - for primeDownloadValidation jobs, a PrimeFile
                 - for predictionExplanationInitialization jobs, a
                   PredictionExplanationsInitialization
                 - for predictionExplanations jobs, a PredictionExplanations
                 - for featureEffects, a FeatureEffects
-                - for featureFit, a FeatureFit
 
         Raises
         ------
         JobNotFinished
             If the job is not finished, the result is not available.
         AsyncProcessUnsuccessfulError
             If the job errored or was aborted
@@ -188,16 +186,14 @@
         elif self.job_type == JOB_TYPE.PREDICT:
             return raw_prediction_response_to_dataframe(server_data, PREDICTION_PREFIX.DEFAULT)
         elif self.job_type == JOB_TYPE.FEATURE_IMPACT:
             # Note: a custom FeatureImpactJob class is used for high level API now.
             return server_data["featureImpacts"]
         elif self.job_type == JOB_TYPE.FEATURE_EFFECTS:
             return FeatureEffects.from_server_data(server_data)
-        elif self.job_type == JOB_TYPE.FEATURE_FIT:
-            return FeatureFit.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PRIME_RULESETS:
             return [Ruleset.from_server_data(ruleset_data) for ruleset_data in server_data]
         elif self.job_type == JOB_TYPE.PRIME_MODEL:
             return PrimeModel.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PRIME_VALIDATION:
             return PrimeFile.from_server_data(server_data)
         elif self.job_type == JOB_TYPE.PREDICTION_EXPLANATIONS_INITIALIZATION:
```

### Comparing `datarobot-3.1.1/datarobot/models/lift_chart.py` & `datarobot-3.2.0b0/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/missing_report.py` & `datarobot-3.2.0b0/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/model.py` & `datarobot-3.2.0b0/datarobot/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 from datarobot.models.external_dataset_scores_insights import ExternalScores
 from datarobot.models.feature_effect import (
     FeatureEffectMetadata,
     FeatureEffectMetadataDatetime,
     FeatureEffects,
     FeatureEffectsMulticlass,
 )
-from datarobot.models.feature_fit import FeatureFit, FeatureFitMetadata, FeatureFitMetadataDatetime
 from datarobot.models.lift_chart import LiftChart
 from datarobot.models.missing_report import MissingValuesReport
 from datarobot.models.pareto_front import ParetoFront
 from datarobot.models.residuals import ResidualsChart
 from datarobot.models.roc_curve import LabelwiseRocCurve, RocCurve
 from datarobot.models.ruleset import Ruleset
 from datarobot.models.segmentation import SegmentInfo
@@ -78,14 +77,15 @@
 from ..utils import from_api, get_id_from_response, parse_time
 from .advanced_tuning import AdvancedTuningSession
 from .api_object import APIObject
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
+    from datarobot.models.blueprint import BlueprintJson
     from datarobot.models.dataset import Dataset
     from datarobot.models.job import Job
     from datarobot.models.modeljob import ModelJob
     from datarobot.models.predict_job import PredictJob
 
     class ConstraintsFloatListType(TypedDict):
         min_length: int
@@ -1186,16 +1186,16 @@
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureEffectsMetadata/"
 
     def get_feature_effect_metadata(self):
         """
         Retrieve Feature Effects metadata. Response contains status and available model sources.
 
-        * Feature Fit for the `training` partition is always available, with the exception of older
-          projects that only supported Feature Fit for `validation`.
+        * Feature Effect for the `training` partition is always available, with the exception of older
+          projects that only supported Feature Effect for `validation`.
 
         * When a model is trained into `validation` or `holdout` without stacked predictions
           (i.e., no out-of-sample predictions in those partitions),
           Feature Effects is not available for `validation` or `holdout`.
 
         * Feature Effects for `holdout` is not available when holdout was not unlocked for
           the project.
@@ -1207,44 +1207,14 @@
         feature_effect_metadata: FeatureEffectMetadata
 
         """
         fe_metadata_url = self._get_feature_effect_metadata_url()
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadata.from_server_data(server_data)
 
-    def _get_feature_fit_metadata_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_model_url() + "featureFitMetadata/"
-
-    def get_feature_fit_metadata(self):
-        """
-         Retrieve Feature Fit metadata. Response contains status and available model sources.
-
-        * Feature Fit of `training` is always available
-          (except for the old project which supports only Feature Fit for `validation`).
-
-        * When a model is trained into `validation` or `holdout` without stacked prediction
-          (e.g. no out-of-sample prediction in `validation` or `holdout`),
-          Feature Fit is not available for `validation` or `holdout`.
-
-        * Feature Fit for `holdout` is not available when there is no holdout configured for
-          the project.
-
-         `source` is expected parameter to retrieve Feature Fit. One of provided sources
-         shall be used.
-
-         Returns
-         -------
-         feature_effect_metadata: FeatureFitMetadata
-
-        """
-        ff_metadata_url = self._get_feature_fit_metadata_url()
-        server_data = self._client.get(ff_metadata_url).json()
-        return FeatureFitMetadata.from_server_data(server_data)
-
     def _get_feature_effect_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureEffects/"
 
     def request_feature_effect(self, row_count: Optional[int] = None):
         """
         Request feature effects to be computed for the model.
@@ -1481,117 +1451,14 @@
             from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
 
             feature_effect_job = Job.get(self.project_id, qid)
 
         params = {"source": source}
         return feature_effect_job.get_result_when_complete(max_wait=max_wait, params=params)
 
-    def _get_feature_fit_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_model_url() + "featureFit/"
-
-    def request_feature_fit(self):
-        """
-        Request feature fit to be computed for the model.
-
-        See :meth:`get_feature_effect <datarobot.models.Model.get_feature_fit>` for more
-        information on the result of the job.
-
-        Returns
-        -------
-         job : Job
-            A Job representing the feature fit computation. To get the completed feature fit
-            data, use `job.get_result` or `job.get_result_when_complete`.
-
-        Raises
-        ------
-        JobAlreadyRequested (422)
-            If the feature effect have already been requested.
-        """
-        from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-        route = self._get_feature_fit_url()
-        response = self._client.post(route)
-        job_id = get_id_from_response(response)
-        return Job.get(self.project_id, job_id)
-
-    def get_feature_fit(self, source: str):
-        """
-        Retrieve Feature Fit for the model.
-
-        Feature Fit provides partial dependence and predicted vs actual values for top-500
-        features ordered by feature importance score.
-
-        The partial dependence shows marginal effect of a feature on the target variable after
-        accounting for the average effects of all other predictive features. It indicates how,
-        holding all other variables except the feature of interest as they were,
-        the value of this feature affects your prediction.
-
-        Requires that Feature Fit has already been computed with
-        :meth:`request_feature_effect <datarobot.models.Model.request_feature_fit>`.
-
-        See :meth:`get_feature_fit_metadata <datarobot.models.Model.get_feature_fit_metadata>`
-        for retrieving information the available sources.
-
-        Parameters
-        ----------
-        source : string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadata.sources].
-
-        Returns
-        -------
-        feature_fit : FeatureFit
-           The feature fit data.
-
-        Raises
-        ------
-        ClientError (404)
-            If the feature fit have not been computed or source is not valid value.
-        """
-        params = {"source": source}
-        fe_url = self._get_feature_fit_url()
-        server_data = self._client.get(fe_url, params=params).json()
-        return FeatureFit.from_server_data(server_data)
-
-    def get_or_request_feature_fit(self, source: str, max_wait: int = DEFAULT_MAX_WAIT):
-        """
-        Retrieve feature fit for the model, requesting a job if it hasn't been run previously
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.Model.get_feature_fit_metadata>`
-        for retrieving information of source.
-
-        Parameters
-        ----------
-        max_wait : int, optional
-            The maximum time to wait for a requested feature fit job to complete before erroring
-
-        source : string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadata.sources].
-
-        Returns
-        -------
-        feature_effects : FeatureFit
-           The feature fit data.
-        """
-        try:
-            feature_fit_job = self.request_feature_fit()
-        except JobAlreadyRequested as e:
-            # if already requested it may be still running
-            # check and get the jobid in that case
-            qid = e.json["jobId"]
-            from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-            feature_fit_job = Job.get(self.project_id, qid)
-
-        params = {"source": source}
-        return feature_fit_job.get_result_when_complete(max_wait=max_wait, params=params)
-
     def get_prime_eligibility(self):
         """Check if this model can be approximated with DataRobot Prime
 
         Returns
         -------
         prime_eligibility : dict
             a dict indicating whether a model can be approximated with DataRobot Prime
@@ -2460,14 +2327,24 @@
             self.project_id, self.id, "true" if source_code else "false"
         )
         response = self._client.get(url, stream=True)
         with open(file_name, "wb") as f:
             for chunk in response.iter_content(chunk_size=1024 * 1024):
                 f.write(chunk)
 
+    def get_model_blueprint_json(self) -> BlueprintJson:
+        """Get the blueprint json representation used by this model.
+
+        Returns
+        -------
+        BlueprintJson
+            Json representation of the blueprint stages.
+        """
+        return self.blueprint.get_json()
+
     def get_model_blueprint_documents(self):
         """Get documentation for tasks used in this model.
 
         Returns
         -------
         list of BlueprintTaskDocument
             All documents available for the model.
@@ -3820,14 +3697,15 @@
         windows_basis_unit=None,
         model_number=None,
         parent_model_id=None,
         use_project_settings=None,
         supports_composable_ml=None,
         n_clusters=None,
         is_n_clusters_dynamically_determined=None,
+        **kwargs,
     ) -> None:
         super().__init__(
             id=id,
             processes=processes,
             featurelist_name=featurelist_name,
             featurelist_id=featurelist_id,
             project_id=project_id,
@@ -4329,55 +4207,14 @@
         feature_effect_metadata: FeatureEffectMetadataDatetime
 
         """
         fe_metadata_url = self._get_feature_effect_metadata_url()
         server_data = self._client.get(fe_metadata_url).json()
         return FeatureEffectMetadataDatetime.from_server_data(server_data)
 
-    def _get_feature_fit_metadata_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_datetime_model_url() + "featureFitMetadata/"
-
-    def get_feature_fit_metadata(self):
-        """
-        Retrieve Feature Fit metadata for each backtest. Response contains status and available
-        sources for each backtest of the model.
-
-        * Each backtest is available for `training` and `validation`
-
-        * If holdout is configured for the project it has `holdout` as `backtestIndex`. It has
-          `training` and `holdout` sources available.
-
-        Start/stop models contain a single response item with `startstop` value for `backtestIndex`.
-
-        * Feature Fit of `training` is always available
-          (except for the old project which supports only Feature Effect for `validation`).
-
-        * When a model is trained into `validation` or `holdout` without stacked prediction
-          (e.g. no out-of-sample prediction in `validation` or `holdout`),
-          Feature Fit is not available for `validation` or `holdout`.
-
-        * Feature Fit for `holdout` is not available when there is no holdout configured for
-          the project.
-
-        `source` is expected parameter to retrieve Feature Fit. One of provided sources
-        shall be used.
-
-        `backtestIndex` is expected parameter to submit compute request and retrieve Feature Fit.
-        One of provided backtest indexes shall be used.
-
-        Returns
-        -------
-        feature_effect_metadata: FeatureFitMetadataDatetime
-
-        """
-        ff_metadata_url = self._get_feature_fit_metadata_url()
-        server_data = self._client.get(ff_metadata_url).json()
-        return FeatureFitMetadataDatetime.from_server_data(server_data)
-
     def _get_feature_effect_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_datetime_model_url() + "featureEffects/"
 
     # pylint: disable-next=arguments-renamed
     def request_feature_effect(self, backtest_index):
         """
@@ -4643,142 +4480,14 @@
                     max_wait=max_wait, params=params
                 )
             else:
                 raise e
 
         return feature_effects
 
-    def _get_feature_fit_url(self) -> str:
-        # This is a method (rather than attribute) for the same reason as _get_model_url.
-        return self._get_datetime_model_url() + "featureFit/"
-
-    # pylint: disable-next=arguments-differ
-    def request_feature_fit(self, backtest_index):
-        """
-        Request feature fit to be computed for the model.
-
-        See :meth:`get_feature_fit <datarobot.models.DatetimeModel.get_feature_fit>` for more
-        information on the result of the job.
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.DatetimeModel.get_feature_fit_metadata>`
-        for retrieving information of backtest_index.
-
-        Parameters
-        ----------
-        backtest_index: string, FeatureFitMetadataDatetime.backtest_index.
-            The backtest index to retrieve Feature Fit for.
-
-        Returns
-        -------
-         job : Job
-            A Job representing the feature fit computation. To get the completed feature fit
-            data, use `job.get_result` or `job.get_result_when_complete`.
-
-        Raises
-        ------
-        JobAlreadyRequested (422)
-            If the feature fit have already been requested.
-        """
-        from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-        payload = {"backtestIndex": backtest_index}
-        route = self._get_feature_fit_url()
-        response = self._client.post(route, data=payload)
-        job_id = get_id_from_response(response)
-        return Job.get(self.project_id, job_id)
-
-    # pylint: disable-next=arguments-differ
-    def get_feature_fit(self, source, backtest_index):
-        """
-        Retrieve Feature Fit for the model.
-
-        Feature Fit provides partial dependence and predicted vs actual values for top-500
-        features ordered by feature impact score.
-
-        The partial dependence shows marginal effect of a feature on the target variable after
-        accounting for the average effects of all other predictive features. It indicates how,
-        holding all other variables except the feature of interest as they were,
-        the value of this feature affects your prediction.
-
-        Requires that Feature Fit has already been computed with
-        :meth:`request_feature_fit <datarobot.models.Model.request_feature_fit>`.
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.DatetimeModel.get_feature_fit_metadata>`
-        for retrieving information of source, backtest_index.
-
-        Parameters
-        ----------
-        source: string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadataDatetime.sources]. To retrieve the available
-            sources for feature fit.
-
-        backtest_index: string, FeatureFitMetadataDatetime.backtest_index.
-            The backtest index to retrieve Feature Fit for.
-
-        Returns
-        -------
-        feature_fit: FeatureFit
-           The feature fit data.
-
-        Raises
-        ------
-        ClientError (404)
-            If the feature fit have not been computed or source is not valid value.
-        """
-        params = {
-            "source": source,
-            "backtestIndex": backtest_index,
-        }
-        fe_url = self._get_feature_fit_url()
-        server_data = self._client.get(fe_url, params=params).json()
-        return FeatureFit.from_server_data(server_data)
-
-    # pylint: disable-next=arguments-renamed
-    def get_or_request_feature_fit(self, source, backtest_index, max_wait=DEFAULT_MAX_WAIT):
-        """
-        Retrieve feature fit for the model, requesting a job if it hasn't been run previously
-
-        See :meth:`get_feature_fit_metadata \
-        <datarobot.models.DatetimeModel.get_feature_fit_metadata>`
-        for retrieving information of source, backtest_index.
-
-        Parameters
-        ----------
-        max_wait : int, optional
-            The maximum time to wait for a requested feature fit job to complete before erroring
-
-        source : string
-            The source Feature Fit are retrieved for.
-            One value of [FeatureFitMetadataDatetime.sources]. To retrieve the available sources
-            for feature effect.
-
-        backtest_index: string, FeatureFitMetadataDatetime.backtest_index.
-            The backtest index to retrieve Feature Fit for.
-
-        Returns
-        -------
-        feature_fit : FeatureFit
-           The feature fit data.
-        """
-        try:
-            feature_fit_job = self.request_feature_fit(backtest_index)
-        except JobAlreadyRequested as e:
-            # if already requested it may be still running
-            # check and get the jobid in that case
-            qid = e.json["jobId"]
-            from .job import Job  # pylint: disable=import-outside-toplevel,cyclic-import
-
-            feature_fit_job = Job.get(self.project_id, qid)
-
-        params = {"source": source}
-        return feature_fit_job.get_result_when_complete(max_wait=max_wait, params=params)
-
     def calculate_prediction_intervals(self, prediction_intervals_size: int) -> Job:
         """
         Calculate prediction intervals for this DatetimeModel for the specified size.
 
         .. versionadded:: v2.19
 
         Parameters
```

### Comparing `datarobot-3.1.1/datarobot/models/modeljob.py` & `datarobot-3.2.0b0/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/pairwise_statistics.py` & `datarobot-3.2.0b0/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/pareto_front.py` & `datarobot-3.2.0b0/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/payoff_matrix.py` & `datarobot-3.2.0b0/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/predict_job.py` & `datarobot-3.2.0b0/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/prediction_dataset.py` & `datarobot-3.2.0b0/datarobot/models/prediction_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             t.Key("num_columns"): Int(),
             t.Key("forecast_point", optional=True): parse_time,
             t.Key("predictions_start_date", optional=True): parse_time,
             t.Key("predictions_end_date", optional=True): parse_time,
             t.Key("relax_known_in_advance_features_check", optional=True): t.Bool(),
             # do not forget to update `test_data_quality_warnings`
             # in datarobot-python-api-tests repo
-            t.Key("data_quality_warnings"): t.Dict(
+            t.Key("data_quality_warnings", optional=True): t.Dict(
                 {
                     t.Key("has_kia_missing_values_in_forecast_window"): t.Bool(),
                     t.Key("insufficient_rows_for_evaluating_models"): t.Bool(),
                     t.Key("single_class_actual_value_column"): t.Bool(),
                 }
             ).allow_extra("*"),
             t.Key("forecast_point_range", optional=True): t.List(parse_time),
```

### Comparing `datarobot-3.1.1/datarobot/models/prediction_explanations.py` & `datarobot-3.2.0b0/datarobot/models/prediction_explanations.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 import abc
 from datetime import datetime
+import json
 
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import TARGET_TYPE
 from datarobot.models.project_options import ProjectOptions
@@ -24,35 +25,54 @@
 
 int_float_string = t.Type(int) | t.Type(float) | String(allow_blank=True)
 
 prediction_values_trafaret = t.Dict(
     {t.Key("label", optional=True): int_float_string, t.Key("value"): t.Float}
 ).ignore_extra("*")
 
+per_ngram_text_explanations_trafaret = t.Or(
+    t.List(
+        t.Dict(
+            {
+                t.Key("ngrams"): t.List(
+                    t.Dict({t.Key("ending_index"): Int, t.Key("starting_index"): Int})
+                ),
+                t.Key("is_unknown"): t.Bool,
+                t.Key("qualitative_strength"): String,
+                t.Key("strength"): t.Float,
+            }
+        )
+    ),
+    t.Null,
+)
+
 prediction_explanations_entry_trafaret = t.Dict(
     {
         t.Key("label", optional=True): int_float_string,
         t.Key("feature"): String,
         t.Key("feature_value"): int_float_string,
         t.Key("strength"): t.Float,
         t.Key("qualitative_strength"): String,
+        t.Key("per_ngram_text_explanations", optional=True): per_ngram_text_explanations_trafaret,
     }
 ).ignore_extra("*")
 
 prediction_explanations_trafaret = t.Dict(
     {
         t.Key("row_id"): Int,
         t.Key("prediction"): int_float_string,
         t.Key("adjusted_prediction", optional=True): int_float_string,
         t.Key("prediction_values"): t.List(prediction_values_trafaret),
         t.Key("adjusted_prediction_values", optional=True): t.List(prediction_values_trafaret),
         t.Key("prediction_explanations"): t.List(prediction_explanations_entry_trafaret),
     }
 ).ignore_extra("*")
 
+KEEP_ATTRS = ["data.prediction_explanations.per_ngram_text_explanations"]
+
 
 class PredictionExplanationsMode:
     """Prediction explanations mode for multiclass models"""
 
     @abc.abstractmethod
     def get_api_parameters(self, batch_route=False):
         """Get parameters passed in corresponding API call
@@ -485,25 +505,29 @@
             - explanation_0_feature_value : the value the feature took on
             - explanation_0_label : the output being driven by this explanation.  For regression
               projects, this is the name of the target feature.  For classification projects, this
               is the class label whose probability increasing would correspond to a positive
               strength.
             - explanation_0_qualitative_strength : a human-readable description of how strongly the
               feature affected the prediction (e.g. '+++', '--', '+') for this explanation
+            - explanation_0_per_ngram_text_explanations : Text prediction explanations data in json
+              formatted string.
             - explanation_0_strength : the amount this feature's value affected the prediction
             - ...
             - explanation_N_feature : the name of the feature contributing to the prediction for
               this explanation
             - explanation_N_feature_value : the value the feature took on
             - explanation_N_label : the output being driven by this explanation.  For regression
               projects, this is the name of the target feature.  For classification projects, this
               is the class label whose probability increasing would correspond to a positive
               strength.
             - explanation_N_qualitative_strength : a human-readable description of how strongly the
               feature affected the prediction (e.g. '+++', '--', '+') for this explanation
+            - explanation_N_per_ngram_text_explanations : Text prediction explanations data in json
+              formatted string.
             - explanation_N_strength : the amount this feature's value affected the prediction
 
         For classification projects, the server does not guarantee any ordering on the prediction
         values, however within this function we sort the values so that `class_X` corresponds to
         the same class from row to row.
 
         Parameters
@@ -517,14 +541,18 @@
         dataframe: pandas.DataFrame
         """
         columns = ["row_id", "prediction"]
         rows = self.get_rows(
             batch_size=1, exclude_adjusted_predictions=exclude_adjusted_predictions
         )
         first_row = next(rows)
+        has_text_explanations = (
+            first_row.prediction_explanations
+            and "per_ngram_text_explanations" in first_row.prediction_explanations[0]
+        )
         adjusted_predictions_in_data = first_row.adjusted_prediction is not None
         if adjusted_predictions_in_data:
             columns.append("adjusted_prediction")
         # for regression, length is 1; for classification, length is number of levels in target
         # i.e. 2 for binary classification
         is_classification = len(first_row.prediction_values) > 1
         # include class label/probability for classification project
@@ -540,25 +568,30 @@
                             f"{prefix}_explanation_{i}_feature",
                             f"{prefix}_explanation_{i}_feature_value",
                             f"{prefix}_explanation_{i}_label",
                             f"{prefix}_explanation_{i}_qualitative_strength",
                             f"{prefix}_explanation_{i}_strength",
                         ]
                     )
+                    if has_text_explanations:
+                        columns.append(f"{prefix}_explanation_{i}_per_ngram_text_explanations")
+
         else:
             for i in range(self.max_explanations):
                 columns.extend(
                     [
                         f"explanation_{i}_feature",
                         f"explanation_{i}_feature_value",
                         f"explanation_{i}_label",
                         f"explanation_{i}_qualitative_strength",
                         f"explanation_{i}_strength",
                     ]
                 )
+                if has_text_explanations:
+                    columns.append(f"explanation_{i}_per_ngram_text_explanations")
         pred_expl_list = []
 
         for i, row in enumerate(
             self.get_rows(exclude_adjusted_predictions=exclude_adjusted_predictions)
         ):
             data = [row.row_id, row.prediction]
             if adjusted_predictions_in_data:
@@ -585,26 +618,34 @@
                             pred_expl["feature"],
                             pred_expl["feature_value"],
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
+                    if has_text_explanations:
+                        data.append(
+                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
+                        )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
             else:
                 for pred_expl in row.prediction_explanations:
                     data.extend(
                         [
                             pred_expl["feature"],
                             pred_expl["feature_value"],
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
+                    if has_text_explanations:
+                        data.append(
+                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
+                        )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
 
         return pd.DataFrame(data=pred_expl_list, columns=columns)
 
     def download_to_csv(self, filename, encoding="utf-8", exclude_adjusted_predictions=True):
         """
         Save prediction explanations rows into CSV file.
@@ -821,13 +862,8 @@
         params = {
             "offset": offset,
             "exclude_adjusted_predictions": "true" if exclude_adjusted_predictions else "false",
         }
         if limit:
             params["limit"] = limit
         path = f"{cls._path_template.format(project_id)}{prediction_explanations_id}/"
-        return cls.from_location(path, params=params)
-
-    @classmethod
-    def from_location(cls, path, params=None):  # pylint: disable=arguments-renamed
-        server_data = cls._client.get(path, params=params).json()
-        return cls.from_server_data(server_data)
+        return cls.from_location(path, keep_attrs=KEEP_ATTRS, params=params)
```

### Comparing `datarobot-3.1.1/datarobot/models/prediction_server.py` & `datarobot-3.2.0b0/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/predictions.py` & `datarobot-3.2.0b0/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/prime_file.py` & `datarobot-3.2.0b0/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/project.py` & `datarobot-3.2.0b0/datarobot/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -20,14 +20,15 @@
 
 from pandas import DataFrame
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import (
     AUTOPILOT_MODE,
+    CredentialTypes,
     CV_METHOD,
     DEFAULT_MAX_WAIT,
     DEFAULT_TIMEOUT,
     LEADERBOARD_SORT_KEY,
     MONOTONICITY_FEATURELIST_DEFAULT,
     NonPersistableProjectOptions,
     PROJECT_STAGE,
@@ -84,14 +85,15 @@
 from datarobot.models.relationships_configuration import RelationshipsConfiguration
 from datarobot.models.restore_discarded_features import (
     DiscardedFeaturesInfo,
     FeatureRestorationStatus,
 )
 from datarobot.models.segmentation import SegmentationTask
 from datarobot.models.sharing import SharingAccess
+from datarobot.models.use_cases.utils import add_to_use_case, resolve_use_cases, UseCaseLike
 from datarobot.utils import (
     assert_single_or_zero_parameter,
     camelize,
     datetime_to_string,
     deprecated,
     from_api,
     get_duplicate_features,
@@ -118,14 +120,39 @@
     from datarobot.models.dataset import Dataset
 
     class SegmentationDict(TypedDict):
         segmentation_task_id: Optional[str]
         parent_project_id: Optional[str]
         segment: Optional[str]
 
+    class BaseCredentialsDataDict(TypedDict):
+        credentialType: CredentialTypes
+
+    class BasicCredentialsDataDict(BaseCredentialsDataDict):
+        user: str
+        password: str
+
+    class S3CredentialsDataDict(BaseCredentialsDataDict):
+        awsAccessKeyId: str
+        awsSecretAccessKey: str
+        awsSessionToken: str
+
+    class OAuthCredentialsDataDict(BaseCredentialsDataDict):
+        oauthRefreshToken: str
+        oauthClientId: str
+        oauthClientSecret: str
+        oauthAccessToken: str
+
+    class BasicCredentialsDict(TypedDict):
+        user: str
+        password: str
+
+    class CredentialIdCredentialsDict(TypedDict):
+        credentialId: str
+
 
 class Project(APIObject, BrowserMixin):
     """A project built from a particular training dataset
 
     Attributes
     ----------
     id : str
@@ -186,14 +213,16 @@
         (New in version v3.0) The partitioning class for this project. This attribute should only be used
         with newly-created projects and before calling `Project.analyze_and_model()`. After the project has been
         aimed, see `Project.partition` for actual partitioning options.
     catalog_id : str
         (New in version v3.0) ID of the dataset used during creation of the project.
     catalog_version_id : str
         (New in version v3.0) The object ID of the ``catalog_version`` which the project's dataset belongs to.
+    use_gpu: bool
+        (New in version v3.2) Whether project allows usage of GPUs
     """
 
     _path = "projects/"
     _clone_path = "projectClones/"
     _scaleout_modeling_mode_converter = String()
     _advanced_options_converter = t.Dict(
         {
@@ -288,14 +317,15 @@
             t.Key("created", optional=True): parse_time,
             t.Key("advanced_options", optional=True): _advanced_options_converter,
             t.Key("max_train_pct", optional=True): t.Float(),
             t.Key("max_train_rows", optional=True): Int(),
             t.Key("file_name", optional=True): String(allow_blank=True),
             t.Key("credentials", optional=True): _feg_credentials_converter,
             t.Key("feature_engineering_prediction_point", optional=True): String(),
+            t.Key("use_gpu", optional=True): t.Bool(),
             t.Key("unsupervised_mode", default=False): t.Bool(),
             t.Key("use_feature_discovery", optional=True, default=False): t.Bool(),
             t.Key("relationships_configuration_id", optional=True): String(),
             t.Key("query_generator_id", optional=True): String(),
             t.Key("segmentation", optional=True): _segmentation_converter,
             t.Key("partitioning_method", optional=True): t.Or(
                 _partitioning_method_converter, DatetimePartitioning._converter
@@ -329,14 +359,15 @@
         relationships_configuration_id: Optional[str] = None,
         project_description: Optional[str] = None,
         query_generator_id: Optional[str] = None,
         segmentation: Optional[SegmentationDict] = None,
         partitioning_method=None,
         catalog_id: Optional[str] = None,
         catalog_version_id: Optional[str] = None,
+        use_gpu: Optional[bool] = None,
     ) -> None:
 
         self.id = id
         self.project_name = project_name
         self.project_description = project_description
         self.mode = mode
         self.target = target
@@ -360,14 +391,15 @@
         self.use_feature_discovery = use_feature_discovery
         self.relationships_configuration_id = relationships_configuration_id
         self.query_generator_id = query_generator_id
         self.segmentation = segmentation
         self.partitioning_method = partitioning_method
         self.catalog_id = catalog_id
         self.catalog_version_id = catalog_version_id
+        self.use_gpu = use_gpu
         self.__options = None
 
     @property
     def use_time_series(self) -> bool:
         return bool(self.partition and self.partition.get("use_time_series"))
 
     @property
@@ -575,22 +607,23 @@
             keep_attrs=[
                 "advanced_options.default_monotonic_increasing_featurelist_id",
                 "advanced_options.default_monotonic_decreasing_featurelist_id",
             ],
         )
 
     @classmethod
+    @add_to_use_case(allow_multiple=False)
     def create(
         cls,
         sourcedata,
         project_name="Untitled Project",
         max_wait=DEFAULT_MAX_WAIT,
         read_timeout=DEFAULT_TIMEOUT.UPLOAD,
         dataset_filename=None,
-    ):
+    ) -> TProject:
         """
         Creates a project with provided data.
 
         Project creation is asynchronous process, which means that after
         initial request we will keep polling status of async process
         that is responsible for project creation until it's finished.
         For SDK users this only means that this method might raise
@@ -610,14 +643,16 @@
             unsuccessful
         read_timeout: int
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         dataset_filename : string or None, optional
             (New in version v2.14) File name to use for dataset.
             Ignored for url and file path sources.
+        use_case: UseCase | string, optional
+            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         project : Project
             Instance with initialized data.
 
         Raises
@@ -724,14 +759,15 @@
         if project_name is not None:
             payload["project_name"] = project_name
 
         response = cls._client.post(hdfs_project_create_endpoint, data=payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
+    @add_to_use_case(allow_multiple=False)
     def create_from_data_source(
         cls: Type[TProject],
         data_source_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         credential_id: Optional[str] = None,
         use_kerberos: Optional[bool] = None,
@@ -762,14 +798,16 @@
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         project_name : str, optional
             optional, a name to give to the project.
         max_wait : int
             optional, the maximum number of seconds to wait before giving up.
+        use_case: UseCase | string, optional
+            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Raises
         ------
         InvalidUsageError
             Raised if either ``username`` or ``password`` is passed without the other.
 
         Returns
@@ -795,14 +833,15 @@
         if "credential_data" in new_payload:
             new_payload["credential_data"] = CredentialDataSchema(new_payload["credential_data"])
 
         response = cls._client.post(cls._path, data=payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
+    @add_to_use_case(allow_multiple=False)
     def create_from_dataset(
         cls: Type[TProject],
         dataset_id: str,
         dataset_version_id: Optional[str] = None,
         project_name: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
@@ -836,14 +875,16 @@
             Server default is False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         max_wait: int
             optional, the maximum number of seconds to wait before giving up.
+        use_case: UseCase | string, optional
+            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         Project
         """
         payload = {
             "dataset_id": dataset_id,
@@ -860,14 +901,15 @@
         if "credential_data" in new_payload:
             new_payload["credential_data"] = CredentialDataSchema(new_payload["credential_data"])
 
         response = cls._client.post(cls._path, data=new_payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
+    @add_to_use_case(allow_multiple=False)
     def create_segmented_project_from_clustering_model(
         cls: Type[TProject],
         clustering_project_id: str,
         clustering_model_id: str,
         target: str,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TProject:
@@ -882,14 +924,16 @@
             The identifier of the clustering model you want to use as the
             segmentation method.
         target : str
             The name of the target column that will be used from the
             clustering project.
         max_wait: int
             optional, the maximum number of seconds to wait before giving up.
+        use_case: UseCase | string, optional
+            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         project : Project
             The created project
         """
         prepare_model_package_path = (
@@ -1005,14 +1049,15 @@
             )
             proj_id = get_id_from_location(finished_location)
             return cls.get(proj_id)
         except AppPlatformError as e:
             raise ProjectAsyncFailureError(repr(e), e.status_code, async_location)
 
     @classmethod
+    @add_to_use_case(allow_multiple=False)
     def start(
         cls: Type[TProject],
         sourcedata: Union[str, DataFrame],
         target: Optional[str] = None,
         project_name: str = "Untitled Project",
         worker_count: Optional[int] = None,
         metric: Optional[str] = None,
@@ -1133,14 +1178,16 @@
             - 'postProcessingRejectionOptionBasedClassification'
             The technique by which we'll mitigate bias, which will inform which bias mitigation task
             we insert into blueprints
         include_bias_mitigation_feature_as_predictor_variable : bool, optional
             Whether we should also use the mitigation feature as in input to the modeler just like
             any other categorical used for training, i.e. do we want the model to "train on" this
             feature in addition to using it for bias mitigation
+        use_case: UseCase | string, optional
+            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         project : Project
             The newly created and initialized project.
 
         Raises
@@ -1220,26 +1267,32 @@
             relationships_configuration_id=relationships_configuration_id,
             unsupervised_type=unsupervised_type,
             autopilot_cluster_list=autopilot_cluster_list,
         )
         return project
 
     @classmethod
-    def list(cls, search_params: Optional[Dict[str, str]] = None) -> List[Project]:
+    def list(
+        cls, search_params: Optional[Dict[str, str]] = None, use_cases: Optional[UseCaseLike] = None
+    ) -> List[Project]:
         """
         Returns the projects associated with this account.
 
         Parameters
         ----------
         search_params : dict, optional.
             If not `None`, the returned projects are filtered by lookup.
             Currently you can query projects by:
 
             * ``project_name``
 
+        use_cases : Union[UseCase, List[UseCase], str, List[str]], optional.
+            If not `None`, the returned projects are filtered to those associated
+            with a specific Use Case or Use Cases. Accepts either the entity or the ID.
+
         Returns
         -------
         projects : list of Project instances
             Contains a list of projects associated with this user
             account.
 
         Raises
@@ -1270,14 +1323,19 @@
                 get_params.update(search_params)
             else:
                 raise TypeError(
                     "Provided search_params argument {} is invalid type {}".format(
                         search_params, type(search_params)
                     )
                 )
+        # This is a special case we needed to cover. A user could pass in "experiment_container_id" themselves to
+        # `search_params`, so we need to check for that and default to `use_cases` if that was passed in.
+        # Then we proceed to check if resolve_use_case(`use_case_id`) arg was set, and use a global use case if
+        # it's available.
+        get_params = resolve_use_cases(use_cases=use_cases, params=get_params)
         r_data = cls._client.get(cls._path, params=get_params).json()
         return [cls.from_server_data(item) for item in r_data]
 
     def _update(self, **data) -> Project:
         """
         Change the project properties.
 
@@ -1391,14 +1449,15 @@
         feature_engineering_prediction_point=None,
         unsupervised_mode=False,
         relationships_configuration_id=None,
         class_mapping_aggregation_settings=None,
         segmentation_task_id=None,
         unsupervised_type=None,
         autopilot_cluster_list=None,
+        use_gpu=None,
     ):
         """
         Set target variable of an existing project and begin the autopilot process or send data to DataRobot
         for feature analysis only if manual mode is specified.
 
         Any options saved using ``set_options`` will be used if nothing is passed to ``advanced_options``.
         However, saved options will be ignored if ``advanced_options`` are passed.
@@ -1476,14 +1535,16 @@
         unsupervised_type : UnsupervisedTypeEnum, optional
             (New in version v2.27) Specifies whether an unsupervised project is anomaly detection
             or clustering.
         autopilot_cluster_list : list(int), optional
             (New in version v2.27) Specifies the list of clusters to build for each model during
             Autopilot. Specifying multiple values in a list will build models with each number
             of clusters for the Leaderboard.
+        use_gpu : bool, optional
+            (New in version v3.2) Specifies whether project should use GPUs
 
         Returns
         -------
         project : Project
             The instance with updated attributes.
 
         Raises
@@ -1569,14 +1630,16 @@
                 aim_payload["segmentation_task_id"] = segmentation_task_id.id
             elif isinstance(segmentation_task_id, str):
                 aim_payload["segmentation_task_id"] = segmentation_task_id
             else:
                 raise ValueError(
                     "segmentation_task_id must be either a string id or a SegmentationTask object"
                 )
+        if use_gpu is not None:
+            aim_payload["use_gpu"] = use_gpu
 
         url = f"{self._path}{self.id}/aim/"
         response = self._client.patch(url, data=aim_payload)
         async_location = response.headers["Location"]
 
         # Waits for project to be ready for modeling, but ignores the return value
         self.from_async(async_location, max_wait=max_wait)
@@ -2062,15 +2125,15 @@
         predictions_start_date=None,
         predictions_end_date=None,
         dataset_filename=None,
         relax_known_in_advance_features_check=None,
         credentials=None,
         actual_value_column=None,
         secondary_datasets_config_id=None,
-    ):
+    ) -> PredictionDataset:
         """Upload a new dataset to make predictions against
 
         Parameters
         ----------
         sourcedata : str, file or pandas.DataFrame
             Data to be used for predictions. If string, can be either a path to a local file,
             a publicly accessible URL (starting with ``http://``, ``https://``, ``file://``), or
@@ -2203,15 +2266,15 @@
         forecast_point=None,
         relax_known_in_advance_features_check=None,
         credentials=None,
         predictions_start_date=None,
         predictions_end_date=None,
         actual_value_column=None,
         secondary_datasets_config_id=None,
-    ):
+    ) -> PredictionDataset:
         """
         Upload a new dataset from a data source to make predictions against
 
         Parameters
         ----------
         data_source_id : str
             The identifier of the data source.
@@ -2284,46 +2347,104 @@
         async_loc = initial_project_post_response.headers["Location"]
         dataset_loc = wait_for_async_resolution(self._client, async_loc, max_wait=max_wait)
         dataset_data = self._client.get(dataset_loc, join_endpoint=False).json()
         return PredictionDataset.from_server_data(dataset_data)
 
     def upload_dataset_from_catalog(
         self,
-        dataset_id,
-        dataset_version_id=None,
-        max_wait=DEFAULT_MAX_WAIT,
-        forecast_point=None,
-        relax_known_in_advance_features_check=None,
-        credentials=None,
-        predictions_start_date=None,
-        predictions_end_date=None,
-        actual_value_column=None,
-        secondary_datasets_config_id=None,
-    ):
+        dataset_id: str,
+        credential_id: Optional[str] = None,
+        credential_data: Optional[
+            Union[BasicCredentialsDataDict, S3CredentialsDataDict, OAuthCredentialsDataDict]
+        ] = None,
+        dataset_version_id: Optional[str] = None,
+        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
+        forecast_point: Optional[datetime] = None,
+        relax_known_in_advance_features_check: Optional[bool] = None,
+        credentials: Optional[
+            List[Union[BasicCredentialsDict, CredentialIdCredentialsDict]]
+        ] = None,
+        predictions_start_date: Optional[datetime] = None,
+        predictions_end_date: Optional[datetime] = None,
+        actual_value_column: Optional[str] = None,
+        secondary_datasets_config_id: Optional[str] = None,
+    ) -> PredictionDataset:
         """Upload a new dataset from a catalog dataset to make predictions against
 
         Parameters
         ----------
         dataset_id : str
             The identifier of the dataset.
+        credential_id : str, optional
+            The credential ID of the AI Catalog dataset to upload.
+        credential_data : BasicCredentialsDataDict | S3CredentialsDataDict | OAuthCredentialsDataDict, optional
+            Credential data of the catalog dataset to upload. `credential_data` can be in
+            one of the following forms:
+
+            Basic Credentials
+                credentialType : str
+                    The credential type. For basic credentials, this value must be CredentialTypes.BASIC.
+                user : str
+                    The username for database authentication.
+                password : str
+                    The password for database authentication.
+                    The password is encrypted at rest and never saved or stored.
+
+            S3 Credentials
+                credentialType : str
+                    The credential type. For S3 credentials, this value must be CredentialTypes.S3.
+                awsAccessKeyId : str
+                    The S3 AWS access key ID.
+                awsSecretAccessKey : str
+                    The S3 AWS secret access key.
+                awsSessionToken : str
+                    The S3 AWS session token.
+
+            OAuth Credentials
+                credentialType : str
+                    The credential type. For OAuth credentials, this value must be CredentialTypes.OAUTH.
+                oauthRefreshToken : str
+                    The oauth refresh token.
+                oauthClientId : str
+                    The oauth client ID.
+                oauthClientSecret : str
+                    The oauth client secret.
+                oauthAccessToken : str
+                    The oauth access token.
         dataset_version_id : str, optional
             The version id of the dataset to use.
         max_wait : int, optional
             Optional, the maximum number of seconds to wait before giving up.
         forecast_point : datetime.datetime or None, optional
             For time series projects only. This is the default point relative
             to which predictions will be generated, based on the forecast window of the project. See
             the time series :ref:`prediction documentation <time_series_predict>` for more
             information.
         relax_known_in_advance_features_check : bool, optional
             For time series projects only. If True, missing values in the
             known in advance features are allowed in the forecast window at the prediction time.
             If omitted or False, missing values are not allowed.
-        credentials: list, optional
+        credentials: list[BasicCredentialsDict | CredentialIdCredentialsDict], optional
             A list of credentials for the datasets used in Feature discovery project.
+
+            Items in `credentials` can have the following forms:
+
+            Basic Credentials
+                user : str
+                    The username for database authentication.
+                password : str
+                    The password (in cleartext) for database authentication. The password
+                    will be encrypted on the server side in scope of HTTP request
+                    and never saved or stored.
+
+            Credential ID
+                credentialId : str
+                    The ID of the set of credentials to use instead of user and password.
+                    Note that with this change, username and password will become optional.
+
         predictions_start_date : datetime.datetime or None, optional
             For time series projects only. The start date for bulk
             predictions. Note that this parameter is for generating historical predictions using the
             training data. This parameter should be provided in conjunction with
             ``predictions_end_date``. Can't be provided with the ``forecast_point`` parameter.
         predictions_end_date : datetime.datetime or None, optional
             For time series projects only. The end date for bulk predictions,
@@ -2333,21 +2454,24 @@
         actual_value_column : string, optional
             Actual value column name, valid for the prediction
             files if the project is unsupervised and the dataset is considered as bulk predictions
             dataset. Cannot be provided with the ``forecast_point`` parameter.
         secondary_datasets_config_id: string or None, optional
             The Id of the alternative secondary dataset config
             to use during prediction for Feature discovery project.
-
         Returns
         -------
         dataset : PredictionDataset
             the newly uploaded dataset
         """
         form_data = {"datasetId": dataset_id}
+        if credential_id:
+            form_data["credentialId"] = credential_id
+        if credential_data:
+            form_data["credentialData"] = credential_data
         if dataset_version_id:
             form_data["datasetVersionId"] = dataset_version_id
         if forecast_point:
             if not isinstance(forecast_point, datetime):
                 raise ValueError("forecast_point must be an instance of datetime.datetime")
             form_data["forecastPoint"] = datetime_to_string(forecast_point)
         if predictions_start_date:
```

### Comparing `datarobot-3.1.1/datarobot/models/project_options.py` & `datarobot-3.2.0b0/datarobot/models/project_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,16 +441,14 @@
         One of BiasMitigationTechnique.
         The technique by which we'll mitigate bias, which will inform which bias mitigation task
         we insert into blueprints and how
     include_bias_mitigation_feature_as_predictor_variable : bool or None, optional
         Whether we should also use the mitigation feature as in input to the modeler just like
         any other categorical used for training, i.e. do we want the model to "train on" this
         feature in addition to using it for bias mitigation
-    force_cpu: bool, optional
-        If GPUs enabled, override and force running everything on CPUs
     min_clusters: int, optional
         The minimum number of clusters allowed when training clustering models.
     max_clusters: int, optional
         The maximum number of clusters allowed when training clustering models
     segmentation_id_column: string, optional
         The segmentation column name or automated segmentation column name specified for the
         project through the UI
@@ -477,14 +475,16 @@
     class_mapping_aggregation_settings: ClassMappingAggregationSettings, optional
         For multiclass additional settings can be specified to control aggregation of target
         values in final classes.
     class_mapping_aggregation_settings_enabled: bool, optional
         Is the class mapping aggregation settings section enabled or not in UI
     datetime_partitioning_id: str, optional
         Id of the datetime partitioning to use
+    use_gpu: bool, optional
+        Whether to allow GPU usage for the project
     """
 
     _backtest_specification_converter = t.Dict(
         {
             t.Key("gap_duration", optional=True): String(),
             t.Key("index", optional=True): Int(),
             t.Key("primary_training_end_date", optional=True): parse_time,
@@ -555,15 +555,14 @@
                 t.Null(), t.Dict({}), FeatureEngineeringOptions._converter
             ),
             t.Key("feature_engineering_prediction_point", optional=True): t.Null()
             | Feature._converter,
             t.Key("featurelist_id", optional=True): t.Null() | String(),
             t.Key("feature_settings", optional=True): t.Null()
             | t.List(_feature_settings_converter),
-            t.Key("force_cpu", optional=True): t.Null() | t.Bool(),
             t.Key("forecast_window_end", optional=True): t.Null() | Int(),
             t.Key("forecast_window_start", optional=True): t.Null() | Int(),
             t.Key("gap_duration", optional=True): t.Null() | String(),
             t.Key("holdout_duration", optional=True): t.Or(t.Null(), String(), Duration._converter),
             t.Key("holdout_end_date", optional=True): t.Null() | parse_time,
             t.Key("holdout_level", optional=True): t.Null() | t.Or(String(), Int()),
             t.Key("holdout_pct", optional=True): t.Null() | Int(),
@@ -603,14 +602,15 @@
             t.Key("segmentation_task_id", optional=True): t.Null() | String(),
             t.Key("segments_count", optional=True): t.Null() | Int(),
             t.Key("target", optional=True): t.Null() | String(),
             t.Key("target_type", optional=True): t.Null() | t.Enum(*TARGET_TYPE.ALL),
             t.Key("training_level", optional=True): t.Null() | t.Or(String(), Int()),
             t.Key("treat_as_exponential", optional=True): t.Null()
             | t.Enum(*TREAT_AS_EXPONENTIAL.ALL),
+            t.Key("use_gpu", optional=True): t.Null() | t.Bool(),
             t.Key("unsupervised_mode", optional=True): t.Null() | t.Bool(),
             t.Key("use_cross_series_features", optional=True): t.Null() | t.Bool(),
             t.Key("use_project_settings", optional=True): t.Null() | t.Bool(),
             t.Key("user_partition_col", optional=True): t.Null() | Feature._converter,
             t.Key("use_time_series", optional=True): t.Null() | t.Bool(),
             t.Key("validation_duration", optional=True): t.Null() | String(),
             t.Key("validation_level", optional=True): t.Null() | t.Or(String(), Int()),
@@ -649,15 +649,14 @@
         feature_derivation_window_end: Optional[int] = None,
         feature_derivation_window_start: Optional[int] = None,
         feature_engineering_graphs: Optional[List[RelationshipGraph]] = None,
         feature_engineering_options: Optional[FeatureEngineeringOptions] = None,
         feature_engineering_prediction_point: Optional[Feature] = None,
         featurelist_id: Optional[str] = None,
         feature_settings: Optional[List[FeatureSettings]] = None,
-        force_cpu: Optional[bool] = None,
         forecast_window_end: Optional[int] = None,
         forecast_window_start: Optional[int] = None,
         gap_duration: Optional[str] = None,
         holdout_duration: Optional[Duration] = None,
         holdout_end_date: Optional[str] = None,
         holdout_level: Optional[Union[str, int]] = None,
         holdout_pct: Optional[int] = None,
@@ -693,14 +692,15 @@
         segmentation_model_package_name: Optional[str] = None,
         segmentation_task_id: Optional[str] = None,
         segments_count: Optional[int] = None,
         target: Optional[str] = None,
         target_type: Optional[TARGET_TYPE] = None,
         training_level: Optional[Union[str, int]] = None,
         treat_as_exponential: Optional[TREAT_AS_EXPONENTIAL] = None,
+        use_gpu: Optional[bool] = None,
         unsupervised_mode: Optional[bool] = None,
         use_cross_series_features: Optional[bool] = None,
         use_project_settings: Optional[bool] = None,
         user_partition_col: Optional[Feature] = None,
         use_time_series: Optional[bool] = None,
         validation_duration: Optional[str] = None,
         validation_level: Optional[Union[str, int]] = None,
@@ -736,15 +736,14 @@
             feature_derivation_window_end=feature_derivation_window_end,
             feature_derivation_window_start=feature_derivation_window_start,
             feature_engineering_graphs=feature_engineering_graphs,
             feature_engineering_options=feature_engineering_options,
             feature_engineering_prediction_point=feature_engineering_prediction_point,
             featurelist_id=featurelist_id,
             feature_settings=feature_settings,
-            force_cpu=force_cpu,
             forecast_window_end=forecast_window_end,
             forecast_window_start=forecast_window_start,
             gap_duration=gap_duration,
             holdout_duration=holdout_duration,
             holdout_end_date=holdout_end_date,
             holdout_level=holdout_level,
             holdout_pct=holdout_pct,
@@ -773,14 +772,15 @@
             segmentation_model_package_name=segmentation_model_package_name,
             segmentation_task_id=segmentation_task_id,
             segments_count=segments_count,
             target=target,
             target_type=target_type,
             training_level=training_level,
             treat_as_exponential=treat_as_exponential,
+            use_gpu=use_gpu,
             unsupervised_mode=unsupervised_mode,
             use_cross_series_features=use_cross_series_features,
             use_project_settings=use_project_settings,
             user_partition_col=user_partition_col,
             use_time_series=use_time_series,
             validation_duration=validation_duration,
             validation_level=validation_level,
@@ -818,15 +818,14 @@
         feature_derivation_window_end: Optional[int] = None,
         feature_derivation_window_start: Optional[int] = None,
         feature_engineering_graphs: Optional[List[RelationshipGraph]] = None,
         feature_engineering_options: Optional[FeatureEngineeringOptions] = None,
         feature_engineering_prediction_point: Optional[Feature] = None,
         featurelist_id: Optional[str] = None,
         feature_settings: Optional[List[FeatureSettings]] = None,
-        force_cpu: Optional[bool] = None,
         forecast_window_end: Optional[int] = None,
         forecast_window_start: Optional[int] = None,
         gap_duration: Optional[str] = None,
         holdout_duration: Optional[Duration] = None,
         holdout_end_date: Optional[str] = None,
         holdout_level: Optional[Union[str, int]] = None,
         holdout_pct: Optional[int] = None,
@@ -857,14 +856,15 @@
         segmentation_model_package_name: Optional[str] = None,
         segmentation_task_id: Optional[str] = None,
         segments_count: Optional[int] = None,
         target: Optional[str] = None,
         target_type: Optional[TARGET_TYPE] = None,
         training_level: Optional[Union[str, int]] = None,
         treat_as_exponential: Optional[TREAT_AS_EXPONENTIAL] = None,
+        use_gpu: Optional[bool] = None,
         unsupervised_mode: Optional[bool] = None,
         use_cross_series_features: Optional[bool] = None,
         use_project_settings: Optional[bool] = None,
         user_partition_col: Optional[Feature] = None,
         use_time_series: Optional[bool] = None,
         validation_duration: Optional[str] = None,
         validation_level: Optional[Union[str, int]] = None,
@@ -942,15 +942,14 @@
                     if "a_priori" not in feature_setting.keys()
                     else {"known_in_advance": feature_setting.pop("a_priori"), **feature_setting}
                 )
                 for feature_setting in feature_settings
             ]
         else:
             self.feature_settings = feature_settings
-        self.force_cpu = force_cpu
         self.forecast_window_end = forecast_window_end
         self.forecast_window_start = forecast_window_start
         self.gap_duration = gap_duration
         if holdout_duration and isinstance(holdout_duration, dict):
             self.holdout_duration = Duration(**holdout_duration)
         else:
             self.holdout_duration = holdout_duration
@@ -985,14 +984,15 @@
         self.segmentation_model_package_name = segmentation_model_package_name
         self.segmentation_task_id = segmentation_task_id
         self.segments_count = segments_count
         self.target = target
         self.target_type = target_type
         self.training_level = training_level
         self.treat_as_exponential = treat_as_exponential
+        self.use_gpu = use_gpu
         self.unsupervised_mode = unsupervised_mode
         self.use_cross_series_features = use_cross_series_features
         self.use_project_settings = use_project_settings
         if user_partition_col and isinstance(user_partition_col, dict):
             self.user_partition_col = Feature(**user_partition_col)
         else:
             self.user_partition_col = user_partition_col
@@ -1091,14 +1091,15 @@
             "model_splits": self.model_splits,
             "number_of_backtests": self.number_of_backtests,
             "prepare_model_for_deployment": self.prepare_model_for_deployment,
             "run_leakage_removed_feature_list": self.run_leakage_removed_feature_list,
             "smart_downsampled": self.smart_downsampled,
             "target": self.target,
             "treat_as_exponential": self.treat_as_exponential,
+            "use_gpu": self.use_gpu,
             "unsupervised_mode": self.unsupervised_mode,
             "use_supervised_feature_reduction": self.use_supervised_feature_reduction,
             "use_time_series": self.use_time_series,
             "validation_duration": self.validation_duration,
             "windows_basis_unit": self.windows_basis_unit,
         }
```

### Comparing `datarobot-3.1.1/datarobot/models/rating_table.py` & `datarobot-3.2.0b0/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/recommended_model.py` & `datarobot-3.2.0b0/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/relationships_configuration.py` & `datarobot-3.2.0b0/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/residuals.py` & `datarobot-3.2.0b0/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/restore_discarded_features.py` & `datarobot-3.2.0b0/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/roc_curve.py` & `datarobot-3.2.0b0/datarobot/models/roc_curve.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,43 +16,26 @@
 import numpy as np
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
 
 if TYPE_CHECKING:
-    from mypy_extensions import TypedDict
-
-    class EstimatedMetric(TypedDict):
-        """Typed dict for estimated metric"""
-
-        accuracy: float
-        f1_score: float
-        false_negative_score: int
-        true_negative_score: int
-        true_negative_rate: float
-        matthews_correlation_coefficient: float
-        true_positive_score: int
-        positive_predictive_value: float
-        false_positive_score: int
-        false_positive_rate: float
-        negative_predictive_value: float
-        true_positive_rate: float
-        threshold: float
+    from datarobot.models.types import RocCurveEstimatedMetric
 
 
 class RocCurveThresholdMixin:  # pylint: disable=missing-class-docstring
-    roc_points: Optional[List[EstimatedMetric]] = None
+    roc_points: Optional[List[RocCurveEstimatedMetric]] = None
 
     @staticmethod
     def _validate_threshold(threshold: float) -> None:
         if threshold > 1 or threshold < 0:
             raise ValueError("threshold must be from [0, 1] interval")
 
-    def estimate_threshold(self, threshold: float) -> EstimatedMetric:
+    def estimate_threshold(self, threshold: float) -> RocCurveEstimatedMetric:
         """Return metrics estimation for given threshold.
 
         Parameters
         ----------
         threshold : float from [0, 1] interval
             Threshold we want estimation for
 
@@ -158,15 +141,15 @@
     """
 
     _converter = RocCurveTrafaret
 
     def __init__(
         self,
         source: str,
-        roc_points: List[EstimatedMetric],
+        roc_points: List[RocCurveEstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
         source_model_id: str,
     ) -> None:
         self.source = source
         self.roc_points = roc_points
         self.negative_class_predictions = negative_class_predictions
@@ -212,15 +195,15 @@
         .merge(RocCurveTrafaret)
         .ignore_extra("*")
     )
 
     def __init__(
         self,
         source: str,
-        roc_points: List[EstimatedMetric],
+        roc_points: List[RocCurveEstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
         source_model_id: str,
         label: str,
         kolmogorov_smirnov_metric: float,
         auc: float,
     ) -> None:
```

### Comparing `datarobot-3.1.1/datarobot/models/ruleset.py` & `datarobot-3.2.0b0/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/secondary_dataset.py` & `datarobot-3.2.0b0/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/segmentation.py` & `datarobot-3.2.0b0/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/service_stats.py` & `datarobot-3.2.0b0/datarobot/models/deployment/service_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from typing import cast, List, Optional, TYPE_CHECKING, Union
 
 import dateutil
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import SERVICE_STAT_METRIC
-from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
+from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         """Type dict for period"""
@@ -51,15 +51,15 @@
         serverErrorRate: float
         numConsumers: int
         cacheHitRatio: float
         medianLoad: float
         peakLoad: float
 
 
-class ServiceStats(APIObject, DeploymentQueryBuilderMixin):
+class ServiceStats(APIObject, MonitoringDataQueryBuilderMixin):
     """Deployment service stats information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve service stats metrics
     period : dict
@@ -175,15 +175,15 @@
         metrics = data.pop("metrics")
 
         data = from_api(data, keep_null_keys=True)
         data["metrics"] = metrics
         return cls.from_data(data)
 
 
-class ServiceStatsOverTime(APIObject, DeploymentQueryBuilderMixin):
+class ServiceStatsOverTime(APIObject, MonitoringDataQueryBuilderMixin):
     """Deployment service stats over time information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metric
     metric : str
```

### Comparing `datarobot-3.1.1/datarobot/models/shap_impact.py` & `datarobot-3.2.0b0/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/shap_matrix.py` & `datarobot-3.2.0b0/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/shap_matrix_job.py` & `datarobot-3.2.0b0/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/sharing.py` & `datarobot-3.2.0b0/datarobot/models/sharing.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import String
+from datarobot.enums import SHARING_RECIPIENT_TYPE, SHARING_ROLE
+from datarobot.errors import InvalidUsageError
 from datarobot.models.api_object import APIObject
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class SharingAccessPayload(TypedDict, total=False):
         username: str
@@ -111,7 +113,62 @@
         """
         payload: SharingAccessPayload = {"username": self.username, "role": self.role}
         if self.can_share is not None:
             payload["can_share"] = self.can_share
         if self.can_use_data is not None:
             payload["can_use_data"] = self.can_use_data
         return payload
+
+
+class SharingRole(APIObject):
+    """
+    Represents metadata about a user who has been granted access to an entity.
+    At least one of `id` or `username` must be set.
+
+    Attributes
+    ----------
+    id : str or None
+        The ID of the user.
+    role : str
+        Represents a particular level of access. Should be one of
+        ``datarobot.enums.SHARING_ROLE``.
+    can_share : bool
+        Indicates whether this user is permitted to share with other users. When False, the
+        user has access to the entity, but can only revoke their own access. They cannot not modify
+        any user's access role. When True, the user can share with any other user at an access
+        role up to their own.
+    share_recipient_type : SHARING_RECIPIENT_TYPE
+        The type of user for the object of the method. Can be ``user`` or ``organization``.
+    user_full_name : str or None
+        The full name of the user.
+    username : str or None
+        The username (usually the email) of the user.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("id", optional=True): t.String,
+            t.Key("user_full_name", optional=True): t.String,
+            t.Key("name", optional=True) >> "username": t.String,
+            t.Key("role"): t.String,
+            t.Key("share_recipient_type"): t.String,
+            t.Key("can_share"): t.Bool,
+        }
+    ).ignore_extra("*")
+
+    def __init__(
+        self,
+        role: SHARING_ROLE,
+        share_recipient_type: SHARING_RECIPIENT_TYPE,
+        can_share: bool,
+        id: Optional[str] = None,
+        user_full_name: Optional[str] = None,
+        username: Optional[str] = None,
+    ):
+        if not id and not username:
+            raise InvalidUsageError("Please include either a username or an ID of a user.")
+        self.id = id
+        self.user_full_name = user_full_name
+        self.role = SHARING_ROLE[role]
+        self.share_recipient_type = share_recipient_type
+        self.username = username
+        self.can_share = can_share
```

### Comparing `datarobot-3.1.1/datarobot/models/trafarets.py` & `datarobot-3.2.0b0/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/training_predictions.py` & `datarobot-3.2.0b0/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/user_blueprints/models.py` & `datarobot-3.2.0b0/datarobot/models/user_blueprints/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
         """
         return cast(
             Response, cls._client.delete(cls._path.format(userBlueprintId=user_blueprint_id))
         )
 
     @classmethod
     def get_input_types(cls) -> UserBlueprintAvailableInput:
@@ -747,15 +747,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
         """
         return UserBlueprintSharingUpdateController.update_shared_roles(
             user_blueprint_id=user_blueprint_id, roles=roles
         )
 
     @classmethod
     def search_catalog(
@@ -1369,15 +1369,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
         """
         roles_json = []
         for role in roles:
             if not isinstance(
                 role,
                 (dict, GrantAccessControlWithUsernameValidator, GrantAccessControlWithIdValidator),
             ):
```

### Comparing `datarobot-3.1.1/datarobot/models/user_blueprints/trafarets.py` & `datarobot-3.2.0b0/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/validators.py` & `datarobot-3.2.0b0/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/visualai/augmentation.py` & `datarobot-3.2.0b0/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/models/visualai/images.py` & `datarobot-3.2.0b0/datarobot/models/visualai/images.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,244 +5,303 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from typing import Optional
+from typing import Any, Dict, List, Optional, Union
 
 import trafaret as t
 
 from datarobot._compat import Int, String
-
-from ...enums import PROJECT_STAGE
-from ..api_object import APIObject
-from ..project import Project
+from datarobot.enums import POST_EDA2_STAGES
+from datarobot.models.api_object import APIObject
+from datarobot.models.project import Project
 
 __all__ = ["Image", "SampleImage", "DuplicateImage"]
 
+PARAMETER_CAN_NOT_YET_BE_USED_ERROR_MSG = (
+    "You are trying to retrieve sample images with certain target values. "
+    "The project is not ready for this yet. "
+    "Either run this method again after your project is ready for "
+    "modeling, or do not pass any target related parameters to this "
+    "method."
+)
+
+TargetValue = Optional[Union[str, int, float, List[str]]]
+
 
 class Image(APIObject):
     """An image stored in a project's dataset.
 
     Attributes
     ----------
-    id: str
+    id : str
         Image ID for this image.
-    image_type: str
+    image_type : str
         Image media type. Accessing this may require a server request
         and an associated delay in returning.
-    image_bytes: [octet]
-        Raw octets of this image. Accessing this may require a server request
+    image_bytes : bytes
+        Raw bytes of this image. Accessing this may require a server request
         and an associated delay in returning.
-    height: int
-        Height of the image in pixels (72 pixels per inch).
-    width: int
-        Width of the image in pixels (72 pixels per inch).
+    height : int
+        Height of the image in pixels.
+    width : int
+        Width of the image in pixels.
     """
 
     _get_path = "projects/{project_id}/images/{image_id}/"
     _bytes_path = "projects/{project_id}/images/{image_id}/file/"
     _converter = t.Dict(
         {
-            t.Key("image_id", optional=True): String(),
-            t.Key("height", optional=True): Int(),
-            t.Key("width", optional=True): Int(),
+            t.Key("image_id"): String(),
+            t.Key("height"): Int(),
+            t.Key("width"): Int(),
+            t.Key("project_id"): String(),
         }
     ).ignore_extra("*")
 
-    def __init__(self, image_id=None, project_id=None, height=0, width=0, **kwargs) -> None:
-        self.id: Optional[str] = image_id
-        self.project_id: Optional[str] = project_id
-        self.__image_type = None
-        self.__image_bytes = None
-        self.height: int = int(height)
-        self.width: int = int(width)
+    def __init__(self, image_id: str, project_id: str, height: int = 0, width: int = 0) -> None:
+        self.id = image_id
+        self.project_id = project_id
+        self.__image_type: Optional[str] = None
+        self.__image_bytes: Optional[bytes] = None
+        self.height = height
+        self.width = width
 
     def __repr__(self) -> str:
         return (
             "datarobot.models.visualai.Image("
             "project_id={0.project_id}, "
             "image_id={0.id}, "
             "height={0.height}, "
             "width={0.width})"
         ).format(self)
 
     @property
-    def image_type(self):
+    def image_type(self) -> Optional[str]:
         if not self.__image_type:
             self.__get_image_bytes()
         return self.__image_type
 
     @property
-    def image_bytes(self):
+    def image_bytes(self) -> Optional[bytes]:
         if not self.__image_bytes:
             self.__get_image_bytes()
         return self.__image_bytes
 
-    def __get_image_bytes(self):
+    def __get_image_bytes(self) -> None:
         path = self._bytes_path.format(project_id=self.project_id, image_id=self.id)
         r_data = self._client.get(path)
         self.__image_type = r_data.headers.get("Content-Type")
         self.__image_bytes = r_data.content
 
     @classmethod
-    def get(cls, project_id, image_id):
+    def get(cls, project_id: str, image_id: str) -> "Image":
         """Get a single image object from project.
 
         Parameters
         ----------
-        project_id: str
-            Project that contains the images.
-        image_id: str
+        project_id : str
+            Id of the project that contains the images.
+        image_id : str
             ID of image to load from the project.
         """
         path = cls._get_path.format(project_id=project_id, image_id=image_id)
         r_data = cls._client.get(path).json()
+        r_data["projectId"] = project_id
         ret = cls.from_server_data(r_data)
-        ret.project_id = project_id
         return ret
 
 
 class SampleImage(APIObject):
     """A sample image in a project's dataset.
 
     If ``Project.stage`` is ``datarobot.enums.PROJECT_STAGE.EDA2`` then
     the ``target_*`` attributes of this class will have values, otherwise
     the values will all be None.
 
     Attributes
     ----------
-    image: Image
+    image : Image
         Image object.
-    target_value: str
+    target_value : TargetValue
         Value associated with the ``feature_name``.
+    project_id : str
+        Id of the project that contains the images.
+
     """
 
-    _list_sample_path = "projects/{project_id}/imageSamples/"
-    _list_images_path = "projects/{project_id}/images/"
+    _list_pre_eda2_path = "projects/{project_id}/imageSamples/"
+    _list_post_eda2_path = "projects/{project_id}/images/"
     _converter = t.Dict(
         {
-            t.Key("image_id", optional=True): String(),
-            t.Key("height", optional=True): Int(),
-            t.Key("width", optional=True): Int(),
+            t.Key("image_id"): String(),
+            t.Key("height"): Int(),
+            t.Key("width"): Int(),
             t.Key("target_value", optional=True): t.Or(
                 t.String(), t.Int(), t.Float(), t.List(String)
             ),
+            t.Key("project_id"): String(),
         }
     ).ignore_extra("*")
 
-    def __init__(self, **kwargs):
-        self.image = Image(**kwargs)
-        self.project_id = kwargs.get("project_id")
-        self.target_value = kwargs.get("target_value")
+    def __init__(
+        self,
+        project_id: str,
+        image_id: str,
+        height: int,
+        width: int,
+        target_value: TargetValue = None,
+    ):
+        self.image = Image(project_id=project_id, image_id=image_id, height=height, width=width)
+        self.project_id = project_id
+        self.target_value = target_value
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             "datarobot.models.visualai.SampleImage("
             "project_id={0.project_id}, "
             "image_id={0.image.id}, "
             "target_value={0.target_value})"
         ).format(self)
 
     @classmethod
-    def list(cls, project_id, feature_name, target_value=None, offset=None, limit=None):
+    def list(
+        cls,
+        project_id: str,
+        feature_name: str,
+        target_value: TargetValue = None,
+        target_bin_start: Optional[Union[int, float]] = None,
+        target_bin_end: Optional[Union[int, float]] = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> List["SampleImage"]:
         """Get sample images from a project.
 
         Parameters
         ----------
-        project_id: str
+        project_id : str
             Project that contains the images.
-        feature_name: str
+        feature_name : str
             Name of feature column that contains images.
-        target_value: str
-            Target value to filter images.
-        offset: int
+        target_value : TargetValue
+            For classification projects - target value to filter images.
+            Please note that you can only use this parameter when the project has finished the EDA2
+            stage.
+        target_bin_start : Optional[Union[int, float]]
+            For regression projects - only images corresponding to the target values above
+            (inclusive) this value will be returned. Must be specified together with target_bin_end.
+            Please note that you can only use this parameter when the project has finished the EDA2
+            stage.
+        target_bin_end : Optional[Union[int, float]]
+            For regression projects - only images corresponding to the target values below
+            (exclusive) this value will be returned. Must be specified together with
+            target_bin_start.
+            Please note that you can only use this parameter when the project has finished the EDA2
+            stage.
+        offset : Optional[int]
             Number of images to be skipped.
-        limit: int
+        limit : Optional[int]
             Number of images to be returned.
         """
         project = Project.get(project_id)
-        list_params = {}
-        if project.stage in [PROJECT_STAGE.EDA2, PROJECT_STAGE.MODELING]:
-            path = cls._list_images_path.format(project_id=project_id)
+        list_params: Dict[str, Any] = {}
+        if project.stage in POST_EDA2_STAGES:
+            path = cls._list_post_eda2_path.format(project_id=project_id)
+            list_params["column"] = feature_name
+            if target_value is not None:
+                list_params["targetValue"] = target_value
+            if target_bin_start is not None:
+                list_params["targetBinStart"] = target_bin_start
+            if target_bin_end is not None:
+                list_params["targetBinEnd"] = target_bin_end
         else:
-            path = cls._list_sample_path.format(project_id=project_id)
-
-        if feature_name:
+            path = cls._list_pre_eda2_path.format(project_id=project_id)
             list_params["featureName"] = feature_name
-        if target_value:
-            list_params["targetValue"] = target_value
+            if (
+                target_value is not None
+                or target_bin_start is not None
+                or target_bin_end is not None
+            ):
+                # This class uses different routes depending on the project stage. Images with
+                # target information are stored as part of the EDA2 workflow. Only the post EDA2
+                # route can query for certain targets.
+                raise RuntimeError(PARAMETER_CAN_NOT_YET_BE_USED_ERROR_MSG)
         if offset:
             list_params["offset"] = int(offset)
         if limit:
             list_params["limit"] = int(limit)
 
         r_data = cls._client.get(path, params=list_params).json()
         ret = []
         for si_data in r_data["data"]:
+            si_data["projectId"] = project_id
             si = cls.from_server_data(si_data)
-            si.project_id = project_id
-            si.image.project_id = project_id
             ret.append(si)
         return ret
 
 
 class DuplicateImage(APIObject):
     """An image that was duplicated in the project dataset.
 
     Attributes
     ----------
-    image: Image
+    image : Image
         Image object.
-    count: int
+    count : int
         Number of times the image was duplicated.
     """
 
     _list_path = "projects/{project_id}/duplicateImages/{feature_name}/"
     _converter = t.Dict(
-        {t.Key("image_id", optional=True): String(), t.Key("row_count", optional=True): Int()}
+        {t.Key("image_id"): String(), t.Key("row_count"): Int(), t.Key("project_id"): String()}
     ).ignore_extra("*")
 
-    def __init__(self, **kwargs):
-        self.image = Image(**kwargs)
-        self.project_id = kwargs.get("project_id")
-        self.count = kwargs.get("row_count")
+    def __init__(self, image_id: str, row_count: int, project_id: str):
+        self.image = Image(project_id=project_id, image_id=image_id, height=0, width=0)
+        self.project_id = project_id
+        self.count = row_count
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             "datarobot.models.visualai.DuplicateImage("
             "project_id={0.project_id}, "
             "image_id={0.image.id}, "
             "count={0.count})"
         ).format(self)
 
     @classmethod
-    def list(cls, project_id, feature_name, offset=None, limit=None):
+    def list(
+        cls,
+        project_id: str,
+        feature_name: str,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> List["DuplicateImage"]:
         """Get all duplicate images in a project.
 
         Parameters
         ----------
-        project_id: str
+        project_id : str
             Project that contains the images.
-        feature_name: str
+        feature_name : str
             Name of feature column that contains images.
-        offset: int
+        offset : Optional[int]
             Number of images to be skipped.
-        limit: int
+        limit : Optional[int]
             Number of images to be returned.
         """
         path = cls._list_path.format(project_id=project_id, feature_name=feature_name)
         list_params = {}
         if offset:
             list_params["offset"] = int(offset)
         if limit:
             list_params["limit"] = int(limit)
         r_data = cls._client.get(path, params=list_params).json()
         ret = []
         for si_data in r_data["data"]:
+            si_data["projectId"] = project_id
             si = cls.from_server_data(si_data)
-            si.project_id = project_id
-            si.image.project_id = project_id
             ret.append(si)
         return ret
```

### Comparing `datarobot-3.1.1/datarobot/models/visualai/insights.py` & `datarobot-3.2.0b0/datarobot/models/visualai/insights.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,296 +5,372 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+# pylint: disable=unsupported-binary-operation
+from typing import Dict, List, Optional, Tuple, Union
+
 import trafaret as t
+from trafaret import Float
 
 from datarobot._compat import Int, String
-
-from ..api_object import APIObject
-from .images import Image
+from datarobot.models.api_object import APIObject
+from datarobot.models.visualai.images import Image, TargetValue
 
 __all__ = ["ImageEmbedding", "ImageActivationMap"]
 
 
 class ImageEmbedding(APIObject):
     """Vector representation of an image in an embedding space.
 
     A vector in an embedding space will allow linear computations to
     be carried out between images: for example computing the Euclidean
     distance of the images.
 
     Attributes
     ----------
-    image: Image
+    image : Image
         Image object used to create this map.
-    feature_name: str
+    feature_name : str
         Name of the feature column this embedding is associated with.
-    position_x: int
+    position_x : int
         X coordinate of the image in the embedding space.
-    position_y: int
+    position_y : int
         Y coordinate of the image in the embedding space.
-    actual_target_value: object
+    actual_target_value : object
         Actual target value of the dataset row.
+    target_values : Optional[List[str]]
+        For classification projects, a list of target values of this project.
+    target_bins : Optional[List[Dict[str, float]]]
+        For regression projects, a list of target bins of this project.
+    project_id : str
+        Id of the project this Image Embedding belongs to.
+    model_id : str
+        Id of the model this Image Embedding belongs to.
     """
 
     _compute_path = "projects/{project_id}/models/{model_id}/imageEmbeddings/"
-    _models_path = "projects/{project_id}/imageEmbeddings/"
-    _list_path = "projects/{project_id}/models/{model_id}/imageEmbeddings/"
+    _list_metadata_path = "projects/{project_id}/imageEmbeddings/"
+    _list_embeddings_path = "projects/{project_id}/models/{model_id}/imageEmbeddings/"
     _converter = t.Dict(
         {
-            t.Key("image_id", optional=True): String(),
-            t.Key("position_x", optional=True): t.Float(),
-            t.Key("position_y", optional=True): t.Float(),
-            t.Key("actual_target_value", optional=True): t.Any(),
-            t.Key("target_values", optional=True): t.Or(t.List(String()), t.Null),
-            t.Key("target_bins", optional=True): t.Or(t.List(t.Any()), t.Null),
+            t.Key("feature_name"): t.String(),
+            t.Key("position_x"): t.Float(),
+            t.Key("position_y"): t.Float(),
+            t.Key("image_id"): String(),
+            t.Key("project_id"): t.String(),
+            t.Key("model_id"): t.String(),
+            t.Key("actual_target_value", optional=True): t.Null()
+            | t.String()
+            | t.Int()
+            | t.Float()
+            | t.List(t.String),
+            t.Key("target_values", optional=True): t.List(String()) | t.Null,
+            t.Key("target_bins", optional=True): t.List(t.Mapping(String(), Float())) | t.Null,
         }
     ).ignore_extra("*")
 
-    def __init__(self, **kwargs):
-        self.project_id = kwargs.get("project_id")
-        self.model_id = kwargs.get("model_id")
-        self.image = Image(**kwargs)
-        self.feature_name = kwargs.get("feature_name")
-        self.position_x = kwargs.get("position_x")
-        self.position_y = kwargs.get("position_y")
-        self.actual_target_value = kwargs.get("actual_target_value")
+    def __init__(
+        self,
+        feature_name: str,
+        position_x: float,
+        position_y: float,
+        image_id: str,
+        project_id: str,
+        model_id: str,
+        actual_target_value: TargetValue = None,
+        target_values: Optional[List[str]] = None,
+        target_bins: Optional[List[Dict[str, float]]] = None,
+    ) -> None:
+        self.project_id = project_id
+        self.model_id = model_id
+        self.image = Image(project_id=project_id, image_id=image_id, width=0, height=0)
+        self.feature_name = feature_name
+        self.position_x = position_x
+        self.position_y = position_y
+        self.actual_target_value = actual_target_value
+        self.target_values = target_values
+        self.target_bins = target_bins
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             "datarobot.models.visualai.ImageEmbedding("
             "project_id={0.project_id}, "
             "model_id={0.model_id}, "
             "feature_name={0.feature_name}, "
             "position_x={0.position_x}, "
             "position_y={0.position_y}, "
             "image_id={0.image.id})"
         ).format(self)
 
     @classmethod
-    def compute(cls, project_id, model_id):
-        """Start creation of image embeddings for the model.
+    def compute(cls, project_id: str, model_id: str) -> str:
+        """Start the computation of image embeddings for the model.
 
         Parameters
         ----------
-        project_id: str
+        project_id : str
             Project to start creation in.
-        model_id: str
+        model_id : str
             Project's model to start creation in.
 
         Returns
         -------
         str
             URL to check for image embeddings progress.
 
         Raises
         ------
         datarobot.errors.ClientError
             Server rejected creation due to client error. Most likely
             cause is bad ``project_id`` or ``model_id``.
         """
         path = cls._compute_path.format(project_id=project_id, model_id=model_id)
-        r_data = cls._client.post(path).json()
+        r_data: Dict[str, str] = cls._client.post(path).json()
         return r_data["url"]
 
     @classmethod
-    def models(cls, project_id):
-        """List the models in a project.
+    def models(cls, project_id: str) -> List[Tuple[str, str]]:
+        """
+        For a given project_id, list all model_id - feature_name pairs with available
+        Image Embeddings.
 
         Parameters
         ----------
-        project_id: str
-            Project that contains the models.
+        project_id : str
+            Id of the project to list model_id - feature_name pairs with available Image Embeddings
+            for.
 
         Returns
         -------
         list( tuple(model_id, feature_name) )
              List of model and feature name pairs.
         """
-        path = cls._models_path.format(project_id=project_id)
+        path = cls._list_metadata_path.format(project_id=project_id)
         r_data = cls._client.get(path).json()
         return [(d["modelId"], d["featureName"]) for d in r_data.get("data", [])]
 
     @classmethod
-    def list(cls, project_id, model_id, feature_name):
+    def list(cls, project_id: str, model_id: str, feature_name: str) -> List["ImageEmbedding"]:
         """Return a list of ImageEmbedding objects.
 
         Parameters
         ----------
         project_id: str
-            Project that contains the images.
+            Id of the project the model belongs to.
         model_id: str
-            Model that contains the images.
+            Id of the model to list Image Embeddings for.
         feature_name: str
-            Name of feature column that contains images.
+            Name of feature column to list Image Embeddings for.
         """
-        path = cls._list_path.format(project_id=project_id, model_id=model_id)
+        path = cls._list_embeddings_path.format(project_id=project_id, model_id=model_id)
         list_params = {}
         list_params["featureName"] = feature_name
         r_data = cls._client.get(path, params=list_params).json()
         ret = []
         for embed_data in r_data.get("embeddings", []):
+            embed_data["targetBins"] = r_data["targetBins"]
+            embed_data["targetValues"] = r_data["targetValues"]
+            embed_data["projectId"] = project_id
+            embed_data["modelId"] = model_id
+            embed_data["featureName"] = feature_name
             embed = cls.from_server_data(embed_data)
-            embed.project_id = project_id
-            embed.model_id = model_id
-            embed.feature_name = feature_name
-            embed.image.project_id = project_id
             ret.append(embed)
         return ret
 
 
 class ImageActivationMap(APIObject):
     """Mark areas of image with weight of impact on training.
 
     This is a technique to display how various areas of the region were
     used in training, and their effect on predictions. Larger values in
     ``activation_values`` indicates a larger impact.
 
     Attributes
     ----------
-    image: Image
+    image : Image
         Image object used to create this map.
-    overlay_image: Image
-        Image object composited with activation heat map.
-    feature_name: str
-        Name of the feature column that contains the value this map is
-        based on.
-    height: int
-        Height of the original image in pixels.
-    width: int
-        Width of the original image in pixels.
-    actual_target_value: object
-        Actual target value of the dataset row.
-    predicted_target_value: object
-        Predicted target value of the dataset row that contains this image.
-    activation_values: [ [ int ] ]
+    overlay_image : Image
+        Image object containing the original image overlaid by the activation heatmap.
+    feature_name : str
+        Name of the feature column that contains the value this map is based on.
+    activation_values : List[List[int]]
         A row-column matrix that contains the activation strengths for
         image regions. Values are integers in the range [0, 255].
+    actual_target_value : TargetValue
+        Actual target value of the dataset row.
+    predicted_target_value : TargetValue
+        Predicted target value of the dataset row that contains this image.
+    target_values : Optional[List[str]]
+        For classification projects a list of target values of this project.
+    target_bins : Optional[List[Dict[str, float]]]
+        For regression projects a list of target bins.
+    project_id : str
+        Id of the project this Activation Map belongs to.
+    model_id : str
+        Id of the model this Activation Map belongs to.
     """
 
     _compute_path = "projects/{project_id}/models/{model_id}/imageActivationMaps/"
-    _models_path = "projects/{project_id}/imageActivationMaps/"
-    _list_path = "projects/{project_id}/models/{model_id}/imageActivationMaps/"
+    _list_metadata_path = "projects/{project_id}/imageActivationMaps/"
+    _list_model_path = "projects/{project_id}/models/{model_id}/imageActivationMaps/"
     _converter = t.Dict(
         {
-            t.Key("image_id", optional=True): String(),
-            t.Key("overlay_image_id", optional=True): String(),
-            t.Key("feature_name", optional=True): String(),
-            t.Key("image_width", to_name="width", optional=True): Int(),
-            t.Key("image_height", to_name="height", optional=True): Int(),
-            t.Key("activation_values", optional=True): t.List(t.List(Int())),
-            t.Key("actual_target_value", optional=True): t.Any(),
-            t.Key("predicted_target_value", optional=True): t.Any(),
+            t.Key("feature_name"): String(),
+            t.Key("activation_values"): t.List(t.List(Int())),
+            t.Key("image_width"): Int(),
+            t.Key("image_height"): Int(),
+            t.Key("image_id"): String(),
+            t.Key("overlay_image_id"): String(),
+            t.Key("project_id"): t.String(),
+            t.Key("model_id"): t.String(),
+            t.Key("actual_target_value", optional=True): t.Null()
+            | t.String()
+            | t.Int()
+            | t.Float()
+            | t.List(t.String),
+            t.Key("predicted_target_value", optional=True): t.Null()
+            | t.String()
+            | t.Int()
+            | t.Float()
+            | t.List(t.String),
             t.Key("target_values", optional=True): t.Or(t.List(String()), t.Null),
-            t.Key("target_bins", optional=True): t.Or(t.List(t.Any()), t.Null),
+            t.Key("target_bins", optional=True): t.List(t.Mapping(String(), Float())) | t.Null,
         }
     ).ignore_extra("*")
 
-    def __init__(self, **kwargs):
-        self.project_id = kwargs.get("project_id")
-        self.model_id = kwargs.get("model_id")
-        self.image = Image(**kwargs)
-        self.overlay_image = Image(
-            image_id=kwargs.get("overlay_image_id", kwargs.get("image_id")),
-            project_id=kwargs.get("project_id"),
-            height=kwargs.get("height", 0),
-            width=kwargs.get("width", 0),
-        )
-        self.feature_name = kwargs.get("feature_name")
-        self.actual_target_value = kwargs.get("actual_target_value")
-        self.predicted_target_value = kwargs.get("predicted_target_value")
-        self.activation_values = kwargs.get("activation_values")
-
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             "datarobot.models.visualai.ActivationMap("
             "project_id={0.project_id}, "
             "model_id={0.model_id}, "
             "feature_name={0.feature_name}, "
             "image_id={0.image.id}, "
             "overlay_image_id={0.overlay_image.id}, "
             "height={0.image.height}, "
             "width={0.image.width})"
         ).format(self)
 
+    def __init__(
+        self,
+        feature_name: str,
+        activation_values: List[List[int]],
+        image_width: int,
+        image_height: int,
+        image_id: str,
+        overlay_image_id: str,
+        project_id: str,
+        model_id: str,
+        actual_target_value: TargetValue = None,
+        predicted_target_value: TargetValue = None,
+        target_values: Optional[List[str]] = None,
+        target_bins: Optional[List[Dict[str, float]]] = None,
+    ):
+        self.project_id = project_id
+        self.model_id = model_id
+        self.image = Image(
+            project_id=project_id, width=image_width, height=image_height, image_id=image_id
+        )
+        self.overlay_image = Image(
+            image_id=overlay_image_id,
+            project_id=project_id,
+            height=0,
+            width=0,
+        )
+        self.feature_name = feature_name
+        self.actual_target_value = actual_target_value
+        self.predicted_target_value = predicted_target_value
+        self.activation_values = activation_values
+        self.target_values = target_values
+        self.target_bins = target_bins
+
     @classmethod
-    def compute(cls, project_id, model_id):
-        """Start creation of a activation map in the given model.
+    def compute(cls, project_id: str, model_id: str) -> str:
+        """Start the computation of activation maps for the given model.
 
         Parameters
         ----------
-        project_id: str
+        project_id : str
             Project to start creation in.
-        model_id: str
+        model_id : str
             Project's model to start creation in.
 
         Returns
         -------
         str
             URL to check for image embeddings progress.
 
         Raises
         ------
         datarobot.errors.ClientError
             Server rejected creation due to client error. Most likely
             cause is bad ``project_id`` or ``model_id``.
         """
         path = cls._compute_path.format(project_id=project_id, model_id=model_id)
-        r_data = cls._client.post(path).json()
+        r_data: Dict[str, str] = cls._client.post(path).json()
         return r_data["url"]
 
     @classmethod
-    def models(cls, project_id):
-        """List the models in a project.
+    def models(cls, project_id: str) -> List[Tuple[str, str]]:
+        """
+        For a given project_id, list all model_id - feature_name pairs with available
+        Image Activation Maps.
 
         Parameters
         ----------
-        project_id: str
-            Project that contains the models.
+        project_id : str
+            Id of the project to list model_id - feature_name pairs with available
+            Image Activation Maps for.
 
         Returns
         -------
         list( tuple(model_id, feature_name) )
              List of model and feature name pairs.
         """
-        path = cls._models_path.format(project_id=project_id)
+        path = cls._list_metadata_path.format(project_id=project_id)
         r_data = cls._client.get(path).json()
         return [(d["modelId"], d["featureName"]) for d in r_data.get("data", [])]
 
     @classmethod
-    def list(cls, project_id, model_id, feature_name, offset=None, limit=None):
+    def list(
+        cls,
+        project_id: str,
+        model_id: str,
+        feature_name: str,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> List["ImageActivationMap"]:
         """Return a list of ImageActivationMap objects.
 
         Parameters
         ----------
-        project_id: str
+        project_id : str
             Project that contains the images.
-        model_id: str
+        model_id : str
             Model that contains the images.
-        feature_name: str
+        feature_name : str
             Name of feature column that contains images.
-        offset: int
+        offset : Optional[int]
             Number of images to be skipped.
-        limit: int
+        limit : Optional[int]
             Number of images to be returned.
         """
-        path = cls._list_path.format(project_id=project_id, model_id=model_id)
-        list_params = {}
+        path = cls._list_model_path.format(project_id=project_id, model_id=model_id)
+        list_params: Dict[str, Union[str, int]] = {}
         list_params["featureName"] = feature_name
-        if offset:
-            list_params["offset"] = int(offset)
-        if limit:
-            list_params["limit"] = int(limit)
+        if offset is not None:
+            list_params["offset"] = offset
+        if limit is not None:
+            list_params["limit"] = limit
         r_data = cls._client.get(path, params=list_params).json()
         ret = []
         for amap_data in r_data.get("activationMaps", []):
+            amap_data["targetBins"] = r_data["targetBins"]
+            amap_data["targetValues"] = r_data["targetValues"]
+            amap_data["projectId"] = project_id
+            amap_data["modelId"] = model_id
             amap = cls.from_server_data(amap_data)
-            amap.project_id = project_id
-            amap.model_id = model_id
-            amap.image.project_id = project_id
-            amap.overlay_image.project_id = project_id
             ret.append(amap)
         return ret
```

### Comparing `datarobot-3.1.1/datarobot/models/word_cloud.py` & `datarobot-3.2.0b0/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/rest.py` & `datarobot-3.2.0b0/datarobot/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -328,15 +328,18 @@
         # pylint rule disabled because we wanted a clearer docstring
         # for this function than what is provided by APIObject, and
         # this is the only way I know to do this other than writing
         # manual docs in the .rst files
         return super(RESTClientObject, self).open_in_browser()
 
 
-def _http_message(response: Response) -> str:  # pylint: disable=missing-function-docstring
+def _http_message(response: Response) -> str:
+    """
+    Helper function to retrieve the message from a Response object.
+    """
     if response.status_code == 401:
         message = (
             "The server is saying you are not properly "
             "authenticated. Please make sure your API "
             "token is valid."
         )
     elif response.headers["content-type"] == "application/json":
@@ -407,33 +410,36 @@
             t.Key("endpoint"): String(),
             t.Key("token"): String(),
             t.Key("connect_timeout", optional=True): Int(),
             t.Key("ssl_verify", optional=True): t.Or(t.Bool(), String()),
             t.Key("user_agent_suffix", optional=True): String(),
             t.Key("max_retries", optional=True): Int(),
             t.Key("token_type", optional=True): String(),
+            t.Key("default_use_case", optional=True): String(),
         }
     ).allow_extra("*")
     _fields = {k.to_name or k.name for k in _converter.keys}
 
     def __init__(
         self,
         endpoint: str,
         token: str,
         connect_timeout: Optional[int] = None,
         ssl_verify: bool = True,
         user_agent_suffix: Optional[str] = None,
         max_retries: Optional[Union[int, Retry]] = None,
         token_type: Optional[str] = None,
+        default_use_case: Optional[str] = None,
     ) -> None:
         self.endpoint = endpoint
         self.token = token
         self.connect_timeout = connect_timeout
         self.ssl_verify = ssl_verify
         self.user_agent_suffix = user_agent_suffix
         self.max_retries = max_retries
         self.token_type = token_type
+        self.default_use_case = default_use_case
 
     @classmethod
     def from_data(cls, data: Dict[str, Any]) -> DataRobotClientConfig:
         checked = {k: v for k, v in cls._converter.check(data).items() if k in cls._fields}
         return cls(**checked)
```

### Comparing `datarobot-3.1.1/datarobot/utils/__init__.py` & `datarobot-3.2.0b0/datarobot/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module is not considered part of the public interface. As of 2.3, anything here
 may change or be removed without warning."""
 from __future__ import annotations
 
 from collections import defaultdict
+from copy import deepcopy
 from datetime import date, datetime
 import re
 from typing import Any, cast, Dict, Iterable, List, Match, Optional, Tuple, TYPE_CHECKING, Union
 
 from dateutil import parser, tz
 import numpy as np
 import pandas as pd
@@ -70,15 +71,17 @@
     do_recursive: bool = True,
     keep_attrs: Optional[Union[Iterable[str], Iterable[List[str]]]] = None,
     keep_null_keys: bool = False,
 ) -> ServerDataType:
     if type(data) not in (dict, list):
         return data
     if isinstance(data, list):
-        return _from_api_list(data, do_recursive=do_recursive, keep_null_keys=keep_null_keys)
+        return _from_api_list(
+            data, do_recursive=do_recursive, keep_attrs=keep_attrs, keep_null_keys=keep_null_keys
+        )
     return _from_api_dict(
         data, do_recursive=do_recursive, keep_attrs=keep_attrs, keep_null_keys=keep_null_keys
     )
 
 
 # pylint: disable-next=missing-function-docstring
 def _from_api_dict(
@@ -105,30 +108,37 @@
         k_under = underscorize(k)
         if v is None and k_under not in current_level and not keep_null_keys:
             continue
         if do_recursive:
             data_val = from_api(
                 v,
                 do_recursive=do_recursive,
-                keep_attrs=next_level_attrs,
+                keep_attrs=deepcopy(next_level_attrs),
                 keep_null_keys=keep_null_keys,
             )
         else:
             data_val = v
         app_data[k_under] = data_val
     return app_data
 
 
 def _from_api_list(
     data: ServerDataListType,
     do_recursive: bool = True,
+    keep_attrs: Optional[Union[Iterable[str], Iterable[List[str]]]] = None,
     keep_null_keys: bool = False,
 ) -> List[Any]:
     return [
-        from_api(datum, do_recursive=do_recursive, keep_null_keys=keep_null_keys) for datum in data
+        from_api(
+            datum,
+            do_recursive=do_recursive,
+            keep_attrs=deepcopy(keep_attrs),
+            keep_null_keys=keep_null_keys,
+        )
+        for datum in data
     ]
 
 
 def remove_empty_keys(
     metadata: Dict[str, Any],
     keep_attrs: Optional[List[str]] = None,
 ) -> Dict[str, Any]:
```

### Comparing `datarobot-3.1.1/datarobot/utils/deprecation.py` & `datarobot-3.2.0b0/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/utils/pagination.py` & `datarobot-3.2.0b0/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/utils/retry.py` & `datarobot-3.2.0b0/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/utils/source.py` & `datarobot-3.2.0b0/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/utils/sourcedata.py` & `datarobot-3.2.0b0/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot/utils/waiters.py` & `datarobot-3.2.0b0/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/datarobot.egg-info/PKG-INFO` & `datarobot-3.2.0b0/datarobot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot
-Version: 3.1.1
+Version: 3.2.0b0
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
@@ -12,14 +12,16 @@
 Project-URL: Changelog, https://datarobot-public-api-client.readthedocs-hosted.com/page/CHANGES.html
 Project-URL: Bug Reporting, https://community.datarobot.com/t5/forums/postpage/board-id/datarobot-api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: dev
 Provides-Extra: examples
```

### Comparing `datarobot-3.1.1/datarobot.egg-info/requires.txt` & `datarobot-3.2.0b0/datarobot.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 pandas>=0.15
 numpy
 pyyaml>=3.11
-requests>=2.21
+requests>=2.28.1
 requests_toolbelt>=0.6
 trafaret!=1.1.0,<2.2,>=0.7
-urllib3>=1.23
+urllib3<2.0.0,>=1.23
 typing-extensions<5,>=4.3.0
+mypy-extensions<2,>=0.4.0
 
 [dev]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
 pytest-asyncio
@@ -20,23 +21,20 @@
 pylint==2.15.0
 mypy==1.0.0
 types-PyYAML==6.0.12
 types-python-dateutil==2.8.19
 types-pytz==2022.2.1.0
 types-requests==2.28.11
 types-urllib3==1.26.25
-Sphinx==1.8.3
-sphinx_rtd_theme==0.1.9
-nbsphinx<1,>=0.2.9
-mistune==0.8.4
-nbconvert==5.3.1
-numpydoc>=0.6.0
+Sphinx==4.3.2
+sphinx_rtd_theme==1.0.0
+nbsphinx==0.8.9
+numpydoc==1.4.0
 jupyter_contrib_nbextensions
-tornado<6.0
-jsonschema<=4.3.1
+sphinx-autodoc-typehints==1.17.1
 
 [examples]
 jupyter<=5.0
 fredapi==0.4.0
 matplotlib>=2.1.0
 seaborn<=0.8
 scikit-learn<=0.18.2
```

### Comparing `datarobot-3.1.1/pyproject.toml` & `datarobot-3.2.0b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 profile = "black"
 # See https://pycqa.github.io/isort/docs/configuration/profiles/
 # Overrides for the profile:
 force_alphabetical_sort_within_sections = true
 force_sort_within_sections = true
 line_length = 100
 skip_gitignore = true
+known_first_party = ["datarobotx", "datarobot"]
 
 
 [tool.mypy]
 python_version = 3.7
 exclude = '''(?x)(
     build/*
     | tests/*
@@ -53,32 +54,24 @@
 
     # Ignore specific files in helpers directory
     "datarobot.helpers.partitioning_methods",
 
     ### START Models directory
     ### These rules are purposely one file at a time in this directory so any new files added _must_ have annotations
     ### And also we can delete an entry for a file and fix the corresponding errors as we piece-meal annotate the whole repo.
-    "datarobot.models.anomaly_assessment",
     "datarobot.models.api_object",
-    "datarobot.models.automated_documentation",
     "datarobot.models.batch_prediction_job",
-    "datarobot.models.compliance_doc_template",
-    "datarobot.models.confusion_chart",
-    "datarobot.models.custom_model",
     "datarobot.models.custom_model_test",
-    "datarobot.models.custom_model_version",
     "datarobot.models.custom_task_version",
-    "datarobot.models.data_drift",
     "datarobot.models.data_engine_query_generator",
     "datarobot.models.datetime_trend_plots",
     "datarobot.models.execution_environment",
     "datarobot.models.execution_environment_version",
     "datarobot.models.feature",
     "datarobot.models.feature_effect",
-    "datarobot.models.feature_fit",
     "datarobot.models.job",
     "datarobot.models.lift_chart",
     "datarobot.models.model",
     "datarobot.models.modeljob",
     "datarobot.models.pairwise_statistics",
     "datarobot.models.pareto_front",
     "datarobot.models.predict_job",
@@ -86,16 +79,15 @@
     "datarobot.models.project",
     "datarobot.models.project_options",
     "datarobot.models.relationships_configuration",
     "datarobot.models.training_predictions",
 
     ### Sub-directories in models
     "datarobot.models.external_dataset_scores_insights.external_confusion_chart",
+    "datarobot.models.deployment.data_drift",
     "datarobot.models.user_blueprints.models",
-    "datarobot.models.visualai.images",
-    "datarobot.models.visualai.insights",
 
     # Ignore specific files in datarobot sub-directory of repo.
     "datarobot.client",
     "datarobot.enums",
 ]
 ignore_errors = true
```

### Comparing `datarobot-3.1.1/setup.py` & `datarobot-3.2.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot-3.1.1/setup_major.py` & `datarobot-3.2.0b0/setup_major.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #
-# Copyright 2021 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from setuptools import find_packages, setup
 
 from common_setup import common_setup_kwargs, DEFAULT_CLASSIFIERS, DESCRIPTION_TEMPLATE, version
 
-if "b" in version:
-    msg = (
-        "Major releases must not have a 'b' for beta in the version. "
-        "Go back and make a release branch with tag, then update the version number."
-    )
-    raise RuntimeError(msg)
+# if "b" in version:
+#     msg = (
+#         "Major releases must not have a 'b' for beta in the version. "
+#         "Go back and make a release branch with tag, then update the version number."
+#     )
+#     raise RuntimeError(msg)
 
 python_versions = ">= 3.7"
 
 description = DESCRIPTION_TEMPLATE.format(
     package_name="datarobot",
     pypi_url_target="https://pypi.python.org/pypi/datarobot/",
     extra_desc="",
```

