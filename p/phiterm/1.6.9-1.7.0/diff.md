# Comparing `tmp/phiterm-1.6.9.tar.gz` & `tmp/phiterm-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.9.tar", last modified: Tue May 23 01:46:30 2023, max compression
+gzip compressed data, was "phiterm-1.7.0.tar", last modified: Mon Jun 12 20:54:11 2023, max compression
```

## Comparing `phiterm-1.6.9.tar` & `phiterm-1.7.0.tar`

### file list

```diff
@@ -1,144 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.912390 phiterm-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-23 01:46:07.000000 phiterm-1.6.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:46:30.912390 phiterm-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 01:46:07.000000 phiterm-1.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36902 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.892389 phiterm-1.6.9/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    45502 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-23 01:46:07.000000 phiterm-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:46:30.912390 phiterm-1.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 01:46:07.000000 phiterm-1.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 01:46:07.000000 phiterm-1.6.9/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.591922 phiterm-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-12 20:53:48.000000 phiterm-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 20:54:11.591922 phiterm-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 20:53:48.000000 phiterm-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.571922 phiterm-1.7.0/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.575922 phiterm-1.7.0/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36902 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.579922 phiterm-1.7.0/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.579922 phiterm-1.7.0/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.579922 phiterm-1.7.0/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.579922 phiterm-1.7.0/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.579922 phiterm-1.7.0/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.579922 phiterm-1.7.0/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.579922 phiterm-1.7.0/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.583922 phiterm-1.7.0/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.571922 phiterm-1.7.0/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.583922 phiterm-1.7.0/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.583922 phiterm-1.7.0/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.583922 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.583922 phiterm-1.7.0/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.587922 phiterm-1.7.0/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.587922 phiterm-1.7.0/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/get_python_objects_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.587922 phiterm-1.7.0/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.591922 phiterm-1.7.0/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-12 20:53:48.000000 phiterm-1.7.0/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.571922 phiterm-1.7.0/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 20:54:11.000000 phiterm-1.7.0/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-12 20:54:11.000000 phiterm-1.7.0/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:54:11.000000 phiterm-1.7.0/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 20:54:11.000000 phiterm-1.7.0/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-12 20:54:11.000000 phiterm-1.7.0/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 20:54:11.000000 phiterm-1.7.0/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-12 20:53:48.000000 phiterm-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:54:11.591922 phiterm-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-12 20:53:48.000000 phiterm-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:54:11.591922 phiterm-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 20:53:48.000000 phiterm-1.7.0/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.9/LICENSE.md` & `phiterm-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/api/client.py` & `phiterm-1.7.0/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/api/routes.py` & `phiterm-1.7.0/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/api/user.py` & `phiterm-1.7.0/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/api/workspace.py` & `phiterm-1.7.0/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/aws/aws_operator.py` & `phiterm-1.7.0/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/cli/dx/dx_app.py` & `phiterm-1.7.0/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.7.0/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.7.0/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.7.0/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/cli/wf/wf_app.py` & `phiterm-1.7.0/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/cli/ws/ws_app.py` & `phiterm-1.7.0/phiterm/cli/ws/ws_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/conf/auth.py` & `phiterm-1.7.0/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/conf/constants.py` & `phiterm-1.7.0/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/conf/phi_conf.py` & `phiterm-1.7.0/phiterm/conf/phi_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,33 +440,33 @@
                     file_path=PHI_CONF_PATH, verify_class=cls
                 )
             elif PHI_CONF_PATH.is_dir():
                 logger.debug(f"{PHI_CONF_PATH} is a directory, deleting and exiting")
                 delete_from_fs(PHI_CONF_PATH)
         return None
 
-    def print_to_cli(self):
+    def print_to_cli(self, show_all: bool = False):
         if self.user:
             print_heading(f"User: {self.user.email}")
         if self.active_ws_name:
             print_heading(f"\nActive workspace: {self.active_ws_name}\n")
         else:
             print_info("* No active workspace, run `phi ws create` to create one")
