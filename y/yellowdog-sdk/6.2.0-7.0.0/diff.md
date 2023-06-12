# Comparing `tmp/yellowdog_sdk-6.2.0-py3-none-any.whl.zip` & `tmp/yellowdog_sdk-7.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,421 +1,416 @@
-Zip file size: 257932 bytes, number of entries: 419
--rw-r--r--  2.0 unx    13499 b- defN 23-May-23 15:10 yellowdog_client/__init__.py
--rw-r--r--  2.0 unx       35 b- defN 23-May-23 15:10 yellowdog_client/_version.py
--rw-r--r--  2.0 unx      388 b- defN 23-May-23 15:10 yellowdog_client/client_collection.py
--rw-r--r--  2.0 unx     6247 b- defN 23-May-23 15:10 yellowdog_client/platform_client.py
--rw-r--r--  2.0 unx      235 b- defN 23-May-23 15:10 yellowdog_client/account/__init__.py
--rw-r--r--  2.0 unx     1089 b- defN 23-May-23 15:10 yellowdog_client/account/keyring_client.py
--rw-r--r--  2.0 unx     1665 b- defN 23-May-23 15:10 yellowdog_client/account/keyring_client_impl.py
--rw-r--r--  2.0 unx     1220 b- defN 23-May-23 15:10 yellowdog_client/account/keyring_service_proxy.py
--rw-r--r--  2.0 unx      234 b- defN 23-May-23 15:10 yellowdog_client/cloud_info/__init__.py
--rw-r--r--  2.0 unx      843 b- defN 23-May-23 15:10 yellowdog_client/cloud_info/cloud_info_client.py
--rw-r--r--  2.0 unx     1917 b- defN 23-May-23 15:10 yellowdog_client/cloud_info/cloud_info_client_impl.py
--rw-r--r--  2.0 unx     1301 b- defN 23-May-23 15:10 yellowdog_client/cloud_info/cloud_info_proxy.py
--rw-r--r--  2.0 unx      400 b- defN 23-May-23 15:10 yellowdog_client/common/__init__.py
--rw-r--r--  2.0 unx      352 b- defN 23-May-23 15:10 yellowdog_client/common/closeable.py
--rw-r--r--  2.0 unx     1090 b- defN 23-May-23 15:10 yellowdog_client/common/countdown_event.py
--rw-r--r--  2.0 unx      640 b- defN 23-May-23 15:10 yellowdog_client/common/iso_datetime.py
--rw-r--r--  2.0 unx      540 b- defN 23-May-23 15:10 yellowdog_client/common/pagination.py
--rw-r--r--  2.0 unx     6792 b- defN 23-May-23 15:10 yellowdog_client/common/proxy.py
--rw-r--r--  2.0 unx     1420 b- defN 23-May-23 15:10 yellowdog_client/common/search_client.py
--rw-r--r--  2.0 unx     1303 b- defN 23-May-23 15:10 yellowdog_client/common/slice_iterator.py
--rw-r--r--  2.0 unx      521 b- defN 23-May-23 15:10 yellowdog_client/common/synchronized_predicated_runner.py
--rw-r--r--  2.0 unx      147 b- defN 23-May-23 15:10 yellowdog_client/common/credentials/__init__.py
--rw-r--r--  2.0 unx      843 b- defN 23-May-23 15:10 yellowdog_client/common/credentials/api_key_authentication_headers_provider.py
--rw-r--r--  2.0 unx       76 b- defN 23-May-23 15:10 yellowdog_client/common/decorators/__init__.py
--rw-r--r--  2.0 unx      257 b- defN 23-May-23 15:10 yellowdog_client/common/decorators/dispatcher.py
--rw-r--r--  2.0 unx     6039 b- defN 23-May-23 15:10 yellowdog_client/common/json/__init__.py
--rw-r--r--  2.0 unx      507 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/__init__.py
--rw-r--r--  2.0 unx     1278 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/delegated_subscription_event_listener.py
--rw-r--r--  2.0 unx     3123 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/subscription.py
--rw-r--r--  2.0 unx     1010 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/subscription_event_listener.py
--rw-r--r--  2.0 unx     2595 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/subscription_manager.py
--rw-r--r--  2.0 unx     1660 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/tracking_subscription_event_listener.py
--rw-r--r--  2.0 unx      689 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/__init__.py
--rw-r--r--  2.0 unx      369 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/chained_thread.py
--rw-r--r--  2.0 unx     2889 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/connected_state.py
--rw-r--r--  2.0 unx     2430 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/connecting_state.py
--rw-r--r--  2.0 unx     1775 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/disconnected_state.py
--rw-r--r--  2.0 unx     3947 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/event_source.py
--rw-r--r--  2.0 unx      124 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/event_source_state.py
--rw-r--r--  2.0 unx      551 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/server_response.py
--rw-r--r--  2.0 unx      282 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/server_sent_event.py
--rw-r--r--  2.0 unx      332 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/web_request_factory.py
--rw-r--r--  2.0 unx     4001 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/web_requester.py
--rw-r--r--  2.0 unx      108 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/abstracts/__init__.py
--rw-r--r--  2.0 unx      756 b- defN 23-May-23 15:10 yellowdog_client/common/server_sent_events/sse4python/abstracts/abstract_connection_state.py
--rw-r--r--  2.0 unx      485 b- defN 23-May-23 15:10 yellowdog_client/compute/__init__.py
--rw-r--r--  2.0 unx    20082 b- defN 23-May-23 15:10 yellowdog_client/compute/compute_client.py
--rw-r--r--  2.0 unx    14378 b- defN 23-May-23 15:10 yellowdog_client/compute/compute_client_impl.py
--rw-r--r--  2.0 unx     4354 b- defN 23-May-23 15:10 yellowdog_client/compute/compute_requirement_helper.py
--rw-r--r--  2.0 unx     6223 b- defN 23-May-23 15:10 yellowdog_client/compute/compute_service_proxy.py
--rw-r--r--  2.0 unx     2151 b- defN 23-May-23 15:10 yellowdog_client/compute/predicated_compute_subscription_event_listener.py
--rw-r--r--  2.0 unx      823 b- defN 23-May-23 15:10 yellowdog_client/images/__init__.py
--rw-r--r--  2.0 unx     2274 b- defN 23-May-23 15:10 yellowdog_client/images/images_client.py
--rw-r--r--  2.0 unx     3349 b- defN 23-May-23 15:10 yellowdog_client/images/images_client_impl.py
--rw-r--r--  2.0 unx     3393 b- defN 23-May-23 15:10 yellowdog_client/images/images_service_proxy.py
--rw-r--r--  2.0 unx      391 b- defN 23-May-23 15:10 yellowdog_client/images/page.py
--rw-r--r--  2.0 unx      296 b- defN 23-May-23 15:10 yellowdog_client/images/pageable.py
--rw-r--r--  2.0 unx      167 b- defN 23-May-23 15:10 yellowdog_client/images/sort.py
--rw-r--r--  2.0 unx    22549 b- defN 23-May-23 15:10 yellowdog_client/model/__init__.py
--rw-r--r--  2.0 unx      470 b- defN 23-May-23 15:10 yellowdog_client/model/access_delegate.py
--rw-r--r--  2.0 unx      472 b- defN 23-May-23 15:10 yellowdog_client/model/account.py
--rw-r--r--  2.0 unx     1021 b- defN 23-May-23 15:10 yellowdog_client/model/account_allowance.py
--rw-r--r--  2.0 unx      270 b- defN 23-May-23 15:10 yellowdog_client/model/account_authentication_properties.py
--rw-r--r--  2.0 unx      156 b- defN 23-May-23 15:10 yellowdog_client/model/add_application_request.py
--rw-r--r--  2.0 unx      253 b- defN 23-May-23 15:10 yellowdog_client/model/add_application_response.py
--rw-r--r--  2.0 unx      619 b- defN 23-May-23 15:10 yellowdog_client/model/add_configured_worker_pool_request.py
--rw-r--r--  2.0 unx      317 b- defN 23-May-23 15:10 yellowdog_client/model/add_configured_worker_pool_response.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-23 15:10 yellowdog_client/model/add_node_actions_request.py
--rw-r--r--  2.0 unx      161 b- defN 23-May-23 15:10 yellowdog_client/model/add_user_request.py
--rw-r--r--  2.0 unx      186 b- defN 23-May-23 15:10 yellowdog_client/model/add_user_response.py
--rw-r--r--  2.0 unx      490 b- defN 23-May-23 15:10 yellowdog_client/model/alibaba_compute_source.py
--rw-r--r--  2.0 unx      553 b- defN 23-May-23 15:10 yellowdog_client/model/alibaba_credential.py
--rw-r--r--  2.0 unx     1773 b- defN 23-May-23 15:10 yellowdog_client/model/alibaba_instance.py
--rw-r--r--  2.0 unx      342 b- defN 23-May-23 15:10 yellowdog_client/model/alibaba_instance_charge_type.py
--rw-r--r--  2.0 unx     3377 b- defN 23-May-23 15:10 yellowdog_client/model/alibaba_instances_compute_source.py
--rw-r--r--  2.0 unx      392 b- defN 23-May-23 15:10 yellowdog_client/model/alibaba_namespace_storage_configuration.py
--rw-r--r--  2.0 unx      426 b- defN 23-May-23 15:10 yellowdog_client/model/alibaba_spot_strategy.py
--rw-r--r--  2.0 unx      554 b- defN 23-May-23 15:10 yellowdog_client/model/all_nodes_inactive_shutdown_condition.py
--rw-r--r--  2.0 unx      562 b- defN 23-May-23 15:10 yellowdog_client/model/all_workers_released_shutdown_condition.py
--rw-r--r--  2.0 unx      167 b- defN 23-May-23 15:10 yellowdog_client/model/allowance.py
--rw-r--r--  2.0 unx      255 b- defN 23-May-23 15:10 yellowdog_client/model/allowance_exhausted_notification.py
--rw-r--r--  2.0 unx      436 b- defN 23-May-23 15:10 yellowdog_client/model/allowance_limit_enforcement.py
--rw-r--r--  2.0 unx      425 b- defN 23-May-23 15:10 yellowdog_client/model/allowance_reset_type.py
--rw-r--r--  2.0 unx      624 b- defN 23-May-23 15:10 yellowdog_client/model/allowance_search.py
--rw-r--r--  2.0 unx      151 b- defN 23-May-23 15:10 yellowdog_client/model/api_key.py
--rw-r--r--  2.0 unx      494 b- defN 23-May-23 15:10 yellowdog_client/model/application.py
--rw-r--r--  2.0 unx      129 b- defN 23-May-23 15:10 yellowdog_client/model/attribute_constraint.py
--rw-r--r--  2.0 unx      162 b- defN 23-May-23 15:10 yellowdog_client/model/attribute_definition.py
--rw-r--r--  2.0 unx      129 b- defN 23-May-23 15:10 yellowdog_client/model/attribute_preference.py
--rw-r--r--  2.0 unx       79 b- defN 23-May-23 15:10 yellowdog_client/model/attribute_source.py
--rw-r--r--  2.0 unx      357 b- defN 23-May-23 15:10 yellowdog_client/model/attribute_source_type.py
--rw-r--r--  2.0 unx      205 b- defN 23-May-23 15:10 yellowdog_client/model/attribute_value.py
--rw-r--r--  2.0 unx      164 b- defN 23-May-23 15:10 yellowdog_client/model/authentication_provider.py
--rw-r--r--  2.0 unx      472 b- defN 23-May-23 15:10 yellowdog_client/model/aws_compute_source.py
--rw-r--r--  2.0 unx      537 b- defN 23-May-23 15:10 yellowdog_client/model/aws_credential.py
--rw-r--r--  2.0 unx     3851 b- defN 23-May-23 15:10 yellowdog_client/model/aws_fleet_compute_source.py
--rw-r--r--  2.0 unx      537 b- defN 23-May-23 15:10 yellowdog_client/model/aws_fleet_instance_override.py
--rw-r--r--  2.0 unx      628 b- defN 23-May-23 15:10 yellowdog_client/model/aws_fleet_on_demand_allocation_strategy.py
--rw-r--r--  2.0 unx     1092 b- defN 23-May-23 15:10 yellowdog_client/model/aws_fleet_on_demand_options.py
--rw-r--r--  2.0 unx      584 b- defN 23-May-23 15:10 yellowdog_client/model/aws_fleet_purchase_option.py
--rw-r--r--  2.0 unx      875 b- defN 23-May-23 15:10 yellowdog_client/model/aws_fleet_spot_allocation_strategy.py
--rw-r--r--  2.0 unx     1292 b- defN 23-May-23 15:10 yellowdog_client/model/aws_fleet_spot_options.py
--rw-r--r--  2.0 unx     1865 b- defN 23-May-23 15:10 yellowdog_client/model/aws_instance.py
--rw-r--r--  2.0 unx     3390 b- defN 23-May-23 15:10 yellowdog_client/model/aws_instances_compute_source.py
--rw-r--r--  2.0 unx      331 b- defN 23-May-23 15:10 yellowdog_client/model/azure_account_authentication_properties.py
--rw-r--r--  2.0 unx      634 b- defN 23-May-23 15:10 yellowdog_client/model/azure_client_credential.py
--rw-r--r--  2.0 unx      242 b- defN 23-May-23 15:10 yellowdog_client/model/azure_compute_credential.py
--rw-r--r--  2.0 unx      478 b- defN 23-May-23 15:10 yellowdog_client/model/azure_compute_source.py
--rw-r--r--  2.0 unx     1760 b- defN 23-May-23 15:10 yellowdog_client/model/azure_instance.py
--rw-r--r--  2.0 unx      584 b- defN 23-May-23 15:10 yellowdog_client/model/azure_instance_credential.py
--rw-r--r--  2.0 unx     2550 b- defN 23-May-23 15:10 yellowdog_client/model/azure_instances_compute_source.py
--rw-r--r--  2.0 unx      373 b- defN 23-May-23 15:10 yellowdog_client/model/azure_namespace_storage_configuration.py
--rw-r--r--  2.0 unx     2428 b- defN 23-May-23 15:10 yellowdog_client/model/azure_scale_set_compute_source.py
--rw-r--r--  2.0 unx      444 b- defN 23-May-23 15:10 yellowdog_client/model/azure_storage_credential.py
--rw-r--r--  2.0 unx     1313 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report.py
--rw-r--r--  2.0 unx      143 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_constraint.py
--rw-r--r--  2.0 unx      446 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_image.py
--rw-r--r--  2.0 unx      311 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_image_availability.py
--rw-r--r--  2.0 unx      429 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_numeric_constraint.py
--rw-r--r--  2.0 unx      233 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_preference.py
--rw-r--r--  2.0 unx      782 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_source.py
--rw-r--r--  2.0 unx      231 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_source_attribute.py
--rw-r--r--  2.0 unx      477 b- defN 23-May-23 15:10 yellowdog_client/model/best_compute_source_report_string_constraint.py
--rw-r--r--  2.0 unx      118 b- defN 23-May-23 15:10 yellowdog_client/model/change_password_request.py
--rw-r--r--  2.0 unx      748 b- defN 23-May-23 15:10 yellowdog_client/model/cloud_provider.py
--rw-r--r--  2.0 unx      256 b- defN 23-May-23 15:10 yellowdog_client/model/compute_namespace_filter.py
--rw-r--r--  2.0 unx      388 b- defN 23-May-23 15:10 yellowdog_client/model/compute_provision_strategy.py
--rw-r--r--  2.0 unx     2937 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_dynamic_template.py
--rw-r--r--  2.0 unx      623 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_dynamic_template_test_result.py
--rw-r--r--  2.0 unx      435 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_search.py
--rw-r--r--  2.0 unx      715 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_static_template.py
--rw-r--r--  2.0 unx      504 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_static_template_test_result.py
--rw-r--r--  2.0 unx     2115 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_status.py
--rw-r--r--  2.0 unx      293 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_supported_operations.py
--rw-r--r--  2.0 unx      216 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_template.py
--rw-r--r--  2.0 unx      320 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_template_summary.py
--rw-r--r--  2.0 unx      146 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_template_test_result.py
--rw-r--r--  2.0 unx      446 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_template_usage.py
--rw-r--r--  2.0 unx      407 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_usage.py
--rw-r--r--  2.0 unx      312 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirement_usage_filter.py
--rw-r--r--  2.0 unx      277 b- defN 23-May-23 15:10 yellowdog_client/model/compute_requirements_summary.py
--rw-r--r--  2.0 unx      403 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source.py
--rw-r--r--  2.0 unx      625 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_exhaustion.py
--rw-r--r--  2.0 unx      245 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_exhaustion_status.py
--rw-r--r--  2.0 unx     1058 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_status.py
--rw-r--r--  2.0 unx      471 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_template.py
--rw-r--r--  2.0 unx      370 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_template_summary.py
--rw-r--r--  2.0 unx      268 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_traits.py
--rw-r--r--  2.0 unx      269 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_traits_filter.py
--rw-r--r--  2.0 unx      200 b- defN 23-May-23 15:10 yellowdog_client/model/compute_source_usage.py
--rw-r--r--  2.0 unx      911 b- defN 23-May-23 15:10 yellowdog_client/model/configured_worker_pool.py
--rw-r--r--  2.0 unx      598 b- defN 23-May-23 15:10 yellowdog_client/model/configured_worker_pool_properties.py
--rw-r--r--  2.0 unx       73 b- defN 23-May-23 15:10 yellowdog_client/model/constants.py
--rw-r--r--  2.0 unx      195 b- defN 23-May-23 15:10 yellowdog_client/model/create_keyring_request.py
--rw-r--r--  2.0 unx      214 b- defN 23-May-23 15:10 yellowdog_client/model/create_keyring_response.py
--rw-r--r--  2.0 unx      237 b- defN 23-May-23 15:10 yellowdog_client/model/credential.py
--rw-r--r--  2.0 unx     2090 b- defN 23-May-23 15:10 yellowdog_client/model/currency.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-23 15:10 yellowdog_client/model/double_range.py
--rw-r--r--  2.0 unx      194 b- defN 23-May-23 15:10 yellowdog_client/model/error_response.py
--rw-r--r--  2.0 unx       96 b- defN 23-May-23 15:10 yellowdog_client/model/existing_password_request.py
--rw-r--r--  2.0 unx      219 b- defN 23-May-23 15:10 yellowdog_client/model/external_attribute_definition.py
--rw-r--r--  2.0 unx      327 b- defN 23-May-23 15:10 yellowdog_client/model/external_attribute_provider_query.py
--rw-r--r--  2.0 unx      246 b- defN 23-May-23 15:10 yellowdog_client/model/external_attribute_provider_query_source.py
--rw-r--r--  2.0 unx      338 b- defN 23-May-23 15:10 yellowdog_client/model/external_attribute_provider_registration.py
--rw-r--r--  2.0 unx      361 b- defN 23-May-23 15:10 yellowdog_client/model/external_attribute_provider_results.py
--rw-r--r--  2.0 unx      192 b- defN 23-May-23 15:10 yellowdog_client/model/external_attribute_provider_results_source.py
--rw-r--r--  2.0 unx      488 b- defN 23-May-23 15:10 yellowdog_client/model/external_attribute_source.py
--rw-r--r--  2.0 unx      847 b- defN 23-May-23 15:10 yellowdog_client/model/external_user.py
--rw-r--r--  2.0 unx       70 b- defN 23-May-23 15:10 yellowdog_client/model/filter.py
--rw-r--r--  2.0 unx      494 b- defN 23-May-23 15:10 yellowdog_client/model/flatten_path.py
--rw-r--r--  2.0 unx      496 b- defN 23-May-23 15:10 yellowdog_client/model/gce_compute_source.py
--rw-r--r--  2.0 unx     1839 b- defN 23-May-23 15:10 yellowdog_client/model/gce_instance.py
--rw-r--r--  2.0 unx     1959 b- defN 23-May-23 15:10 yellowdog_client/model/gce_instance_group_compute_source.py
--rw-r--r--  2.0 unx     2520 b- defN 23-May-23 15:10 yellowdog_client/model/gce_instances_compute_source.py
--rw-r--r--  2.0 unx      366 b- defN 23-May-23 15:10 yellowdog_client/model/gcs_namespace_storage_configuration.py
--rw-r--r--  2.0 unx      408 b- defN 23-May-23 15:10 yellowdog_client/model/google_cloud_credential.py
--rw-r--r--  2.0 unx      228 b- defN 23-May-23 15:10 yellowdog_client/model/grant_application_access_request.py
--rw-r--r--  2.0 unx      177 b- defN 23-May-23 15:10 yellowdog_client/model/grant_user_access_request.py
--rw-r--r--  2.0 unx      182 b- defN 23-May-23 15:10 yellowdog_client/model/identified.py
--rw-r--r--  2.0 unx      151 b- defN 23-May-23 15:10 yellowdog_client/model/image_access.py
--rw-r--r--  2.0 unx      149 b- defN 23-May-23 15:10 yellowdog_client/model/image_os_type.py
--rw-r--r--  2.0 unx      382 b- defN 23-May-23 15:10 yellowdog_client/model/instance.py
--rw-r--r--  2.0 unx      292 b- defN 23-May-23 15:10 yellowdog_client/model/instance_id.py
--rw-r--r--  2.0 unx      712 b- defN 23-May-23 15:10 yellowdog_client/model/instance_search.py
--rw-r--r--  2.0 unx     1154 b- defN 23-May-23 15:10 yellowdog_client/model/instance_status.py
--rw-r--r--  2.0 unx     1081 b- defN 23-May-23 15:10 yellowdog_client/model/instance_summary.py
--rw-r--r--  2.0 unx      528 b- defN 23-May-23 15:10 yellowdog_client/model/instance_type.py
--rw-r--r--  2.0 unx      560 b- defN 23-May-23 15:10 yellowdog_client/model/instance_type_price.py
--rw-r--r--  2.0 unx      662 b- defN 23-May-23 15:10 yellowdog_client/model/instance_type_price_search.py
--rw-r--r--  2.0 unx      181 b- defN 23-May-23 15:10 yellowdog_client/model/instance_type_region.py
--rw-r--r--  2.0 unx      689 b- defN 23-May-23 15:10 yellowdog_client/model/instance_type_search.py
--rw-r--r--  2.0 unx      471 b- defN 23-May-23 15:10 yellowdog_client/model/instance_usage.py
--rw-r--r--  2.0 unx      347 b- defN 23-May-23 15:10 yellowdog_client/model/instance_usage_filter.py
--rw-r--r--  2.0 unx      228 b- defN 23-May-23 15:10 yellowdog_client/model/instant_range.py
--rw-r--r--  2.0 unx      188 b- defN 23-May-23 15:10 yellowdog_client/model/integer_range.py
--rw-r--r--  2.0 unx      397 b- defN 23-May-23 15:10 yellowdog_client/model/internal_attribute_source.py
--rw-r--r--  2.0 unx      666 b- defN 23-May-23 15:10 yellowdog_client/model/internal_user.py
--rw-r--r--  2.0 unx      435 b- defN 23-May-23 15:10 yellowdog_client/model/keyring.py
--rw-r--r--  2.0 unx      186 b- defN 23-May-23 15:10 yellowdog_client/model/keyring_access_secrets.py
--rw-r--r--  2.0 unx      213 b- defN 23-May-23 15:10 yellowdog_client/model/keyring_accessor.py
--rw-r--r--  2.0 unx      233 b- defN 23-May-23 15:10 yellowdog_client/model/keyring_credential.py
--rw-r--r--  2.0 unx      243 b- defN 23-May-23 15:10 yellowdog_client/model/keyring_summary.py
--rw-r--r--  2.0 unx      185 b- defN 23-May-23 15:10 yellowdog_client/model/long_range.py
--rw-r--r--  2.0 unx     1535 b- defN 23-May-23 15:10 yellowdog_client/model/machine_image.py
--rw-r--r--  2.0 unx     1456 b- defN 23-May-23 15:10 yellowdog_client/model/machine_image_family.py
--rw-r--r--  2.0 unx      952 b- defN 23-May-23 15:10 yellowdog_client/model/machine_image_family_search.py
--rw-r--r--  2.0 unx     1188 b- defN 23-May-23 15:10 yellowdog_client/model/machine_image_family_summary.py
--rw-r--r--  2.0 unx     1182 b- defN 23-May-23 15:10 yellowdog_client/model/machine_image_group.py
--rw-r--r--  2.0 unx      142 b- defN 23-May-23 15:10 yellowdog_client/model/metadata_filter.py
--rw-r--r--  2.0 unx       78 b- defN 23-May-23 15:10 yellowdog_client/model/model_exception.py
--rw-r--r--  2.0 unx      143 b- defN 23-May-23 15:10 yellowdog_client/model/named.py
--rw-r--r--  2.0 unx      189 b- defN 23-May-23 15:10 yellowdog_client/model/namespace_objects_response.py
--rw-r--r--  2.0 unx      139 b- defN 23-May-23 15:10 yellowdog_client/model/namespace_storage_configuration.py
--rw-r--r--  2.0 unx       91 b- defN 23-May-23 15:10 yellowdog_client/model/new_password_request.py
--rw-r--r--  2.0 unx      446 b- defN 23-May-23 15:10 yellowdog_client/model/no_registered_workers_shutdown_condition.py
--rw-r--r--  2.0 unx     1099 b- defN 23-May-23 15:10 yellowdog_client/model/node.py
--rw-r--r--  2.0 unx      122 b- defN 23-May-23 15:10 yellowdog_client/model/node_action.py
--rw-r--r--  2.0 unx      566 b- defN 23-May-23 15:10 yellowdog_client/model/node_action_failed_shutdown_condition.py
--rw-r--r--  2.0 unx      161 b- defN 23-May-23 15:10 yellowdog_client/model/node_action_group.py
--rw-r--r--  2.0 unx      467 b- defN 23-May-23 15:10 yellowdog_client/model/node_action_queue_snapshot.py
--rw-r--r--  2.0 unx      534 b- defN 23-May-23 15:10 yellowdog_client/model/node_action_queue_status.py
--rw-r--r--  2.0 unx      500 b- defN 23-May-23 15:10 yellowdog_client/model/node_create_workers_action.py
--rw-r--r--  2.0 unx     1707 b- defN 23-May-23 15:10 yellowdog_client/model/node_details.py
--rw-r--r--  2.0 unx      591 b- defN 23-May-23 15:10 yellowdog_client/model/node_event.py
--rw-r--r--  2.0 unx      144 b- defN 23-May-23 15:10 yellowdog_client/model/node_id_filter.py
--rw-r--r--  2.0 unx      466 b- defN 23-May-23 15:10 yellowdog_client/model/node_run_command_action.py
--rw-r--r--  2.0 unx     1025 b- defN 23-May-23 15:10 yellowdog_client/model/node_search.py
--rw-r--r--  2.0 unx      137 b- defN 23-May-23 15:10 yellowdog_client/model/node_slot_numbering.py
--rw-r--r--  2.0 unx      832 b- defN 23-May-23 15:10 yellowdog_client/model/node_status.py
--rw-r--r--  2.0 unx      604 b- defN 23-May-23 15:10 yellowdog_client/model/node_summary.py
--rw-r--r--  2.0 unx      323 b- defN 23-May-23 15:10 yellowdog_client/model/node_type.py
--rw-r--r--  2.0 unx      513 b- defN 23-May-23 15:10 yellowdog_client/model/node_worker_target.py
--rw-r--r--  2.0 unx      166 b- defN 23-May-23 15:10 yellowdog_client/model/node_worker_target_type.py
--rw-r--r--  2.0 unx      401 b- defN 23-May-23 15:10 yellowdog_client/model/node_write_file_action.py
--rw-r--r--  2.0 unx      375 b- defN 23-May-23 15:10 yellowdog_client/model/numeric_attribute_constraint.py
--rw-r--r--  2.0 unx      664 b- defN 23-May-23 15:10 yellowdog_client/model/numeric_attribute_definition.py
--rw-r--r--  2.0 unx      459 b- defN 23-May-23 15:10 yellowdog_client/model/numeric_attribute_preference.py
--rw-r--r--  2.0 unx      168 b- defN 23-May-23 15:10 yellowdog_client/model/numeric_attribute_range.py
--rw-r--r--  2.0 unx      189 b- defN 23-May-23 15:10 yellowdog_client/model/numeric_attribute_rank_order.py
--rw-r--r--  2.0 unx      275 b- defN 23-May-23 15:10 yellowdog_client/model/numeric_attribute_value.py
--rw-r--r--  2.0 unx       94 b- defN 23-May-23 15:10 yellowdog_client/model/o_auth2_authentication_properties.py
--rw-r--r--  2.0 unx      586 b- defN 23-May-23 15:10 yellowdog_client/model/object_detail.py
--rw-r--r--  2.0 unx      115 b- defN 23-May-23 15:10 yellowdog_client/model/object_download_request.py
--rw-r--r--  2.0 unx      324 b- defN 23-May-23 15:10 yellowdog_client/model/object_download_response.py
--rw-r--r--  2.0 unx      170 b- defN 23-May-23 15:10 yellowdog_client/model/object_path.py
--rw-r--r--  2.0 unx      193 b- defN 23-May-23 15:10 yellowdog_client/model/object_paths_request.py
--rw-r--r--  2.0 unx      335 b- defN 23-May-23 15:10 yellowdog_client/model/object_paths_slice_request.py
--rw-r--r--  2.0 unx      153 b- defN 23-May-23 15:10 yellowdog_client/model/object_upload_request.py
--rw-r--r--  2.0 unx      472 b- defN 23-May-23 15:10 yellowdog_client/model/oci_compute_source.py
--rw-r--r--  2.0 unx      702 b- defN 23-May-23 15:10 yellowdog_client/model/oci_credential.py
--rw-r--r--  2.0 unx     2077 b- defN 23-May-23 15:10 yellowdog_client/model/oci_instance.py
--rw-r--r--  2.0 unx     2284 b- defN 23-May-23 15:10 yellowdog_client/model/oci_instance_pool_compute_source.py
--rw-r--r--  2.0 unx     2241 b- defN 23-May-23 15:10 yellowdog_client/model/oci_instances_compute_source.py
--rw-r--r--  2.0 unx      408 b- defN 23-May-23 15:10 yellowdog_client/model/oci_namespace_storage_configuration.py
--rw-r--r--  2.0 unx      347 b- defN 23-May-23 15:10 yellowdog_client/model/operating_system_licence.py
--rw-r--r--  2.0 unx      163 b- defN 23-May-23 15:10 yellowdog_client/model/password_state.py
--rw-r--r--  2.0 unx      194 b- defN 23-May-23 15:10 yellowdog_client/model/price.py
--rw-r--r--  2.0 unx      157 b- defN 23-May-23 15:10 yellowdog_client/model/processor_architecture.py
--rw-r--r--  2.0 unx      416 b- defN 23-May-23 15:10 yellowdog_client/model/provision_template_worker_pool_request.py
--rw-r--r--  2.0 unx     1047 b- defN 23-May-23 15:10 yellowdog_client/model/provisioned_worker_pool.py
--rw-r--r--  2.0 unx     1908 b- defN 23-May-23 15:10 yellowdog_client/model/provisioned_worker_pool_properties.py
--rw-r--r--  2.0 unx      135 b- defN 23-May-23 15:10 yellowdog_client/model/range.py
--rw-r--r--  2.0 unx      208 b- defN 23-May-23 15:10 yellowdog_client/model/region.py
--rw-r--r--  2.0 unx      355 b- defN 23-May-23 15:10 yellowdog_client/model/region_search.py
--rw-r--r--  2.0 unx     1052 b- defN 23-May-23 15:10 yellowdog_client/model/requirement_allowance.py
--rw-r--r--  2.0 unx     1197 b- defN 23-May-23 15:10 yellowdog_client/model/requirements_allowance.py
--rw-r--r--  2.0 unx      559 b- defN 23-May-23 15:10 yellowdog_client/model/retry_properties.py
--rw-r--r--  2.0 unx     2046 b- defN 23-May-23 15:10 yellowdog_client/model/run_specification.py
--rw-r--r--  2.0 unx      380 b- defN 23-May-23 15:10 yellowdog_client/model/s3_namespace_storage_configuration.py
--rw-r--r--  2.0 unx     1894 b- defN 23-May-23 15:10 yellowdog_client/model/services_schema.py
--rw-r--r--  2.0 unx      145 b- defN 23-May-23 15:10 yellowdog_client/model/set_password_request.py
--rw-r--r--  2.0 unx     2473 b- defN 23-May-23 15:10 yellowdog_client/model/simulator_compute_source.py
--rw-r--r--  2.0 unx     1882 b- defN 23-May-23 15:10 yellowdog_client/model/simulator_instance.py
--rw-r--r--  2.0 unx      634 b- defN 23-May-23 15:10 yellowdog_client/model/single_source_provision_strategy.py
--rw-r--r--  2.0 unx      216 b- defN 23-May-23 15:10 yellowdog_client/model/slice.py
--rw-r--r--  2.0 unx      162 b- defN 23-May-23 15:10 yellowdog_client/model/slice_reference.py
--rw-r--r--  2.0 unx      165 b- defN 23-May-23 15:10 yellowdog_client/model/sort_direction.py
--rw-r--r--  2.0 unx     1037 b- defN 23-May-23 15:10 yellowdog_client/model/source_allowance.py
--rw-r--r--  2.0 unx     1281 b- defN 23-May-23 15:10 yellowdog_client/model/sources_allowance.py
--rw-r--r--  2.0 unx      646 b- defN 23-May-23 15:10 yellowdog_client/model/split_provision_strategy.py
--rw-r--r--  2.0 unx      423 b- defN 23-May-23 15:10 yellowdog_client/model/string_attribute_constraint.py
--rw-r--r--  2.0 unx      403 b- defN 23-May-23 15:10 yellowdog_client/model/string_attribute_definition.py
--rw-r--r--  2.0 unx      435 b- defN 23-May-23 15:10 yellowdog_client/model/string_attribute_preference.py
--rw-r--r--  2.0 unx      316 b- defN 23-May-23 15:10 yellowdog_client/model/string_attribute_value.py
--rw-r--r--  2.0 unx      244 b- defN 23-May-23 15:10 yellowdog_client/model/sub_region.py
--rw-r--r--  2.0 unx      391 b- defN 23-May-23 15:10 yellowdog_client/model/sub_region_search.py
--rw-r--r--  2.0 unx      172 b- defN 23-May-23 15:10 yellowdog_client/model/tagged.py
--rw-r--r--  2.0 unx     2698 b- defN 23-May-23 15:10 yellowdog_client/model/task.py
--rw-r--r--  2.0 unx      453 b- defN 23-May-23 15:10 yellowdog_client/model/task_error.py
--rw-r--r--  2.0 unx     1851 b- defN 23-May-23 15:10 yellowdog_client/model/task_group.py
--rw-r--r--  2.0 unx     3100 b- defN 23-May-23 15:10 yellowdog_client/model/task_group_status.py
--rw-r--r--  2.0 unx     1975 b- defN 23-May-23 15:10 yellowdog_client/model/task_input.py
--rw-r--r--  2.0 unx      423 b- defN 23-May-23 15:10 yellowdog_client/model/task_input_source.py
--rw-r--r--  2.0 unx      477 b- defN 23-May-23 15:10 yellowdog_client/model/task_input_verification.py
--rw-r--r--  2.0 unx      444 b- defN 23-May-23 15:10 yellowdog_client/model/task_input_verification_status.py
--rw-r--r--  2.0 unx     2006 b- defN 23-May-23 15:10 yellowdog_client/model/task_output.py
--rw-r--r--  2.0 unx      547 b- defN 23-May-23 15:10 yellowdog_client/model/task_output_source.py
--rw-r--r--  2.0 unx      702 b- defN 23-May-23 15:10 yellowdog_client/model/task_search.py
--rw-r--r--  2.0 unx     1554 b- defN 23-May-23 15:10 yellowdog_client/model/task_status.py
--rw-r--r--  2.0 unx      294 b- defN 23-May-23 15:10 yellowdog_client/model/task_summary.py
--rw-r--r--  2.0 unx      341 b- defN 23-May-23 15:10 yellowdog_client/model/transfer_status_response.py
--rw-r--r--  2.0 unx      409 b- defN 23-May-23 15:10 yellowdog_client/model/transfer_summary_response.py
--rw-r--r--  2.0 unx      598 b- defN 23-May-23 15:10 yellowdog_client/model/unclaimed_after_startup_shutdown_condition.py
--rw-r--r--  2.0 unx      176 b- defN 23-May-23 15:10 yellowdog_client/model/update_application_request.py
--rw-r--r--  2.0 unx      141 b- defN 23-May-23 15:10 yellowdog_client/model/update_keyring_request.py
--rw-r--r--  2.0 unx      203 b- defN 23-May-23 15:10 yellowdog_client/model/update_user_request.py
--rw-r--r--  2.0 unx      340 b- defN 23-May-23 15:10 yellowdog_client/model/usage_type.py
--rw-r--r--  2.0 unx      253 b- defN 23-May-23 15:10 yellowdog_client/model/user.py
--rw-r--r--  2.0 unx      128 b- defN 23-May-23 15:10 yellowdog_client/model/user_login_request.py
--rw-r--r--  2.0 unx      727 b- defN 23-May-23 15:10 yellowdog_client/model/waterfall_provision_strategy.py
--rw-r--r--  2.0 unx     1869 b- defN 23-May-23 15:10 yellowdog_client/model/work_requirement.py
--rw-r--r--  2.0 unx     1913 b- defN 23-May-23 15:10 yellowdog_client/model/work_requirement_status.py
--rw-r--r--  2.0 unx     1374 b- defN 23-May-23 15:10 yellowdog_client/model/work_requirement_summary.py
--rw-r--r--  2.0 unx      964 b- defN 23-May-23 15:10 yellowdog_client/model/worker.py
--rw-r--r--  2.0 unx      453 b- defN 23-May-23 15:10 yellowdog_client/model/worker_action.py
--rw-r--r--  2.0 unx      255 b- defN 23-May-23 15:10 yellowdog_client/model/worker_pool.py
--rw-r--r--  2.0 unx      355 b- defN 23-May-23 15:10 yellowdog_client/model/worker_pool_node_configuration.py
--rw-r--r--  2.0 unx       84 b- defN 23-May-23 15:10 yellowdog_client/model/worker_pool_properties.py
--rw-r--r--  2.0 unx      227 b- defN 23-May-23 15:10 yellowdog_client/model/worker_pool_shutdown_condition.py
--rw-r--r--  2.0 unx     1240 b- defN 23-May-23 15:10 yellowdog_client/model/worker_pool_status.py
--rw-r--r--  2.0 unx     1347 b- defN 23-May-23 15:10 yellowdog_client/model/worker_pool_summary.py
--rw-r--r--  2.0 unx      350 b- defN 23-May-23 15:10 yellowdog_client/model/worker_pool_token.py
--rw-r--r--  2.0 unx     1055 b- defN 23-May-23 15:10 yellowdog_client/model/worker_status.py
--rw-r--r--  2.0 unx      819 b- defN 23-May-23 15:10 yellowdog_client/model/worker_summary.py
--rw-r--r--  2.0 unx     1434 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/__init__.py
--rw-r--r--  2.0 unx      665 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/base_custom_exception.py
--rw-r--r--  2.0 unx      282 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/chunk_transfer_exception.py
--rw-r--r--  2.0 unx     1655 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/error_type.py
--rw-r--r--  2.0 unx      276 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/file_transfer_failure.py
--rw-r--r--  2.0 unx      296 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/insufficient_capacity_exception.py
--rw-r--r--  2.0 unx      284 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/internal_server_exception.py
--rw-r--r--  2.0 unx       53 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/invalid_operation_exception.py
--rw-r--r--  2.0 unx      284 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/invalid_request_exception.py
--rw-r--r--  2.0 unx      284 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/invalid_session_exception.py
--rw-r--r--  2.0 unx      282 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/not_authorised_exception.py
--rw-r--r--  2.0 unx      250 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/object_not_found_exception.py
--rw-r--r--  2.0 unx      692 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/server_error_exception.py
--rw-r--r--  2.0 unx      776 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/service_client_exception.py
--rw-r--r--  2.0 unx      280 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/session_close_exception.py
--rw-r--r--  2.0 unx      286 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/session_not_found_exception.py
--rw-r--r--  2.0 unx      261 b- defN 23-May-23 15:10 yellowdog_client/model/exceptions/unknown_exception.py
--rw-r--r--  2.0 unx      272 b- defN 23-May-23 15:10 yellowdog_client/object_store/__init__.py
--rw-r--r--  2.0 unx    16479 b- defN 23-May-23 15:10 yellowdog_client/object_store/object_store_client.py
--rw-r--r--  2.0 unx     6028 b- defN 23-May-23 15:10 yellowdog_client/object_store/object_store_service_proxy.py
--rw-r--r--  2.0 unx     1771 b- defN 23-May-23 15:10 yellowdog_client/object_store/service_session_facade.py
--rw-r--r--  2.0 unx      905 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/__init__.py
--rw-r--r--  2.0 unx      229 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_chunk_download_task.py
--rw-r--r--  2.0 unx      596 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_chunk_transfer_task.py
--rw-r--r--  2.0 unx      223 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_chunk_upload_task.py
--rw-r--r--  2.0 unx      314 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_notification_dispatcher.py
--rw-r--r--  2.0 unx     3716 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_object_store_service_proxy.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_self_binding_status_predicate.py
--rw-r--r--  2.0 unx     2006 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_service_session_facade.py
--rw-r--r--  2.0 unx    22303 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_session.py
--rw-r--r--  2.0 unx     9494 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_transfer_batch.py
--rw-r--r--  2.0 unx     6443 b- defN 23-May-23 15:10 yellowdog_client/object_store/abstracts/abstract_transfer_engine.py
--rw-r--r--  2.0 unx      374 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/__init__.py
--rw-r--r--  2.0 unx      141 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/chunk_download_task.py
--rw-r--r--  2.0 unx      708 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/download_batch.py
--rw-r--r--  2.0 unx     6720 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/download_batch_builder.py
--rw-r--r--  2.0 unx     4859 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/download_engine.py
--rw-r--r--  2.0 unx     3075 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/download_session.py
--rw-r--r--  2.0 unx      216 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/abstracts/__init__.py
--rw-r--r--  2.0 unx     1365 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/abstracts/abstract_download_batch_builder.py
--rw-r--r--  2.0 unx      827 b- defN 23-May-23 15:10 yellowdog_client/object_store/download/abstracts/abstract_download_engine.py
--rw-r--r--  2.0 unx      991 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/__init__.py
--rw-r--r--  2.0 unx      594 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/batch_transfer_event_args.py
--rw-r--r--  2.0 unx     1113 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/client_error_event_args.py
--rw-r--r--  2.0 unx      232 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/file_transfer_direction.py
--rw-r--r--  2.0 unx     1695 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/file_transfer_error_event_args.py
--rw-r--r--  2.0 unx     1084 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/file_transfer_event_args.py
--rw-r--r--  2.0 unx      802 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/file_transfer_exception.py
--rw-r--r--  2.0 unx     3033 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/file_transfer_progress_event_args.py
--rw-r--r--  2.0 unx     1378 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/file_transfer_status.py
--rw-r--r--  2.0 unx      130 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/transfer_properties.py
--rw-r--r--  2.0 unx     3596 b- defN 23-May-23 15:10 yellowdog_client/object_store/model/transfer_statistics.py
--rw-r--r--  2.0 unx      352 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/__init__.py
--rw-r--r--  2.0 unx      135 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/chunk_upload_task.py
--rw-r--r--  2.0 unx      700 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/upload_batch.py
--rw-r--r--  2.0 unx     5359 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/upload_batch_builder.py
--rw-r--r--  2.0 unx     4906 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/upload_engine.py
--rw-r--r--  2.0 unx     2117 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/upload_session.py
--rw-r--r--  2.0 unx      204 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/abstracts/__init__.py
--rw-r--r--  2.0 unx      850 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/abstracts/abstract_upload_batch_builder.py
--rw-r--r--  2.0 unx      745 b- defN 23-May-23 15:10 yellowdog_client/object_store/upload/abstracts/abstract_upload_engine.py
--rw-r--r--  2.0 unx      956 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/__init__.py
--rw-r--r--  2.0 unx      897 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/action_utils.py
--rw-r--r--  2.0 unx      503 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/background_thread.py
--rw-r--r--  2.0 unx      258 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/background_thread_factory.py
--rw-r--r--  2.0 unx     2594 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/chunk_transfer_throttle.py
--rw-r--r--  2.0 unx     1305 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/external_notification_dispatcher.py
--rw-r--r--  2.0 unx     1186 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/file_utils.py
--rw-r--r--  2.0 unx     1619 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/hash_utils.py
--rw-r--r--  2.0 unx     1253 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/internal_notification_dispatcher.py
--rw-r--r--  2.0 unx      664 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/memory_mapped_file_reader.py
--rw-r--r--  2.0 unx      265 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/memory_mapped_file_reader_factory.py
--rw-r--r--  2.0 unx      303 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/memory_mapped_file_writer_factory.py
--rw-r--r--  2.0 unx     1373 b- defN 23-May-23 15:10 yellowdog_client/object_store/utils/memory_mapped_file_writter.py
--rw-r--r--  2.0 unx      927 b- defN 23-May-23 15:10 yellowdog_client/scheduler/__init__.py
--rw-r--r--  2.0 unx     2105 b- defN 23-May-23 15:10 yellowdog_client/scheduler/predicated_work_subscription_event_listener.py
--rw-r--r--  2.0 unx     2006 b- defN 23-May-23 15:10 yellowdog_client/scheduler/predicated_worker_pool_subscription_event_listener.py
--rw-r--r--  2.0 unx    12226 b- defN 23-May-23 15:10 yellowdog_client/scheduler/work_client.py
--rw-r--r--  2.0 unx     6652 b- defN 23-May-23 15:10 yellowdog_client/scheduler/work_client_impl.py
--rw-r--r--  2.0 unx     4252 b- defN 23-May-23 15:10 yellowdog_client/scheduler/work_requirement_helper.py
--rw-r--r--  2.0 unx     2694 b- defN 23-May-23 15:10 yellowdog_client/scheduler/work_service_proxy.py
--rw-r--r--  2.0 unx    14454 b- defN 23-May-23 15:10 yellowdog_client/scheduler/worker_pool_client.py
--rw-r--r--  2.0 unx     8213 b- defN 23-May-23 15:10 yellowdog_client/scheduler/worker_pool_client_impl.py
--rw-r--r--  2.0 unx     1263 b- defN 23-May-23 15:10 yellowdog_client/scheduler/worker_pool_helper.py
--rw-r--r--  2.0 unx     3553 b- defN 23-May-23 15:10 yellowdog_client/scheduler/worker_pool_service_proxy.py
--rw-r--r--  2.0 unx      263 b- defN 23-May-23 15:10 yellowdog_client/usage/__init__.py
--rw-r--r--  2.0 unx     1301 b- defN 23-May-23 15:10 yellowdog_client/usage/allowances_client.py
--rw-r--r--  2.0 unx     2061 b- defN 23-May-23 15:10 yellowdog_client/usage/allowances_client_impl.py
--rw-r--r--  2.0 unx     1320 b- defN 23-May-23 15:10 yellowdog_client/usage/allowances_service_proxy.py
--rw-r--r--  2.0 unx    11356 b- defN 23-May-23 15:11 yellowdog_sdk-6.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2812 b- defN 23-May-23 15:11 yellowdog_sdk-6.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 15:11 yellowdog_sdk-6.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-23 15:11 yellowdog_sdk-6.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    44849 b- defN 23-May-23 15:11 yellowdog_sdk-6.2.0.dist-info/RECORD
-419 files, 596738 bytes uncompressed, 183442 bytes compressed:  69.3%
+Zip file size: 254898 bytes, number of entries: 414
+-rw-r--r--  2.0 unx    13499 b- defN 23-Jun-09 09:00 yellowdog_client/__init__.py
+-rw-r--r--  2.0 unx       35 b- defN 23-Jun-09 09:00 yellowdog_client/_version.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jun-09 09:00 yellowdog_client/client_collection.py
+-rw-r--r--  2.0 unx     6247 b- defN 23-Jun-09 09:00 yellowdog_client/platform_client.py
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-09 09:00 yellowdog_client/account/__init__.py
+-rw-r--r--  2.0 unx     1089 b- defN 23-Jun-09 09:00 yellowdog_client/account/keyring_client.py
+-rw-r--r--  2.0 unx     1665 b- defN 23-Jun-09 09:00 yellowdog_client/account/keyring_client_impl.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-09 09:00 yellowdog_client/account/keyring_service_proxy.py
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-09 09:00 yellowdog_client/cloud_info/__init__.py
+-rw-r--r--  2.0 unx      843 b- defN 23-Jun-09 09:00 yellowdog_client/cloud_info/cloud_info_client.py
+-rw-r--r--  2.0 unx     1917 b- defN 23-Jun-09 09:00 yellowdog_client/cloud_info/cloud_info_client_impl.py
+-rw-r--r--  2.0 unx     1301 b- defN 23-Jun-09 09:00 yellowdog_client/cloud_info/cloud_info_proxy.py
+-rw-r--r--  2.0 unx      400 b- defN 23-Jun-09 09:00 yellowdog_client/common/__init__.py
+-rw-r--r--  2.0 unx      352 b- defN 23-Jun-09 09:00 yellowdog_client/common/closeable.py
+-rw-r--r--  2.0 unx     1090 b- defN 23-Jun-09 09:00 yellowdog_client/common/countdown_event.py
+-rw-r--r--  2.0 unx      640 b- defN 23-Jun-09 09:00 yellowdog_client/common/iso_datetime.py
+-rw-r--r--  2.0 unx      540 b- defN 23-Jun-09 09:00 yellowdog_client/common/pagination.py
+-rw-r--r--  2.0 unx     6792 b- defN 23-Jun-09 09:00 yellowdog_client/common/proxy.py
+-rw-r--r--  2.0 unx     1420 b- defN 23-Jun-09 09:00 yellowdog_client/common/search_client.py
+-rw-r--r--  2.0 unx     1303 b- defN 23-Jun-09 09:00 yellowdog_client/common/slice_iterator.py
+-rw-r--r--  2.0 unx      521 b- defN 23-Jun-09 09:00 yellowdog_client/common/synchronized_predicated_runner.py
+-rw-r--r--  2.0 unx      147 b- defN 23-Jun-09 09:00 yellowdog_client/common/credentials/__init__.py
+-rw-r--r--  2.0 unx      843 b- defN 23-Jun-09 09:00 yellowdog_client/common/credentials/api_key_authentication_headers_provider.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-09 09:00 yellowdog_client/common/decorators/__init__.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Jun-09 09:00 yellowdog_client/common/decorators/dispatcher.py
+-rw-r--r--  2.0 unx     6039 b- defN 23-Jun-09 09:00 yellowdog_client/common/json/__init__.py
+-rw-r--r--  2.0 unx      507 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/__init__.py
+-rw-r--r--  2.0 unx     1278 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/delegated_subscription_event_listener.py
+-rw-r--r--  2.0 unx     3123 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/subscription.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/subscription_event_listener.py
+-rw-r--r--  2.0 unx     2595 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/subscription_manager.py
+-rw-r--r--  2.0 unx     1660 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/tracking_subscription_event_listener.py
+-rw-r--r--  2.0 unx      689 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/__init__.py
+-rw-r--r--  2.0 unx      369 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/chained_thread.py
+-rw-r--r--  2.0 unx     2889 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/connected_state.py
+-rw-r--r--  2.0 unx     2430 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/connecting_state.py
+-rw-r--r--  2.0 unx     1775 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/disconnected_state.py
+-rw-r--r--  2.0 unx     3947 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/event_source.py
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/event_source_state.py
+-rw-r--r--  2.0 unx      551 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/server_response.py
+-rw-r--r--  2.0 unx      282 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/server_sent_event.py
+-rw-r--r--  2.0 unx      332 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/web_request_factory.py
+-rw-r--r--  2.0 unx     4001 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/web_requester.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/abstracts/__init__.py
+-rw-r--r--  2.0 unx      756 b- defN 23-Jun-09 09:00 yellowdog_client/common/server_sent_events/sse4python/abstracts/abstract_connection_state.py
+-rw-r--r--  2.0 unx      485 b- defN 23-Jun-09 09:00 yellowdog_client/compute/__init__.py
+-rw-r--r--  2.0 unx    20082 b- defN 23-Jun-09 09:00 yellowdog_client/compute/compute_client.py
+-rw-r--r--  2.0 unx    14378 b- defN 23-Jun-09 09:00 yellowdog_client/compute/compute_client_impl.py
+-rw-r--r--  2.0 unx     4354 b- defN 23-Jun-09 09:00 yellowdog_client/compute/compute_requirement_helper.py
+-rw-r--r--  2.0 unx     6223 b- defN 23-Jun-09 09:00 yellowdog_client/compute/compute_service_proxy.py
+-rw-r--r--  2.0 unx     2151 b- defN 23-Jun-09 09:00 yellowdog_client/compute/predicated_compute_subscription_event_listener.py
+-rw-r--r--  2.0 unx      823 b- defN 23-Jun-09 09:00 yellowdog_client/images/__init__.py
+-rw-r--r--  2.0 unx     2274 b- defN 23-Jun-09 09:00 yellowdog_client/images/images_client.py
+-rw-r--r--  2.0 unx     3349 b- defN 23-Jun-09 09:00 yellowdog_client/images/images_client_impl.py
+-rw-r--r--  2.0 unx     3393 b- defN 23-Jun-09 09:00 yellowdog_client/images/images_service_proxy.py
+-rw-r--r--  2.0 unx      391 b- defN 23-Jun-09 09:00 yellowdog_client/images/page.py
+-rw-r--r--  2.0 unx      296 b- defN 23-Jun-09 09:00 yellowdog_client/images/pageable.py
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-09 09:00 yellowdog_client/images/sort.py
+-rw-r--r--  2.0 unx    21842 b- defN 23-Jun-09 09:00 yellowdog_client/model/__init__.py
+-rw-r--r--  2.0 unx      470 b- defN 23-Jun-09 09:00 yellowdog_client/model/access_delegate.py
+-rw-r--r--  2.0 unx      472 b- defN 23-Jun-09 09:00 yellowdog_client/model/account.py
+-rw-r--r--  2.0 unx     1021 b- defN 23-Jun-09 09:00 yellowdog_client/model/account_allowance.py
+-rw-r--r--  2.0 unx      270 b- defN 23-Jun-09 09:00 yellowdog_client/model/account_authentication_properties.py
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-09 09:00 yellowdog_client/model/add_application_request.py
+-rw-r--r--  2.0 unx      253 b- defN 23-Jun-09 09:00 yellowdog_client/model/add_application_response.py
+-rw-r--r--  2.0 unx      619 b- defN 23-Jun-09 09:00 yellowdog_client/model/add_configured_worker_pool_request.py
+-rw-r--r--  2.0 unx      317 b- defN 23-Jun-09 09:00 yellowdog_client/model/add_configured_worker_pool_response.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-09 09:00 yellowdog_client/model/add_node_actions_request.py
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-09 09:00 yellowdog_client/model/add_user_request.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-09 09:00 yellowdog_client/model/add_user_response.py
+-rw-r--r--  2.0 unx      490 b- defN 23-Jun-09 09:00 yellowdog_client/model/alibaba_compute_source.py
+-rw-r--r--  2.0 unx      553 b- defN 23-Jun-09 09:00 yellowdog_client/model/alibaba_credential.py
+-rw-r--r--  2.0 unx     1773 b- defN 23-Jun-09 09:00 yellowdog_client/model/alibaba_instance.py
+-rw-r--r--  2.0 unx      342 b- defN 23-Jun-09 09:00 yellowdog_client/model/alibaba_instance_charge_type.py
+-rw-r--r--  2.0 unx     3377 b- defN 23-Jun-09 09:00 yellowdog_client/model/alibaba_instances_compute_source.py
+-rw-r--r--  2.0 unx      392 b- defN 23-Jun-09 09:00 yellowdog_client/model/alibaba_namespace_storage_configuration.py
+-rw-r--r--  2.0 unx      426 b- defN 23-Jun-09 09:00 yellowdog_client/model/alibaba_spot_strategy.py
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-09 09:00 yellowdog_client/model/allowance.py
+-rw-r--r--  2.0 unx      255 b- defN 23-Jun-09 09:00 yellowdog_client/model/allowance_exhausted_notification.py
+-rw-r--r--  2.0 unx      436 b- defN 23-Jun-09 09:00 yellowdog_client/model/allowance_limit_enforcement.py
+-rw-r--r--  2.0 unx      425 b- defN 23-Jun-09 09:00 yellowdog_client/model/allowance_reset_type.py
+-rw-r--r--  2.0 unx      624 b- defN 23-Jun-09 09:00 yellowdog_client/model/allowance_search.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-09 09:00 yellowdog_client/model/api_key.py
+-rw-r--r--  2.0 unx      494 b- defN 23-Jun-09 09:00 yellowdog_client/model/application.py
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-09 09:00 yellowdog_client/model/attribute_constraint.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-09 09:00 yellowdog_client/model/attribute_definition.py
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-09 09:00 yellowdog_client/model/attribute_preference.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-09 09:00 yellowdog_client/model/attribute_source.py
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-09 09:00 yellowdog_client/model/attribute_source_type.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-09 09:00 yellowdog_client/model/attribute_value.py
+-rw-r--r--  2.0 unx      164 b- defN 23-Jun-09 09:00 yellowdog_client/model/authentication_provider.py
+-rw-r--r--  2.0 unx      201 b- defN 23-Jun-09 09:00 yellowdog_client/model/auto_shutdown.py
+-rw-r--r--  2.0 unx      472 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_compute_source.py
+-rw-r--r--  2.0 unx      537 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_credential.py
+-rw-r--r--  2.0 unx     3851 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_fleet_compute_source.py
+-rw-r--r--  2.0 unx      537 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_fleet_instance_override.py
+-rw-r--r--  2.0 unx      628 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_fleet_on_demand_allocation_strategy.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_fleet_on_demand_options.py
+-rw-r--r--  2.0 unx      584 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_fleet_purchase_option.py
+-rw-r--r--  2.0 unx      875 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_fleet_spot_allocation_strategy.py
+-rw-r--r--  2.0 unx     1292 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_fleet_spot_options.py
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_instance.py
+-rw-r--r--  2.0 unx     3390 b- defN 23-Jun-09 09:00 yellowdog_client/model/aws_instances_compute_source.py
+-rw-r--r--  2.0 unx      331 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_account_authentication_properties.py
+-rw-r--r--  2.0 unx      634 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_client_credential.py
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_compute_credential.py
+-rw-r--r--  2.0 unx      478 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_compute_source.py
+-rw-r--r--  2.0 unx     1760 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_instance.py
+-rw-r--r--  2.0 unx      584 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_instance_credential.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_instances_compute_source.py
+-rw-r--r--  2.0 unx      373 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_namespace_storage_configuration.py
+-rw-r--r--  2.0 unx     2428 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_scale_set_compute_source.py
+-rw-r--r--  2.0 unx      444 b- defN 23-Jun-09 09:00 yellowdog_client/model/azure_storage_credential.py
+-rw-r--r--  2.0 unx     1313 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report.py
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_constraint.py
+-rw-r--r--  2.0 unx      446 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_image.py
+-rw-r--r--  2.0 unx      311 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_image_availability.py
+-rw-r--r--  2.0 unx      429 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_numeric_constraint.py
+-rw-r--r--  2.0 unx      233 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_preference.py
+-rw-r--r--  2.0 unx      782 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_source.py
+-rw-r--r--  2.0 unx      231 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_source_attribute.py
+-rw-r--r--  2.0 unx      477 b- defN 23-Jun-09 09:00 yellowdog_client/model/best_compute_source_report_string_constraint.py
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-09 09:00 yellowdog_client/model/change_password_request.py
+-rw-r--r--  2.0 unx      748 b- defN 23-Jun-09 09:00 yellowdog_client/model/cloud_provider.py
+-rw-r--r--  2.0 unx      256 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_namespace_filter.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_provision_strategy.py
+-rw-r--r--  2.0 unx     2937 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_dynamic_template.py
+-rw-r--r--  2.0 unx      623 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_dynamic_template_test_result.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_search.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_static_template.py
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_static_template_test_result.py
+-rw-r--r--  2.0 unx     2115 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_status.py
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_supported_operations.py
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_template.py
+-rw-r--r--  2.0 unx      320 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_template_summary.py
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_template_test_result.py
+-rw-r--r--  2.0 unx      446 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_template_usage.py
+-rw-r--r--  2.0 unx      407 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_usage.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirement_usage_filter.py
+-rw-r--r--  2.0 unx      277 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_requirements_summary.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source.py
+-rw-r--r--  2.0 unx      625 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_exhaustion.py
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_exhaustion_status.py
+-rw-r--r--  2.0 unx     1058 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_status.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_template.py
+-rw-r--r--  2.0 unx      370 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_template_summary.py
+-rw-r--r--  2.0 unx      268 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_traits.py
+-rw-r--r--  2.0 unx      269 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_traits_filter.py
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-09 09:00 yellowdog_client/model/compute_source_usage.py
+-rw-r--r--  2.0 unx      911 b- defN 23-Jun-09 09:00 yellowdog_client/model/configured_worker_pool.py
+-rw-r--r--  2.0 unx      598 b- defN 23-Jun-09 09:00 yellowdog_client/model/configured_worker_pool_properties.py
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-09 09:00 yellowdog_client/model/constants.py
+-rw-r--r--  2.0 unx      195 b- defN 23-Jun-09 09:00 yellowdog_client/model/create_keyring_request.py
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-09 09:00 yellowdog_client/model/create_keyring_response.py
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-09 09:00 yellowdog_client/model/credential.py
+-rw-r--r--  2.0 unx     2090 b- defN 23-Jun-09 09:00 yellowdog_client/model/currency.py
+-rw-r--r--  2.0 unx      191 b- defN 23-Jun-09 09:00 yellowdog_client/model/double_range.py
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-09 09:00 yellowdog_client/model/error_response.py
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-09 09:00 yellowdog_client/model/existing_password_request.py
+-rw-r--r--  2.0 unx      219 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_attribute_definition.py
+-rw-r--r--  2.0 unx      327 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_attribute_provider_query.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_attribute_provider_query_source.py
+-rw-r--r--  2.0 unx      338 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_attribute_provider_registration.py
+-rw-r--r--  2.0 unx      361 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_attribute_provider_results.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_attribute_provider_results_source.py
+-rw-r--r--  2.0 unx      488 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_attribute_source.py
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-09 09:00 yellowdog_client/model/external_user.py
+-rw-r--r--  2.0 unx       70 b- defN 23-Jun-09 09:00 yellowdog_client/model/filter.py
+-rw-r--r--  2.0 unx      494 b- defN 23-Jun-09 09:00 yellowdog_client/model/flatten_path.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jun-09 09:00 yellowdog_client/model/gce_compute_source.py
+-rw-r--r--  2.0 unx     1839 b- defN 23-Jun-09 09:00 yellowdog_client/model/gce_instance.py
+-rw-r--r--  2.0 unx     1959 b- defN 23-Jun-09 09:00 yellowdog_client/model/gce_instance_group_compute_source.py
+-rw-r--r--  2.0 unx     2520 b- defN 23-Jun-09 09:00 yellowdog_client/model/gce_instances_compute_source.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-09 09:00 yellowdog_client/model/gcs_namespace_storage_configuration.py
+-rw-r--r--  2.0 unx      408 b- defN 23-Jun-09 09:00 yellowdog_client/model/google_cloud_credential.py
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-09 09:00 yellowdog_client/model/grant_application_access_request.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-09 09:00 yellowdog_client/model/grant_user_access_request.py
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-09 09:00 yellowdog_client/model/identified.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-09 09:00 yellowdog_client/model/image_access.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-09 09:00 yellowdog_client/model/image_os_type.py
+-rw-r--r--  2.0 unx      382 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_id.py
+-rw-r--r--  2.0 unx      712 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_search.py
+-rw-r--r--  2.0 unx     1154 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_status.py
+-rw-r--r--  2.0 unx     1081 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_summary.py
+-rw-r--r--  2.0 unx      528 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_type.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_type_price.py
+-rw-r--r--  2.0 unx      662 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_type_price_search.py
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_type_region.py
+-rw-r--r--  2.0 unx      689 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_type_search.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_usage.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Jun-09 09:00 yellowdog_client/model/instance_usage_filter.py
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-09 09:00 yellowdog_client/model/instant_range.py
+-rw-r--r--  2.0 unx      188 b- defN 23-Jun-09 09:00 yellowdog_client/model/integer_range.py
+-rw-r--r--  2.0 unx      397 b- defN 23-Jun-09 09:00 yellowdog_client/model/internal_attribute_source.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Jun-09 09:00 yellowdog_client/model/internal_user.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-09 09:00 yellowdog_client/model/keyring.py
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-09 09:00 yellowdog_client/model/keyring_access_secrets.py
+-rw-r--r--  2.0 unx      213 b- defN 23-Jun-09 09:00 yellowdog_client/model/keyring_accessor.py
+-rw-r--r--  2.0 unx      233 b- defN 23-Jun-09 09:00 yellowdog_client/model/keyring_credential.py
+-rw-r--r--  2.0 unx      243 b- defN 23-Jun-09 09:00 yellowdog_client/model/keyring_summary.py
+-rw-r--r--  2.0 unx      185 b- defN 23-Jun-09 09:00 yellowdog_client/model/long_range.py
+-rw-r--r--  2.0 unx     1535 b- defN 23-Jun-09 09:00 yellowdog_client/model/machine_image.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jun-09 09:00 yellowdog_client/model/machine_image_family.py
+-rw-r--r--  2.0 unx      952 b- defN 23-Jun-09 09:00 yellowdog_client/model/machine_image_family_search.py
+-rw-r--r--  2.0 unx     1188 b- defN 23-Jun-09 09:00 yellowdog_client/model/machine_image_family_summary.py
+-rw-r--r--  2.0 unx     1182 b- defN 23-Jun-09 09:00 yellowdog_client/model/machine_image_group.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-09 09:00 yellowdog_client/model/metadata_filter.py
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-09 09:00 yellowdog_client/model/model_exception.py
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-09 09:00 yellowdog_client/model/named.py
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-09 09:00 yellowdog_client/model/namespace_objects_response.py
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-09 09:00 yellowdog_client/model/namespace_storage_configuration.py
+-rw-r--r--  2.0 unx       91 b- defN 23-Jun-09 09:00 yellowdog_client/model/new_password_request.py
+-rw-r--r--  2.0 unx     1099 b- defN 23-Jun-09 09:00 yellowdog_client/model/node.py
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_action.py
+-rw-r--r--  2.0 unx      161 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_action_group.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_action_queue_snapshot.py
+-rw-r--r--  2.0 unx      534 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_action_queue_status.py
+-rw-r--r--  2.0 unx      500 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_create_workers_action.py
+-rw-r--r--  2.0 unx     1707 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_details.py
+-rw-r--r--  2.0 unx      591 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_event.py
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_id_filter.py
+-rw-r--r--  2.0 unx      466 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_run_command_action.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_search.py
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_slot_numbering.py
+-rw-r--r--  2.0 unx      832 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_status.py
+-rw-r--r--  2.0 unx      604 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_summary.py
+-rw-r--r--  2.0 unx      323 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_type.py
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_worker_target.py
+-rw-r--r--  2.0 unx      166 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_worker_target_type.py
+-rw-r--r--  2.0 unx      401 b- defN 23-Jun-09 09:00 yellowdog_client/model/node_write_file_action.py
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-09 09:00 yellowdog_client/model/numeric_attribute_constraint.py
+-rw-r--r--  2.0 unx      664 b- defN 23-Jun-09 09:00 yellowdog_client/model/numeric_attribute_definition.py
+-rw-r--r--  2.0 unx      459 b- defN 23-Jun-09 09:00 yellowdog_client/model/numeric_attribute_preference.py
+-rw-r--r--  2.0 unx      168 b- defN 23-Jun-09 09:00 yellowdog_client/model/numeric_attribute_range.py
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-09 09:00 yellowdog_client/model/numeric_attribute_rank_order.py
+-rw-r--r--  2.0 unx      275 b- defN 23-Jun-09 09:00 yellowdog_client/model/numeric_attribute_value.py
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-09 09:00 yellowdog_client/model/o_auth2_authentication_properties.py
+-rw-r--r--  2.0 unx      586 b- defN 23-Jun-09 09:00 yellowdog_client/model/object_detail.py
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-09 09:00 yellowdog_client/model/object_download_request.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Jun-09 09:00 yellowdog_client/model/object_download_response.py
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-09 09:00 yellowdog_client/model/object_path.py
+-rw-r--r--  2.0 unx      193 b- defN 23-Jun-09 09:00 yellowdog_client/model/object_paths_request.py
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-09 09:00 yellowdog_client/model/object_paths_slice_request.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-09 09:00 yellowdog_client/model/object_upload_request.py
+-rw-r--r--  2.0 unx      472 b- defN 23-Jun-09 09:00 yellowdog_client/model/oci_compute_source.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Jun-09 09:00 yellowdog_client/model/oci_credential.py
+-rw-r--r--  2.0 unx     2077 b- defN 23-Jun-09 09:00 yellowdog_client/model/oci_instance.py
+-rw-r--r--  2.0 unx     2284 b- defN 23-Jun-09 09:00 yellowdog_client/model/oci_instance_pool_compute_source.py
+-rw-r--r--  2.0 unx     2241 b- defN 23-Jun-09 09:00 yellowdog_client/model/oci_instances_compute_source.py
+-rw-r--r--  2.0 unx      408 b- defN 23-Jun-09 09:00 yellowdog_client/model/oci_namespace_storage_configuration.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Jun-09 09:00 yellowdog_client/model/operating_system_licence.py
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-09 09:00 yellowdog_client/model/password_state.py
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-09 09:00 yellowdog_client/model/price.py
+-rw-r--r--  2.0 unx      157 b- defN 23-Jun-09 09:00 yellowdog_client/model/processor_architecture.py
+-rw-r--r--  2.0 unx      416 b- defN 23-Jun-09 09:00 yellowdog_client/model/provision_template_worker_pool_request.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-Jun-09 09:00 yellowdog_client/model/provisioned_worker_pool.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-Jun-09 09:00 yellowdog_client/model/provisioned_worker_pool_properties.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Jun-09 09:00 yellowdog_client/model/range.py
+-rw-r--r--  2.0 unx      208 b- defN 23-Jun-09 09:00 yellowdog_client/model/region.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Jun-09 09:00 yellowdog_client/model/region_search.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-Jun-09 09:00 yellowdog_client/model/requirement_allowance.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-09 09:00 yellowdog_client/model/requirements_allowance.py
+-rw-r--r--  2.0 unx      559 b- defN 23-Jun-09 09:00 yellowdog_client/model/retry_properties.py
+-rw-r--r--  2.0 unx     2046 b- defN 23-Jun-09 09:00 yellowdog_client/model/run_specification.py
+-rw-r--r--  2.0 unx      380 b- defN 23-Jun-09 09:00 yellowdog_client/model/s3_namespace_storage_configuration.py
+-rw-r--r--  2.0 unx     1894 b- defN 23-Jun-09 09:00 yellowdog_client/model/services_schema.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-09 09:00 yellowdog_client/model/set_password_request.py
+-rw-r--r--  2.0 unx     2473 b- defN 23-Jun-09 09:00 yellowdog_client/model/simulator_compute_source.py
+-rw-r--r--  2.0 unx     1882 b- defN 23-Jun-09 09:00 yellowdog_client/model/simulator_instance.py
+-rw-r--r--  2.0 unx      634 b- defN 23-Jun-09 09:00 yellowdog_client/model/single_source_provision_strategy.py
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-09 09:00 yellowdog_client/model/slice.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-09 09:00 yellowdog_client/model/slice_reference.py
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-09 09:00 yellowdog_client/model/sort_direction.py
+-rw-r--r--  2.0 unx     1037 b- defN 23-Jun-09 09:00 yellowdog_client/model/source_allowance.py
+-rw-r--r--  2.0 unx     1281 b- defN 23-Jun-09 09:00 yellowdog_client/model/sources_allowance.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jun-09 09:00 yellowdog_client/model/split_provision_strategy.py
+-rw-r--r--  2.0 unx      423 b- defN 23-Jun-09 09:00 yellowdog_client/model/string_attribute_constraint.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Jun-09 09:00 yellowdog_client/model/string_attribute_definition.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-09 09:00 yellowdog_client/model/string_attribute_preference.py
+-rw-r--r--  2.0 unx      316 b- defN 23-Jun-09 09:00 yellowdog_client/model/string_attribute_value.py
+-rw-r--r--  2.0 unx      244 b- defN 23-Jun-09 09:00 yellowdog_client/model/sub_region.py
+-rw-r--r--  2.0 unx      391 b- defN 23-Jun-09 09:00 yellowdog_client/model/sub_region_search.py
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-09 09:00 yellowdog_client/model/tagged.py
+-rw-r--r--  2.0 unx     2698 b- defN 23-Jun-09 09:00 yellowdog_client/model/task.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_error.py
+-rw-r--r--  2.0 unx     1851 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_group.py
+-rw-r--r--  2.0 unx     3100 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_group_status.py
+-rw-r--r--  2.0 unx     1975 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_input.py
+-rw-r--r--  2.0 unx      423 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_input_source.py
+-rw-r--r--  2.0 unx      477 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_input_verification.py
+-rw-r--r--  2.0 unx      444 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_input_verification_status.py
+-rw-r--r--  2.0 unx     2006 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_output.py
+-rw-r--r--  2.0 unx      547 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_output_source.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_search.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_status.py
+-rw-r--r--  2.0 unx      294 b- defN 23-Jun-09 09:00 yellowdog_client/model/task_summary.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-09 09:00 yellowdog_client/model/transfer_status_response.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Jun-09 09:00 yellowdog_client/model/transfer_summary_response.py
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-09 09:00 yellowdog_client/model/update_application_request.py
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-09 09:00 yellowdog_client/model/update_keyring_request.py
+-rw-r--r--  2.0 unx      203 b- defN 23-Jun-09 09:00 yellowdog_client/model/update_user_request.py
+-rw-r--r--  2.0 unx      340 b- defN 23-Jun-09 09:00 yellowdog_client/model/usage_type.py
+-rw-r--r--  2.0 unx      253 b- defN 23-Jun-09 09:00 yellowdog_client/model/user.py
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-09 09:00 yellowdog_client/model/user_login_request.py
+-rw-r--r--  2.0 unx      727 b- defN 23-Jun-09 09:00 yellowdog_client/model/waterfall_provision_strategy.py
+-rw-r--r--  2.0 unx     1869 b- defN 23-Jun-09 09:00 yellowdog_client/model/work_requirement.py
+-rw-r--r--  2.0 unx     1913 b- defN 23-Jun-09 09:00 yellowdog_client/model/work_requirement_status.py
+-rw-r--r--  2.0 unx     1374 b- defN 23-Jun-09 09:00 yellowdog_client/model/work_requirement_summary.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_action.py
+-rw-r--r--  2.0 unx      255 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_pool.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_pool_node_configuration.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_pool_properties.py
+-rw-r--r--  2.0 unx     1240 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_pool_status.py
+-rw-r--r--  2.0 unx     1347 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_pool_summary.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_pool_token.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_status.py
+-rw-r--r--  2.0 unx      819 b- defN 23-Jun-09 09:00 yellowdog_client/model/worker_summary.py
+-rw-r--r--  2.0 unx     1434 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/__init__.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/base_custom_exception.py
+-rw-r--r--  2.0 unx      282 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/chunk_transfer_exception.py
+-rw-r--r--  2.0 unx     1655 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/error_type.py
+-rw-r--r--  2.0 unx      276 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/file_transfer_failure.py
+-rw-r--r--  2.0 unx      296 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/insufficient_capacity_exception.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/internal_server_exception.py
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/invalid_operation_exception.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/invalid_request_exception.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/invalid_session_exception.py
+-rw-r--r--  2.0 unx      282 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/not_authorised_exception.py
+-rw-r--r--  2.0 unx      250 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/object_not_found_exception.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/server_error_exception.py
+-rw-r--r--  2.0 unx      776 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/service_client_exception.py
+-rw-r--r--  2.0 unx      280 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/session_close_exception.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/session_not_found_exception.py
+-rw-r--r--  2.0 unx      261 b- defN 23-Jun-09 09:00 yellowdog_client/model/exceptions/unknown_exception.py
+-rw-r--r--  2.0 unx      272 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/__init__.py
+-rw-r--r--  2.0 unx    16479 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/object_store_client.py
+-rw-r--r--  2.0 unx     6028 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/object_store_service_proxy.py
+-rw-r--r--  2.0 unx     1771 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/service_session_facade.py
+-rw-r--r--  2.0 unx      905 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/__init__.py
+-rw-r--r--  2.0 unx      229 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_chunk_download_task.py
+-rw-r--r--  2.0 unx      596 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_chunk_transfer_task.py
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_chunk_upload_task.py
+-rw-r--r--  2.0 unx      314 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_notification_dispatcher.py
+-rw-r--r--  2.0 unx     3716 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_object_store_service_proxy.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_self_binding_status_predicate.py
+-rw-r--r--  2.0 unx     2006 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_service_session_facade.py
+-rw-r--r--  2.0 unx    22303 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_session.py
+-rw-r--r--  2.0 unx     9494 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_transfer_batch.py
+-rw-r--r--  2.0 unx     6443 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/abstracts/abstract_transfer_engine.py
+-rw-r--r--  2.0 unx      374 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/__init__.py
+-rw-r--r--  2.0 unx      141 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/chunk_download_task.py
+-rw-r--r--  2.0 unx      708 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/download_batch.py
+-rw-r--r--  2.0 unx     6720 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/download_batch_builder.py
+-rw-r--r--  2.0 unx     4859 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/download_engine.py
+-rw-r--r--  2.0 unx     3075 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/download_session.py
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/abstracts/__init__.py
+-rw-r--r--  2.0 unx     1365 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/abstracts/abstract_download_batch_builder.py
+-rw-r--r--  2.0 unx      827 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/download/abstracts/abstract_download_engine.py
+-rw-r--r--  2.0 unx      991 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/__init__.py
+-rw-r--r--  2.0 unx      594 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/batch_transfer_event_args.py
+-rw-r--r--  2.0 unx     1113 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/client_error_event_args.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/file_transfer_direction.py
+-rw-r--r--  2.0 unx     1695 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/file_transfer_error_event_args.py
+-rw-r--r--  2.0 unx     1084 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/file_transfer_event_args.py
+-rw-r--r--  2.0 unx      802 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/file_transfer_exception.py
+-rw-r--r--  2.0 unx     3033 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/file_transfer_progress_event_args.py
+-rw-r--r--  2.0 unx     1378 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/file_transfer_status.py
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/transfer_properties.py
+-rw-r--r--  2.0 unx     3596 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/model/transfer_statistics.py
+-rw-r--r--  2.0 unx      352 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/__init__.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/chunk_upload_task.py
+-rw-r--r--  2.0 unx      700 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/upload_batch.py
+-rw-r--r--  2.0 unx     5359 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/upload_batch_builder.py
+-rw-r--r--  2.0 unx     4906 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/upload_engine.py
+-rw-r--r--  2.0 unx     2117 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/upload_session.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/abstracts/__init__.py
+-rw-r--r--  2.0 unx      850 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/abstracts/abstract_upload_batch_builder.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/upload/abstracts/abstract_upload_engine.py
+-rw-r--r--  2.0 unx      956 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/__init__.py
+-rw-r--r--  2.0 unx      897 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/action_utils.py
+-rw-r--r--  2.0 unx      503 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/background_thread.py
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/background_thread_factory.py
+-rw-r--r--  2.0 unx     2594 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/chunk_transfer_throttle.py
+-rw-r--r--  2.0 unx     1305 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/external_notification_dispatcher.py
+-rw-r--r--  2.0 unx     1186 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/file_utils.py
+-rw-r--r--  2.0 unx     1619 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/hash_utils.py
+-rw-r--r--  2.0 unx     1253 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/internal_notification_dispatcher.py
+-rw-r--r--  2.0 unx      664 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/memory_mapped_file_reader.py
+-rw-r--r--  2.0 unx      265 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/memory_mapped_file_reader_factory.py
+-rw-r--r--  2.0 unx      303 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/memory_mapped_file_writer_factory.py
+-rw-r--r--  2.0 unx     1373 b- defN 23-Jun-09 09:00 yellowdog_client/object_store/utils/memory_mapped_file_writter.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/__init__.py
+-rw-r--r--  2.0 unx     2105 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/predicated_work_subscription_event_listener.py
+-rw-r--r--  2.0 unx     2006 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/predicated_worker_pool_subscription_event_listener.py
+-rw-r--r--  2.0 unx    12312 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/work_client.py
+-rw-r--r--  2.0 unx     6652 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/work_client_impl.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/work_requirement_helper.py
+-rw-r--r--  2.0 unx     2694 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/work_service_proxy.py
+-rw-r--r--  2.0 unx    14596 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/worker_pool_client.py
+-rw-r--r--  2.0 unx     8213 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/worker_pool_client_impl.py
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/worker_pool_helper.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-Jun-09 09:00 yellowdog_client/scheduler/worker_pool_service_proxy.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-09 09:00 yellowdog_client/usage/__init__.py
+-rw-r--r--  2.0 unx     1301 b- defN 23-Jun-09 09:00 yellowdog_client/usage/allowances_client.py
+-rw-r--r--  2.0 unx     2061 b- defN 23-Jun-09 09:00 yellowdog_client/usage/allowances_client_impl.py
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jun-09 09:00 yellowdog_client/usage/allowances_service_proxy.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jun-09 09:01 yellowdog_sdk-7.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2812 b- defN 23-Jun-09 09:01 yellowdog_sdk-7.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 09:01 yellowdog_sdk-7.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-09 09:01 yellowdog_sdk-7.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    44227 b- defN 23-Jun-09 09:01 yellowdog_sdk-7.0.0.dist-info/RECORD
+414 files, 592458 bytes uncompressed, 181472 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -225,20 +225,14 @@
 
 Filename: yellowdog_client/model/alibaba_namespace_storage_configuration.py
 Comment: 
 
 Filename: yellowdog_client/model/alibaba_spot_strategy.py
 Comment: 
 
