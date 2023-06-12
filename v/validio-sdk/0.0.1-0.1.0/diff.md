# Comparing `tmp/validio_sdk-0.0.1.tar.gz` & `tmp/validio_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_sdk-0.0.1.tar", max compression
+gzip compressed data, was "validio_sdk-0.1.0.tar", max compression
```

## Comparing `validio_sdk-0.0.1.tar` & `validio_sdk-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,198 @@
--rw-r--r--   0        0        0    11340 2023-05-04 06:18:28.959331 validio_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0      939 2023-05-05 14:49:06.709303 validio_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-04 06:18:28.961393 validio_sdk-0.0.1/validio_sdk/__init__.py
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 validio_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-12 09:21:57.913576 validio_sdk-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4718 2023-06-12 09:22:09.649622 validio_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/apply.py
+-rw-r--r--   0        0        0     4155 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/plan.py
+-rw-r--r--   0        0        0     1565 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/scaffold.py
+-rw-r--r--   0        0        0      305 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/settings.py
+-rw-r--r--   0        0        0     5644 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/config.py
+-rw-r--r--   0        0        0   244487 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/__init__.py
+-rw-r--r--   0        0        0      573 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/apply_validator_recommendation.py
+-rw-r--r--   0        0        0     7251 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      526 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/aws_credential_secret_changed.py
+-rw-r--r--   0        0        0      613 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
+-rw-r--r--   0        0        0      614 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/backfill_source.py
+-rw-r--r--   0        0        0     1899 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/base_model.py
+-rw-r--r--   0        0        0   578403 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/client.py
+-rw-r--r--   0        0        0      445 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_credential.py
+-rw-r--r--   0        0        0      528 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_kinesis_source.py
+-rw-r--r--   0        0        0      526 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_redshift_credential.py
+-rw-r--r--   0        0        0      480 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_redshift_source.py
+-rw-r--r--   0        0        0      418 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_s3_source.py
+-rw-r--r--   0        0        0      843 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      823 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      455 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_demo_credential.py
+-rw-r--r--   0        0        0      407 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_demo_source.py
+-rw-r--r--   0        0        0      407 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_file_window.py
+-rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_fixed_batch_window.py
+-rw-r--r--   0        0        0      702 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      682 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      539 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      481 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_big_query_source.py
+-rw-r--r--   0        0        0      445 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_credential.py
+-rw-r--r--   0        0        0      500 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      459 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_storage_source.py
+-rw-r--r--   0        0        0      514 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_notification_rule_v2.py
+-rw-r--r--   0        0        0      753 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      803 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      783 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      823 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      682 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      662 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      702 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      516 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_postgre_sql_credential.py
+-rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_postgre_sql_source.py
+-rw-r--r--   0        0        0      733 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      713 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      753 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      753 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      528 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_saml_identity_provider.py
+-rw-r--r--   0        0        0      438 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_segmentation.py
+-rw-r--r--   0        0        0      477 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_sessionized_window.py
+-rw-r--r--   0        0        0      429 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_slack_channel.py
+-rw-r--r--   0        0        0      505 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_snowflake_credential.py
+-rw-r--r--   0        0        0      517 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_snowflake_destination.py
+-rw-r--r--   0        0        0      457 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_snowflake_source.py
+-rw-r--r--   0        0        0      447 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_tumbling_window.py
+-rw-r--r--   0        0        0      328 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_user.py
+-rw-r--r--   0        0        0      672 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      652 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      449 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_webhook_channel.py
+-rw-r--r--   0        0        0      364 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_channel.py
+-rw-r--r--   0        0        0      614 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_credential.py
+-rw-r--r--   0        0        0      622 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_credentials.py
+-rw-r--r--   0        0        0      630 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_destination.py
+-rw-r--r--   0        0        0      638 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_destinations.py
+-rw-r--r--   0        0        0      376 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_identity.py
+-rw-r--r--   0        0        0      487 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_identity_provider.py
+-rw-r--r--   0        0        0      514 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_notification_rule_v2.py
+-rw-r--r--   0        0        0      646 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_segmentation.py
+-rw-r--r--   0        0        0      536 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_source.py
+-rw-r--r--   0        0        0      544 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_sources.py
+-rw-r--r--   0        0        0      328 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_user.py
+-rw-r--r--   0        0        0      606 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_validators.py
+-rw-r--r--   0        0        0      536 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_window.py
+-rw-r--r--   0        0        0      544 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_windows.py
+-rw-r--r--   0        0        0      589 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py
+-rw-r--r--   0        0        0     3065 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/enums.py
+-rw-r--r--   0        0        0     2314 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/exceptions.py
+-rw-r--r--   0        0        0   172648 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/fragments.py
+-rw-r--r--   0        0        0      526 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py
+-rw-r--r--   0        0        0     2896 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_channel_by_resource_name.py
+-rw-r--r--   0        0        0     2427 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_channels.py
+-rw-r--r--   0        0        0     4965 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_credential_by_resource_name.py
+-rw-r--r--   0        0        0     5997 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_destination_by_resource_name.py
+-rw-r--r--   0        0        0     2218 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
+-rw-r--r--   0        0        0     2033 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_identity_providers.py
+-rw-r--r--   0        0        0      652 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_notification_rule_v2_by_resource_name.py
+-rw-r--r--   0        0        0      505 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_notification_rules_v2.py
+-rw-r--r--   0        0        0     3324 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_segment_incidents.py
+-rw-r--r--   0        0        0      357 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_segmentation.py
+-rw-r--r--   0        0        0      572 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
+-rw-r--r--   0        0        0    20258 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_source.py
+-rw-r--r--   0        0        0    24833 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_source_by_resource_name.py
+-rw-r--r--   0        0        0    21532 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_source_recommended_validators.py
+-rw-r--r--   0        0        0      476 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_user_by_resource_name.py
+-rw-r--r--   0        0        0      300 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_users.py
+-rw-r--r--   0        0        0    40168 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator.py
+-rw-r--r--   0        0        0    48254 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_by_resource_name.py
+-rw-r--r--   0        0        0     3404 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_incidents.py
+-rw-r--r--   0        0        0     3691 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_segment_incidents.py
+-rw-r--r--   0        0        0     3986 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_segment_metrics.py
+-rw-r--r--   0        0        0     5711 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_window_by_resource_name.py
+-rw-r--r--   0        0        0      290 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
+-rw-r--r--   0        0        0      308 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_aws_redshift_schema.py
+-rw-r--r--   0        0        0      270 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_aws_s3_schema.py
+-rw-r--r--   0        0        0      265 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_demo_schema.py
+-rw-r--r--   0        0        0      309 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
+-rw-r--r--   0        0        0      318 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
+-rw-r--r--   0        0        0      287 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
+-rw-r--r--   0        0        0      290 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_storage_schema.py
+-rw-r--r--   0        0        0      290 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_postgre_sql_schema.py
+-rw-r--r--   0        0        0      285 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_snowflake_schema.py
+-rw-r--r--   0        0        0    34024 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/input_types.py
+-rw-r--r--   0        0        0     4316 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_credentials.py
+-rw-r--r--   0        0        0     5202 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_destinations.py
+-rw-r--r--   0        0        0      457 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_segmentations.py
+-rw-r--r--   0        0        0    21364 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_sources.py
+-rw-r--r--   0        0        0    42237 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_validators.py
+-rw-r--r--   0        0        0     4976 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_windows.py
+-rw-r--r--   0        0        0      603 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
+-rw-r--r--   0        0        0      522 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/scalars.py
+-rw-r--r--   0        0        0      592 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
+-rw-r--r--   0        0        0      566 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/start_source.py
+-rw-r--r--   0        0        0      550 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/stop_source.py
+-rw-r--r--   0        0        0      441 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_credential.py
+-rw-r--r--   0        0        0      524 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_kinesis_source.py
+-rw-r--r--   0        0        0      522 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_redshift_credential.py
+-rw-r--r--   0        0        0      476 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_redshift_source.py
+-rw-r--r--   0        0        0      414 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_s3_source.py
+-rw-r--r--   0        0        0      636 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py
+-rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_fixed_batch_window.py
+-rw-r--r--   0        0        0      491 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_freshness_validator.py
+-rw-r--r--   0        0        0      535 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      477 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_big_query_source.py
+-rw-r--r--   0        0        0      441 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_credential.py
+-rw-r--r--   0        0        0      496 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      455 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_storage_source.py
+-rw-r--r--   0        0        0      534 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_local_identity_provider.py
+-rw-r--r--   0        0        0      510 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_notification_rule_v2.py
+-rw-r--r--   0        0        0      540 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
+-rw-r--r--   0        0        0      596 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_validator.py
+-rw-r--r--   0        0        0      512 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_postgre_sql_credential.py
+-rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_postgre_sql_source.py
+-rw-r--r--   0        0        0      520 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_relative_time_validator.py
+-rw-r--r--   0        0        0      540 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_relative_volume_validator.py
+-rw-r--r--   0        0        0      524 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_saml_identity_provider.py
+-rw-r--r--   0        0        0      473 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_sessionized_window.py
+-rw-r--r--   0        0        0      425 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_slack_channel.py
+-rw-r--r--   0        0        0      501 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_snowflake_credential.py
+-rw-r--r--   0        0        0      513 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_snowflake_destination.py
+-rw-r--r--   0        0        0      453 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_snowflake_source.py
+-rw-r--r--   0        0        0      443 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_tumbling_window.py
+-rw-r--r--   0        0        0      324 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_user.py
+-rw-r--r--   0        0        0    57176 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0    56052 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0    58306 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      459 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_volume_validator.py
+-rw-r--r--   0        0        0      445 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_webhook_channel.py
+-rw-r--r--   0        0        0      265 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/metadata.py
+-rw-r--r--   0        0        0        0 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/py.typed
+-rw-r--r--   0        0        0      135 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/__init__.py
+-rw-r--r--   0        0        0    20662 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_diff.py
+-rw-r--r--   0        0        0     1208 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_diff_util.py
+-rw-r--r--   0        0        0     1229 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_diffable.py
+-rw-r--r--   0        0        0     1579 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_errors.py
+-rw-r--r--   0        0        0     4262 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_field_selector.py
+-rw-r--r--   0        0        0    17664 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_resource.py
+-rw-r--r--   0        0        0      914 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_resource_graph.py
+-rw-r--r--   0        0        0     5350 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_serde.py
+-rw-r--r--   0        0        0    17500 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_server_resources.py
+-rw-r--r--   0        0        0      844 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_util.py
+-rw-r--r--   0        0        0     5043 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/channels.py
+-rw-r--r--   0        0        0     7709 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/credentials.py
+-rw-r--r--   0        0        0     5398 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/destinations.py
+-rw-r--r--   0        0        0     5523 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/filters.py
+-rw-r--r--   0        0        0     4628 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/notification_rules_v2.py
+-rw-r--r--   0        0        0     2040 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/segmentations.py
+-rw-r--r--   0        0        0    23033 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/sources.py
+-rw-r--r--   0        0        0        0 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/tests/__init__.py
+-rw-r--r--   0        0        0    15565 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test__diff.py
+-rw-r--r--   0        0        0     1905 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test__field_selector.py
+-rw-r--r--   0        0        0    16378 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test__resource.py
+-rw-r--r--   0        0        0      868 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test_sources.py
+-rw-r--r--   0        0        0     5638 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/thresholds.py
+-rw-r--r--   0        0        0    32119 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/validators.py
+-rw-r--r--   0        0        0     5995 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/windows.py
+-rw-r--r--   0        0        0     1316 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/scalars.py
+-rw-r--r--   0        0        0     1813 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/util.py
+-rw-r--r--   0        0        0     2453 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/validio_client.py
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 validio_sdk-0.1.0/PKG-INFO
```

### Comparing `validio_sdk-0.0.1/LICENSE` & `validio_sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

