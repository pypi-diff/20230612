# Comparing `tmp/lab-partner-0.7.55.tar.gz` & `tmp/lab-partner-0.7.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.7.55.tar", last modified: Mon Jun 12 02:05:09 2023, max compression
+gzip compressed data, was "lab-partner-0.7.56.tar", last modified: Mon Jun 12 02:12:19 2023, max compression
```

## Comparing `lab-partner-0.7.55.tar` & `lab-partner-0.7.56.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.206467 lab-partner-0.7.55/
--rw-r--r--   0 root         (0) root         (0)     2847 2023-06-12 02:04:34.000000 lab-partner-0.7.55/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.194467 lab-partner-0.7.55/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.198467 lab-partner-0.7.55/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-12 02:04:34.000000 lab-partner-0.7.55/.github/workflows/build-deploy.yml
--rw-r--r--   0 root         (0) root         (0)     3519 2023-06-12 02:04:34.000000 lab-partner-0.7.55/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4228 2023-06-12 02:04:34.000000 lab-partner-0.7.55/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1094 2023-06-12 02:04:34.000000 lab-partner-0.7.55/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 02:05:09.206467 lab-partner-0.7.55/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-12 02:04:34.000000 lab-partner-0.7.55/README.md
--rwxr-xr-x   0 root         (0) root         (0)      841 2023-06-12 02:04:34.000000 lab-partner-0.7.55/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.194467 lab-partner-0.7.55/environments/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.198467 lab-partner-0.7.55/environments/local/
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     4368 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.202467 lab-partner-0.7.55/environments/local/telemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.202467 lab-partner-0.7.55/environments/local/telemetry/certs/
--rw-r--r--   0 root         (0) root         (0)      985 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/telemetry/certs/demo-data-prepper.crt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/telemetry/certs/demo-data-prepper.key
--rw-r--r--   0 root         (0) root         (0)     1444 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/telemetry/certs/root-ca.pem
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/telemetry/certs/test_keystore.p12
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/telemetry/data-prepper-config.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/telemetry/otel-collector-config.yml
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 02:04:34.000000 lab-partner-0.7.55/environments/local/telemetry/pipelines.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.198467 lab-partner-0.7.55/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.202467 lab-partner-0.7.55/images/cli/
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-12 02:04:34.000000 lab-partner-0.7.55/images/cli/bashrc
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-12 02:04:34.000000 lab-partner-0.7.55/images/cli/cli_sudoers
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 02:04:34.000000 lab-partner-0.7.55/images/cli/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       35 2023-06-12 02:04:34.000000 lab-partner-0.7.55/images/cli/start-cli.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.202467 lab-partner-0.7.55/images/jupyter/
--rw-r--r--   0 root         (0) root         (0)    33547 2023-06-12 02:04:34.000000 lab-partner-0.7.55/images/jupyter/jupyter_lab_config.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-12 02:04:34.000000 lab-partner-0.7.55/images/jupyter/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      363 2023-06-12 02:04:34.000000 lab-partner-0.7.55/images/jupyter/start-jupyter.sh
--rwxr-xr-x   0 root         (0) root         (0)      647 2023-06-12 02:04:34.000000 lab-partner-0.7.55/install_from_source.sh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-12 02:04:34.000000 lab-partner-0.7.55/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      280 2023-06-12 02:04:34.000000 lab-partner-0.7.55/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 02:05:09.206467 lab-partner-0.7.55/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.198467 lab-partner-0.7.55/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.202467 lab-partner-0.7.55/src/lab_partner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.206467 lab-partner-0.7.55/src/lab_partner/docker/
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4416 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/docker/daemon_info.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/docker/rootless_container.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/docker/run_builder.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/docker/unix_user.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/process_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2595 2023-06-12 02:04:34.000000 lab-partner-0.7.55/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.206467 lab-partner-0.7.55/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 02:05:09.000000 lab-partner-0.7.55/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-12 02:05:09.000000 lab-partner-0.7.55/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:05:09.000000 lab-partner-0.7.55/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-12 02:05:09.000000 lab-partner-0.7.55/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-12 02:05:09.000000 lab-partner-0.7.55/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 02:05:09.000000 lab-partner-0.7.55/src/lab_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.206467 lab-partner-0.7.55/tools/
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/README.md
--rw-r--r--   0 root         (0) root         (0)     1652 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      846 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.198467 lab-partner-0.7.55/tools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.206467 lab-partner-0.7.55/tools/src/lab_partner_tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/src/lab_partner_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:05:09.206467 lab-partner-0.7.55/tools/src/lab_partner_tools/compose/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/src/lab_partner_tools/dist.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/src/lab_partner_tools/services.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-12 02:04:34.000000 lab-partner-0.7.55/tools/src/lab_partner_tools/web_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.249570 lab-partner-0.7.56/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-12 02:11:54.000000 lab-partner-0.7.56/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.237569 lab-partner-0.7.56/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.241569 lab-partner-0.7.56/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-12 02:11:54.000000 lab-partner-0.7.56/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3519 2023-06-12 02:11:54.000000 lab-partner-0.7.56/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-06-12 02:11:54.000000 lab-partner-0.7.56/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-06-12 02:11:54.000000 lab-partner-0.7.56/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 02:12:19.249570 lab-partner-0.7.56/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-12 02:11:54.000000 lab-partner-0.7.56/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-06-12 02:11:54.000000 lab-partner-0.7.56/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.237569 lab-partner-0.7.56/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.241569 lab-partner-0.7.56/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.241569 lab-partner-0.7.56/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.241569 lab-partner-0.7.56/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-12 02:11:54.000000 lab-partner-0.7.56/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.237569 lab-partner-0.7.56/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.241569 lab-partner-0.7.56/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-12 02:11:54.000000 lab-partner-0.7.56/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-12 02:11:54.000000 lab-partner-0.7.56/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 02:11:54.000000 lab-partner-0.7.56/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-06-12 02:11:54.000000 lab-partner-0.7.56/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.245570 lab-partner-0.7.56/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-06-12 02:11:54.000000 lab-partner-0.7.56/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-12 02:11:54.000000 lab-partner-0.7.56/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-06-12 02:11:54.000000 lab-partner-0.7.56/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      647 2023-06-12 02:11:54.000000 lab-partner-0.7.56/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-12 02:11:54.000000 lab-partner-0.7.56/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-06-12 02:11:54.000000 lab-partner-0.7.56/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 02:12:19.249570 lab-partner-0.7.56/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.237569 lab-partner-0.7.56/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.245570 lab-partner-0.7.56/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.245570 lab-partner-0.7.56/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/docker/unix_user.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2595 2023-06-12 02:11:54.000000 lab-partner-0.7.56/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.245570 lab-partner-0.7.56/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-12 02:12:19.000000 lab-partner-0.7.56/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-12 02:12:19.000000 lab-partner-0.7.56/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:12:19.000000 lab-partner-0.7.56/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-12 02:12:19.000000 lab-partner-0.7.56/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-12 02:12:19.000000 lab-partner-0.7.56/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 02:12:19.000000 lab-partner-0.7.56/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.245570 lab-partner-0.7.56/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.241569 lab-partner-0.7.56/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.245570 lab-partner-0.7.56/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:12:19.245570 lab-partner-0.7.56/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-12 02:11:54.000000 lab-partner-0.7.56/tools/src/lab_partner_tools/web_proxy.py
```

### Comparing `lab-partner-0.7.55/.gitattributes` & `lab-partner-0.7.56/.gitattributes`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/.github/workflows/build-deploy.yml` & `lab-partner-0.7.56/.github/workflows/build-deploy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/.gitignore` & `lab-partner-0.7.56/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/Dockerfile` & `lab-partner-0.7.56/Dockerfile`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/LICENSE.md` & `lab-partner-0.7.56/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/PKG-INFO` & `lab-partner-0.7.56/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.55
+Version: 0.7.56
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.55/build.sh` & `lab-partner-0.7.56/build.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/environments/local/docker-compose.yml` & `lab-partner-0.7.56/environments/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/environments/local/telemetry/certs/demo-data-prepper.crt` & `lab-partner-0.7.56/environments/local/telemetry/certs/demo-data-prepper.crt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/environments/local/telemetry/certs/demo-data-prepper.key` & `lab-partner-0.7.56/environments/local/telemetry/certs/demo-data-prepper.key`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/environments/local/telemetry/certs/root-ca.pem` & `lab-partner-0.7.56/environments/local/telemetry/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/environments/local/telemetry/certs/test_keystore.p12` & `lab-partner-0.7.56/environments/local/telemetry/certs/test_keystore.p12`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/environments/local/telemetry/pipelines.yaml` & `lab-partner-0.7.56/environments/local/telemetry/pipelines.yaml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/images/cli/bashrc` & `lab-partner-0.7.56/images/cli/bashrc`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/images/jupyter/jupyter_lab_config.py` & `lab-partner-0.7.56/images/jupyter/jupyter_lab_config.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/install_from_source.sh` & `lab-partner-0.7.56/install_from_source.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/pyproject.toml` & `lab-partner-0.7.56/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/src/lab_partner/docker/daemon_info.py` & `lab-partner-0.7.56/src/lab_partner/docker/daemon_info.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/src/lab_partner/docker/rootless_container.py` & `lab-partner-0.7.56/src/lab_partner/docker/rootless_container.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/src/lab_partner/docker/run_builder.py` & `lab-partner-0.7.56/src/lab_partner/docker/run_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/src/lab_partner/docker/unix_user.py` & `lab-partner-0.7.56/src/lab_partner/docker/unix_user.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/src/lab_partner/process_utils.py` & `lab-partner-0.7.56/src/lab_partner/process_utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/src/lab_partner/start_cli.py` & `lab-partner-0.7.56/src/lab_partner/start_cli.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/src/lab_partner.egg-info/PKG-INFO` & `lab-partner-0.7.56/src/lab_partner.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.55
+Version: 0.7.56
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.55/src/lab_partner.egg-info/SOURCES.txt` & `lab-partner-0.7.56/src/lab_partner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/tools/pyproject.toml` & `lab-partner-0.7.56/tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/tools/setup.cfg` & `lab-partner-0.7.56/tools/setup.cfg`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml` & `lab-partner-0.7.56/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/tools/src/lab_partner_tools/dist.py` & `lab-partner-0.7.56/tools/src/lab_partner_tools/dist.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/tools/src/lab_partner_tools/services.py` & `lab-partner-0.7.56/tools/src/lab_partner_tools/services.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.55/tools/src/lab_partner_tools/web_proxy.py` & `lab-partner-0.7.56/tools/src/lab_partner_tools/web_proxy.py`

 * *Files identical despite different names*