-Filename: yellowdog_client/model/all_nodes_inactive_shutdown_condition.py
-Comment: 
-
-Filename: yellowdog_client/model/all_workers_released_shutdown_condition.py
-Comment: 
-
 Filename: yellowdog_client/model/allowance.py
 Comment: 
 
 Filename: yellowdog_client/model/allowance_exhausted_notification.py
 Comment: 
 
 Filename: yellowdog_client/model/allowance_limit_enforcement.py
@@ -273,14 +267,17 @@
 
 Filename: yellowdog_client/model/attribute_value.py
 Comment: 
 
 Filename: yellowdog_client/model/authentication_provider.py
 Comment: 
 
+Filename: yellowdog_client/model/auto_shutdown.py
+Comment: 
+
 Filename: yellowdog_client/model/aws_compute_source.py
 Comment: 
 
 Filename: yellowdog_client/model/aws_credential.py
 Comment: 
 
 Filename: yellowdog_client/model/aws_fleet_compute_source.py
@@ -639,26 +636,20 @@
 
 Filename: yellowdog_client/model/namespace_storage_configuration.py
 Comment: 
 
 Filename: yellowdog_client/model/new_password_request.py
 Comment: 
 
-Filename: yellowdog_client/model/no_registered_workers_shutdown_condition.py
-Comment: 
-
 Filename: yellowdog_client/model/node.py
 Comment: 
 
 Filename: yellowdog_client/model/node_action.py
 Comment: 
 
