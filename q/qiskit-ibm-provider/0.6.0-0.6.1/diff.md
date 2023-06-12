# Comparing `tmp/qiskit-ibm-provider-0.6.0.tar.gz` & `tmp/qiskit-ibm-provider-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-provider-0.6.0.tar", last modified: Thu May 18 18:05:33 2023, max compression
+gzip compressed data, was "qiskit-ibm-provider-0.6.1.tar", last modified: Mon Jun 12 17:47:35 2023, max compression
```

## Comparing `qiskit-ibm-provider-0.6.0.tar` & `qiskit-ibm-provider-0.6.1.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.055960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.055960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.059960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.059960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.059960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.059960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/apiconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    39027 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    29727 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_backend_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.063960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31717 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/ibm_circuit_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    48877 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/ibm_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/job_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/queueinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/sub_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.063960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/backend_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.063960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/gates_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/jobs_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/qubits_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.063960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/proxies/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.067960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.067960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40086 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/type_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.071960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.071960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.071960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.071960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23938 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.075960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/json_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/qobj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.075960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/device_layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.075960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/gate_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.055960 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-18 18:05:32.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-18 18:05:33.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:05:32.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 18:05:32.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:05:32.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 18:05:32.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 18:05:32.000000 qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-18 18:05:33.087960 qiskit-ibm-provider-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.079960 qiskit-ibm-provider-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.079960 qiskit-ibm-provider-0.6.0/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/e2e/test_real_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.079960 qiskit-ibm-provider-0.6.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    40183 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_filter_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_ibm_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_ibm_job_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_ibm_qasm_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/integration/test_websocket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/jobtestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/mock/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/mock/fake_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/test_ibm_job_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/test_ibm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/test_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/test/unit/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:05:33.083960 qiskit-ibm-provider-0.6.0/test/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/unit/utils/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-18 18:05:18.000000 qiskit-ibm-provider-0.6.0/test/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.724488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.728488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.728488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.732488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.732488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.732488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/apiconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39657 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29933 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.736488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31784 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_circuit_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48877 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/job_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/queueinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/sub_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.736488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/backend_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.736488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/gates_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/jobs_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/qubits_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40086 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/type_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.740488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.744488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23938 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.744488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/qobj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.744488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/device_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.748488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/gate_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.728488 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 17:47:35.000000 qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.748488 qiskit-ibm-provider-0.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.748488 qiskit-ibm-provider-0.6.1/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/e2e/test_real_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.752488 qiskit-ibm-provider-0.6.1/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40183 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_filter_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21105 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_ibm_qasm_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/integration/test_websocket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/jobtestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.752488 qiskit-ibm-provider-0.6.1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/mock/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/mock/fake_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_ibm_job_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_ibm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:47:35.756488 qiskit-ibm-provider-0.6.1/test/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/unit/utils/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-12 17:47:15.000000 qiskit-ibm-provider-0.6.1/test/ws_server.py
```

### Comparing `qiskit-ibm-provider-0.6.0/LICENSE.txt` & `qiskit-ibm-provider-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/PKG-INFO` & `qiskit-ibm-provider-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.6.0
+Version: 0.6.1
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.6.0/README.md` & `qiskit-ibm-provider-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/account.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/exceptions.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/management.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/accounts/storage.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/auth.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/client_parameters.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/account.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/auth.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/base.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/runtime.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,24 +143,24 @@
             session_id=session_id,
             job_tags=job_tags,
             max_execution_time=max_execution_time,
             start_session=start_session,
             **hgp_dict
         )
 
-    def job_get(self, job_id: str) -> Dict:
+    def job_get(self, job_id: str, exclude_params: bool = None) -> Dict:
         """Get job data.
 
         Args:
             job_id: Job ID.
 
         Returns:
             JSON response.
         """
-        response = self._api.program_job(job_id).get()
+        response = self._api.program_job(job_id).get(exclude_params=exclude_params)
         logger.debug("Runtime job get response: %s", response)
         return response
 
     def job_type(self, job_id: str) -> str:
         """Get job type.
 
         Args:
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/runtime_ws.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/version.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/clients/websocket.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/exceptions.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/backend.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/base.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/job.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/program_job.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/program_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,21 +43,29 @@
         Args:
             session: Session to be used in the adapter.
             job_id: ID of the program job.
             url_prefix: Prefix to use in the URL.
         """
         super().__init__(session, "{}/jobs/{}".format(url_prefix, job_id))
 
