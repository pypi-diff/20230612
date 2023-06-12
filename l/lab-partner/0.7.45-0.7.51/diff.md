# Comparing `tmp/lab-partner-0.7.45.tar.gz` & `tmp/lab-partner-0.7.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.7.45.tar", last modified: Tue May 30 00:35:07 2023, max compression
+gzip compressed data, was "lab-partner-0.7.51.tar", last modified: Mon Jun 12 00:50:14 2023, max compression
```

## Comparing `lab-partner-0.7.45.tar` & `lab-partner-0.7.51.tar`

### file list

```diff
@@ -1,81 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.739121 lab-partner-0.7.45/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.711121 lab-partner-0.7.45/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.719121 lab-partner-0.7.45/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-05-30 00:34:39.000000 lab-partner-0.7.45/.github/workflows/build-deploy.yml
--rw-r--r--   0 root         (0) root         (0)     3537 2023-05-30 00:34:39.000000 lab-partner-0.7.45/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4298 2023-05-30 00:34:39.000000 lab-partner-0.7.45/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-30 00:34:39.000000 lab-partner-0.7.45/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-30 00:35:07.739121 lab-partner-0.7.45/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-30 00:34:39.000000 lab-partner-0.7.45/README.md
--rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-30 00:34:39.000000 lab-partner-0.7.45/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.711121 lab-partner-0.7.45/environments/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.719121 lab-partner-0.7.45/environments/local/
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     4368 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.719121 lab-partner-0.7.45/environments/local/telemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.723121 lab-partner-0.7.45/environments/local/telemetry/certs/
--rw-r--r--   0 root         (0) root         (0)      985 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/telemetry/certs/demo-data-prepper.crt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/telemetry/certs/demo-data-prepper.key
--rw-r--r--   0 root         (0) root         (0)     1444 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/telemetry/certs/root-ca.pem
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/telemetry/certs/test_keystore.p12
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/telemetry/data-prepper-config.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/telemetry/otel-collector-config.yml
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-30 00:34:39.000000 lab-partner-0.7.45/environments/local/telemetry/pipelines.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.715121 lab-partner-0.7.45/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.727121 lab-partner-0.7.45/images/cli/
--rw-r--r--   0 root         (0) root         (0)      716 2023-05-30 00:34:39.000000 lab-partner-0.7.45/images/cli/bashrc
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-30 00:34:39.000000 lab-partner-0.7.45/images/cli/cli_sudoers
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 00:34:39.000000 lab-partner-0.7.45/images/cli/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-30 00:34:39.000000 lab-partner-0.7.45/images/cli/start-cli.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.727121 lab-partner-0.7.45/images/jupyter/
--rw-r--r--   0 root         (0) root         (0)    33547 2023-05-30 00:34:39.000000 lab-partner-0.7.45/images/jupyter/jupyter_lab_config.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-30 00:34:39.000000 lab-partner-0.7.45/images/jupyter/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-30 00:34:39.000000 lab-partner-0.7.45/images/jupyter/start-jupyter.sh
--rwxr-xr-x   0 root         (0) root         (0)      647 2023-05-30 00:34:39.000000 lab-partner-0.7.45/install_from_source.sh
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-30 00:34:39.000000 lab-partner-0.7.45/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-30 00:34:39.000000 lab-partner-0.7.45/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 00:35:07.739121 lab-partner-0.7.45/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.715121 lab-partner-0.7.45/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.727121 lab-partner-0.7.45/src/lab_partner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.731121 lab-partner-0.7.45/src/lab_partner/docker/
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4416 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/docker/daemon_info.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/docker/rootless_container.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/docker/run_builder.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/docker/unix_user.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/process_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2595 2023-05-30 00:34:39.000000 lab-partner-0.7.45/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.731121 lab-partner-0.7.45/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-30 00:35:07.000000 lab-partner-0.7.45/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1916 2023-05-30 00:35:07.000000 lab-partner-0.7.45/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:35:07.000000 lab-partner-0.7.45/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-30 00:35:07.000000 lab-partner-0.7.45/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-30 00:35:07.000000 lab-partner-0.7.45/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-30 00:35:07.000000 lab-partner-0.7.45/src/lab_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.735121 lab-partner-0.7.45/tools/
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/README.md
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.715121 lab-partner-0.7.45/tools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.735121 lab-partner-0.7.45/tools/src/lab_partner_tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/src/lab_partner_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.735121 lab-partner-0.7.45/tools/src/lab_partner_tools/compose/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/src/lab_partner_tools/dist.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/src/lab_partner_tools/services.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-30 00:34:39.000000 lab-partner-0.7.45/tools/src/lab_partner_tools/web_proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.735121 lab-partner-0.7.45/utils/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/README.md
--rw-r--r--   0 root         (0) root         (0)     1743 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/run.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.715121 lab-partner-0.7.45/utils/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:07.739121 lab-partner-0.7.45/utils/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-30 00:34:39.000000 lab-partner-0.7.45/utils/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-12 00:49:39.000000 lab-partner-0.7.51/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-12 00:49:39.000000 lab-partner-0.7.51/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3519 2023-06-12 00:49:39.000000 lab-partner-0.7.51/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-06-12 00:49:39.000000 lab-partner-0.7.51/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-06-12 00:49:39.000000 lab-partner-0.7.51/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 00:50:14.160714 lab-partner-0.7.51/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-12 00:49:39.000000 lab-partner-0.7.51/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-06-12 00:49:39.000000 lab-partner-0.7.51/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      647 2023-06-12 00:49:39.000000 lab-partner-0.7.51/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-12 00:49:39.000000 lab-partner-0.7.51/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-06-12 00:49:39.000000 lab-partner-0.7.51/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 00:50:14.160714 lab-partner-0.7.51/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/unix_user.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2595 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/web_proxy.py
```

### Comparing `lab-partner-0.7.45/.github/workflows/build-deploy.yml` & `lab-partner-0.7.51/.github/workflows/build-deploy.yml`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,14 @@
           target: lab_packages
           tags: ${{ env.DOCKERHUB_USERNAME }}/lab-partner-packages:${{ github.ref_name }}
       - name: Copy python wheels from docker image
         run: |
           container_id=$(docker create ${{ env.DOCKERHUB_USERNAME }}/lab-partner-packages:${{ github.ref_name }}) \
           && mkdir -p dist \
           && docker cp ${container_id}:/opt/lab/dist/init/. dist/ \
-          && docker cp ${container_id}:/opt/lab/dist/utils/. dist/ \
           && docker rm -f ${container_id}
       - name: Publish package distributions to PyPI
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           verbose: true
           print-hash: true
```

