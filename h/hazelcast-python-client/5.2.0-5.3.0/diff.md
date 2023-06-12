# Comparing `tmp/hazelcast-python-client-5.2.0.tar.gz` & `tmp/hazelcast-python-client-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazelcast-python-client-5.2.0.tar", last modified: Fri Mar 31 15:03:32 2023, max compression
+gzip compressed data, was "hazelcast-python-client-5.3.0.tar", last modified: Mon Jun 12 14:29:20 2023, max compression
```

## Comparing `hazelcast-python-client-5.2.0.tar` & `hazelcast-python-client-5.3.0.tar`

### file list

```diff
@@ -1,382 +1,382 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11358 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/LICENSE.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       47 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/MANIFEST.in
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8776 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7576 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/README.rst
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.335516 hazelcast-python-client-5.2.0/hazelcast/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      246 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16433 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/aggregator.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    22523 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/client.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    13634 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/cluster.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6168 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/compact.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    72382 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/config.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    38921 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/connection.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14181 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/core.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    17582 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/cp.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16593 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/db.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4502 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/discovery.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    15384 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/errors.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9302 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/future.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1650 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/hash.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16602 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/invocation.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3385 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/lifecycle.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11857 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/listener.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12904 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/metrics.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    10787 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/near_cache.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5420 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/partition.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    23360 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/predicate.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3225 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/projection.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.335516 hazelcast-python-client-5.2.0/hazelcast/protocol/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4297 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    25744 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/builtin.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9174 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/client_message.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.385517 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1257 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_alter_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      888 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_apply_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      910 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1341 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1168 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1084 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      835 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1223 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1819 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1677 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3002 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_authentication_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2963 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_authentication_custom_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      547 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_create_proxy_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      547 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      893 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_fetch_schema_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      401 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_ping_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      921 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      601 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      649 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_send_schema_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      895 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_statistics_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1314 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_await_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1105 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      678 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      700 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1036 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_close_session_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1429 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_create_session_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      821 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      809 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.385517 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1289 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/address_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1150 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1549 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      905 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1424 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1919 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/error_holder_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1375 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      762 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1918 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/index_config_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2704 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/member_info_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1844 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/member_version_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2940 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1627 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1044 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/schema_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4880 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1925 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2157 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/sql_error_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2434 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1729 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/executor_service_shutdown_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1168 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      994 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1553 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1475 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1644 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1478 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1397 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      972 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1157 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      833 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_with_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      963 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_contains_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_get_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      944 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_index_of_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      779 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_iterator_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_last_index_of_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      955 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_list_iterator_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_remove_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      945 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_remove_with_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      991 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1079 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_sub_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2696 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2738 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2786 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2750 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      634 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      684 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_interceptor_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3168 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      755 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_aggregate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      803 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1075 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      872 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_contains_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      849 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_delete_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1121 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      772 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      718 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_entry_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_evict_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1076 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_evict_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      785 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1067 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_on_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      910 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      833 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_flush_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      863 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_force_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      850 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_get_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1006 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1355 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_get_entry_view_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      777 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      868 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_is_locked_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      710 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1113 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      764 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      834 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_load_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1014 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_load_given_keys_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1161 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      784 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_project_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      832 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1003 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_if_absent_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1023 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_transient_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      590 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1007 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1014 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1116 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      814 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1047 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_replace_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_replace_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1023 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1046 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_set_ttl_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      773 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1552 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_try_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_try_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1230 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_try_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1027 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      710 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1113 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      764 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2512 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2554 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1117 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1077 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      720 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      865 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1019 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1163 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      746 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_put_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1020 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1554 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1029 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1073 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_value_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1842 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/pn_counter_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1487 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/pn_counter_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      777 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_add_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_contains_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      971 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      713 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_iterator_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1107 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_offer_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      702 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_peek_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      992 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_poll_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      590 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_remove_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      702 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_take_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2322 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2364 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2412 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2376 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      720 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      743 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      779 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1019 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      744 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1206 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1109 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2019 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      963 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1799 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_acquire_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1630 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_change_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1474 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_drain_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      791 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1108 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_init_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1630 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_release_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      972 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_add_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      962 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_contains_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      713 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_get_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_remove_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      537 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/sql_close_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2720 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/sql_execute_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1308 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/sql_fetch_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1763 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      683 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_publish_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      594 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_publish_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      860 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transaction_commit_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1413 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transaction_create_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      860 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transaction_rollback_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_list_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_list_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_list_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1227 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1000 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_delete_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1136 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1127 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1332 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1198 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1198 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_replace_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1323 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1040 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1132 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1127 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1169 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1169 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1132 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1223 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_take_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_set_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_set_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_set_size_codec.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/hazelcast/proxy/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3366 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8853 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/base.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/hazelcast/proxy/cp/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2777 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/cp/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12255 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/cp/atomic_long.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    13673 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/cp/atomic_reference.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7013 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/cp/count_down_latch.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    20531 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/cp/fenced_lock.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    26238 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/cp/semaphore.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6450 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/executor.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7363 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/flake_id_generator.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    22954 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/list.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    91050 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    28442 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/multi_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14045 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/pn_counter.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    19223 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/queue.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    30702 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/reliable_topic.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    20727 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/replicated_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    18381 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/ringbuffer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12795 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/set.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5301 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/topic.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2495 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_list.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16519 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5995 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_multi_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3983 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_queue.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2450 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_set.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    19104 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/reactor.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      924 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/security.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/hazelcast/serialization/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      139 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    79208 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/api.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/bits.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    85139 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/compact.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2556 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/data.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7609 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/input.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3964 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/objects.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9182 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/output.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/hazelcast/serialization/portable/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       48 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/portable/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    26041 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/portable/classdef.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6619 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/portable/context.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    24966 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/portable/reader.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4427 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/portable/serializer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    17762 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/portable/writer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1343 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/serialization_const.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    10152 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/serializer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21275 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/service.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4129 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/serialization/util.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    48167 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/sql.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14211 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/statistics.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9670 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/transaction.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      385 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/types.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11858 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/hazelcast/util.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8776 2023-03-31 15:03:32.000000 hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    18352 2023-03-31 15:03:32.000000 hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-03-31 15:03:32.000000 hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-03-31 15:03:32.000000 hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/requires.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       10 2023-03-31 15:03:32.000000 hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/top_level.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-03-31 15:03:32.395517 hazelcast-python-client-5.2.0/setup.cfg
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-03-31 15:02:04.000000 hazelcast-python-client-5.2.0/setup.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11358 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/LICENSE.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       47 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/MANIFEST.in
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8829 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7578 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/README.rst
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:19.989891 hazelcast-python-client-5.3.0/hazelcast/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      246 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16433 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/aggregator.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    22523 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/client.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    13634 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/cluster.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/compact.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    72382 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/config.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    38921 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/connection.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/core.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    17582 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/cp.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16593 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/db.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4502 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/discovery.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    15384 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/errors.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9302 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/future.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1650 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/hash.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16602 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/invocation.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3385 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/lifecycle.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11857 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/listener.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12904 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/metrics.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    10787 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/near_cache.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5420 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/partition.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    23360 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/predicate.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3225 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/projection.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:19.999891 hazelcast-python-client-5.3.0/hazelcast/protocol/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4297 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    25744 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/builtin.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9174 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/client_message.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1257 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_alter_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      888 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_apply_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      910 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1341 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1084 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      835 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1223 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1819 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1677 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2963 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_custom_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      547 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_create_proxy_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      547 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      893 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_fetch_schema_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      401 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_ping_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      921 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      601 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      649 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_schema_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      895 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_statistics_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1314 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_await_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1105 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      678 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      700 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1036 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_close_session_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1429 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_create_session_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      821 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      809 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1289 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/address_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1150 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1549 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      905 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1424 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1919 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/error_holder_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1375 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      762 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1918 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/index_config_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2704 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_info_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1844 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_version_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2940 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1627 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1044 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/schema_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4880 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1925 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2157 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_error_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2434 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1729 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_shutdown_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      994 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1553 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1475 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1644 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1478 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1397 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      972 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1157 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      833 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_with_index_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_clear_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      963 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      944 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_index_of_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      779 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_is_empty_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_iterator_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_last_index_of_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      955 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_list_iterator_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      945 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_with_index_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      991 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1079 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_sub_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2696 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2738 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2786 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2750 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      634 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_index_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      684 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_interceptor_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      755 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      803 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_clear_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1075 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      872 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_value_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      849 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_delete_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1121 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      772 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      718 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entry_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_evict_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1076 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_evict_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      785 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1067 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      910 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      833 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_flush_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      863 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_force_unlock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      850 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1006 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1355 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_entry_view_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      777 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_empty_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      868 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_locked_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      710 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1113 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      764 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      834 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1014 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_given_keys_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1161 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_lock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      784 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      832 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1003 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1023 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      590 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1007 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1014 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1116 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_if_same_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      814 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1047 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_if_same_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1023 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1046 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_ttl_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      773 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1552 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_lock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_put_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1230 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1027 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_unlock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      710 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1113 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      764 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2512 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2554 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_clear_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1117 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1077 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      720 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      865 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1019 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_key_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1163 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_lock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      746 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1020 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1554 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1029 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_unlock_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1073 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_value_count_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_values_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1842 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_add_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1487 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      777 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_clear_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      971 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_is_empty_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      713 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_iterator_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1107 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_offer_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      702 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_peek_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      992 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_poll_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      590 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_put_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      702 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_take_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2322 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2364 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2412 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2376 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_clear_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      720 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      743 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      779 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1019 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      744 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_values_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1206 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1109 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2019 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      963 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1799 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_acquire_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1630 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_change_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1474 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_drain_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      791 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1108 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_init_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1630 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_release_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      972 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_clear_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      962 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      713 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_get_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_is_empty_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      537 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_close_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2720 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_execute_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1308 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_fetch_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1763 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      683 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_all_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      594 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      860 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_commit_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1413 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_create_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      860 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_rollback_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_add_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1227 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1000 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_delete_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1136 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1127 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1332 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1198 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1198 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1323 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1040 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_set_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1132 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1127 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1169 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1169 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1132 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1223 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_size_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_take_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_add_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_remove_codec.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_size_codec.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/proxy/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3366 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8853 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/base.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2777 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12255 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_long.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    13673 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_reference.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7013 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/count_down_latch.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    20531 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/fenced_lock.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    26238 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/semaphore.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6450 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/executor.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7363 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/flake_id_generator.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    22954 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/list.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    91050 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/map.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    28442 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/multi_map.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14045 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/pn_counter.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    19223 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/queue.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    30702 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/reliable_topic.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    20727 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/replicated_map.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    18381 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/ringbuffer.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12795 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/set.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5301 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/topic.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_list.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16519 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_map.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5995 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_multi_map.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3983 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_queue.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2450 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_set.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    19104 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/reactor.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      924 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/security.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/hazelcast/serialization/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      139 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    79208 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/api.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/bits.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    85139 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/compact.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2556 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/data.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7609 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/input.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/objects.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9182 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/output.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       48 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    26041 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/classdef.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6619 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/context.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    24966 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/reader.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4427 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/serializer.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    17762 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/writer.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1343 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/serialization_const.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    10152 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/serializer.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21275 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/service.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4129 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/util.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    48167 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/sql.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14211 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/statistics.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9670 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/transaction.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      385 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/types.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11858 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/util.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8829 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    18352 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/requires.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       10 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/top_level.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/setup.cfg
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1984 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/setup.py
```

### Comparing `hazelcast-python-client-5.2.0/LICENSE.txt` & `hazelcast-python-client-5.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/PKG-INFO` & `hazelcast-python-client-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazelcast-python-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: Hazelcast Python Client
 Home-page: https://github.com/hazelcast/hazelcast-python-client
 Author: Hazelcast Inc. Developers
 Author-email: hazelcast@googlegroups.com
 License: Apache 2.0
 Keywords: hazelcast,hazelcast client,In-Memory Data Grid,Distributed Computing
 Platform: UNKNOWN
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: stats
 License-File: LICENSE.txt
 
 Hazelcast Python Client
 =======================