-    def get(self) -> Dict:
+    def get(self, exclude_params: bool = None) -> Dict:
         """Return program job information.
 
+        Args:
+            exclude_params: If ``True``, the params will not be included in the response.
+
         Returns:
             JSON response.
         """
-        return self.session.get(self.get_url("self")).json(cls=RuntimeDecoder)
+        payload = {}
+        if exclude_params:
+            payload["exclude_params"] = "true"
+        return self.session.get(self.get_url("self"), params=payload).json(
+            cls=RuntimeDecoder
+        )
 
     def job_type(self) -> str:
         """Return job type:
 
         Returns:
             Job type, either "IQX" or "RUNTIME".
         """
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/root.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/runtime.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/utils/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/rest/utils/data_mapper.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/api/session.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/api/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/apiconstants.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/apiconstants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/exceptions.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/hub_group_project.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/hub_group_project.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_backend.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
     def __getattr__(self, name: str) -> Any:
         """Gets attribute from self or configuration
         This magic method executes when user accesses an attribute that
         does not yet exist on IBMBackend class.
         """
         # Prevent recursion since these properties are accessed within __getattr__
-        if name in ["_properties", "_defaults", "_target"]:
+        if name in ["_properties", "_defaults", "_target", "_configuration"]:
             raise AttributeError(
                 "'{}' object has no attribute '{}'".format(
                     self.__class__.__name__, name
                 )
             )
         try:
             return super().__getattribute__(name)
@@ -324,15 +324,15 @@
             Target with properties found on `datetime`
         """
         return self._get_target(datetime=datetime)
 
     def run(
         self,
         circuits: Union[
-            QuantumCircuit, Schedule, List[Union[QuantumCircuit, Schedule]]
+            QuantumCircuit, Schedule, str, List[Union[QuantumCircuit, Schedule, str]]
         ],
         dynamic: bool = None,
         job_tags: Optional[List[str]] = None,
         init_circuit: Optional[QuantumCircuit] = None,
         init_num_resets: Optional[int] = None,
         header: Optional[Dict] = None,
         shots: Optional[Union[int, float]] = None,
@@ -427,30 +427,21 @@
             IBMBackendApiError: If an unexpected error occurred while submitting
                 the job.
             IBMBackendApiProtocolError: If an unexpected value received from
                  the server.
             IBMBackendValueError:
                 - If an input parameter value is not valid.
                 - If ESP readout is used and the backend does not support this.
-                - If Schedule is given as an input circuit.
         """
         # pylint: disable=arguments-differ
         validate_job_tags(job_tags, IBMBackendValueError)
-        if isinstance(circuits, (QuantumCircuit, Schedule)):
+        if not isinstance(circuits, List):
             circuits = [circuits]
+        self._check_circuits_attributes(circuits)
 
-        schedule_error_msg = (
-            "Class 'Schedule' is no longer supported as an input circuit. "
-            "Use 'pulse gates' instead. See `tutorial "
-            "https://qiskit.org/documentation/tutorials/circuits_advanced/05_pulse_gates.html` "
-            "on how to use pulse gates."
-        )
-        for circ in circuits:
-            if isinstance(circ, Schedule):
-                raise IBMBackendValueError(schedule_error_msg)
         if (
             use_measure_esp
             and getattr(self.configuration(), "measure_esp_enabled", False) is False
         ):
             raise IBMBackendValueError(
                 "ESP readout not supported on this device. Please make sure the flag "
                 "'use_measure_esp' is unset or set to 'False'."
@@ -513,17 +504,14 @@
         )
 
         run_config_dict["circuits"] = circuits
         if not program_id.startswith(QASM3RUNNERPROGRAMID):
             # Transpiling in circuit-runner is deprecated.
             run_config_dict["skip_transpilation"] = True
 
-        for circ in circuits:
-            self.check_faulty(circ)
-
         return self._runtime_run(
             program_id=program_id,
             inputs=run_config_dict,
             options=options,
             job_tags=job_tags,
         )
 