-        # if len(self._ws_data_map) > 0:
-        #     print_heading("Available workspaces:\n")
-        #     c = 1
-        #     for k, v in self._ws_data_map.items():
-        #         print_info(f"  {c}. Name: {v.ws_name}")
-        #         print_info(f"     Dir: {v.ws_root_path}")
-        #         if v.ws_schema:
-        #             logger.debug(
-        #                 f"     Schema: {v.ws_schema.json(exclude_none=True, indent=2)}"
-        #             )
-        #         print_info(f"  -*-\n")
-        #         c += 1
+        if show_all and len(self._ws_data_map) > 0:
+            print_heading("Available workspaces:\n")
+            c = 1
+            for k, v in self._ws_data_map.items():
+                print_info(f"  {c}. Name: {v.ws_name}")
+                print_info(f"     Dir: {v.ws_root_path}")
+                if v.ws_schema:
+                    logger.debug(
+                        f"     Schema: {v.ws_schema.json(exclude_none=True, indent=2)}"
+                    )
+                print_info(f"  -*-\n")
+                c += 1
 
     ######################################################
     ## Deprecated functions
     ######################################################
     #
     # def add_ws_data_using_config_file(
     #     self, ws_root_path: Path, ws_config_file_path: Optional[Path]
```

### Comparing `phiterm-1.6.9/phiterm/databox/databox_operator.py` & `phiterm-1.7.0/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/docker/docker_operator.py` & `phiterm-1.7.0/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/enums/user.py` & `phiterm-1.7.0/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/k8s/k8s_operator.py` & `phiterm-1.7.0/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.7.0/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.7.0/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.7.0/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.7.0/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/local/local_operator.py` & `phiterm-1.7.0/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/release/release_schemas.py` & `phiterm-1.7.0/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/release/ws_releases.py` & `phiterm-1.7.0/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/schemas/user.py` & `phiterm-1.7.0/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/schemas/user_schemas.py` & `phiterm-1.7.0/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/schemas/workspace.py` & `phiterm-1.7.0/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.7.0/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.7.0/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.7.0/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.7.0/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.7.0/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.7.0/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.7.0/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.7.0/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/cli_auth_server.py` & `phiterm-1.7.0/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/cli_console.py` & `phiterm-1.7.0/phiterm/utils/cli_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     console.print(
         "This feature is not yet supported. Please reach out to ashpreet@phidata.com for more info",
         style=info_style,
     )
 
 
 def print_conf_not_available_msg() -> None:
-    logger.error("PhidataConf not available, please run `phi init`")
+    logger.error("Phidata not initialized, please run `phi init`")
 
 
 def print_generic_error_msg() -> None:
     console.print("Something went wrong, please try again", style=error_style)
 
 
 def log_ws_not_available_msg():
```

### Comparing `phiterm-1.6.9/phiterm/utils/common.py` & `phiterm-1.7.0/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/dttm.py` & `phiterm-1.7.0/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/enums.py` & `phiterm-1.7.0/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/filesystem.py` & `phiterm-1.7.0/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/git.py` & `phiterm-1.7.0/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/load_env.py` & `phiterm-1.7.0/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/log.py` & `phiterm-1.7.0/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/pyproject.py` & `phiterm-1.7.0/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/utils/ws_filter.py` & `phiterm-1.7.0/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/workflow/wf_operator.py` & `phiterm-1.7.0/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/workflow/wf_utils.py` & `phiterm-1.7.0/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/workspace/phi_ws_data.py` & `phiterm-1.7.0/phiterm/workspace/phi_ws_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,28 +63,26 @@
             raise WorkspaceException("Workspace root not set")
 
         from phiterm.workspace.ws_loader import add_ws_dir_to_path, load_workspace
 
         # NOTE: When loading a workspace, relative imports or package imports dont work.
         # This is a known problem in python :(
         #     eg: https://stackoverflow.com/questions/6323860/sibling-package-imports/50193944#50193944
-        # To make them work, we need to install the workspace as a python module
-        #   But when we run `phi ws setup`, the ws module is not yet installed
-        # So we add workspace_root to sys.path so is treated as a module
+        # To make them work, we add workspace_root to sys.path so is treated as a module
         add_ws_dir_to_path(self.ws_root_path)
 
         logger.debug(f"**--> Loading WorkspaceConfig")
         loaded_config: WorkspaceConfig = load_workspace(ws_root_path=self.ws_root_path)
 
         # Update cached_ws_config
         self.cached_ws_config = loaded_config
         self.cached_ws_config.workspace_root_path = self.ws_root_path
         self.cached_ws_config.workspace_config_file_path = self.ws_config_file_path
 