-Filename: yellowdog_client/model/node_action_failed_shutdown_condition.py
-Comment: 
-
 Filename: yellowdog_client/model/node_action_group.py
 Comment: 
 
 Filename: yellowdog_client/model/node_action_queue_snapshot.py
 Comment: 
 
 Filename: yellowdog_client/model/node_action_queue_status.py
@@ -903,17 +894,14 @@
 
 Filename: yellowdog_client/model/transfer_status_response.py
 Comment: 
 
 Filename: yellowdog_client/model/transfer_summary_response.py
 Comment: 
 
-Filename: yellowdog_client/model/unclaimed_after_startup_shutdown_condition.py
-Comment: 
-
 Filename: yellowdog_client/model/update_application_request.py
 Comment: 
 
 Filename: yellowdog_client/model/update_keyring_request.py
 Comment: 
 
 Filename: yellowdog_client/model/update_user_request.py
@@ -951,17 +939,14 @@
 
 Filename: yellowdog_client/model/worker_pool_node_configuration.py
 Comment: 
 
 Filename: yellowdog_client/model/worker_pool_properties.py
 Comment: 
 
-Filename: yellowdog_client/model/worker_pool_shutdown_condition.py
-Comment: 
-
 Filename: yellowdog_client/model/worker_pool_status.py
 Comment: 
 
 Filename: yellowdog_client/model/worker_pool_summary.py
 Comment: 
 
 Filename: yellowdog_client/model/worker_pool_token.py