@@ -746,16 +734,15 @@
         """
         return self._configuration.control(qubits=qubits)
 
     def __repr__(self) -> str:
         return "<{}('{}')>".format(self.__class__.__name__, self.name)
 
     def _deprecate_id_instruction(
-        self,
-        circuits: List[Union[QuantumCircuit, Schedule]],
+        self, circuits: List[Union[QuantumCircuit, Schedule]]
     ) -> List[Union[QuantumCircuit, Schedule]]:
         """Raise a DeprecationWarning if any circuit contains an 'id' instruction.
 
         Additionally, if 'delay' is a 'supported_instruction', replace each 'id'
         instruction (in-place) with the equivalent ('sx'-length) 'delay' instruction.
 
         Args:
@@ -817,15 +804,38 @@
 
         return circuits
 
     def get_translation_stage_plugin(self) -> str:
         """Return the default translation stage plugin name for IBM backends."""
         return "ibm_dynamic_circuits"
 
-    def check_faulty(self, circuit: QuantumCircuit) -> None:
+    def _check_circuits_attributes(self, circuits: List[QuantumCircuit]) -> None:
+        """Check that circuits can be executed on backend.
+        Raises:
+            IBMBackendValueError:
+                - If Schedule is given as an input circuit.
+                - If one of the circuits contains more qubits than on the backend."""
+        schedule_error_msg = (
+            "Class 'Schedule' is no longer supported as an input circuit. "
+            "Use 'pulse gates' instead. See `tutorial "
+            "https://qiskit.org/documentation/tutorials/circuits_advanced/05_pulse_gates.html` "
+            "on how to use pulse gates."
+        )
+        for circ in circuits:
+            if isinstance(circ, Schedule):
+                raise IBMBackendValueError(schedule_error_msg)
+            if isinstance(circ, QuantumCircuit):
+                if circ.num_qubits > self._configuration.num_qubits:
+                    raise IBMBackendValueError(
+                        f"Circuit contains {circ.num_qubits} qubits, "
+                        f"but backend has only {self.num_qubits}."
+                    )
+                self._check_faulty(circ)
+
+    def _check_faulty(self, circuit: QuantumCircuit) -> None:
         """Check if the input circuit uses faulty qubits or edges.
 
         Args:
             circuit: Circuit to check.
 
         Raises:
             ValueError: If an instruction operating on a faulty qubit or edge is found.
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_backend_service.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_backend_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,36 +164,39 @@
             if name not in self._backends:
                 raise QiskitBackendNotFoundError("No backend matches the criteria")
             if not self._backends[name] or instance != self._backends[name]._instance:
                 self._set_backend_config(name)
                 self._backends[name] = self._create_backend_obj(
                     self._backend_configs[name], instance, self._provider._get_hgps()
                 )
-            backends.append(self._backends[name])
+            if self._backends[name]:
+                backends.append(self._backends[name])
         elif instance:
             hgp = self._provider._get_hgp(instance=instance)
             for backend_name in hgp.backends.keys():
                 if (
                     not self._backends[backend_name]
                     or instance != self._backends[backend_name]._instance
                 ):
                     self._set_backend_config(backend_name, instance)
                     self._backends[backend_name] = self._create_backend_obj(
                         self._backend_configs[backend_name], instance
                     )
-                backends.append(self._backends[backend_name])
+                if self._backends[backend_name]:
+                    backends.append(self._backends[backend_name])
         else:
             hgps = self._provider._get_hgps()
             for backend_name, backend_config in self._backends.items():
                 if not backend_config:
                     self._set_backend_config(backend_name)
                     self._backends[backend_name] = self._create_backend_obj(
                         self._backend_configs[backend_name], hgps=hgps
                     )
-                backends.append(self._backends[backend_name])
+                if self._backends[backend_name]:
+                    backends.append(self._backends[backend_name])
         # Special handling of the `name` parameter, to support alias resolution.
         if name:
             aliases = self._aliased_backend_names()
             aliases.update(self._deprecated_backend_names())
             name = aliases.get(name, name)
             kwargs["backend_name"] = name
         if min_num_qubits:
@@ -632,15 +635,17 @@
         """
         try:
             legacy = False
             if self._provider._runtime_client.job_type(job_id) == "IQX":
                 legacy = True
                 job_info = self._default_hgp._api_client.job_get(job_id)
             else:
