# Comparing `tmp/lab-partner-0.7.51.tar.gz` & `tmp/lab-partner-0.7.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.7.51.tar", last modified: Mon Jun 12 00:50:14 2023, max compression
+gzip compressed data, was "lab-partner-0.7.52.tar", last modified: Mon Jun 12 00:56:53 2023, max compression
```

## Comparing `lab-partner-0.7.51.tar` & `lab-partner-0.7.52.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/
--rw-r--r--   0 root         (0) root         (0)     2847 2023-06-12 00:49:39.000000 lab-partner-0.7.51/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-12 00:49:39.000000 lab-partner-0.7.51/.github/workflows/build-deploy.yml
--rw-r--r--   0 root         (0) root         (0)     3519 2023-06-12 00:49:39.000000 lab-partner-0.7.51/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4225 2023-06-12 00:49:39.000000 lab-partner-0.7.51/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1094 2023-06-12 00:49:39.000000 lab-partner-0.7.51/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 00:50:14.160714 lab-partner-0.7.51/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-12 00:49:39.000000 lab-partner-0.7.51/README.md
--rwxr-xr-x   0 root         (0) root         (0)      841 2023-06-12 00:49:39.000000 lab-partner-0.7.51/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/environments/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/environments/local/
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     4368 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/environments/local/telemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/environments/local/telemetry/certs/
--rw-r--r--   0 root         (0) root         (0)      985 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.crt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.key
--rw-r--r--   0 root         (0) root         (0)     1444 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/root-ca.pem
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/certs/test_keystore.p12
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/data-prepper-config.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/otel-collector-config.yml
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 00:49:39.000000 lab-partner-0.7.51/environments/local/telemetry/pipelines.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/images/cli/
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/bashrc
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/cli_sudoers
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       35 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/cli/start-cli.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/images/jupyter/
--rw-r--r--   0 root         (0) root         (0)    33547 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/jupyter/jupyter_lab_config.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/jupyter/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      363 2023-06-12 00:49:39.000000 lab-partner-0.7.51/images/jupyter/start-jupyter.sh
--rwxr-xr-x   0 root         (0) root         (0)      647 2023-06-12 00:49:39.000000 lab-partner-0.7.51/install_from_source.sh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-12 00:49:39.000000 lab-partner-0.7.51/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      280 2023-06-12 00:49:39.000000 lab-partner-0.7.51/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 00:50:14.160714 lab-partner-0.7.51/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.156714 lab-partner-0.7.51/src/lab_partner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/src/lab_partner/docker/
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4416 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/daemon_info.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/rootless_container.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/run_builder.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/docker/unix_user.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/process_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2595 2023-06-12 00:49:39.000000 lab-partner-0.7.51/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 00:50:14.000000 lab-partner-0.7.51/src/lab_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/tools/
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/README.md
--rw-r--r--   0 root         (0) root         (0)     1652 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      846 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.152713 lab-partner-0.7.51/tools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/tools/src/lab_partner_tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:50:14.160714 lab-partner-0.7.51/tools/src/lab_partner_tools/compose/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/dist.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/services.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-12 00:49:39.000000 lab-partner-0.7.51/tools/src/lab_partner_tools/web_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.753031 lab-partner-0.7.52/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-12 00:56:10.000000 lab-partner-0.7.52/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.745030 lab-partner-0.7.52/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.745030 lab-partner-0.7.52/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-12 00:56:10.000000 lab-partner-0.7.52/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3519 2023-06-12 00:56:10.000000 lab-partner-0.7.52/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-06-12 00:56:10.000000 lab-partner-0.7.52/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-06-12 00:56:10.000000 lab-partner-0.7.52/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 00:56:53.753031 lab-partner-0.7.52/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-12 00:56:10.000000 lab-partner-0.7.52/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-06-12 00:56:10.000000 lab-partner-0.7.52/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.745030 lab-partner-0.7.52/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.749030 lab-partner-0.7.52/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.749030 lab-partner-0.7.52/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.749030 lab-partner-0.7.52/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 00:56:10.000000 lab-partner-0.7.52/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.745030 lab-partner-0.7.52/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.749030 lab-partner-0.7.52/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-12 00:56:10.000000 lab-partner-0.7.52/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-12 00:56:10.000000 lab-partner-0.7.52/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 00:56:10.000000 lab-partner-0.7.52/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-06-12 00:56:10.000000 lab-partner-0.7.52/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.749030 lab-partner-0.7.52/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-06-12 00:56:10.000000 lab-partner-0.7.52/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-12 00:56:10.000000 lab-partner-0.7.52/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-06-12 00:56:10.000000 lab-partner-0.7.52/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      647 2023-06-12 00:56:10.000000 lab-partner-0.7.52/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-12 00:56:10.000000 lab-partner-0.7.52/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-06-12 00:56:10.000000 lab-partner-0.7.52/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 00:56:53.753031 lab-partner-0.7.52/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.745030 lab-partner-0.7.52/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.749030 lab-partner-0.7.52/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.753031 lab-partner-0.7.52/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/docker/unix_user.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2595 2023-06-12 00:56:10.000000 lab-partner-0.7.52/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.753031 lab-partner-0.7.52/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 00:56:53.000000 lab-partner-0.7.52/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-12 00:56:53.000000 lab-partner-0.7.52/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 00:56:53.000000 lab-partner-0.7.52/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-12 00:56:53.000000 lab-partner-0.7.52/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-12 00:56:53.000000 lab-partner-0.7.52/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 00:56:53.000000 lab-partner-0.7.52/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.753031 lab-partner-0.7.52/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.745030 lab-partner-0.7.52/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.753031 lab-partner-0.7.52/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 00:56:53.753031 lab-partner-0.7.52/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-12 00:56:10.000000 lab-partner-0.7.52/tools/src/lab_partner_tools/web_proxy.py
```

### Comparing `lab-partner-0.7.51/.gitattributes` & `lab-partner-0.7.52/.gitattributes`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/.github/workflows/build-deploy.yml` & `lab-partner-0.7.52/.github/workflows/build-deploy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/.gitignore` & `lab-partner-0.7.52/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/Dockerfile` & `lab-partner-0.7.52/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
   && rm -rf /tmp/act*
 
 COPY images/cli/requirements.txt /tmp/cli-requirements.txt
 RUN echo "Installing Python dependencies" \
   && pip install --upgrade pip \
   && pip install -r /tmp/cli-requirements.txt
 
-COPY --from=lab_packages ${LAB_DIST} ${LAB_DIST}
-RUN echo "Installing Lab Partner utilities" \
-    && pip install ${LAB_DIST}/utils/lab_partner_utils-${LAB_VERSION}-py3-none-any.whl
+#COPY --from=lab_packages ${LAB_DIST} ${LAB_DIST}
+#RUN echo "Installing Lab Partner utilities" \
+#    && pip install ${LAB_DIST}/utils/lab_partner_utils-${LAB_VERSION}-py3-none-any.whl
 
 COPY images/cli/bashrc ${HOME}/.bashrc
 COPY images/cli/start-cli.sh /opt/bin/
 COPY environments/local /opt/lab/
 COPY images/cli/cli_sudoers /etc/sudoers.d/
 
 CMD ["/opt/bin/start-cli.sh"]
```