@@ -1236,23 +1221,23 @@
 
 Filename: yellowdog_client/usage/allowances_client_impl.py
 Comment: 
 
 Filename: yellowdog_client/usage/allowances_service_proxy.py
 Comment: 
 
-Filename: yellowdog_sdk-6.2.0.dist-info/LICENSE
+Filename: yellowdog_sdk-7.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: yellowdog_sdk-6.2.0.dist-info/METADATA
+Filename: yellowdog_sdk-7.0.0.dist-info/METADATA
 Comment: 
 
-Filename: yellowdog_sdk-6.2.0.dist-info/WHEEL
+Filename: yellowdog_sdk-7.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: yellowdog_sdk-6.2.0.dist-info/top_level.txt
+Filename: yellowdog_sdk-7.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: yellowdog_sdk-6.2.0.dist-info/RECORD
+Filename: yellowdog_sdk-7.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yellowdog_client/_version.py

```diff
@@ -1 +1 @@
-__version__ = '6.2.0'  # YEL-11447
+__version__ = '7.0.0'  # YEL-11514
```

## yellowdog_client/model/__init__.py

```diff
@@ -12,30 +12,29 @@
 from .alibaba_compute_source import AlibabaComputeSource
 from .alibaba_credential import AlibabaCredential
 from .alibaba_instance import AlibabaInstance
 from .alibaba_instance_charge_type import AlibabaInstanceChargeType
 from .alibaba_instances_compute_source import AlibabaInstancesComputeSource
 from .alibaba_namespace_storage_configuration import AlibabaNamespaceStorageConfiguration
 from .alibaba_spot_strategy import AlibabaSpotStrategy
-from .all_nodes_inactive_shutdown_condition import AllNodesInactiveShutdownCondition
-from .all_workers_released_shutdown_condition import AllWorkersReleasedShutdownCondition
 from .allowance import Allowance
 from .allowance_exhausted_notification import AllowanceExhaustedNotification
 from .allowance_limit_enforcement import AllowanceLimitEnforcement
 from .allowance_reset_type import AllowanceResetType
 from .allowance_search import AllowanceSearch
 from .api_key import ApiKey
 from .application import Application
 from .attribute_constraint import AttributeConstraint
 from .attribute_definition import AttributeDefinition
 from .attribute_preference import AttributePreference
 from .attribute_source import AttributeSource
 from .attribute_source_type import AttributeSourceType
 from .attribute_value import AttributeValue
 from .authentication_provider import AuthenticationProvider
+from .auto_shutdown import AutoShutdown
 from .aws_compute_source import AwsComputeSource
 from .aws_credential import AwsCredential
 from .aws_fleet_compute_source import AwsFleetComputeSource
 from .aws_fleet_instance_override import AwsFleetInstanceOverride
 from .aws_fleet_on_demand_allocation_strategy import AwsFleetOnDemandAllocationStrategy
 from .aws_fleet_on_demand_options import AwsFleetOnDemandOptions
 from .aws_fleet_purchase_option import AwsFleetPurchaseOption
@@ -150,18 +149,16 @@
 from .machine_image_group import MachineImageGroup
 from .metadata_filter import MetadataFilter
 from .model_exception import ModelException
 from .named import Named
 from .namespace_objects_response import NamespaceObjectsResponse
 from .namespace_storage_configuration import NamespaceStorageConfiguration
 from .new_password_request import NewPasswordRequest
-from .no_registered_workers_shutdown_condition import NoRegisteredWorkersShutdownCondition
 from .node import Node
 from .node_action import NodeAction
-from .node_action_failed_shutdown_condition import NodeActionFailedShutdownCondition
 from .node_action_group import NodeActionGroup
 from .node_action_queue_snapshot import NodeActionQueueSnapshot
 from .node_action_queue_status import NodeActionQueueStatus
 from .node_create_workers_action import NodeCreateWorkersAction
 from .node_details import NodeDetails
 from .node_event import NodeEvent
 from .node_id_filter import NodeIdFilter
@@ -238,15 +235,14 @@
 from .task_output import TaskOutput
 from .task_output_source import TaskOutputSource
 from .task_search import TaskSearch
 from .task_status import TaskStatus
 from .task_summary import TaskSummary
 from .transfer_status_response import TransferStatusResponse
 from .transfer_summary_response import TransferSummaryResponse
-from .unclaimed_after_startup_shutdown_condition import UnclaimedAfterStartupShutdownCondition
 from .update_application_request import UpdateApplicationRequest
 from .update_keyring_request import UpdateKeyringRequest
 from .update_user_request import UpdateUserRequest
 from .usage_type import UsageType
 from .user import User
 from .user_login_request import UserLoginRequest
 from .waterfall_provision_strategy import WaterfallProvisionStrategy
@@ -254,15 +250,14 @@
 from .work_requirement_status import WorkRequirementStatus
 from .work_requirement_summary import WorkRequirementSummary
 from .worker import Worker
 from .worker_action import WorkerAction
 from .worker_pool import WorkerPool
 from .worker_pool_node_configuration import WorkerPoolNodeConfiguration
 from .worker_pool_properties import WorkerPoolProperties
-from .worker_pool_shutdown_condition import WorkerPoolShutdownCondition
 from .worker_pool_status import WorkerPoolStatus
 from .worker_pool_summary import WorkerPoolSummary
 from .worker_pool_token import WorkerPoolToken
 from .worker_status import WorkerStatus
 from .worker_summary import WorkerSummary
 
 __all__ = [
@@ -280,30 +275,29 @@
     "AlibabaComputeSource",
     "AlibabaCredential",
     "AlibabaInstance",
     "AlibabaInstanceChargeType",
     "AlibabaInstancesComputeSource",
     "AlibabaNamespaceStorageConfiguration",
     "AlibabaSpotStrategy",
-    "AllNodesInactiveShutdownCondition",
-    "AllWorkersReleasedShutdownCondition",
     "Allowance",
     "AllowanceExhaustedNotification",
     "AllowanceLimitEnforcement",
     "AllowanceResetType",
     "AllowanceSearch",
     "ApiKey",
     "Application",
     "AttributeConstraint",
     "AttributeDefinition",
     "AttributePreference",
     "AttributeSource",
     "AttributeSourceType",
     "AttributeValue",
     "AuthenticationProvider",
+    "AutoShutdown",
     "AwsComputeSource",
     "AwsCredential",
     "AwsFleetComputeSource",
     "AwsFleetInstanceOverride",
     "AwsFleetOnDemandAllocationStrategy",
     "AwsFleetOnDemandOptions",
     "AwsFleetPurchaseOption",
@@ -418,18 +412,16 @@
     "MachineImageGroup",
     "MetadataFilter",
     "ModelException",
     "Named",
     "NamespaceObjectsResponse",
     "NamespaceStorageConfiguration",
     "NewPasswordRequest",
-    "NoRegisteredWorkersShutdownCondition",
     "Node",
     "NodeAction",
-    "NodeActionFailedShutdownCondition",
     "NodeActionGroup",
     "NodeActionQueueSnapshot",
     "NodeActionQueueStatus",
     "NodeCreateWorkersAction",
     "NodeDetails",
     "NodeEvent",
     "NodeIdFilter",
@@ -506,15 +498,14 @@
     "TaskOutput",
     "TaskOutputSource",
     "TaskSearch",
     "TaskStatus",
     "TaskSummary",
     "TransferStatusResponse",
     "TransferSummaryResponse",
-    "UnclaimedAfterStartupShutdownCondition",
     "UpdateApplicationRequest",
     "UpdateKeyringRequest",
     "UpdateUserRequest",
     "UsageType",
     "User",
     "UserLoginRequest",
     "WaterfallProvisionStrategy",
@@ -522,14 +513,13 @@
     "WorkRequirementStatus",
     "WorkRequirementSummary",
     "Worker",
     "WorkerAction",
     "WorkerPool",
     "WorkerPoolNodeConfiguration",
     "WorkerPoolProperties",
-    "WorkerPoolShutdownCondition",
     "WorkerPoolStatus",
     "WorkerPoolSummary",
     "WorkerPoolToken",
     "WorkerStatus",
     "WorkerSummary",
 ]
```