-                job_info = self._provider._runtime_client.job_get(job_id)
+                job_info = self._provider._runtime_client.job_get(
+                    job_id, exclude_params=True
+                )
                 if job_info.get("program", {}).get("id") not in [
                     "circuit-runner",
                     "qasm3-runner",
                 ]:
                     raise IBMInputValueError(
                         f"Job {job_id} was not run with qiskit-ibm-provider, "
                         f"please try retrieving job results from qiskit-ibm-runtime"
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_provider.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/ibm_qubit_properties.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/constants.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/exceptions.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/ibm_circuit_job.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_circuit_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,17 @@
             self.refresh()
 
         # Note: By default, `None` should be returned if no time per step info is available.
         time_per_step_local = None
         if self._time_per_step:
             time_per_step_local = {}
             for step_name, time_data_utc in self._time_per_step.items():
-                time_per_step_local[step_name] = utc_to_local(time_data_utc)
+                time_per_step_local[step_name] = (
+                    utc_to_local(time_data_utc) if time_data_utc else None
+                )
 
         return time_per_step_local
 
     @property
     def client_version(self) -> Dict[str, str]:
         """Return version of the client used for this job.
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/ibm_composite_job.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/ibm_job.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/job_monitor.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/job_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/queueinfo.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/queueinfo.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/sub_job.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/sub_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/job/utils.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/job/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/backend_info.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/backend_info.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/config_widget.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/config_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/backend_update.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_update.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/constants.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/dashboard.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/utils.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/gates_widget.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/gates_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/jobs_widget.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/jobs_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/jupyter/qubits_widget.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/jupyter/qubits_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/proxies/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/proxies/configuration.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/circuits.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/schedules.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/schedules.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/binary_io/value.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/binary_io/value.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/common.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/common.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/exceptions.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/formats.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/formats.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/interface.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/interface.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/qpy/type_keys.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/qpy/type_keys.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/basis/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/transpiler/plugin.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/transpiler/plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/backend_decoder.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/converters.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/hgp.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/json.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,24 +199,28 @@
         if isinstance(obj, complex):
             return {"__type__": "complex", "__value__": [obj.real, obj.imag]}
         if isinstance(obj, np.ndarray):
             if obj.dtype == object:
                 return {"__type__": "ndarray", "__value__": obj.tolist()}
             value = _serialize_and_encode(obj, np.save, allow_pickle=False)
             return {"__type__": "ndarray", "__value__": value}
+        if isinstance(obj, np.int64):
+            return {"__type__": "int", "__value__": int(obj)}
         if isinstance(obj, set):
             return {"__type__": "set", "__value__": list(obj)}
         if isinstance(obj, Result):
             return {"__type__": "Result", "__value__": obj.to_dict()}
         if hasattr(obj, "to_json"):
             return {"__type__": "to_json", "__value__": obj.to_json()}
         if isinstance(obj, QuantumCircuit):
             value = _serialize_and_encode(
                 data=obj,
-                serializer=lambda buff, data: dump(data, buff),  # type: ignore[no-untyped-call]
+                serializer=lambda buff, data: dump(
+                    data, buff, RuntimeEncoder
+                ),  # type: ignore[no-untyped-call]
             )
             return {"__type__": "QuantumCircuit", "__value__": value}
         if isinstance(obj, Parameter):
             value = _serialize_and_encode(
                 data=obj,
                 serializer=_write_parameter,
                 compress=False,
@@ -257,14 +261,15 @@
         return super().default(obj)
 
 
 class RuntimeDecoder(json.JSONDecoder):
     """JSON Decoder used by runtime service."""
 
     def __init__(self, *args: Any, **kwargs: Any):
+        kwargs.pop("encoding", None)
         super().__init__(object_hook=self.object_hook, *args, **kwargs)
         self.__parameter_vectors: Dict[str, Tuple[ParameterVector, set]] = {}
         self.__read_parameter_expression = (
             functools.partial(
                 _read_parameter_expression_v3,
                 vectors=self.__parameter_vectors,
             )
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/json_decoder.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 def target_from_server_data(
     configuration: Union[QasmBackendConfiguration, PulseBackendConfiguration],
     pulse_defaults: Optional[Dict] = None,
     properties: Optional[Dict] = None,
 ) -> Target:
     """Decode transpiler target from backend data set.
 
-    This function directly generate ``Target`` instance without generate
+    This function directly generates ``Target`` instance without generating
     intermediate legacy objects such as ``BackendProperties`` and ``PulseDefaults``.
 
     Args:
         configuration: Backend configuration.
         pulse_defaults: Backend pulse defaults dictionary.
         properties: Backend property dictionary.
 
@@ -126,14 +126,15 @@
     basis_gates = set(getattr(configuration, "basis_gates", []))
     gate_configs = {gate.name: gate for gate in configuration.gates}
     inst_name_map = {}  # type: Dict[str, Instruction]
     prop_name_map = {}  # type: Dict[str, Dict[Tuple[int, ...], InstructionProperties]]
     all_instructions = set.union(supported_instructions, basis_gates, set(required))
     faulty_qubits = set()
     faulty_ops = set()
+    unsupported_instructions = []
 
     # Create name to Qiskit instruction object repr mapping
     for name in all_instructions:
         if name in qiskit_control_flow_mapping:
             continue
         if name in qiskit_inst_mapping:
             inst_name_map[name] = qiskit_inst_mapping[name]
@@ -151,16 +152,18 @@
                 "Definition of instruction %s is not found in the Qiskit namespace and "
                 "GateConfig is not provided by the BackendConfiguration payload. "
                 "Qiskit Gate model cannot be instantiated for this instruction and "
                 "this instruction is silently excluded from the Target. "
                 "Please add new gate class to Qiskit or provide GateConfig for this name.",
                 name,
             )