-        logger.debug("WorkspaceConfig: {}".format(self.cached_ws_config.args))
+        # logger.debug("WorkspaceConfig: {}".format(self.cached_ws_config.args))
         return self.cached_ws_config
 
     ######################################################
     ## Print functions
     ######################################################
 
     def print_to_cli(self):
```

### Comparing `phiterm-1.6.9/phiterm/workspace/ws_enums.py` & `phiterm-1.7.0/phiterm/workspace/ws_enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     PUBLIC = "PUBLIC"
 
 
 class WorkspaceStarterTemplate(ExtendedEnum):
     ai_app = "ai-app"
     ml_app = "ml-app"
     api_app = "api-app"
+    llm_app = "llm-app"
     django_app = "django-app"
     streamlit_app = "streamlit-app"
     aws_dp = "data-platform"
     aws_spark_dp = "spark-data-platform"
     aws_snowflake_dp = "snowflake-data-platform"
```

### Comparing `phiterm-1.6.9/phiterm/workspace/ws_operator.py` & `phiterm-1.7.0/phiterm/workspace/ws_operator.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,29 +18,32 @@
 )
 from phiterm.utils.log import logger
 from phiterm.workspace.ws_enums import (
     WorkspaceConfigType,
     WorkspaceStarterTemplate,
 )
 from phiterm.workspace.exceptions import WorkspaceException
+from phiterm.utils.prep_infra_config import filter_and_prep_configs
 
 TEMPLATE_TO_NAME_MAP: Dict[WorkspaceStarterTemplate, str] = {
     WorkspaceStarterTemplate.ai_app: "ai-app",
     WorkspaceStarterTemplate.ml_app: "ml-app",
     WorkspaceStarterTemplate.api_app: "api-app",
+    WorkspaceStarterTemplate.llm_app: "api-app",
     WorkspaceStarterTemplate.django_app: "django-app",
     WorkspaceStarterTemplate.streamlit_app: "streamlit-app",
     WorkspaceStarterTemplate.aws_dp: "data-platform",
     WorkspaceStarterTemplate.aws_spark_dp: "spark-data-platform",
     WorkspaceStarterTemplate.aws_snowflake_dp: "snowflake-data-platform",
 }
 TEMPLATE_TO_REPO_MAP: Dict[WorkspaceStarterTemplate, str] = {
     WorkspaceStarterTemplate.ai_app: "https://github.com/phidatahq/ai-app.git",
     WorkspaceStarterTemplate.ml_app: "https://github.com/phidatahq/ml-app.git",
     WorkspaceStarterTemplate.api_app: "https://github.com/phidatahq/api-app.git",
+    WorkspaceStarterTemplate.llm_app: "https://github.com/phidatahq/llm-app.git",
     WorkspaceStarterTemplate.django_app: "https://github.com/phidatahq/django-app.git",
     WorkspaceStarterTemplate.streamlit_app: "https://github.com/phidatahq/streamlit-app.git",
     WorkspaceStarterTemplate.aws_dp: "https://github.com/phidatahq/aws-dp-template.git",
     WorkspaceStarterTemplate.aws_spark_dp: "https://github.com/phidatahq/aws-spark-dp-template.git",
     WorkspaceStarterTemplate.aws_snowflake_dp: "https://github.com/phidatahq/aws-snowflake-dp-template.git",
 }
 
@@ -363,95 +366,14 @@
         return False
 
     ######################################################
     ## End Workspace setup
     ######################################################
 
 