## yellowdog_client/model/provisioned_worker_pool_properties.py

```diff
@@ -1,32 +1,28 @@
 from dataclasses import dataclass
 from datetime import timedelta
-from typing import List, Optional
+from typing import Optional
 
+from .auto_shutdown import AutoShutdown
 from .node_worker_target import NodeWorkerTarget
 from .worker_pool_node_configuration import WorkerPoolNodeConfiguration
 from .worker_pool_properties import WorkerPoolProperties
-from .worker_pool_shutdown_condition import WorkerPoolShutdownCondition
 
 
 @dataclass
 class ProvisionedWorkerPoolProperties(WorkerPoolProperties):
     """Defines properties to determine the behaviour that the Scheduler service should use when managing a provisioned worker pool."""
     createNodeWorkers: Optional[NodeWorkerTarget] = None
     """How many workers to create on each node."""
     minNodes: Optional[int] = None
     """The minimum number of nodes that the worker pool can be scaled down to."""
     maxNodes: Optional[int] = None
     """The maximum number of nodes that the worker pool can be scaled up to."""
-    nodeBootTimeLimit: Optional[timedelta] = None
+    nodeBootTimeout: Optional[timedelta] = None
     """The time given for a node to be registered before it is considered to have failed."""
-    nodeIdleTimeLimit: Optional[timedelta] = None
-    """The time that a node can be idle with all workers unclaimed before it is terminated."""
-    nodeIdleGracePeriod: Optional[timedelta] = None
-    """The time after a node registers where the idle check is not applied."""
-    autoShutdown: Optional[bool] = None
-    """If true, the worker pool will be automatically shutdown, according to the configured autoShutdownConditions."""
-    autoShutdownConditions: Optional[List[WorkerPoolShutdownCondition]] = None
-    """A list of conditions that can cause the worker pool to be automatically shutdown if one or more conditions is met."""
+    idleNodeShutdown: Optional[AutoShutdown] = None
+    """Determines the auto shutdown behaviour applied for idle nodes."""
+    idlePoolShutdown: Optional[AutoShutdown] = None
+    """Determines the auto shutdown behaviour applied for an idle pool."""
     workerTag: Optional[str] = None
     """An optional tag value that will be attached to all workers in this pool and used to constrain worker allocation."""
     nodeConfiguration: Optional[WorkerPoolNodeConfiguration] = None
```