-            all_instructions.remove(name)
-            continue
+            unsupported_instructions.append(name)
+
+    for name in unsupported_instructions:
+        all_instructions.remove(name)
 
     # Create empty inst properties from gate configs
     for name, spec in gate_configs.items():
         if hasattr(spec, "coupling_map"):
             coupling_map = spec.coupling_map
             prop_name_map[name] = dict.fromkeys(map(tuple, coupling_map))
         else:
@@ -220,25 +223,31 @@
         pulse_lib = list(
             map(PulseLibraryItem.from_dict, pulse_defaults["pulse_library"])
         )
         converter = QobjToInstructionConverter(pulse_lib)
         for cmd in map(Command.from_dict, pulse_defaults["cmd_def"]):
             name = cmd.name
             qubits = tuple(cmd.qubits)
-            if (name, qubits) in faulty_ops:
-                continue
-            if name not in all_instructions or qubits not in prop_name_map[name]:
+            if (
+                name not in all_instructions
+                or name not in prop_name_map
+                or qubits not in prop_name_map[name]
+            ):
                 logger.info(
                     "Gate calibration for instruction %s on qubits %s is found "
                     "in the PulseDefaults payload. However, this entry is not defined in "
                     "the gate mapping of Target. This calibration is ignored.",
                     name,
                     qubits,
                 )
                 continue
