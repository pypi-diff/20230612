# Comparing `tmp/googleapis-common-protos-1.6.0b8.tar.gz` & `tmp/googleapis-common-protos-1.6.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/googleapis-common-protos-1.6.0b8.tar", last modified: Fri Feb 22 18:21:53 2019, max compression
+gzip compressed data, was "dist/googleapis-common-protos-1.6.0b9.tar", last modified: Tue Feb 26 16:43:15 2019, max compression
```

## Comparing `googleapis-common-protos-1.6.0b8.tar` & `googleapis-common-protos-1.6.0b9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11352 2018-07-03 22:23:59.000000 googleapis-common-protos-1.6.0b8/LICENSE
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       27 2018-07-03 22:23:59.000000 googleapis-common-protos-1.6.0b8/MANIFEST.in
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1169 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/PKG-INFO
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)      275 2018-07-03 22:31:05.000000 googleapis-common-protos-1.6.0b8/README.rst
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       56 2018-07-03 22:27:00.000000 googleapis-common-protos-1.6.0b8/google/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/api/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:23.000000 googleapis-common-protos-1.6.0b8/google/api/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2080 2019-02-08 21:38:33.000000 googleapis-common-protos-1.6.0b8/google/api/annotations_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11462 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/auth_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4745 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/backend_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4341 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/billing_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6227 2019-02-13 04:02:06.000000 googleapis-common-protos-1.6.0b8/google/api/client_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6531 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/config_change_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5651 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/consumer_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4257 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/context_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2230 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/control_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    16037 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/distribution_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     8350 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/documentation_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4030 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/endpoint_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3618 2019-02-08 21:36:46.000000 googleapis-common-protos-1.6.0b8/google/api/field_behavior_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    10228 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/http_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3313 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/httpbody_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4162 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/label_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3816 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/log_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4896 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/logging_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4753 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/metadata_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11759 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/metric_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    12433 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/monitored_resource_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5059 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/monitoring_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    13136 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/quota_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     7879 2019-02-08 21:36:46.000000 googleapis-common-protos-1.6.0b8/google/api/resource_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    17859 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/service_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2553 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/source_info_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6374 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/system_parameter_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5334 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b8/google/api/usage_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/iam/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:30.000000 googleapis-common-protos-1.6.0b8/google/iam/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/iam/admin/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:37.000000 googleapis-common-protos-1.6.0b8/google/iam/admin/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/iam/v1/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:41.000000 googleapis-common-protos-1.6.0b8/google/iam/v1/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9717 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/iam/v1/iam_policy_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9233 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/iam/v1/policy_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/logging/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       56 2018-07-03 22:27:29.000000 googleapis-common-protos-1.6.0b8/google/logging/__init__.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/logging/type/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:52:16.000000 googleapis-common-protos-1.6.0b8/google/logging/type/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9056 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/logging/type/http_request_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3541 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/logging/type/log_severity_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/longrunning/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:52.000000 googleapis-common-protos-1.6.0b8/google/longrunning/__init__.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)      220 2019-02-22 17:26:13.000000 googleapis-common-protos-1.6.0b8/google/longrunning/operations_grpc.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1978 2019-02-22 18:17:43.000000 googleapis-common-protos-1.6.0b8/google/longrunning/operations_grpc_pb2.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1115 2019-02-22 18:18:17.000000 googleapis-common-protos-1.6.0b8/google/longrunning/operations_pb2.py
--rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)      221 2019-02-22 17:26:09.000000 googleapis-common-protos-1.6.0b8/google/longrunning/operations_proto.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    19093 2019-02-08 22:15:36.000000 googleapis-common-protos-1.6.0b8/google/longrunning/operations_proto_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/rpc/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:57.000000 googleapis-common-protos-1.6.0b8/google/rpc/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4612 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/rpc/code_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    22299 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/rpc/error_details_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3234 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/rpc/status_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/google/type/
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:52:02.000000 googleapis-common-protos-1.6.0b8/google/type/__init__.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3632 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/type/color_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2904 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/type/date_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2977 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/type/dayofweek_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2574 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/type/latlng_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2941 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/type/money_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6647 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/type/postal_address_pb2.py
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3403 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b8/google/type/timeofday_pb2.py
-drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)     1169 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/PKG-INFO
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)     1983 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/SOURCES.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)        1 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/dependency_links.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)       22 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/namespace_packages.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)       16 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/requires.txt
--rw-r-----   0 lukesneeringer (439724) primarygroup (89939)        7 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/top_level.txt
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       38 2019-02-22 18:21:53.000000 googleapis-common-protos-1.6.0b8/setup.cfg
--rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     1103 2019-02-22 18:18:25.000000 googleapis-common-protos-1.6.0b8/setup.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11352 2018-07-03 22:23:59.000000 googleapis-common-protos-1.6.0b9/LICENSE
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       27 2018-07-03 22:23:59.000000 googleapis-common-protos-1.6.0b9/MANIFEST.in
+-rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1190 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/PKG-INFO
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)      275 2018-07-03 22:31:05.000000 googleapis-common-protos-1.6.0b9/README.rst
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       56 2018-07-03 22:27:00.000000 googleapis-common-protos-1.6.0b9/google/__init__.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/api/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:23.000000 googleapis-common-protos-1.6.0b9/google/api/__init__.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2080 2019-02-08 21:38:33.000000 googleapis-common-protos-1.6.0b9/google/api/annotations_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11462 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/auth_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4745 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/backend_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4341 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/billing_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6227 2019-02-13 04:02:06.000000 googleapis-common-protos-1.6.0b9/google/api/client_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6531 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/config_change_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5651 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/consumer_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4257 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/context_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2230 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/control_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    16037 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/distribution_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     8350 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/documentation_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4030 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/endpoint_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3618 2019-02-08 21:36:46.000000 googleapis-common-protos-1.6.0b9/google/api/field_behavior_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    10228 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/http_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3313 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/httpbody_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4162 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/label_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3816 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/log_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4896 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/logging_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4753 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/metadata_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    11759 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/metric_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    12433 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/monitored_resource_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5059 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/monitoring_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    13136 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/quota_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     7879 2019-02-08 21:36:46.000000 googleapis-common-protos-1.6.0b9/google/api/resource_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    17859 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/service_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2553 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/source_info_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6374 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/system_parameter_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     5334 2018-09-28 22:27:23.000000 googleapis-common-protos-1.6.0b9/google/api/usage_pb2.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/iam/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:30.000000 googleapis-common-protos-1.6.0b9/google/iam/__init__.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/iam/admin/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:37.000000 googleapis-common-protos-1.6.0b9/google/iam/admin/__init__.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:41.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/__init__.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9717 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/iam_policy_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9233 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/iam/v1/policy_pb2.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/logging/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       56 2018-07-03 22:27:29.000000 googleapis-common-protos-1.6.0b9/google/logging/__init__.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/logging/type/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:52:16.000000 googleapis-common-protos-1.6.0b9/google/logging/type/__init__.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     9056 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/logging/type/http_request_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3541 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/logging/type/log_severity_pb2.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/longrunning/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:52.000000 googleapis-common-protos-1.6.0b9/google/longrunning/__init__.py
+-rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)      220 2019-02-22 17:26:13.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_grpc.py
+-rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1978 2019-02-22 18:17:43.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_grpc_pb2.py
+-rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)     1115 2019-02-22 18:18:17.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_pb2.py
+-rw-r--r--   0 lukesneeringer (439724) primarygroup (89939)      221 2019-02-22 17:26:09.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_proto.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    19093 2019-02-08 22:15:36.000000 googleapis-common-protos-1.6.0b9/google/longrunning/operations_proto_pb2.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/rpc/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:51:57.000000 googleapis-common-protos-1.6.0b9/google/rpc/__init__.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     4612 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/rpc/code_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)    22299 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/rpc/error_details_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3234 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/rpc/status_pb2.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/google/type/
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)        0 2018-07-04 17:52:02.000000 googleapis-common-protos-1.6.0b9/google/type/__init__.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3632 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/color_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2904 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/date_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2977 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/dayofweek_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2574 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/latlng_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     2941 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/money_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     6647 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/postal_address_pb2.py
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     3403 2018-07-03 22:18:16.000000 googleapis-common-protos-1.6.0b9/google/type/timeofday_pb2.py
+drwxr-xr-x   0 lukesneeringer (439724) primarygroup (89939)        0 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/
+-rw-r-----   0 lukesneeringer (439724) primarygroup (89939)     1190 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/PKG-INFO
+-rw-r-----   0 lukesneeringer (439724) primarygroup (89939)     1983 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/SOURCES.txt
+-rw-r-----   0 lukesneeringer (439724) primarygroup (89939)        1 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/dependency_links.txt
+-rw-r-----   0 lukesneeringer (439724) primarygroup (89939)       22 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/namespace_packages.txt
+-rw-r-----   0 lukesneeringer (439724) primarygroup (89939)       38 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/requires.txt
+-rw-r-----   0 lukesneeringer (439724) primarygroup (89939)        7 2019-02-26 16:43:14.000000 googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/top_level.txt
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)       38 2019-02-26 16:43:15.000000 googleapis-common-protos-1.6.0b9/setup.cfg
+-rw-rw-r--   0 lukesneeringer (439724) primarygroup (89939)     1191 2019-02-26 16:42:30.000000 googleapis-common-protos-1.6.0b9/setup.py
```

### Comparing `googleapis-common-protos-1.6.0b8/LICENSE` & `googleapis-common-protos-1.6.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/PKG-INFO` & `googleapis-common-protos-1.6.0b9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: googleapis-common-protos
-Version: 1.6.0b8
+Version: 1.6.0b9
 Summary: Common protobufs used in Google APIs
 Home-page: https://github.com/googleapis/api-common-protos
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache-2.0
 Description: =========================
         Google APIs common protos
