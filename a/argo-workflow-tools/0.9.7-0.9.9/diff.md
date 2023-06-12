# Comparing `tmp/argo-workflow-tools-0.9.7.tar.gz` & `tmp/argo-workflow-tools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argo-workflow-tools-0.9.7.tar", max compression
+gzip compressed data, was "argo-workflow-tools-0.9.9.tar", max compression
```

## Comparing `argo-workflow-tools-0.9.7.tar` & `argo-workflow-tools-0.9.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    10735 2021-10-24 05:23:52.502078 argo-workflow-tools-0.9.7/LICENSE
--rw-r--r--   0        0        0     6566 2021-12-08 05:01:53.765166 argo-workflow-tools-0.9.7/README.md
--rw-r--r--   0        0        0      389 2021-12-12 13:43:01.108482 argo-workflow-tools-0.9.7/argo_workflow_tools/__init__.py
--rw-r--r--   0        0        0     6296 2021-12-03 11:51:05.423853 argo-workflow-tools-0.9.7/argo_workflow_tools/argo_client.py
--rw-r--r--   0        0        0     5025 2021-12-03 11:49:51.352259 argo-workflow-tools-0.9.7/argo_workflow_tools/argo_http_client.py
--rw-r--r--   0        0        0     1013 2021-10-27 06:07:42.612716 argo-workflow-tools-0.9.7/argo_workflow_tools/argo_options.py
--rw-r--r--   0        0        0       76 2021-10-27 04:52:58.757304 argo-workflow-tools-0.9.7/argo_workflow_tools/artifact.py
--rw-r--r--   0        0        0      139 2021-12-12 16:41:48.933555 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/__init__.py
--rw-r--r--   0        0        0      308 2021-11-27 19:49:08.437000 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/building_mode_context.py
--rw-r--r--   0        0        0     2534 2021-12-07 08:07:33.739199 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/condition.py
--rw-r--r--   0        0        0    14512 2021-12-13 05:25:56.443588 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/dag_compiler.py
--rw-r--r--   0        0        0     1271 2021-12-12 16:41:49.084606 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/dag_task.py
--rw-r--r--   0        0        0     4137 2021-12-12 16:41:49.412649 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/dsl_decorators.py
--rw-r--r--   0        0        0     4622 2021-12-12 16:48:03.458767 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/input_definition.py
--rw-r--r--   0        0        0    14617 2021-12-12 20:56:18.240759 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/node.py
--rw-r--r--   0        0        0      200 2021-12-03 11:51:05.432239 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/node_properties/__init__.py
--rw-r--r--   0        0        0      539 2021-12-12 16:41:49.245025 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/node_properties/dag_node_properties.py
--rw-r--r--   0        0        0      969 2021-12-12 16:41:49.305931 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/node_properties/task_node_properties.py
--rw-r--r--   0        0        0      127 2021-12-08 05:01:53.783995 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/parameter_builders/__init__.py
--rw-r--r--   0        0        0     1900 2021-12-12 15:37:03.270485 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/parameter_builders/default_parameter_builder.py
--rw-r--r--   0        0        0     1138 2021-12-12 16:41:49.358038 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/parameter_builders/multiple_output_parameter_builder.py
--rw-r--r--   0        0        0      621 2021-12-12 16:41:49.356381 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/parameter_builders/parameter_builder.py
--rw-r--r--   0        0        0        0 2021-11-22 18:46:35.813000 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/utils/__init__.py
--rw-r--r--   0        0        0      511 2021-11-28 06:19:49.969000 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/utils/path_builder.py
--rw-r--r--   0        0        0     2587 2021-12-12 20:56:18.027288 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/utils/utils.py
--rw-r--r--   0        0        0     6014 2021-12-12 15:40:06.001080 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/workflow.py
--rw-r--r--   0        0        0     1764 2021-12-12 15:47:29.500470 argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/workflow_template_collector.py
--rw-r--r--   0        0        0        0 2021-10-24 04:32:28.529447 argo-workflow-tools-0.9.7/argo_workflow_tools/exceptions/__init__.py
--rw-r--r--   0        0        0       53 2021-10-27 05:06:34.842818 argo-workflow-tools-0.9.7/argo_workflow_tools/exceptions/workflow_not_found_exception.py
--rw-r--r--   0        0        0      321 2021-11-13 19:15:49.242000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/__init__.py
--rw-r--r--   0        0        0     1454 2021-12-02 17:49:18.140000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/eventsource.py
--rw-r--r--   0        0        0        0 2021-11-15 06:04:48.649000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/__init__.py
--rw-r--r--   0        0        0        0 2021-11-15 06:04:48.673000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      185 2021-11-13 19:15:49.247000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0    86595 2021-11-28 05:19:41.849000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0      185 2021-11-13 19:15:49.248000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   133917 2021-11-28 05:19:42.358000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0        0 2021-11-15 06:04:48.643000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2021-11-15 06:04:48.636000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      185 2021-11-13 19:15:49.249000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   101063 2021-11-27 19:45:16.591000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0      185 2021-11-13 19:15:49.250000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1385 2021-11-28 05:19:40.246000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0        0 2021-11-15 06:04:48.663000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2021-11-15 06:04:48.658000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      185 2021-11-13 19:15:49.252000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     2784 2021-11-13 19:15:49.252000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0        0 2021-11-15 06:04:48.668000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      185 2021-11-13 19:15:49.253000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    20609 2021-11-28 05:19:40.503000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0      185 2021-11-13 19:15:49.254000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      303 2021-11-13 19:15:49.255000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0     1500 2021-11-28 05:19:40.319000 argo-workflow-tools-0.9.7/argo_workflow_tools/models/sensor.py
--rw-r--r--   0        0        0     1040 2021-10-27 05:14:00.630311 argo-workflow-tools-0.9.7/argo_workflow_tools/terminal_loading_animation.py
--rw-r--r--   0        0        0     2612 2021-12-03 11:49:51.372785 argo-workflow-tools-0.9.7/argo_workflow_tools/workflow_result.py
--rw-r--r--   0        0        0      418 2021-10-27 05:56:03.533602 argo-workflow-tools-0.9.7/argo_workflow_tools/workflow_status.py
--rw-r--r--   0        0        0     2535 2021-12-03 11:50:19.454584 argo-workflow-tools-0.9.7/argo_workflow_tools/workflow_status_checker.py
--rw-r--r--   0        0        0      969 2021-12-13 06:39:24.932123 argo-workflow-tools-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     8621 2021-12-13 06:39:42.536974 argo-workflow-tools-0.9.7/setup.py
--rw-r--r--   0        0        0     7490 2021-12-13 06:39:42.538040 argo-workflow-tools-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0    10735 2021-10-24 05:23:52.502078 argo-workflow-tools-0.9.9/LICENSE
+-rw-r--r--   0        0        0     6566 2021-12-08 05:01:53.765166 argo-workflow-tools-0.9.9/README.md
+-rw-r--r--   0        0        0      389 2021-12-12 13:43:01.108482 argo-workflow-tools-0.9.9/argo_workflow_tools/__init__.py
+-rw-r--r--   0        0        0     6296 2021-12-03 11:51:05.423853 argo-workflow-tools-0.9.9/argo_workflow_tools/argo_client.py
+-rw-r--r--   0        0        0     5025 2021-12-03 11:49:51.352259 argo-workflow-tools-0.9.9/argo_workflow_tools/argo_http_client.py
+-rw-r--r--   0        0        0     1013 2021-10-27 06:07:42.612716 argo-workflow-tools-0.9.9/argo_workflow_tools/argo_options.py
+-rw-r--r--   0        0        0       76 2021-10-27 04:52:58.757304 argo-workflow-tools-0.9.9/argo_workflow_tools/artifact.py
+-rw-r--r--   0        0        0      139 2021-12-12 16:41:48.933555 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/__init__.py
+-rw-r--r--   0        0        0      308 2021-11-27 19:49:08.437000 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/building_mode_context.py
+-rw-r--r--   0        0        0     2534 2021-12-07 08:07:33.739199 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/condition.py
+-rw-r--r--   0        0        0    14667 2021-12-13 13:38:14.621760 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/dag_compiler.py
+-rw-r--r--   0        0        0     1271 2021-12-12 16:41:49.084606 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/dag_task.py
+-rw-r--r--   0        0        0     4137 2021-12-12 16:41:49.412649 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/dsl_decorators.py
+-rw-r--r--   0        0        0     4622 2021-12-12 16:48:03.458767 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/input_definition.py
+-rw-r--r--   0        0        0    14729 2021-12-13 13:38:14.572278 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/node.py
+-rw-r--r--   0        0        0      200 2021-12-03 11:51:05.432239 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/node_properties/__init__.py
+-rw-r--r--   0        0        0      539 2021-12-12 16:41:49.245025 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/node_properties/dag_node_properties.py
+-rw-r--r--   0        0        0      969 2021-12-12 16:41:49.305931 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/node_properties/task_node_properties.py
+-rw-r--r--   0        0        0      127 2021-12-08 05:01:53.783995 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/parameter_builders/__init__.py
+-rw-r--r--   0        0        0     1900 2021-12-12 15:37:03.270485 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/parameter_builders/default_parameter_builder.py
+-rw-r--r--   0        0        0     1138 2021-12-12 16:41:49.358038 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/parameter_builders/multiple_output_parameter_builder.py
+-rw-r--r--   0        0        0      621 2021-12-12 16:41:49.356381 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/parameter_builders/parameter_builder.py
+-rw-r--r--   0        0        0        0 2021-11-22 18:46:35.813000 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/utils/__init__.py
+-rw-r--r--   0        0        0      511 2021-11-28 06:19:49.969000 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/utils/path_builder.py
+-rw-r--r--   0        0        0     2677 2021-12-13 13:38:14.595502 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/utils/utils.py
+-rw-r--r--   0        0        0     6014 2021-12-12 15:40:06.001080 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/workflow.py
+-rw-r--r--   0        0        0     1764 2021-12-12 15:47:29.500470 argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/workflow_template_collector.py
+-rw-r--r--   0        0        0        0 2021-10-24 04:32:28.529447 argo-workflow-tools-0.9.9/argo_workflow_tools/exceptions/__init__.py
+-rw-r--r--   0        0        0       53 2021-10-27 05:06:34.842818 argo-workflow-tools-0.9.9/argo_workflow_tools/exceptions/workflow_not_found_exception.py
+-rw-r--r--   0        0        0      321 2021-11-13 19:15:49.242000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/__init__.py
+-rw-r--r--   0        0        0     1454 2021-12-02 17:49:18.140000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/eventsource.py
+-rw-r--r--   0        0        0        0 2021-11-15 06:04:48.649000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-15 06:04:48.673000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      185 2021-11-13 19:15:49.247000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0    86595 2021-11-28 05:19:41.849000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0      185 2021-11-13 19:15:49.248000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   133917 2021-11-28 05:19:42.358000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0        0 2021-11-15 06:04:48.643000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-15 06:04:48.636000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      185 2021-11-13 19:15:49.249000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   101063 2021-11-27 19:45:16.591000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0      185 2021-11-13 19:15:49.250000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1385 2021-11-28 05:19:40.246000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0        0 2021-11-15 06:04:48.663000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-15 06:04:48.658000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      185 2021-11-13 19:15:49.252000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     2784 2021-11-13 19:15:49.252000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0        0 2021-11-15 06:04:48.668000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      185 2021-11-13 19:15:49.253000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    20609 2021-11-28 05:19:40.503000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0      185 2021-11-13 19:15:49.254000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      303 2021-11-13 19:15:49.255000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0     1500 2021-11-28 05:19:40.319000 argo-workflow-tools-0.9.9/argo_workflow_tools/models/sensor.py
+-rw-r--r--   0        0        0     1040 2021-10-27 05:14:00.630311 argo-workflow-tools-0.9.9/argo_workflow_tools/terminal_loading_animation.py
+-rw-r--r--   0        0        0     2612 2021-12-03 11:49:51.372785 argo-workflow-tools-0.9.9/argo_workflow_tools/workflow_result.py
+-rw-r--r--   0        0        0      418 2021-10-27 05:56:03.533602 argo-workflow-tools-0.9.9/argo_workflow_tools/workflow_status.py
+-rw-r--r--   0        0        0     2535 2021-12-03 11:50:19.454584 argo-workflow-tools-0.9.9/argo_workflow_tools/workflow_status_checker.py
+-rw-r--r--   0        0        0      967 2021-12-13 13:39:14.667021 argo-workflow-tools-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     8619 2021-12-13 13:39:23.290978 argo-workflow-tools-0.9.9/setup.py
+-rw-r--r--   0        0        0     7488 2021-12-13 13:39:23.291789 argo-workflow-tools-0.9.9/PKG-INFO
```

### Comparing `argo-workflow-tools-0.9.7/LICENSE` & `argo-workflow-tools-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/README.md` & `argo-workflow-tools-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/argo_client.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/argo_client.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/argo_http_client.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/argo_http_client.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/argo_options.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/argo_options.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/condition.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/condition.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/dag_compiler.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/dag_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,19 +141,21 @@
     ):
         duplicate_nodes = list(group)
 
         if len(duplicate_nodes) == 1:
             node_names_by_id[duplicate_nodes[0].id] = name
         else:
             for i in range(0, len(duplicate_nodes)):