@@ -73,15 +74,15 @@
 
 The quickest way to start a single member cluster for development
 purposes is to use our `Docker
 images <https://hub.docker.com/r/hazelcast/hazelcast/>`__.
 
 .. code:: bash
 
-   docker run -p 5701:5701 hazelcast/hazelcast:5.2
+   docker run -p 5701:5701 hazelcast/hazelcast:5.3.0
 
 You can also use our ZIP or TAR
 `distributions <https://hazelcast.com/open-source-projects/downloads/>`__.
 Once you have downloaded, you can start the Hazelcast member using
 the ``bin/hz-start`` script.
 
 Client
```

### Comparing `hazelcast-python-client-5.2.0/README.rst` & `hazelcast-python-client-5.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 The quickest way to start a single member cluster for development
 purposes is to use our `Docker
 images <https://hub.docker.com/r/hazelcast/hazelcast/>`__.
 
 .. code:: bash
 
-   docker run -p 5701:5701 hazelcast/hazelcast:5.2
+   docker run -p 5701:5701 hazelcast/hazelcast:5.3.0
 
 You can also use our ZIP or TAR
 `distributions <https://hazelcast.com/open-source-projects/downloads/>`__.
 Once you have downloaded, you can start the Hazelcast member using
 the ``bin/hz-start`` script.
 
 Client