## yellowdog_client/scheduler/work_client.py

```diff
@@ -1,12 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import List
 
-from pip._internal.utils.deprecation import deprecated
-
 from .work_requirement_helper import WorkRequirementHelper
 from yellowdog_client.common import Closeable, SearchClient
 from yellowdog_client.common.server_sent_events import SubscriptionEventListener
 from yellowdog_client.model import Slice, SliceReference, Task, TaskGroup, TaskSearch, WorkRequirement, WorkRequirementSummary
 
 
 class WorkClient(ABC, Closeable):
@@ -290,26 +288,28 @@
         """
         Returns tasks within the system that match the specified search.
         WARNING: If your search matches too many tasks to fit into your application's memory limits, consider using
         #streamTasks(TaskSearch) or #findTasks(TaskSearch, SliceReference).
 
         :param search: the search
         :return: a list of tasks
+        @deprecated use #getTasks(TaskSearch) instead to search tasks.
         """
 
         pass
 
     @abstractmethod
     def find_tasks_slice(self, search: TaskSearch, slice_reference: SliceReference) -> Slice[Task]:
         """
         Returns a slice of tasks that match the specified search and slice reference.
 
         :param search:         the search
         :param slice_reference: the slice reference
         :return: a slice of tasks
+        @deprecated use #getTasks(TaskSearch) instead to search tasks.
         """
 
         pass
 
     @abstractmethod
     def get_tasks(self, search: TaskSearch) -> SearchClient[Task]:
         """
```