### Comparing `lab-partner-0.7.45/.gitignore` & `lab-partner-0.7.51/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-data
-node_modules
 .idea
 
 ##
 # Python
 ##
 
 # Byte-compiled / optimized / DLL files
```

### Comparing `lab-partner-0.7.45/Dockerfile` & `lab-partner-0.7.51/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 RUN pip install --upgrade pip build \
     && mkdir -p ${LAB_DIST}
 
 RUN cd ${LAB_BUILD} \
     && python -m build \
     && cp -R ${LAB_BUILD}/dist ${LAB_DIST}/init
 
-RUN cd ${LAB_BUILD}/utils \
-    && sed -i "s|^version.*|version = \"${LAB_VERSION}\"|" pyproject.toml \
-    && python -m build \
-    && cp -R ${LAB_BUILD}/utils/dist ${LAB_DIST}/utils
+#RUN cd ${LAB_BUILD} \
+#    && python -m build utils \
+#    && cp -R ${LAB_BUILD}/utils/dist ${LAB_DIST}/utils
 
 #RUN cd ${LAB_BUILD}/tools \
 #    && sed -i "s|^version.*|version = \"${LAB_VERSION}\"|" pyproject.toml \
 #    && python -m build \
 #    && cp -R ${LAB_BUILD}/tools/dist ${LAB_DIST}/tools
 
 #################################################################