-                node_names_by_id[duplicate_nodes[i].id] = f"{name}-{i+1}"
+                node_names_by_id[duplicate_nodes[i].id] = f"{name}-{i + 1}"
     return node_names_by_id
 
 
-def _build_with(params: List[InputDefinition],unique_node_names_map: Dict[str, str]) -> Optional[str]:
+def _build_with(
+    params: List[InputDefinition], unique_node_names_map: Dict[str, str]
+) -> Optional[str]:
     """
     builds "with" param for loop DAGs by analyzing the inputs and looking iterable inputs.
     Parameters
     ----------
     params : list of inputs
 
     Returns
@@ -183,20 +185,22 @@
         filter(
             lambda dependency: dependency,
             [
                 input_dep.source_node_id
                 for input_dep in filter(
                     lambda x: isinstance(x, InputDefinition)
                     and not x.source_type == SourceType.PARAMETER,
-                    list(dag_task.arguments.values()) + dag_task.wait_for,
+                    list(dag_task.arguments.values()) + list()
+                    if dag_task.wait_for is None
+                    else dag_task.wait_for,
                 )
             ],
         )
     )
-    with_param = _build_with(dag_task.arguments.values(),unique_node_names_map)
+    with_param = _build_with(dag_task.arguments.values(), unique_node_names_map)
     arguments = [
         _build_node_input(input_name, input_type)
         for input_name, input_type in dag_task.arguments.items()
     ]
 
     if isinstance(dag_task, DAGReference):
         dag = _build_dag_template(dag_task.node)
@@ -234,24 +238,24 @@
         )
         return task
     else:
         raise AssertionError("only DAG or task nodes are supported")
 
 
 def _build_node_input(input_name: str, input_def: InputDefinition) -> argo.Parameter:
-    return argo.Parameter(name=sanitize_name(input_name), value=input_def.path())
+    return argo.Parameter(name=sanitize_name(input_name,snake_case=True), value=input_def.path())
 
 
 def _build_input_parameter(parameter: InputDefinition) -> argo.Parameter:
     """
     Builds Argo Parameter out of InputDefinition
     """
     if parameter.source_type == SourceType.PARAMETER:
         argo_parameter = argo.Parameter(
-            name=sanitize_name(parameter.name), default=parameter.default
+            name=sanitize_name(parameter.name,snake_case=True), default=parameter.default
         )
         return argo_parameter
     else:
         argo_parameter = argo.Parameter(
             name=parameter.name, value=parameter.path(), default=parameter.default
         )
         return argo_parameter
@@ -302,15 +306,15 @@
     -------
     Argo Script Template
 
     """
     parameters = {
         param_name: InputDefinition(
             source_type=SourceType.PARAMETER,
-            name=sanitize_name(param_name),
+            name=sanitize_name(param_name,snake_case=True),
             default=None
             if isinstance(param_definition.default, type)
             and param_definition.default.__name__ == "_empty"
             else param_definition.default,
         )
         for param_name, param_definition in inspect.signature(
             task_node.func
@@ -363,15 +367,15 @@
     -------
     Argo DAG Template
 
     """
     parameters = {
         param_name: InputDefinition(
             source_type=SourceType.PARAMETER,
-            name=sanitize_name(param_name),
+            name=sanitize_name(param_name,snake_case=True),
             default=None
             if isinstance(param_definition.default, type)
             and param_definition.default.__name__ == "_empty"
             else param_definition.default,
         )
         for param_name, param_definition in inspect.signature(
             node.func
```

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/dag_task.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/dag_task.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/dsl_decorators.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/dsl_decorators.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/input_definition.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/input_definition.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/node.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             and len(arg) == 1
             and isinstance(arg[0], InputDefinition)
             and arg[0].is_node_output
             and arg[0].reference
         ):
             return InputDefinition(
                 SourceType.REDUCE,
-                name=sanitize_name(arg[0].name),
+                name=sanitize_name(arg[0].name,snake_case=True),
                 source_node_id=arg[0].source_node_id,
                 references=arg[0],
             )
 
         if (
             not isinstance(arg, str)
             and isinstance(arg, Sequence)
@@ -210,27 +210,27 @@
             )
 
         if len(self.properties.outputs.items()) == 0:
             outputs = {
                 "result": InputDefinition(
                     source_type=SourceType.NODE_OUTPUT,
                     source_node_id=guid,
-                    name=sanitize_name("result"),
+                    name=sanitize_name("result",snake_case=True),
                     references=partitioned_arguments,
                     parameter_builder=self.properties.outputs.get(
                         "result", DefaultParameterBuilder(None)
                     ),
                 )
             }
         else:
             outputs = {
                 name: InputDefinition(
                     source_type=SourceType.NODE_OUTPUT,
                     source_node_id=guid,
-                    name=sanitize_name(name),
+                    name=sanitize_name(name,snake_case=True),
                     references=partitioned_arguments,
                     parameter_builder=parameter_builder,
                 )
                 for name, parameter_builder in self.properties.outputs.items()
             }
 
         conditions = collect_conditions()
@@ -296,27 +296,27 @@
             condition.condition_string() for condition in collect_conditions()
         ]
         if len(self.properties.outputs.items()) == 0:
             outputs = {
                 "result": InputDefinition(
                     source_type=SourceType.NODE_OUTPUT,
                     source_node_id=guid,
-                    name=sanitize_name("result"),
+                    name=sanitize_name("result",snake_case=True),
                     references=partitioned_arguments,
                     parameter_builder=self.properties.outputs.get(
                         "result", DefaultParameterBuilder(None)
                     ),
                 )
             }
         else:
             outputs = {
                 name: InputDefinition(
                     source_type=SourceType.NODE_OUTPUT,
                     source_node_id=guid,
-                    name=sanitize_name(name),
+                    name=sanitize_name(name,snake_case=True),
                     references=partitioned_arguments,
                     parameter_builder=parameter_builder,
                 )
                 for name, parameter_builder in self.properties.outputs.items()
             }
 
         add_task(
@@ -379,27 +379,27 @@
             )
 
         if len(self.properties.outputs.items()) == 0:
             outputs = {
                 "result": InputDefinition(
                     source_type=SourceType.NODE_OUTPUT,
                     source_node_id=guid,
-                    name=sanitize_name("result"),
+                    name=sanitize_name("result",snake_case=True),
                     references=partitioned_arguments,
                     parameter_builder=self.properties.outputs.get(
                         "result", DefaultParameterBuilder(None)
                     ),
                 )
             }
         else:
             outputs = {
                 name: InputDefinition(
                     source_type=SourceType.NODE_OUTPUT,
                     source_node_id=guid,
-                    name=sanitize_name(name),
+                    name=sanitize_name(name,snake_case=True),
                     references=partitioned_arguments,
                     parameter_builder=parameter_builder,
                 )
                 for name, parameter_builder in self.properties.outputs.items()
             }
 
         conditions = collect_conditions()
```

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/node_properties/dag_node_properties.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/node_properties/dag_node_properties.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/node_properties/task_node_properties.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/node_properties/task_node_properties.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/parameter_builders/default_parameter_builder.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/parameter_builders/default_parameter_builder.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/parameter_builders/multiple_output_parameter_builder.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/parameter_builders/multiple_output_parameter_builder.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/parameter_builders/parameter_builder.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/parameter_builders/parameter_builder.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/utils/utils.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def _convert_params(
     args: Union[Dict[str, str], List[Union[argo.Arguments, argo.Parameter]]]
 ) -> Tuple[List[argo.Artifact], List[argo.Parameter]]:
     if isinstance(args, dict):
         parameters = [
-            argo.Parameter(name=sanitize_name(key), value=value)
+            argo.Parameter(name=sanitize_name(key,snake_case=True), value=value)
             for key, value in args.items()
         ]
         artifacts = []
         return parameters, artifacts
 
     if isinstance(args, list):
         parameters = list(filter(lambda arg: isinstance(arg, argo.Parameter), args))
@@ -63,17 +63,19 @@
 def get_outputs(
     args: Union[Dict[str, str], List[Union[argo.Arguments, argo.Parameter]]]
 ) -> argo.Outputs:
     parameters, artifacts = _convert_params(args)
     return argo.Outputs(parameters=parameters, artifacts=artifacts)
 
 
-def sanitize_name(name: str) -> str:
+def sanitize_name(name: str,snake_case=False) -> str:
     if name is None:
         return None
+    if snake_case:
+        return name.replace("-", "_")
     return name.replace("_", "-")
 
 
 def convert_str(value: any) -> str:
     if value is None:
         return None
     if isinstance(value, bool):
```

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/workflow.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/workflow.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/dsl/workflow_template_collector.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/dsl/workflow_template_collector.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/eventsource.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/argoproj/events/v1alpha1.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/argoproj/workflow/v1alpha1.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/api/core/v1.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/api/policy/v1beta1.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/api/resource.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/models/sensor.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/models/sensor.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/terminal_loading_animation.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/terminal_loading_animation.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/workflow_result.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/workflow_result.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/argo_workflow_tools/workflow_status_checker.py` & `argo-workflow-tools-0.9.9/argo_workflow_tools/workflow_status_checker.py`

 * *Files identical despite different names*

### Comparing `argo-workflow-tools-0.9.7/pyproject.toml` & `argo-workflow-tools-0.9.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "argo-workflow-tools"
-version = "0.9.7"
+version = "0.9.9"
 description = "A suite of tools to ease ML pipeline development with Argo Workflows"
 authors = ["Diagnostic Robotics"]
 license = "Apache 2.0"
 repository = "https://github.com/DiagnosticRobotics/argo-workflow-tools"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 PyYAML = ">=5.0"
 pydantic = "^1.7.4"
 contextvars = "^2.4"
 shortuuid = "^1.0.8"
-urllib3 = "<=1.26.0"
+urllib3 = "<2.0.0"
 certifi = "<=2021.10.8"
 requests = "^2.26.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 black = "^21.11b"
 isort = "^5.7.0"
```

### Comparing `argo-workflow-tools-0.9.7/setup.py` & `argo-workflow-tools-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 install_requires = \
 ['PyYAML>=5.0',
  'certifi<=2021.10.8',
  'contextvars>=2.4,<3.0',
  'pydantic>=1.7.4,<2.0.0',
  'requests>=2.26.0,<3.0.0',
  'shortuuid>=1.0.8,<2.0.0',
- 'urllib3<=1.26.0']
+ 'urllib3<2.0.0']
 
 setup_kwargs = {
     'name': 'argo-workflow-tools',
-    'version': '0.9.7',
+    'version': '0.9.9',
     'description': 'A suite of tools to ease ML pipeline development with Argo Workflows',
     'long_description': '# Argo Workflow Tools\nargo-workflow-tools is a set of tools intended to easue the usage of argo for data science and data engineerign workflows\n![Python Versions Supported](https://img.shields.io/badge/python-3.7+-blue.svg)\n\n## Installation\nargo-workflow-tools is published to the Python Package Index (PyPI) under the name argo-workflow-tools. To install it, run:\n\n``` shell\npip install argo-workflow-tools\n```\n\n## Argo Submitter\nArgo Submitter is an easy to use argo client that allows data scientists to easily execute and control Argo Workflows from code and interactive notebooks.\n\n### Quick Start\n\n#### Running workflows from templates\nThe simplest way to submit a new workflow is by running a workflow from template \n```python\nARGO_CLIENT = \'http://localhost:2746\'\nclient = ArgoClient(ARGO_CLIENT, options=ArgoOptions(client_side_validation=False, namespace=\'argo\'))\nresult = client.submit(\'test-workflow\', params={\'message\':\'hello world\'})\nresult.wait_for_completion()\n```\n\nYou can wait for template completion by setting _wait=True_ parameter, or calling wait_for_completion()\n```python\nresult = client.submit(\'test-workflow\', params={\'message\':\'hello world\'}, wait=True)\n```\n\nYou may send parameters, through the params dictionary\n```python\nresult = client.submit(\'test-workflow\', params={\'message\':\'hello world\'}, wait=True)\n```\n\nYou send objects as parameters, and they will be automatically serialized to json. \n```python\nARGO_CLIENT = \'http://localhost:2746\'\nclient = ArgoClient(ARGO_CLIENT, options=ArgoOptions(client_side_validation=False, namespace=\'argo\'))\nresult = client.submit(\'test-workflow\',\n                                     params={\'name\':\n                                                {\'first\':\'Lorne\',\'last\':\'Malvo\'}\n                                             },\n                                     wait=True)\n```\n#### Running workflows from specification\nif you have a custom workflow manifest , you can run it by using _create_\n```python\nresult = client.create(workflow_manifest, wait=True)\n```\n#### Working with workflow results\nYou can check the status of a workflow by calling the status field\n```python\nresult.status\n```\n\nYou can fetch output parametes and artifacts throut the output field\n```python\nprint(result.outputs[\'message\'])\n```\nAs well as reach artifacts through the s3 path property\n```python\npandas.read_csv(result.outputs[\'users\'].s3)\n```\n#### Controlling workflows\nYou may cancel a running flow through the cancel method\n```python\nresult.cancel()\n```\nYou may ssuspend, resume or cancel your workflow at any time \n```python\nresult = client.submit(\'test-workflow\', params={\'message\':\'hello world\'}, wait=False)\nresult.suspend()\n...\nresult.resume()\n```\nYou can retry a failing workflow through the retry method\n```python\nresult.retry()\n```\n\n## Pythonic workflow DSL\n\nFargo is a library for autoring Argo Workflows in a Python and friendly way. The main goal of Hera are\n* Make Argo Workflows accessible by leveraging pythonic style of dag\n* Allow seamlless local runs, for debug or testing while maintaining the same codebase for running DAG\'s at scale\n\npythonic DSL is an opinionate subset of writing Argo workflows, it favors simplicity, readability and "pythonic flow" over leveraging the entire capability set Argo Workflows brings. \n\n### Concepts\n* task - atomic python code\n* DAG - atonic workflows code\n\n### Quick start\n\n####Hello World\n```python\n\ndef say_hello(name):\n    message = f"hello {name}"\n    print(message)\n    return message\n\nsay_hello("Brian")\n\n```\nto run this simple task in argo all we need to do is to decorate our code in a task decorator\n\n```python\n@dsl.Task(image="python3:3.10")\ndef say_hello(name:str):\n    message = f"hello {name}"\n    print(message)\n    return message\n\n\nworkflow = Workflow(name="hello-world", entrypoint=say_hello, arguments={"name": "Brian"})\nprint(workflow.to_yaml())\n\n```\n#### DAG\nDAG functions are functions that define a workflow by calling other tasks or nested DAGs, \nWe support task depndency declaration implicitly by analyzing inputs and outputs of each task. \n\nWhen writing DAG functions make sure you keep it a simple as possible, call only DAG or TASK flows.\n\n```python\n@dsl.Task(image="python:3.10")\ndef multiply_task(x: int):\n    return x * 2\n\n\n@dsl.Task(image="python:3.10")\ndef sum_task(x: int, y: int):\n    return x + y\n\n\n@dsl.DAG()\ndef diamond(num: int):\n    a = multiply_task(num)\n    b = multiply_task(a)\n    c = multiply_task(num)\n    return sum_task(b, c)\n\n ```\n\n#### Explicit depndencies \nIn case a task does not return a parameter, you can set an explicit dependency by sending wait_for argument to the next task\n```python\n@dsl.Task(image="python:3.10")\ndef print_task():\n    print(f"text")\n\n\n@dsl.DAG()\ndef diamond():\n    a = print_task()\n    b = print_task(wait_for=a)\n    c = print_task(wait_for=a)\n    print_task(wait_for=[c, b])\n\n```\n\n#### Loops\nwe support map reduce workflows through ```[for in]``` loop, the iterable input must be a parameter, an output of a previous task, or a sequence object. \n\ncurrently only one level of nesting is supported, in case you wish to use nested loops, extract the second loop into a fucntion and decorate it as well with a DAG decorater.\n```python\n@dsl.Task(image="python:3.10")\ndef generate_list(partitions: int, partition_size: int):\n    items = []\n    for i in range(partitions):\n        items.append(list(range(1, partition_size)))\n\n    return items\n\n\n@dsl.Task(image="python:3.10")\ndef sum_task(items:list[int]):\n    return sum(items)\n\n\n@dsl.DAG()\ndef map_reduce(partitions, partition_size):\n    partition_list = generate_list(partitions, partition_size)\n    partition_sums = [sum_task(partition) for partition in partition_list]\n    return sum_task(partition_sums)\n```\n\n#### Conditions \nwe support conditional task run by employing the \'with condition\' syntax\n\n```python\n    @Task(image="python:3.10")\n    def say_hello(name: str):\n        message = f"hello {name}"\n        print(message)\n        return message\n    \n    @Task(image="python:3.10")\n    def say_goodbye(name: str):\n        message = f"goodbye {name}"\n        print(message)\n        return message\n\n\n    @DAG()\n    def command_hello(name, command):\n        with Condition().equals(command, "hello"):\n            say_hello(name)\n        with Condition().equals(command, "goodbye"):\n            say_goodbye(name)\n```\n\n## How to contribute\n\nHave any feedback? Wish to implement an extenstion or new capability? Want to help us make argo better and easier to use?\nEvery contribution to _Argo Workflow Tools_ is greatly appreciated.\n\n',
     'author': 'Diagnostic Robotics',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/DiagnosticRobotics/argo-workflow-tools',
```

### Comparing `argo-workflow-tools-0.9.7/PKG-INFO` & `argo-workflow-tools-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argo-workflow-tools
-Version: 0.9.7
+Version: 0.9.9
 Summary: A suite of tools to ease ML pipeline development with Argo Workflows
 Home-page: https://github.com/DiagnosticRobotics/argo-workflow-tools
 License: Apache 2.0
 Author: Diagnostic Robotics
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=5.0)
 Requires-Dist: certifi (<=2021.10.8)
 Requires-Dist: contextvars (>=2.4,<3.0)
 Requires-Dist: pydantic (>=1.7.4,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: shortuuid (>=1.0.8,<2.0.0)
-Requires-Dist: urllib3 (<=1.26.0)
+Requires-Dist: urllib3 (<2.0.0)
 Project-URL: Repository, https://github.com/DiagnosticRobotics/argo-workflow-tools
 Description-Content-Type: text/markdown
 
 # Argo Workflow Tools
 argo-workflow-tools is a set of tools intended to easue the usage of argo for data science and data engineerign workflows
 ![Python Versions Supported](https://img.shields.io/badge/python-3.7+-blue.svg)
```