### Comparing `lab-partner-0.7.51/LICENSE.md` & `lab-partner-0.7.52/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/PKG-INFO` & `lab-partner-0.7.52/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.51
+Version: 0.7.52
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.51/build.sh` & `lab-partner-0.7.52/build.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/environments/local/docker-compose.yml` & `lab-partner-0.7.52/environments/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.crt` & `lab-partner-0.7.52/environments/local/telemetry/certs/demo-data-prepper.crt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/environments/local/telemetry/certs/demo-data-prepper.key` & `lab-partner-0.7.52/environments/local/telemetry/certs/demo-data-prepper.key`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/environments/local/telemetry/certs/root-ca.pem` & `lab-partner-0.7.52/environments/local/telemetry/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/environments/local/telemetry/certs/test_keystore.p12` & `lab-partner-0.7.52/environments/local/telemetry/certs/test_keystore.p12`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/environments/local/telemetry/pipelines.yaml` & `lab-partner-0.7.52/environments/local/telemetry/pipelines.yaml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/images/cli/bashrc` & `lab-partner-0.7.52/images/cli/bashrc`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/images/jupyter/jupyter_lab_config.py` & `lab-partner-0.7.52/images/jupyter/jupyter_lab_config.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/install_from_source.sh` & `lab-partner-0.7.52/install_from_source.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/pyproject.toml` & `lab-partner-0.7.52/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/src/lab_partner/docker/daemon_info.py` & `lab-partner-0.7.52/src/lab_partner/docker/daemon_info.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/src/lab_partner/docker/rootless_container.py` & `lab-partner-0.7.52/src/lab_partner/docker/rootless_container.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/src/lab_partner/docker/run_builder.py` & `lab-partner-0.7.52/src/lab_partner/docker/run_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/src/lab_partner/docker/unix_user.py` & `lab-partner-0.7.52/src/lab_partner/docker/unix_user.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/src/lab_partner/process_utils.py` & `lab-partner-0.7.52/src/lab_partner/process_utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/src/lab_partner/start_cli.py` & `lab-partner-0.7.52/src/lab_partner/start_cli.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/src/lab_partner.egg-info/PKG-INFO` & `lab-partner-0.7.52/src/lab_partner.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.51
+Version: 0.7.52
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.51/src/lab_partner.egg-info/SOURCES.txt` & `lab-partner-0.7.52/src/lab_partner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/tools/pyproject.toml` & `lab-partner-0.7.52/tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/tools/setup.cfg` & `lab-partner-0.7.52/tools/setup.cfg`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml` & `lab-partner-0.7.52/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/tools/src/lab_partner_tools/dist.py` & `lab-partner-0.7.52/tools/src/lab_partner_tools/dist.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/tools/src/lab_partner_tools/services.py` & `lab-partner-0.7.52/tools/src/lab_partner_tools/services.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.51/tools/src/lab_partner_tools/web_proxy.py` & `lab-partner-0.7.52/tools/src/lab_partner_tools/web_proxy.py`

 * *Files identical despite different names*