+
+            if (name, qubits) in faulty_ops:
+                continue
+
             entry = PulseQobjDef(converter=converter, name=cmd.name)
             entry.define(cmd.sequence)
             try:
                 prop_name_map[name][qubits].calibration = entry
             except AttributeError:
                 logger.info(
                     "The PulseDefaults payload received contains an instruction %s on "
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/json_encoder.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/options.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/options.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 class CommonOptions:
     """Options common for both paths."""
 
     shots: int = 4000
     meas_level: Union[int, MeasLevel] = MeasLevel.CLASSIFIED
     init_qubits: bool = True
     rep_delay: Optional[float] = None
+    memory: bool = False
+    meas_return: Union[str, MeasReturnType] = MeasReturnType.AVERAGE
 
     def to_transport_dict(self) -> Dict[str, Any]:
         """Remove None values so runtime defaults are used."""
         dict_ = asdict(self)
         for key in list(dict_.keys()):
             if dict_[key] is None:
                 del dict_[key]
@@ -47,22 +49,20 @@
 
 
 @dataclass
 class QASM2Options(CommonOptions):
     """Options for the QASM2 path."""
 
     header: Optional[Dict] = None
-    memory: bool = False
     qubit_lo_freq: Optional[List[int]] = None
     meas_lo_freq: Optional[List[int]] = None
     schedule_los: Optional[
         Union[
             List[Union[Dict[PulseChannel, float], LoConfig]],
             Union[Dict[PulseChannel, float], LoConfig],
         ]
     ] = None
-    meas_return: Union[str, MeasReturnType] = MeasReturnType.AVERAGE
     init_qubits: bool = True
     use_measure_esp: Optional[bool] = None
     # Simulator only
     noise_model: Any = None
     seed_simulator: Optional[int] = None
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/qobj_utils.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/qobj_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/utils/utils.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,16 @@
             elif isinstance(value, dict):
                 _filter_value(value, filter_keys)
 
 
 def are_circuits_dynamic(circuits: List[QuantumCircuit]) -> bool:
     """Checks if the input circuits are dynamic."""
     for circuit in circuits:
+        if isinstance(circuit, str):
+            return True
         for inst in circuit:
             if (
                 isinstance(inst.operation, ControlFlowOp)
                 or getattr(inst.operation, "condition", None) is not None
             ):
                 return True
     return False
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/version.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/colormaps.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/colormaps.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/device_layouts.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/device_layouts.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/exceptions.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/__init__.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/error_map.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/error_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/gate_map.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/gate_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/PKG-INFO` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.6.0
+Version: 0.6.1
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.6.0/qiskit_ibm_provider.egg-info/SOURCES.txt` & `qiskit-ibm-provider-0.6.1/qiskit_ibm_provider.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 qiskit_ibm_provider/VERSION.txt
 qiskit_ibm_provider/__init__.py
 qiskit_ibm_provider/apiconstants.py
 qiskit_ibm_provider/exceptions.py
 qiskit_ibm_provider/hub_group_project.py
```

### Comparing `qiskit-ibm-provider-0.6.0/setup.cfg` & `qiskit-ibm-provider-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/setup.py` & `qiskit-ibm-provider-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/__init__.py` & `qiskit-ibm-provider-0.6.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/account.py` & `qiskit-ibm-provider-0.6.1/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/contextmanagers.py` & `qiskit-ibm-provider-0.6.1/test/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/decorators.py` & `qiskit-ibm-provider-0.6.1/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/e2e/test_real_devices.py` & `qiskit-ibm-provider-0.6.1/test/e2e/test_real_devices.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/e2e/test_tutorials.py` & `qiskit-ibm-provider-0.6.1/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/fake_account_client.py` & `qiskit-ibm-provider-0.6.1/test/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/http_server.py` & `qiskit-ibm-provider-0.6.1/test/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/ibm_test_case.py` & `qiskit-ibm-provider-0.6.1/test/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_account_client.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_backend.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from qiskit import QuantumCircuit, transpile
 from qiskit.providers.models import QasmBackendConfiguration
 from qiskit.providers.exceptions import QiskitBackendNotFoundError
 from qiskit.test.reference_circuits import ReferenceCircuits
 from qiskit.pulse import Schedule
 
-from qiskit_ibm_provider import IBMBackend, IBMProvider
+from qiskit_ibm_provider import IBMBackend, IBMProvider, least_busy
 from qiskit_ibm_provider.ibm_qubit_properties import IBMQubitProperties
 from qiskit_ibm_provider.exceptions import IBMBackendValueError
 
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup_with_backend,
 )
@@ -205,7 +205,25 @@
         for circuit in [schedule, [schedule]]:
             with self.assertRaises(IBMBackendValueError) as err:
                 backend.run(circuit)
             self.assertIn(
                 "Class 'Schedule' is no longer supported as an input circuit",
                 str(err.exception),
             )