```

### Comparing `lab-partner-0.7.45/LICENSE.md` & `lab-partner-0.7.51/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/PKG-INFO` & `lab-partner-0.7.51/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.45
+Version: 0.7.51
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.45/build.sh` & `lab-partner-0.7.51/build.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/environments/local/docker-compose.yml` & `lab-partner-0.7.51/environments/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/environments/local/telemetry/certs/demo-data-prepper.crt` & `lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.crt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/environments/local/telemetry/certs/demo-data-prepper.key` & `lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.key`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/environments/local/telemetry/certs/root-ca.pem` & `lab-partner-0.7.51/environments/local/telemetry/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/environments/local/telemetry/certs/test_keystore.p12` & `lab-partner-0.7.51/environments/local/telemetry/certs/test_keystore.p12`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/environments/local/telemetry/pipelines.yaml` & `lab-partner-0.7.51/environments/local/telemetry/pipelines.yaml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/images/cli/bashrc` & `lab-partner-0.7.51/images/cli/bashrc`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/images/jupyter/jupyter_lab_config.py` & `lab-partner-0.7.51/images/jupyter/jupyter_lab_config.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/install_from_source.sh` & `lab-partner-0.7.51/install_from_source.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/pyproject.toml` & `lab-partner-0.7.51/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lab-partner"
 #version = "0.7.34"
 description = "A toolkit that partners with you to build software projects"
 dynamic = ["version", "readme"]
@@ -38,15 +38,14 @@
 homepage = "https://github.com/enclarify/lab-partner"
 # documentation = "https://github.com/enclarify/lab-partner"
 # changelog = "https://github.com/enclarify/lab-partner"
 
 [tool.setuptools_scm]
 version_scheme = "no-guess-dev"
 local_scheme="no-local-version"
-git_describe_command = "git describe --dirty --tags --long --match v* --first-parent"
 
 [tool.setuptools.dynamic]
 version = { attr = "setuptools_scm.get_version" }
 readme = {file = ["README.md"]}
 
 [tool.setuptools]
 package-dir = {"" = "src"}
```

### Comparing `lab-partner-0.7.45/src/lab_partner/docker/daemon_info.py` & `lab-partner-0.7.51/src/lab_partner/docker/daemon_info.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/src/lab_partner/docker/rootless_container.py` & `lab-partner-0.7.51/src/lab_partner/docker/rootless_container.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/src/lab_partner/docker/run_builder.py` & `lab-partner-0.7.51/src/lab_partner/docker/run_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/src/lab_partner/docker/unix_user.py` & `lab-partner-0.7.51/src/lab_partner/docker/unix_user.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/src/lab_partner/process_utils.py` & `lab-partner-0.7.51/src/lab_partner/process_utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/src/lab_partner/start_cli.py` & `lab-partner-0.7.51/src/lab_partner/start_cli.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/src/lab_partner.egg-info/PKG-INFO` & `lab-partner-0.7.51/src/lab_partner.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.45
+Version: 0.7.51
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.45/src/lab_partner.egg-info/SOURCES.txt` & `lab-partner-0.7.51/src/lab_partner.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.gitattributes
 .gitignore
 Dockerfile
 LICENSE.md
 README.md
 build.sh
 install_from_source.sh
 pyproject.toml
@@ -41,18 +42,8 @@
 tools/README.md
 tools/pyproject.toml
 tools/setup.cfg
 tools/src/lab_partner_tools/__init__.py
 tools/src/lab_partner_tools/dist.py
 tools/src/lab_partner_tools/services.py
 tools/src/lab_partner_tools/web_proxy.py
-tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
-utils/LICENSE.md
-utils/README.md
-utils/pyproject.toml
-utils/run.sh
-utils/src/lab_partner_utils/__init__.py
-utils/src/lab_partner_utils/cli_command_factory.py
-utils/src/lab_partner_utils/command_builder.py
-utils/src/lab_partner_utils/commands.py
-utils/src/lab_partner_utils/kernel_launcher.py
-utils/src/lab_partner_utils/utils.py
+tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
```

### Comparing `lab-partner-0.7.45/tools/pyproject.toml` & `lab-partner-0.7.51/tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/tools/setup.cfg` & `lab-partner-0.7.51/tools/setup.cfg`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml` & `lab-partner-0.7.51/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/tools/src/lab_partner_tools/dist.py` & `lab-partner-0.7.51/tools/src/lab_partner_tools/dist.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/tools/src/lab_partner_tools/services.py` & `lab-partner-0.7.51/tools/src/lab_partner_tools/services.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.45/tools/src/lab_partner_tools/web_proxy.py` & `lab-partner-0.7.51/tools/src/lab_partner_tools/web_proxy.py`

 * *Files identical despite different names*