@@ -23,7 +23,8 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: grpc
```

### Comparing `googleapis-common-protos-1.6.0b8/google/api/annotations_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/auth_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/backend_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/backend_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/billing_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/client_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/config_change_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/config_change_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/consumer_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/consumer_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/context_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/context_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/control_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/control_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/distribution_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/documentation_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/documentation_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/endpoint_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/field_behavior_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/http_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/httpbody_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/label_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/label_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/log_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/log_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/logging_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/logging_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/metadata_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/metric_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/monitored_resource_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/monitored_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/monitoring_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/quota_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/resource_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/service_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/service_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/source_info_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/source_info_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/system_parameter_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/system_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/api/usage_pb2.py` & `googleapis-common-protos-1.6.0b9/google/api/usage_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/iam/v1/iam_policy_pb2.py` & `googleapis-common-protos-1.6.0b9/google/iam/v1/iam_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/iam/v1/policy_pb2.py` & `googleapis-common-protos-1.6.0b9/google/iam/v1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/logging/type/http_request_pb2.py` & `googleapis-common-protos-1.6.0b9/google/logging/type/http_request_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/logging/type/log_severity_pb2.py` & `googleapis-common-protos-1.6.0b9/google/logging/type/log_severity_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/longrunning/operations_grpc_pb2.py` & `googleapis-common-protos-1.6.0b9/google/longrunning/operations_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/longrunning/operations_pb2.py` & `googleapis-common-protos-1.6.0b9/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/longrunning/operations_proto_pb2.py` & `googleapis-common-protos-1.6.0b9/google/longrunning/operations_proto_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/rpc/code_pb2.py` & `googleapis-common-protos-1.6.0b9/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/rpc/error_details_pb2.py` & `googleapis-common-protos-1.6.0b9/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/rpc/status_pb2.py` & `googleapis-common-protos-1.6.0b9/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/type/color_pb2.py` & `googleapis-common-protos-1.6.0b9/google/type/color_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/type/date_pb2.py` & `googleapis-common-protos-1.6.0b9/google/type/date_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/type/dayofweek_pb2.py` & `googleapis-common-protos-1.6.0b9/google/type/dayofweek_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/type/latlng_pb2.py` & `googleapis-common-protos-1.6.0b9/google/type/latlng_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/type/money_pb2.py` & `googleapis-common-protos-1.6.0b9/google/type/money_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/type/postal_address_pb2.py` & `googleapis-common-protos-1.6.0b9/google/type/postal_address_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/google/type/timeofday_pb2.py` & `googleapis-common-protos-1.6.0b9/google/type/timeofday_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/PKG-INFO` & `googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: googleapis-common-protos
-Version: 1.6.0b8
+Version: 1.6.0b9
 Summary: Common protobufs used in Google APIs
 Home-page: https://github.com/googleapis/api-common-protos
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache-2.0
 Description: =========================
         Google APIs common protos
@@ -23,7 +23,8 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: grpc
```

### Comparing `googleapis-common-protos-1.6.0b8/googleapis_common_protos.egg-info/SOURCES.txt` & `googleapis-common-protos-1.6.0b9/googleapis_common_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.6.0b8/setup.py` & `googleapis-common-protos-1.6.0b9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from setuptools import setup, find_packages
 
 install_requires = [
-    'protobuf >= 3.0.0',
+    'protobuf >= 3.6.0',
 ]
 
+extras_require = {
+  'grpc': ['grpcio >= 1.0.0']
+}
+
+
 setup(
     name='googleapis-common-protos',
-    version='1.6.0b8',
+    version='1.6.0b9',
     author='Google LLC',
     author_email='googleapis-packages@google.com',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
@@ -21,12 +26,13 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     description='Common protobufs used in Google APIs',
     long_description=open('README.rst').read(),
     install_requires=install_requires,
+    extras_require=extras_require,
     license='Apache-2.0',
     packages=find_packages(),
     namespace_packages=['google', 'google.logging'],
     url='https://github.com/googleapis/api-common-protos',
 )
```