```

### Comparing `hazelcast-python-client-5.2.0/hazelcast/aggregator.py` & `hazelcast-python-client-5.3.0/hazelcast/aggregator.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/client.py` & `hazelcast-python-client-5.3.0/hazelcast/client.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/cluster.py` & `hazelcast-python-client-5.3.0/hazelcast/cluster.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/compact.py` & `hazelcast-python-client-5.3.0/hazelcast/compact.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/config.py` & `hazelcast-python-client-5.3.0/hazelcast/config.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/connection.py` & `hazelcast-python-client-5.3.0/hazelcast/connection.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/core.py` & `hazelcast-python-client-5.3.0/hazelcast/core.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/cp.py` & `hazelcast-python-client-5.3.0/hazelcast/cp.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/db.py` & `hazelcast-python-client-5.3.0/hazelcast/db.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/discovery.py` & `hazelcast-python-client-5.3.0/hazelcast/discovery.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/errors.py` & `hazelcast-python-client-5.3.0/hazelcast/errors.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/future.py` & `hazelcast-python-client-5.3.0/hazelcast/future.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/hash.py` & `hazelcast-python-client-5.3.0/hazelcast/hash.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/invocation.py` & `hazelcast-python-client-5.3.0/hazelcast/invocation.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/lifecycle.py` & `hazelcast-python-client-5.3.0/hazelcast/lifecycle.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/listener.py` & `hazelcast-python-client-5.3.0/hazelcast/listener.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/metrics.py` & `hazelcast-python-client-5.3.0/hazelcast/metrics.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/near_cache.py` & `hazelcast-python-client-5.3.0/hazelcast/near_cache.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/partition.py` & `hazelcast-python-client-5.3.0/hazelcast/partition.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/predicate.py` & `hazelcast-python-client-5.3.0/hazelcast/predicate.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/projection.py` & `hazelcast-python-client-5.3.0/hazelcast/projection.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/__init__.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/builtin.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/builtin.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/client_message.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/client_message.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_alter_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_alter_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_apply_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_apply_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_long_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/atomic_ref_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_authentication_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_authentication_custom_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_custom_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_create_proxy_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_create_proxy_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_fetch_schema_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_fetch_schema_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_send_schema_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_schema_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/client_statistics_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_statistics_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_await_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_await_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_close_session_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_close_session_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_create_session_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_create_session_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/address_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/address_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/error_holder_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/error_holder_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/index_config_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/index_config_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/member_info_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_info_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/member_version_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_version_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/schema_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/schema_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/sql_error_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_error_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_add_with_index_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_with_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_contains_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_contains_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_get_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_index_of_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_index_of_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_is_empty_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_iterator_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_iterator_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_last_index_of_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_last_index_of_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_list_iterator_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_list_iterator_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_remove_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_remove_with_index_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_with_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/list_sub_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_sub_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_index_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_interceptor_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_interceptor_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_aggregate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_contains_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_contains_value_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_delete_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_delete_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_entry_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entry_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_evict_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_evict_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_on_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_force_unlock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_force_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_get_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_get_entry_view_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_entry_view_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_is_empty_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_is_locked_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_locked_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_key_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_load_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_load_given_keys_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_given_keys_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_lock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_project_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_if_absent_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_transient_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_if_same_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_replace_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_replace_if_same_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_set_ttl_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_ttl_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_try_lock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_try_put_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_try_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_unlock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_values_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_key_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_lock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_put_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_put_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_unlock_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_value_count_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_value_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/multi_map_values_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/pn_counter_add_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/pn_counter_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_add_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_add_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_contains_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_contains_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_is_empty_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_iterator_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_iterator_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_offer_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_offer_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_peek_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_peek_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_poll_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_poll_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_put_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_remove_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/queue_take_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_take_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_put_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/replicated_map_values_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_add_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_acquire_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_acquire_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_change_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_change_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_drain_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_drain_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_init_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_init_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/semaphore_release_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_release_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_add_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_add_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_add_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_contains_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_contains_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_get_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_get_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_is_empty_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_remove_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/set_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/sql_close_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_close_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/sql_execute_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_execute_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/sql_fetch_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_fetch_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_publish_all_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_publish_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transaction_commit_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_commit_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transaction_create_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_create_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transaction_rollback_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_rollback_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_list_add_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_list_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_list_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_delete_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_delete_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_put_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_replace_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_set_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_values_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_queue_take_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_take_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_set_add_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_set_remove_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/protocol/codec/transactional_set_size_codec.py` & `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/__init__.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/base.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/base.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/cp/__init__.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/cp/atomic_long.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_long.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/cp/atomic_reference.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_reference.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/cp/count_down_latch.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/count_down_latch.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/cp/fenced_lock.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/fenced_lock.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/cp/semaphore.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/semaphore.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/executor.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/executor.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/flake_id_generator.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/flake_id_generator.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/list.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/list.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/map.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/multi_map.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/multi_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/pn_counter.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/pn_counter.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/queue.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/queue.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/reliable_topic.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/reliable_topic.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/replicated_map.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/replicated_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/ringbuffer.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/set.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/set.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/topic.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/topic.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_list.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_list.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_map.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_multi_map.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_multi_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_queue.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_queue.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/proxy/transactional_set.py` & `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_set.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/reactor.py` & `hazelcast-python-client-5.3.0/hazelcast/reactor.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/security.py` & `hazelcast-python-client-5.3.0/hazelcast/security.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/api.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/api.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/bits.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/bits.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/compact.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/compact.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/data.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/data.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/input.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/input.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/objects.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/objects.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/output.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/output.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/portable/classdef.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/classdef.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/portable/context.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/context.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/portable/reader.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/reader.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/portable/serializer.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/serializer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/portable/writer.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/writer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/serialization_const.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/serialization_const.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/serializer.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/service.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/service.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/serialization/util.py` & `hazelcast-python-client-5.3.0/hazelcast/serialization/util.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/sql.py` & `hazelcast-python-client-5.3.0/hazelcast/sql.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/statistics.py` & `hazelcast-python-client-5.3.0/hazelcast/statistics.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/transaction.py` & `hazelcast-python-client-5.3.0/hazelcast/transaction.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast/util.py` & `hazelcast-python-client-5.3.0/hazelcast/util.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/PKG-INFO` & `hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazelcast-python-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: Hazelcast Python Client
 Home-page: https://github.com/hazelcast/hazelcast-python-client
 Author: Hazelcast Inc. Developers
 Author-email: hazelcast@googlegroups.com
 License: Apache 2.0
 Keywords: hazelcast,hazelcast client,In-Memory Data Grid,Distributed Computing
 Platform: UNKNOWN
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: stats
 License-File: LICENSE.txt
 
 Hazelcast Python Client
 =======================
@@ -73,15 +74,15 @@
 
 The quickest way to start a single member cluster for development
 purposes is to use our `Docker
 images <https://hub.docker.com/r/hazelcast/hazelcast/>`__.
 
 .. code:: bash
 
-   docker run -p 5701:5701 hazelcast/hazelcast:5.2
+   docker run -p 5701:5701 hazelcast/hazelcast:5.3.0
 
 You can also use our ZIP or TAR
 `distributions <https://hazelcast.com/open-source-projects/downloads/>`__.
 Once you have downloaded, you can start the Hazelcast member using
 the ``bin/hz-start`` script.
 
 Client
```

### Comparing `hazelcast-python-client-5.2.0/hazelcast_python_client.egg-info/SOURCES.txt` & `hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.2.0/setup.py` & `hazelcast-python-client-5.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     license="Apache 2.0",
     keywords="hazelcast,hazelcast client,In-Memory Data Grid,Distributed Computing",
     packages=find_packages(
         exclude=["benchmarks", "examples", "examples.*", "docs", "docs.*", "tests", "tests.*"]
```