+
+    def test_too_many_qubits_in_circuit(self):
+        """Check error message if circuit contains more qubits than supported on the backend."""
+        backends = self.dependencies.provider.backends(
+            instance=self.dependencies.instance, simulator=False
+        )
+        least_busy_backend = least_busy(backends)
+        self.assertTrue(least_busy_backend)
+
+        num = len(least_busy_backend.properties().qubits)
+        num_qubits = num + 1
+        circuit = QuantumCircuit(num_qubits, num_qubits)
+        with self.assertRaises(IBMBackendValueError) as err:
+            _ = least_busy_backend.run(circuit)
+        self.assertIn(
+            f"Circuit contains {num_qubits} qubits, but backend has only {num}.",
+            str(err.exception),
+        )
```

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_basic_server_paths.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_basic_server_paths.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_composite_job.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_filter_backends.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_filter_backends.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_ibm_integration.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_ibm_job.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -511,7 +511,16 @@
 
     def test_job_header(self):
         """Test job header."""
         custom_header = {"test": "test_job_header"}
         job = self.sim_backend.run(self.bell, header=custom_header)
         self.assertEqual(custom_header["test"], job.header()["test"])
         self.assertLessEqual(custom_header.items(), job.header().items())
+
+    def test_lazy_loading_params(self):
+        """Test lazy loading job params."""
+        job = self.sim_backend.run(self.bell)
+        job.wait_for_final_state()
+
+        rjob = self.provider.backend.retrieve_job(job.job_id())
+        self.assertFalse(rjob._params)
+        self.assertTrue(rjob.circuits)
```

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_ibm_job_attributes.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_job_attributes.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_ibm_provider.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_ibm_qasm_simulator.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_ibm_qasm_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_jupyter.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_proxies.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_proxies.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_serialization.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/integration/test_websocket_integration.py` & `qiskit-ibm-provider-0.6.1/test/integration/test_websocket_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/jobtestcase.py` & `qiskit-ibm-provider-0.6.1/test/jobtestcase.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/proxy_server.py` & `qiskit-ibm-provider-0.6.1/test/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/mock/fake_account_client.py` & `qiskit-ibm-provider-0.6.1/test/unit/mock/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/mock/fake_provider.py` & `qiskit-ibm-provider-0.6.1/test/unit/mock/fake_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/test_account.py` & `qiskit-ibm-provider-0.6.1/test/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/test_ibm_job_states.py` & `qiskit-ibm-provider-0.6.1/test/unit/test_ibm_job_states.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/test_ibm_logger.py` & `qiskit-ibm-provider-0.6.1/test/unit/test_ibm_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/test_serialization.py` & `qiskit-ibm-provider-0.6.1/test/unit/test_serialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Test serializing and deserializing data sent to the server."""
 
 import json
-
+import numpy as np
 from qiskit import assemble
 from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister
 from qiskit.circuit import Parameter
 
 from qiskit_ibm_provider.utils.json_encoder import IBMJsonEncoder
+from qiskit_ibm_provider.utils.json import RuntimeEncoder
 from ..ibm_test_case import IBMTestCase
 
 
 class TestSerialization(IBMTestCase):
     """Test data serialization."""
 
     def test_exception_message(self):
-        """Test executing job with Parameter in methadata."""
+        """Test executing job with Parameter in metadata."""
         quantum_register = QuantumRegister(1)
         classical_register = ClassicalRegister(1)
         my_circ_str = "test_metadata"
         my_circ = QuantumCircuit(
             quantum_register,
             classical_register,
             name=my_circ_str,
@@ -61,7 +62,16 @@
             "list": [1, 2, {"ld": 1, 2: 3, Parameter("alfa"): 0.1}],
         }
 
         self.assertEqual(
             '{"t1": 1, "null": null, "a": 0.2, "list": [1, 2, {"ld": 1, "2": 3, "alfa": 0.1}]}',
             IBMJsonEncoder().encode(test_dir),
         )
+
+    def test_circuit_metadata(self):
+        """Test serializing circuit metadata."""
+
+        circ = QuantumCircuit(1)
+        circ.metadata = {"test": np.arange(0, 10)}
+        payload = {"circuits": [circ]}
+
+        self.assertTrue(json.dumps(payload, cls=RuntimeEncoder))
```

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/test_websocket.py` & `qiskit-ibm-provider-0.6.1/test/unit/test_websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py` & `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/control_flow_test_case.py` & `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/control_flow_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py` & `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/test_scheduler.py` & `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/transpiler/passes/scheduling/test_utils.py` & `qiskit-ibm-provider-0.6.1/test/unit/transpiler/passes/scheduling/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/unit/utils/ws_handler.py` & `qiskit-ibm-provider-0.6.1/test/unit/utils/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/utils.py` & `qiskit-ibm-provider-0.6.1/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.6.0/test/ws_server.py` & `qiskit-ibm-provider-0.6.1/test/ws_server.py`

 * *Files identical despite different names*