-def filter_and_prep_configs(
-    ws_config: WorkspaceConfig,
-    target_env: Optional[str] = None,
-    target_config: Optional[WorkspaceConfigType] = None,
-    order: Optional[str] = "create",
-) -> List[InfraConfig]:
-    from phidata.utils.prep_infra_config import prep_infra_config
-
-    # Step 1. Filter configs
-    # 1.1: Filter by config type: docker/k8s/aws
-    filtered_configs: List[InfraConfig] = []
-    if target_config is None:
-        if ws_config.docker is not None:
-            filtered_configs.extend(ws_config.docker)
-        if order == "delete":
-            if ws_config.k8s is not None:
-                filtered_configs.extend(ws_config.k8s)
-            if ws_config.aws is not None:
-                filtered_configs.extend(ws_config.aws)
-        else:
-            if ws_config.aws is not None:
-                filtered_configs.extend(ws_config.aws)
-            if ws_config.k8s is not None:
-                filtered_configs.extend(ws_config.k8s)
-    elif target_config == WorkspaceConfigType.docker:
-        if ws_config.docker is not None:
-            filtered_configs.extend(ws_config.docker)
-        else:
-            logger.error("No DockerConfig provided")
-    elif target_config == WorkspaceConfigType.k8s:
-        if ws_config.k8s is not None:
-            filtered_configs.extend(ws_config.k8s)
-        else:
-            logger.error("No K8sConfig provided")
-    elif target_config == WorkspaceConfigType.aws:
-        if ws_config.aws is not None:
-            filtered_configs.extend(ws_config.aws)
-        else:
-            logger.error("No AwsConfig provided")
-
-    # 1.2: Filter by env: dev/stg/prd
-    configs_after_env_filter: List[InfraConfig] = []
-    if target_env is None or target_env == "all":
-        configs_after_env_filter = filtered_configs
-    else:
-        for config in filtered_configs:
-            if config.env is None:
-                continue
-            if target_env == config.env:
-                configs_after_env_filter.append(config)
-    # logger.debug("Filtered configs: {}`".format(configs_after_env_filter))
-
-    # Step 2. Prepare configs
-    ready_to_use_configs: List[InfraConfig] = []
-    for config in configs_after_env_filter:
-        if not isinstance(config, InfraConfig):
-            logger.error(f"{config} is not an instance of InfraConfig")
-            continue
-        if not config.is_valid():
-            logger.warning(f"Skipping {config.__class__}\n")
-            continue
-        if not config.enabled:
-            logger.debug(
-                f"{config.__class__.__name__} for env {config.__class__.env} disabled"
-            )
-            continue
-
-        ######################################################################
-        # NOTE: VERY IMPORTANT TO GET RIGHT
-        ######################################################################
-
-        _config = prep_infra_config(
-            infra_config=config,
-            ws_config=ws_config,
-        )
-        ready_to_use_configs.append(_config)
-
-    # Return filtered and prepared configs
-    return ready_to_use_configs
-
-
 def deploy_workspace(
     ws_data: PhiWsData,
     target_env: Optional[str] = None,
     target_config: Optional[WorkspaceConfigType] = None,
     target_name: Optional[str] = None,
     target_type: Optional[str] = None,
     target_app: Optional[str] = None,
@@ -869,289 +791,7 @@
             #     app_filter=target_app,
             #     dry_run=dry_run,
             #     auto_confirm=auto_confirm,
             # )
             num_configs_patched += 1
         # white space between runs
         print_info("")
-
-
-######################################################
-## TODO: Delete deprecated functions
-######################################################
-#
-# def create_new_workspace(ws_name: str, template: WorkspaceStarterTemplate) -> bool:
-#     """Creates a new workspace for the user.
-#     This function clones a phidata template on the users machine at the path:
-#         cwd/ws_name
-#     cwd: current working dir - where the command was run from.
-#
-#     Steps:
-#     1. Validate ws_name and if we can create a folder with that name
-#     2. Clone the starter template in cwd/ws_name
-#     3. Delete the .git folder
-#     4. Provide the user with steps to add a remote origin for this workspace
-#
-#     NOTE: till the user runs `phi ws setup` the workspace is not registered with phidata
-#         and can only be used locally
-#     """
-#     from shutil import copytree
-#     from phiterm.utils.filesystem import rmdir_recursive
-#     from phiterm.workspace.ws_utils import get_ws_config_dir_path
-#     from phiterm.utils.git import GitCloneProgress
-#
-#     current_dir: Path = Path(".").resolve()
-#
-#     # Phidata should be initialized before creating a workspace
-#     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
-#     if not phi_conf:
-#         print_conf_not_available_msg()
-#         return False
-#
-#     # Check if a workspace with the same name exists
-#     _existing_ws_data: Optional[PhiWsData] = phi_conf.get_ws_data_by_name(ws_name)
-#     if _existing_ws_data is not None:
-#         logger.error(f"Found existing record for a workspace: {ws_name}")
-#         delete_existing_ws_data = typer.confirm(
-#             "Replace the existing record?", default=True
-#         )
-#         if delete_existing_ws_data:
-#             phi_conf.delete_ws(ws_name)
-#         else:
-#             return False
-#
-#     # Check if we can create the workspace in the current dir
-#     ws_root_path: Path = current_dir.joinpath(ws_name)
-#     if ws_root_path.exists():
-#         logger.error(
-#             f"Directory {ws_root_path} exists, please delete files manually or choose another name for workspace"
-#         )
-#         return False
-#
-#     print_info(f"Creating {str(ws_root_path)}")
-#     # Clone the starter repo for this cloud in the new directory
-#     repo_to_clone = TEMPLATE_TO_REPO_MAP.get(template)
-#     logger.debug("Cloning: {}".format(repo_to_clone))
-#     try:
-#         _cloned_git_repo: git.Repo = git.Repo.clone_from(
-#             repo_to_clone, str(ws_root_path), progress=GitCloneProgress()  # type: ignore
-#         )
-#     except Exception as e:
-#         logger.error(e)
-#         return False
-#
-#     # Remove existing .git folder
-#     _dot_git_folder = ws_root_path.joinpath(".git")
-#     _dot_git_exists = _dot_git_folder.exists()
-#     if _dot_git_exists:
-#         logger.debug(f"Deleting {_dot_git_folder}")
-#         try:
-#             _dot_git_exists = not rmdir_recursive(_dot_git_folder)
-#         except Exception as e:
-#             logger.warning(f"Failed to delete {_dot_git_folder}: {e}")
-#             logger.info("Please delete the .git folder manually")
-#             pass
-#
-#     phi_conf.add_new_ws_to_config(
-#         ws_name=ws_name,
-#         ws_root_path=ws_root_path,
-#     )
-#
-#     try:
-#         ws_config_dir_path: Path = get_ws_config_dir_path(ws_root_path)
-#         ws_config_secrets_dir = ws_config_dir_path.joinpath("secrets").resolve()
-#         ws_config_example_secrets_dir = ws_config_dir_path.joinpath(
-#             "example_secrets"
-#         ).resolve()
-#
-#         print_info(f"Creating {str(ws_config_secrets_dir)}")
-#         copytree(
-#             str(ws_config_example_secrets_dir),
-#             str(ws_config_secrets_dir),
-#         )
-#     except Exception as e:
-#         logger.warning(f"Could not create workspace/secrets: {e}")
-#         logger.warning(
-#             "Please manually copy workspace/example_secrets to workspace/secrets"
-#         )
-#
-#     print_info(f"Your new workspace is available at {str(ws_root_path)}\n")
-#     return setup_workspace(ws_root_path=ws_root_path)
-#
-#
-# def create_workspace_using_input():
-#     """Takes input from the user and calls create_new_workspace()"""
-#
-#     from phiterm.utils.common import is_empty, str_to_int
-#
-#     # Display available starter templates and ask user to select one
-#     print_info("Input Template Number (default: ai-app)")
-#     templates = WorkspaceStarterTemplate.values_list()
-#     for idx, prvdr in enumerate(templates, start=1):
-#         print_info("  [{}] {}".format(idx, prvdr))
-#
-#     # Get starter template from the user
-#     template_inp_raw = input(": ")
-#     # Convert input to int value.
-#     template_inp = str_to_int(template_inp_raw)
-#     template: WorkspaceStarterTemplate = WorkspaceStarterTemplate.api_app
-#
-#     if template_inp is not None:
-#         try:
-#             template = cast(
-#                 WorkspaceStarterTemplate,
-#                 WorkspaceStarterTemplate.from_str(templates[template_inp - 1]),
-#             )
-#         except Exception as e:
-#             logger.error(e)
-#     logger.debug("Selected: {}".format(template.value))
-#
-#     # Get workspace name from user
-#     default_ws_name = TEMPLATE_TO_NAME_MAP.get(template, DEFAULT_WS_NAME)
-#     ws_name_inp_raw = input(f"Workspace name (default: {default_ws_name}): ")
-#     if is_empty(ws_name_inp_raw):
-#         ws_name_inp_raw = default_ws_name
-#
-#     print_info(
-#         f"Creating workspace {ws_name_inp_raw} using the {template.value} template\n"
-#     )
-#     create_new_workspace(ws_name_inp_raw, template)
-#
-#
-# def initialize_workspace() -> None:
-#     """Initialize a phidata workspace.
-#
-#     This function is called by `phi ws create` to create a new workspace.
-#     """
-#     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
-#     if not phi_conf:
-#         print_conf_not_available_msg()
-#         return
-#
-#     print_heading("New phidata workspace")
-#     create_workspace_using_input()
-#
-# def print_git_setup(
-#     ws_name: str,
-#     ws_root_path: Path,
-#     version_control_provider: Optional[
-#         VersionControlProviderEnum
-#     ] = VersionControlProviderEnum.GITHUB,
-# ) -> None:
-#     """Prints commands to setup a remote git repo for a workspace"""
-#     from phiterm.utils.git import get_remote_origin_for_dir
-#
-#     # Check if a remote origin is available
-#     _remote_origin_url: Optional[str] = get_remote_origin_for_dir(ws_root_path)
-#     # logger.debug("_remote_origin_url: {}".format(_remote_origin_url))
-#     if _remote_origin_url:
-#         print_info(f"Remote origin already set: {_remote_origin_url}")
-#         return
-#
-#     create_new_git_repo_url = "https://github.com/new"
-#     create_remote_repo_url: str
-#     # TODO: Add more repo urls
-#     if version_control_provider == VersionControlProviderEnum.GITHUB:
-#         create_remote_repo_url = create_new_git_repo_url
-#     else:
-#         create_remote_repo_url = create_new_git_repo_url
-#
-#     print_subheading(f"\nSteps to setup a git repo for workspace: {ws_name}")
-#     print_info(f"\nCreate a new git repo named {ws_name} at {create_remote_repo_url}")
-#     print_info(
-#         f"Then follow the following steps to initialize the directory {ws_name} as a git repo and run git push"
-#     )
-#     print_info(
-#         f"NOTE: These steps will be provided by your version control provider (github, gitlab..), but would look something like:"
-#     )
-#     print_info(f"       git init")
-#     print_info(f"       git add .")
-#     print_info(f"       git commit -m 'Init Phidata Workspace'")
-#     print_info(f"       git branch -M main")
-#     print_info(
-#         f"       git remote add origin https://github.com/<USERNAME>/{ws_name}.git"
-#     )
-#     print_info(f"       git push -u origin main")
-#     print_info(f"Run `phi ws setup` after running git push to update your workspace\n")
-#
-#     _open_browser = typer.confirm(
-#         f"Would you like to open your browser to visit: {create_remote_repo_url}\n-->"
-#     )
-#     if _open_browser:
-#         typer.launch(create_remote_repo_url)
-#
-#
-# def clone_workspace(ws_to_clone: WorkspaceSchema, phi_conf: PhiConf) -> None:
-#     """Clones an available phidata workspace on the users machine. To clone a ws, the PhiConf
-#     already has the ws_data and ws_schema available. We then update the
-#     ws_root_path and ws_config_file_path in the ws_data. After updating the
-#     path, we're call setup_workspace() to go through our usual setup flow
-#     """
-#     from phiterm.utils.git import GitCloneProgress
-#     from phiterm.workspace.ws_utils import get_ws_config_file_path
-#
-#     # Check if we can create the workspace in the current dir
-#     current_dir: Path = Path("../../workspace").resolve()
-#     logger.debug(f"current_dir: {current_dir}")
-#     ws_root_path: Path = current_dir.joinpath(ws_to_clone.name)
-#     if ws_root_path.exists():
-#         logger.error(
-#             f"{ws_root_path} already exists, please choose another directory to clone or delete the existing dir and run `phi ws create` again"
-#         )
-#         return
-#
-#     print_info(f"Creating {str(ws_root_path)}")
-#     # Clone the workspace repo in ws_root_path
-#     repo_to_clone = ws_to_clone.git_url
-#     _cloned_git_repo: git.Repo = git.Repo.clone_from(
-#         repo_to_clone, str(ws_root_path), progress=GitCloneProgress()  # type: ignore
-#     )
-#     # Validate ws_root_path exists and is a directory
-#     if not (ws_root_path.exists() and ws_root_path.is_dir()):
-#         logger.error(f"Could not clone workspace, please try again")
-#         return
-#     # Get ws_config_file_path and validate
-#     ws_config_file_path: Path = get_ws_config_file_path(ws_root_path)
-#     if not (ws_config_file_path.exists() and ws_config_file_path.is_file()):
-#         logger.error(f"Could not find workspace config at: {ws_config_file_path}")
-#         return
-#     # Update the ws_data in PhiConf
-#     phi_conf.update_ws_data(
-#         ws_name=ws_to_clone.ws_name,
-#         ws_root_path=ws_root_path,
-#         ws_config_file_path=ws_config_file_path,
-#     )
-#     setup_workspace(ws_root_path)
-#
-#
-# def init_workspace_data(ws_schema: WorkspaceSchema, phi_conf: PhiConf):
-#     """Initializes workspace data like cloud projects"""
-#
-#     logger.debug("*=* Initializing workspace data for: {}".format(ws_schema.name))
-#     logger.debug("TO_BE_IMPLEMENTED")
-#     logger.debug("*=* Workspace data init complete: {}".format(ws_schema.name))
-#
-# def import_workspace():
-#     # TODO: use code to clone/import existing workspace later
-#     available_ws = phi_conf.available_ws
-#     if available_ws:
-#         print_info("Would you like to:")
-#         print_info("  [1] Create a new workspace")
-#         print_info("  [2] Clone an existing workspace")
-#         print_info("  [3] Enter any other key to exit")
-#         ws_inp_raw = input("--> ")
-#         ws_inp_int = str_to_int(ws_inp_raw)
-#         if ws_inp_int == 1:
-#             create_workspace_using_input()
-#         elif ws_inp_int == 2:
-#             print_info("\nSelect workspace to clone:")
-#             for idx, avl_ws in enumerate(available_ws, start=1):
-#                 print_info("  [{}] {}".format(idx, avl_ws.name))
-#             clone_ws_inp_raw = input("--> ")
-#             clone_ws_inp_int = str_to_int(clone_ws_inp_raw)
-#             if clone_ws_inp_int:
-#                 ws_to_clone = available_ws[clone_ws_inp_int - 1]
-#                 clone_workspace(ws_to_clone, phi_conf)
-#             return
-#         return
-#     else:
-#
```

### Comparing `phiterm-1.6.9/phiterm/workspace/ws_schemas.py` & `phiterm-1.7.0/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.9/phiterm/workspace/ws_utils.py` & `phiterm-1.7.0/phiterm/workspace/ws_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from typing import Dict, Optional, Set, Tuple
 
 from phiterm.conf.phi_conf import PhiWsData
 from phiterm.utils.cli_console import (
     print_info,
-    print_info,
     print_error,
     print_subheading,
 )
 from phiterm.utils.log import logger
 from phiterm.utils.pyproject import read_pyproject_phidata
 from phiterm.workspace.ws_enums import WorkspaceSetupActions
```

### Comparing `phiterm-1.6.9/phiterm.egg-info/SOURCES.txt` & `phiterm-1.7.0/phiterm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,19 @@
 phiterm/utils/__init__.py
 phiterm/utils/cli_auth_server.py
 phiterm/utils/cli_console.py
 phiterm/utils/common.py
 phiterm/utils/dttm.py
 phiterm/utils/enums.py
 phiterm/utils/filesystem.py
+phiterm/utils/get_python_objects_from_module.py
 phiterm/utils/git.py
 phiterm/utils/load_env.py
 phiterm/utils/log.py
+phiterm/utils/prep_infra_config.py
 phiterm/utils/pyproject.py
 phiterm/utils/ws_filter.py
 phiterm/workflow/__init__.py
 phiterm/workflow/exceptions.py
 phiterm/workflow/wf_enums.py
 phiterm/workflow/wf_operator.py
 phiterm/workflow/wf_utils.py
```

### Comparing `phiterm-1.6.9/pyproject.toml` & `phiterm-1.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.9"
+version = "1.7.0"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
@@ -14,15 +14,15 @@
     "kubernetes",
     "pydantic",
     "python-dotenv",
     "pyyaml",
     "rich",
     "tomli",
     "typer",
-    "typing-extensions",
+    "typing-extensions==4.5.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "black",
     "pytest",
```

