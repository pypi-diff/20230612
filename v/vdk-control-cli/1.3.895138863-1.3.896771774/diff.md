# Comparing `tmp/vdk-control-cli-1.3.895138863.tar.gz` & `tmp/vdk-control-cli-1.3.896771774.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.895138863.tar", last modified: Fri Jun  9 13:38:08 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.896771774.tar", last modified: Mon Jun 12 08:45:26 2023, max compression
```

## Comparing `vdk-control-cli-1.3.895138863.tar` & `vdk-control-cli-1.3.896771774.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    11236 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14343 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    12040 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9834 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-09 13:37:55.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2371 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-09 13:37:55.000000 vdk-control-cli-1.3.895138863/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14343 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    12040 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-12 08:45:11.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-12 08:45:15.000000 vdk-control-cli-1.3.896771774/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-12 08:45:26.000000 vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-12 08:45:15.000000 vdk-control-cli-1.3.896771774/version.txt
```

### Comparing `vdk-control-cli-1.3.895138863/PKG-INFO` & `vdk-control-cli-1.3.896771774/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.895138863
+Version: 1.3.896771774
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.895138863/README.md` & `vdk-control-cli-1.3.896771774/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/setup.cfg` & `vdk-control-cli-1.3.896771774/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.896771774/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,25 +26,31 @@
 class JobCreate:
     def __init__(self, rest_api_url: str):
         self.__rest_api_url = rest_api_url
         self.__vdk_config = VDKConfig()
 
     @ApiClientErrorDecorator()
     def create_job(
-        self, name: str, team: str, path: str, cloud: bool, local: bool
+        self,
+        name: str,
+        team: str,
+        path: str,
+        cloud: bool,
+        local: bool,
+        sample_job_directory: pathlib.Path = None,
     ) -> None:
         self.__validate_job_name(name)
         if local:
             self.validate_job_path(path, name)
 
         if cloud:
             self.__create_cloud_job(team, name)
         if local:
             job_path = self.__get_job_path(path, name)
-            self.__create_local_job(team, name, job_path)
+            self.__create_local_job(team, name, job_path, sample_job_directory)
             if cloud:
                 self.__download_key(team, name, path)
 
     def __create_cloud_job(self, team: str, name: str) -> None:
         jobs_api = ApiClientFactory(self.__rest_api_url).get_jobs_api()
         job_config = DataJobConfig(schedule=DataJobSchedule())
         # TODO: currently there's bug and description is not persisted, so it's not exposed to CLI for now
@@ -59,23 +65,52 @@
                 )
             else:
                 raise
         log.info(
             f"Data Job with name {name} created and registered in cloud runtime by Control Service."
         )
 
-    def __create_local_job(self, team: str, name: str, job_path: str) -> None:
-        sample_job = self.__vdk_config.sample_job_directory
+    def __create_local_job(
+        self, team: str, name: str, job_path: str, sample_job_directory: pathlib.Path
+    ) -> None:
+        sample_job = self.__create_sample_job_dir(sample_job_directory)
         log.debug(f"Create sample job from directory: {sample_job} into {job_path}")
         cli_utils.copy_directory(sample_job, job_path)
         local_config = JobConfig(job_path)
         if not local_config.set_team_if_exists(team):
             log.warning(f"Failed to write Data Job team {team} in config.ini.")
         log.info(f"Data Job with name {name} created locally in {job_path}.")
 
+    def __create_sample_job_dir(self, sample_job_directory: pathlib.Path):
+        """
+        This method generates the directory for the sample job which will be created when invoking `vdk create`.
+        Its control flow is as follows:
+         - if the configuration variable VDK_CONTROL_SAMPLE_JOB_DIRECTORY is set, it takes precedent over
+         everything else
+         - next, if a sample_job_directory is passed to the method by its invoking class, it takes precedent next; the
+         purpose of this is to allow plugins and extensions to set a new default sample job, but still not overwrite
+         one which was set by the user
+         - finally, the default sample job is used
+
+        :param sample_job_directory: a Python module containing the files for a sample job
+        :return: an absolute path in the current environment where the sample job is so the files located there can
+        be copied over to the target directory when creating a new job
+        """
+        if self.__vdk_config.sample_job_directory:
+            return self.__vdk_config.sample_job_directory
+
+        if sample_job_directory:
+            return sample_job_directory
+
+        import vdk.internal.control.job.sample_job
+
+        template_module_path = vdk.internal.control.job.sample_job.__path__._path[0]
+
+        return os.path.abspath(template_module_path)
+
     def __download_key(self, team, name, path):
         job_download_key = JobDownloadKey(self.__rest_api_url)
         try:
             log.info("Will download keytab of the job now ...")
             job_download_key.download(team, name, path)
         except Exception as e:
             log.warning(
```

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,21 +125,15 @@
             "true",
             "1",
             "t",
         )
 
     @property
     def sample_job_directory(self) -> str:
-        sample_job_dir = os.getenv("VDK_CONTROL_SAMPLE_JOB_DIRECTORY", None)
-        if not sample_job_dir:
-            import vdk.internal.control.job.sample_job
-
-            template_module_path = vdk.internal.control.job.sample_job.__path__._path[0]
-            sample_job_dir = os.path.abspath(template_module_path)
-        return sample_job_dir
+        return os.getenv("VDK_CONTROL_SAMPLE_JOB_DIRECTORY", None)
 
 
 class VDKConfigFolder:
     """
     A class responsible for managing the configuration files in the vdk configuration
     folder
     """
```

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.896771774/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.895138863
+Version: 1.3.896771774
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.896771774/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