## yellowdog_client/scheduler/worker_pool_client.py

```diff
@@ -244,26 +244,28 @@
         """
         Returns worker pool nodes within the system that match the specified search.
         WARNING: If your search matches too many workers to fit into your application's memory limits, consider using
         #streamNodes(NodeSearch) or #findNodes(NodeSearch, SliceReference).
 
         :param search: the search
         :return: a list of nodes
+        @deprecated use #getNodes(NodeSearch) instead to search nodes.
         """
 
         pass
 
     @abstractmethod
     def find_nodes_slice(self, search: NodeSearch, slice_reference: SliceReference) -> Slice[Node]:
         """
         Returns a slice of nodes that match the specified search and slice reference.
 
         :param search:         the search
         :param slice_reference: the slice reference
         :return: a slice of nodes
+        @deprecated use #getNodes(NodeSearch) instead to search nodes.
         """
 
         pass
 
     @abstractmethod
     def get_node(self, node: Node) -> Node:
         """
```

## Comparing `yellowdog_sdk-6.2.0.dist-info/LICENSE` & `yellowdog_sdk-7.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `yellowdog_sdk-6.2.0.dist-info/METADATA` & `yellowdog_sdk-7.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-sdk
-Version: 6.2.0
+Version: 7.0.0
 Summary: SDK for the YellowDog Platform
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://yellowdog.co
 Project-URL: Source, https://github.com/yellowdog/yellowdog-sdk-python-public
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `yellowdog_sdk-6.2.0.dist-info/RECORD` & `yellowdog_sdk-7.0.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 yellowdog_client/__init__.py,sha256=I5CmYfMNDEpVNl2X7178KIx7syg2cIYiTe_SnJnlIhw,13499
-yellowdog_client/_version.py,sha256=LDI7ZIT_v6-FZbxqjy7UKzCCPzqgX1Lcc1BWfygY7tM,35
+yellowdog_client/_version.py,sha256=K93QETNaia3tjKdxOK8cdBhtPg9plumwsXo9byLzPaI,35
 yellowdog_client/client_collection.py,sha256=VSEzjf6iR1qCQ0YGLyDq_Kgvw8r832QDwTp6-MLB4Vs,388
 yellowdog_client/platform_client.py,sha256=ifZQjNv7kTu5uZnnI1xPPmx8anWvHkVjvroF85SXT3o,6247
 yellowdog_client/account/__init__.py,sha256=wx5GbsoODMdXbOmRoNZu5VYgDJX-RqsFb9ph14HXoV4,235
 yellowdog_client/account/keyring_client.py,sha256=LtT4V4clPQVJHdodY5TVvOotovQiVqAIufL4l5WuZjM,1089
 yellowdog_client/account/keyring_client_impl.py,sha256=s_IltFtozR7lYdR9XNEZVj885pgJ0DoInv0B24GtblI,1665
 yellowdog_client/account/keyring_service_proxy.py,sha256=8oK6lK3FxHOIbq--qcKSAd5bqkPGMN023CrX_Q8RKeI,1220
 yellowdog_client/cloud_info/__init__.py,sha256=ku93SVbWErx_YG5El3q3bUQOZsYjMSwy3r7B8H3tEGA,234
@@ -52,15 +52,15 @@
 yellowdog_client/images/__init__.py,sha256=E5EeflQVqAIlff0ZQzQs5cCQKFOqmDn3ARAla0Hbr7s,823
 yellowdog_client/images/images_client.py,sha256=1cAgtKSIbM2v37Zrf0Y3fLbaDWyJB9e8SnSTntuKT8U,2274
 yellowdog_client/images/images_client_impl.py,sha256=kGadXCEUr_vjBeWfNeTThMrSoC7yKZ6xFMJQoHlx1vI,3349
 yellowdog_client/images/images_service_proxy.py,sha256=eyP4u6FoIH1WJvNM_m8tacTCsodW29S0bQ5Ul09Ywzk,3393
 yellowdog_client/images/page.py,sha256=UIvlxvzdcfnKvbcq2Cn6IB7ZtQMc3dzcBTUfElvVPwQ,391
 yellowdog_client/images/pageable.py,sha256=msD8uGGJ2F5jEqTNDYaFrh6z6drlxOXZ1AmB0T3edM0,296
 yellowdog_client/images/sort.py,sha256=YS05DlIRg1Cm3QLBi6KFjFdB3g-b3WrqFFitlMJUEMM,167
-yellowdog_client/model/__init__.py,sha256=rUcgrcK64LlSxCCPpMQM_PQETyMy4Taa3TNGWtY5m5A,22549
+yellowdog_client/model/__init__.py,sha256=h24siFemWwU21w-FlBH3bCeeDDx5K7yFOZYBIQ16C50,21842
 yellowdog_client/model/access_delegate.py,sha256=GjmiR1_4H89F4ObVV5fOOTV-hesnU7G63PezR2-1kxU,470
 yellowdog_client/model/account.py,sha256=rOWzqc0Xy-egWnJNaB3IEr99kicavndAzL4AcxDSXJw,472
 yellowdog_client/model/account_allowance.py,sha256=c-MkSSRLB5Y5TMDZl5h5fipj4vzLLlO_AQXPeRJ0AYw,1021
 yellowdog_client/model/account_authentication_properties.py,sha256=PLVLHV_V2Bs8rv4TTl9K6sMj3A94YwulhfMd8wo89N0,270
 yellowdog_client/model/add_application_request.py,sha256=kuFqYt7tdl7edAORY_o993AmMddjqWPnHtM3FsHBTjU,156
 yellowdog_client/model/add_application_response.py,sha256=n0maRi4HEZe4v1nNGu3gX9ExzDulaCAI09PHyRbuCr0,253
 yellowdog_client/model/add_configured_worker_pool_request.py,sha256=Fez-5cettaYPcGFE50I1ZDO_SN0Tfz9F6W0UrSXb4dc,619
@@ -71,30 +71,29 @@
 yellowdog_client/model/alibaba_compute_source.py,sha256=x9UR1DBmOsv47OTmrbz3yltLxFM8f_QTOIhIuqTdbz4,490
 yellowdog_client/model/alibaba_credential.py,sha256=I9tE0VPU03I5UDX5lGWDvMWBETNdY1pQg5DYBUTntyY,553
 yellowdog_client/model/alibaba_instance.py,sha256=_hX8nbMetWeq4u9QuIliv8OlaINbZ7agQpzuiObYwso,1773
 yellowdog_client/model/alibaba_instance_charge_type.py,sha256=KwKCNj4IXn8cQGTrhbGjyiHualS6kJpDvw0ObLgZkW0,342
 yellowdog_client/model/alibaba_instances_compute_source.py,sha256=iJIxzxbO8D8GZ2v9h02j8w9YMtP_11w9XloEqLsD4WM,3377
 yellowdog_client/model/alibaba_namespace_storage_configuration.py,sha256=fSps3B7IUcm0G4C_fc7dR-Uy0xbJhRux1EmD7QtzG6k,392
 yellowdog_client/model/alibaba_spot_strategy.py,sha256=_zZx01-CWKlb-enNnTE7cjf1yL8OtwuGde2B53qyQks,426
-yellowdog_client/model/all_nodes_inactive_shutdown_condition.py,sha256=f9XP-iG6Y4rsLdLVBTklThxMtLoYXq1uHZv58GxRFmI,554
-yellowdog_client/model/all_workers_released_shutdown_condition.py,sha256=bROOrvGS4ZmVk2pzZXURZwZXXJUUjPTuEbrlbq2zbsc,562
 yellowdog_client/model/allowance.py,sha256=9BMKrxuT4UKTgvLhYnlyiXI2wkfcO9GYElbKLuYubcU,167
 yellowdog_client/model/allowance_exhausted_notification.py,sha256=l38uP4l0CmC6v1qsPksCA-go-00Kt1Ec1t_RrhD1fKo,255
 yellowdog_client/model/allowance_limit_enforcement.py,sha256=uvU86l0iY3-lcb3i0YHN3EVF6dxbWOM7ATYGgEPh0XE,436
 yellowdog_client/model/allowance_reset_type.py,sha256=XtF2mbVm0Kn4Vb1xANYKJfXw4iPNTFwhd6n4DO5zdaI,425
 yellowdog_client/model/allowance_search.py,sha256=p-FV1YkDsbLVu5_IxetGIVw7UDKC0WjjCxOai5pH5qg,624
 yellowdog_client/model/api_key.py,sha256=yQeXeMuoNqgYFAHMtWRzHWnBS8F-tVfZZ5zCB-klxT4,151
 yellowdog_client/model/application.py,sha256=6L4PBLoLfWCJ8H8HqgsXcXoJwJfdHORBWW7MIDTo-CU,494
 yellowdog_client/model/attribute_constraint.py,sha256=6GqpFsQuDMY3UnMKHn337Erlkt0qnBadHJJ0fL6MF3s,129
 yellowdog_client/model/attribute_definition.py,sha256=7sl6txIaF-3E27D5btpRe40QRrV0n5w2U59i1Sr2isE,162
 yellowdog_client/model/attribute_preference.py,sha256=Ve7b0SNKvjxc8LXUqvYyOzvi3zyM7BrKiMoILPTf90c,129
 yellowdog_client/model/attribute_source.py,sha256=OOzkboniwpMDaULq2H5X5ceDPex669yPi488pKgxRx8,79
 yellowdog_client/model/attribute_source_type.py,sha256=OBEwtfoUjNooLrdQaxLIYzk7f2s7yB8Wk8PDKN7QjZU,357
 yellowdog_client/model/attribute_value.py,sha256=u_b6nieOJitvl32Wfs__dHOYcNCcgEG5wEXafHBqD_Q,205
 yellowdog_client/model/authentication_provider.py,sha256=95Md8EboLF927bOEMDKh9UoDOingkc9t5ETufyySd9o,164
+yellowdog_client/model/auto_shutdown.py,sha256=xCFXO1oxMO6TGBqO1mqtFIHVx4xnruJ4080bs-Lpb2s,201
 yellowdog_client/model/aws_compute_source.py,sha256=bnoRWsJ-SD7gwydkdU3OL-VHFFwrhU6rtgdD87fyMW4,472
 yellowdog_client/model/aws_credential.py,sha256=Z7e5YadXGbE0PIbqDqoFN4curD2dBPI4--ubCgyCubM,537
 yellowdog_client/model/aws_fleet_compute_source.py,sha256=CKqiZpqNynmI-IGIjb7B-sVGqFvtj6bgSJXuaDEtNGQ,3851
 yellowdog_client/model/aws_fleet_instance_override.py,sha256=SaQhKm7i_KYzovZ3Ou8djgq1KLAo2NlL5lnfapgBPvc,537
 yellowdog_client/model/aws_fleet_on_demand_allocation_strategy.py,sha256=CS1oTf-BeKu3yRtUSuZn-rBgeuPTqu2wn47lulxq0vE,628
 yellowdog_client/model/aws_fleet_on_demand_options.py,sha256=DSVCB7KaX1-dMZSqSVdxjHH2QUCJHKjlWrO_WZ0b1fs,1092
 yellowdog_client/model/aws_fleet_purchase_option.py,sha256=Rpwk3pwohjXH9aL0rpQZn1mYur_gSQuH1fCm3VV5YZs,584
@@ -209,18 +208,16 @@
 yellowdog_client/model/machine_image_group.py,sha256=dLjupIpqVJmCJV9Dssn5NvIQxDxXzhL8WjLm6FOdJTY,1182
 yellowdog_client/model/metadata_filter.py,sha256=FqFd531NmmUUSjmPOaBVkYrAYGfq2vwJFOMPPmNYVMU,142
 yellowdog_client/model/model_exception.py,sha256=QNUX9qwJSnPw1IdLcg29z4274y6pnmykqf0uV82Nxqg,78
 yellowdog_client/model/named.py,sha256=pWp_0aDBEogJNySzq0-RgNT4z0SjE621eJRJ-8es0ng,143
 yellowdog_client/model/namespace_objects_response.py,sha256=icPFUDS5AaTGd0eJK1uRKt4cBHNE-TDFQVRIuH_ykh4,189
 yellowdog_client/model/namespace_storage_configuration.py,sha256=6JSDmRbrsWhJqOeqz3skdR8t2hlP40kvPoW0CV4hYbc,139
 yellowdog_client/model/new_password_request.py,sha256=7zJkK_3GJde6QQidaxFaj49DKIQg52FTJrbmgdfTxrE,91
-yellowdog_client/model/no_registered_workers_shutdown_condition.py,sha256=_-c0VBt6ri47ZBEWk3uX1jF3pJmcrjEps7CcGMO-icw,446
 yellowdog_client/model/node.py,sha256=3WzRtFfnpF9xlVq67PUqEndCzNMqjO-voyUvUuja_K8,1099
 yellowdog_client/model/node_action.py,sha256=4NTsvuwlIVC5Fd-VQ9dg0no-93UTyhcaKAG_CG7dV3g,122
-yellowdog_client/model/node_action_failed_shutdown_condition.py,sha256=gRqUBMUIoYKYtaSxDYJF6n2D_z6zuckn1IghjrN6cw0,566
 yellowdog_client/model/node_action_group.py,sha256=hLKSy9MrLWvJrVgdiqT9jXy-3vTAeAMYiw8zNUvmeQM,161
 yellowdog_client/model/node_action_queue_snapshot.py,sha256=PcY8jVyKM93GGkSyGyTlDw-YzgH4OV54SHfmHfI9-pc,467
 yellowdog_client/model/node_action_queue_status.py,sha256=1wGQNsT998N-Bek82lD2OxNZEFJaqZu-6Uw-pQbbUUI,534
 yellowdog_client/model/node_create_workers_action.py,sha256=4iqZA1RqkEyZg3GcPo0uraZGaNq8YAYXMQ_xBXd0f_Y,500
 yellowdog_client/model/node_details.py,sha256=lfzGHPQaf64kyrEQA84w_iHoiSnN9ySK1RIuLGFeaSE,1707
 yellowdog_client/model/node_event.py,sha256=AssuGpCASFE1utM3cyWyjMPNTgQ20L9Q-aBo0EGceNA,591
 yellowdog_client/model/node_id_filter.py,sha256=jQushAfXGtvUEzRfr_1iUZQeyD4eFC6oJk7ZhAYIoXo,144
@@ -255,15 +252,15 @@
 yellowdog_client/model/oci_namespace_storage_configuration.py,sha256=YsbDhzC_FT1rQMeHEuYFpfZJSuiQKOwdGs72ksdF69g,408
 yellowdog_client/model/operating_system_licence.py,sha256=nYL3U4d8pE1qtQlBrBPxJx7fUq6FWMAj--9lbya-Srs,347
 yellowdog_client/model/password_state.py,sha256=RULlqm2R_5neOhz3I0HAt72geLgxb4jFabg06ba4dKM,163
 yellowdog_client/model/price.py,sha256=kPZw5VGPg5vKRXL5brX8eZrH_GePvlBhdfMsm5fF6Dc,194
 yellowdog_client/model/processor_architecture.py,sha256=hkbyplz2R5SeVtINaB3CcU86yR64elm5qi9W48LHVms,157
 yellowdog_client/model/provision_template_worker_pool_request.py,sha256=FEGUv-882NQJOF8KH22wQatzHwiz9_TPSUBWWSE2H-E,416
 yellowdog_client/model/provisioned_worker_pool.py,sha256=pPWrnj4V3XKsFopNVph4OLCud-twZGTIeTiP9beRygU,1047
-yellowdog_client/model/provisioned_worker_pool_properties.py,sha256=2AzZzdOfPWGCOw5JwACULN6h1dI2u9wXk3gxSNCpp6Q,1908
+yellowdog_client/model/provisioned_worker_pool_properties.py,sha256=ObTIEl06JBevzfW8metBmX2UlrjCBnKUTVvW2-F_Hbs,1481
 yellowdog_client/model/range.py,sha256=epjfe_G9T5FrUNQ37kPNYIXBUrzAUVOdHA_kZEVPVrE,135
 yellowdog_client/model/region.py,sha256=eJtoRWRk_fNscZ5zo7an-LFD76AkfGjO0r6lzNLx67Y,208
 yellowdog_client/model/region_search.py,sha256=mr61SruzGuJj02aI6gHE6cuXUUYwN7TEFSiDBmTGhr4,355
 yellowdog_client/model/requirement_allowance.py,sha256=ovCvZlKFeosV3kNxtJyGD4W7NdKviPSSvuunHjEWs3E,1052
 yellowdog_client/model/requirements_allowance.py,sha256=qp6MVWChl_RzrzslVrf2bOfUoSNsA3I4jlM0DLnlnJk,1197
 yellowdog_client/model/retry_properties.py,sha256=cccJRb-r1PkUixb-V26GIGf1iOXBnnhl1HGLy_Yr-Q8,559
 yellowdog_client/model/run_specification.py,sha256=LZ4jubi32PGwnPYIyXBsRfPc1eiRgMW8etMgAIDaGl4,2046
@@ -297,15 +294,14 @@
 yellowdog_client/model/task_output.py,sha256=-3hj9WB2OLpowdWgqtc_t_L14or6E8_I2W0-DesNneg,2006
 yellowdog_client/model/task_output_source.py,sha256=-_5cMlfvMXY5ehBDF4lKKxW6Iu26Gi9QIXA6fiz3oAY,547
 yellowdog_client/model/task_search.py,sha256=2FakY4abnkclo6orZXJYtNI76vRxB8kSJY7EO6PjiAE,702
 yellowdog_client/model/task_status.py,sha256=aN5icJ39UULR8pZhuLtK-8lYS1ajAUwyiQyZ_KImymI,1554
 yellowdog_client/model/task_summary.py,sha256=GN__WCspp6rDcE627KsnFTruIt4r4XiP-8RQ7DhTMfI,294
 yellowdog_client/model/transfer_status_response.py,sha256=wE2-4kdyRtxPHAoaUqH69J33AsNIhKLV11rDiMbCNYM,341
 yellowdog_client/model/transfer_summary_response.py,sha256=doUaSzP5zgvFL-21DgLnt_6DkGYGzCfUCAjbRK_KHC0,409
-yellowdog_client/model/unclaimed_after_startup_shutdown_condition.py,sha256=RMPjzQQ8zCyGo9k8WvvqIFM6lPdftKCyQVoCcN-BdV8,598
 yellowdog_client/model/update_application_request.py,sha256=WYmSU3FvmUKOkWOEU7KHGIvw5GpU9nRKvN__l5sVTVA,176
 yellowdog_client/model/update_keyring_request.py,sha256=h8tnBW1jzNQ4mxi6X5-I2Hn9E3lrEll3AwoZhM8Z2B4,141
 yellowdog_client/model/update_user_request.py,sha256=6OEGwM_sMeTRFP4Wi-_jsaBMgpWSBycyoPNxhdNVTTI,203
 yellowdog_client/model/usage_type.py,sha256=vZKtclWVaGLeiHS-CYeDRAIj4hAt_gM-JyXzk8C484w,340
 yellowdog_client/model/user.py,sha256=sS16xGlDC3BsFeCfWRhYUv9Wp3Do8unZMT_VLr1MEd8,253
 yellowdog_client/model/user_login_request.py,sha256=dkDB05LDmX17eglFQu1LMD6LodI9t21OkUw8L_v-K-U,128
 yellowdog_client/model/waterfall_provision_strategy.py,sha256=1mAIACbWcVrsy3Bjulgh3TaPx83WoqRM443-jQ9FgaQ,727
@@ -313,15 +309,14 @@
 yellowdog_client/model/work_requirement_status.py,sha256=kzD9ix66mTuYkCt2fQO9-X-23riDim7TfZP7C7p-N7g,1913
 yellowdog_client/model/work_requirement_summary.py,sha256=jEvsqI6IBykpP5_LAyoTiS5elHXfaQJ2Zj1FOwxQtMU,1374
 yellowdog_client/model/worker.py,sha256=KqUNIYwy9F-R4eY3Vk2JkZIyhERE-2CxmQe-6JgkI5Q,964
 yellowdog_client/model/worker_action.py,sha256=2OzTY1b5Q8QpVXTaGy5YzxPeMghb9AuzVxh8_J-OKHQ,453
 yellowdog_client/model/worker_pool.py,sha256=1dPTMPzXmqrlJq2PKo294Ay7OgmkZn_jO7qWVppS0Uk,255
 yellowdog_client/model/worker_pool_node_configuration.py,sha256=HaUkJIVlF-xzF931wjJnqIk5oL_71atBsgQIVqUILMo,355
 yellowdog_client/model/worker_pool_properties.py,sha256=41_GIgO1KdzwM6qmeey5dAK8yoKTsnkfrCSCzQq4QJE,84
-yellowdog_client/model/worker_pool_shutdown_condition.py,sha256=nEx_DDFZ5QkFk48IrFa2JLG0GkR7ByP-HL7qjkpGpfY,227
 yellowdog_client/model/worker_pool_status.py,sha256=NEOuZuuwlAa0h16Feh76qUtaJ_t26qO_AoHFjJBVWLc,1240
 yellowdog_client/model/worker_pool_summary.py,sha256=cMRt3QrVR9LB1C9xDwF-DRwZcnRC0AF4jeONBeKlNA4,1347
 yellowdog_client/model/worker_pool_token.py,sha256=aHJcumKO7CiyjqpUoognxCg9SRg6AOdZh01pBIAos74,350
 yellowdog_client/model/worker_status.py,sha256=onjbsuYUDiwtlxzkaCExHJZ1QR4EeB5zIlK89dyH3uU,1055
 yellowdog_client/model/worker_summary.py,sha256=PZI7Ay4i2C4UxiSKfaQpPG6t_IF0sfL4ve7uMdsiuts,819
 yellowdog_client/model/exceptions/__init__.py,sha256=JuFyrrvXegTRdsERsGLbK6ZNOIpp1kwAOdODb-G1W0s,1434
 yellowdog_client/model/exceptions/base_custom_exception.py,sha256=5WsA_nVwr8D8orn5kPjKSh9I2IJcsJcWMrpEZQUl1-4,665
@@ -396,24 +391,24 @@
 yellowdog_client/object_store/utils/memory_mapped_file_reader.py,sha256=_Fs4FDMsCiHjK8zPLF2E65rkE2LPN_OFaLTmM9og_IA,664
 yellowdog_client/object_store/utils/memory_mapped_file_reader_factory.py,sha256=mh6hD-y3bIvBx1bJvB6yc0uHJRcW2DwOT6En0Mrp0sE,265
 yellowdog_client/object_store/utils/memory_mapped_file_writer_factory.py,sha256=RmoSO4i82sxvbifTN4VG73NtZ5f-3WbntXtLWtiPGFo,303
 yellowdog_client/object_store/utils/memory_mapped_file_writter.py,sha256=a9Mr30WH4Z8Z24hY7xOhylBZD6uYQwA4hTaxCbuzj3o,1373
 yellowdog_client/scheduler/__init__.py,sha256=ZORtc_LUBoTcplpoDhCHZNannI3qjeohghNcoBYU3ts,927
 yellowdog_client/scheduler/predicated_work_subscription_event_listener.py,sha256=KaDqy98tsZLSIXisdU9F-zePD1TMlf1A8gJSYud131A,2105
 yellowdog_client/scheduler/predicated_worker_pool_subscription_event_listener.py,sha256=HpWy4wOqsDvKJMxNLuFvQZ3KN-uievx94xAZfQQ9SNo,2006
-yellowdog_client/scheduler/work_client.py,sha256=O8tSFbQ8dxHuqrUeBC3twcsLHc4WSH0_LiRu4h19cik,12226
+yellowdog_client/scheduler/work_client.py,sha256=4OZosXZkrcLyVaubCgNwSXx6MQuRTZejMEUL4KHA6ZI,12312
 yellowdog_client/scheduler/work_client_impl.py,sha256=Jt6ddC5FNXRCSwZmlGXpZkBamYqVSjBGPqvHyT6h5oE,6652
 yellowdog_client/scheduler/work_requirement_helper.py,sha256=DeGmGJS1zymzSYQ2bGhpjc6zteM_Jxzc1n8w-91pucE,4252
 yellowdog_client/scheduler/work_service_proxy.py,sha256=_sjFile_mV3BKkMaz3Ty_3vW78JeS5XgBkwDg1G3w1w,2694
-yellowdog_client/scheduler/worker_pool_client.py,sha256=ZQBegr7lc7XJ-GmEQjdwqh3-7w5JgT7nsx35mVBI_nQ,14454
+yellowdog_client/scheduler/worker_pool_client.py,sha256=llrCfZSlFBtYHHe1-ldz8GPjMhqfOmOqPsupa4Q-7TM,14596
 yellowdog_client/scheduler/worker_pool_client_impl.py,sha256=2gPs8PhN5TxAq_Z3j1Xex2t-UrBE7oMPrLw4GvFiYZg,8213
 yellowdog_client/scheduler/worker_pool_helper.py,sha256=TklGtINgDastoBglqNpuxQHnCTo65FipJNKAVkLoW3k,1263
 yellowdog_client/scheduler/worker_pool_service_proxy.py,sha256=7c9I6bktN1pQ7-fhWmh3G-tAcdBojKbcCDd8wSDJuMY,3553
 yellowdog_client/usage/__init__.py,sha256=XQwRJqTdxKZa1QUTsxBEL0TqQJeQHGyPklFeqc1GFqI,263
 yellowdog_client/usage/allowances_client.py,sha256=LFmJ3ZXoVfGZhyT20gOfrPbexu-oBWSTFxX5b11ZaPw,1301
 yellowdog_client/usage/allowances_client_impl.py,sha256=nQPnSzJKhL3WvyCn5fmiDkwE84xZryH9YvV5Z1GjU4M,2061
 yellowdog_client/usage/allowances_service_proxy.py,sha256=uO6LWnpjIzUcZTGdOxPXn7SyYX7NMRqO5KUiHUGr490,1320
-yellowdog_sdk-6.2.0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-yellowdog_sdk-6.2.0.dist-info/METADATA,sha256=EnErc6-_TBX9iiJC0y5aglsPA4MWBZyjT0DR_a10lsI,2812
-yellowdog_sdk-6.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-yellowdog_sdk-6.2.0.dist-info/top_level.txt,sha256=BN8KuscAS3tvmnghsAPsvxL7J6PVawfkuKf0zZE9Ea8,17
-yellowdog_sdk-6.2.0.dist-info/RECORD,,
+yellowdog_sdk-7.0.0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+yellowdog_sdk-7.0.0.dist-info/METADATA,sha256=VZdz8PbmWRJ84jNgbmV3sCSbeY3SLuABZ8w4KlLqmIU,2812
+yellowdog_sdk-7.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+yellowdog_sdk-7.0.0.dist-info/top_level.txt,sha256=BN8KuscAS3tvmnghsAPsvxL7J6PVawfkuKf0zZE9Ea8,17
+yellowdog_sdk-7.0.0.dist-info/RECORD,,
```

