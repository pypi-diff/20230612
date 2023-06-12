# Comparing `tmp/fabric-credmgr-1.4.0.tar.gz` & `tmp/fabric-credmgr-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-credmgr-1.4.0.tar", last modified: Thu Jan 19 19:28:37 2023, max compression
+gzip compressed data, was "fabric-credmgr-1.5.0.tar", last modified: Mon Jun 12 18:35:22 2023, max compression
```

## Comparing `fabric-credmgr-1.4.0.tar` & `fabric-credmgr-1.5.0.tar`

### file list

```diff
@@ -1,92 +1,117 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.295639 fabric-credmgr-1.4.0/
--rw-r--r--   0 kthare10   (503) staff       (20)     1071 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)       59 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/MANIFEST.in
--rw-r--r--   0 kthare10   (503) staff       (20)    17615 2023-01-19 19:28:37.294930 fabric-credmgr-1.4.0/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)    17107 2023-01-19 19:25:25.000000 fabric-credmgr-1.4.0/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.240874 fabric-credmgr-1.4.0/fabric_cm/
--rw-r--r--   0 kthare10   (503) staff       (20)       96 2023-01-04 15:58:40.000000 fabric-credmgr-1.4.0/fabric_cm/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.241414 fabric-credmgr-1.4.0/fabric_cm/credmgr/
--rw-r--r--   0 kthare10   (503) staff       (20)     2422 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/__init__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.242430 fabric-credmgr-1.4.0/fabric_cm/credmgr/common/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/common/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1313 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/common/exceptions.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.244630 fabric-credmgr-1.4.0/fabric_cm/credmgr/config/
--rw-r--r--   0 kthare10   (503) staff       (20)     1295 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/config/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     9183 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/config/config.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.246876 fabric-credmgr-1.4.0/fabric_cm/credmgr/credential_managers/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/credential_managers/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2967 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/credential_managers/abstract_credential_manager.py
--rw-r--r--   0 kthare10   (503) staff       (20)     9595 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/credential_managers/oauth_credmgr.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.249476 fabric-credmgr-1.4.0/fabric_cm/credmgr/external_apis/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/external_apis/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5298 2022-12-15 16:46:05.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/external_apis/core_api.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4814 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/external_apis/ldap.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.251676 fabric-credmgr-1.4.0/fabric_cm/credmgr/logging/
--rw-r--r--   0 kthare10   (503) staff       (20)     1263 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/logging/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2724 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/logging/log.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.256583 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/
--rw-r--r--   0 kthare10   (503) staff       (20)     1571 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2207 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/__main__.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.260083 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/controllers/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/controllers/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)      151 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/controllers/authorization_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)      333 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/controllers/default_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1774 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/controllers/tokens_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)      295 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/controllers/version_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)      626 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/encoder.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.275910 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/
--rw-r--r--   0 kthare10   (503) staff       (20)     1910 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1884 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/base_model_.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1601 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/jwks.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4628 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/jwks_keys.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1871 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3881 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2454 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content_data.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2860 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status200_ok_single.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1968 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4493 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3969 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2502 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3864 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2451 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3831 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status404_not_found.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2436 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status404_not_found_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4218 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2625 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error_errors.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3515 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/token.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3439 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/tokens.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3520 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/version.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2526 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/version_data.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.281581 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)      126 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/authorization_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1558 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/constants.py
--rw-r--r--   0 kthare10   (503) staff       (20)     5429 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/cors_response.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2187 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/default_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)     6842 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/tokens_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)     1285 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/version_controller.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.282325 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/swagger/
--rw-r--r--   0 kthare10   (503) staff       (20)    13635 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/swagger/swagger.yaml
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.287013 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/
--rw-r--r--   0 kthare10   (503) staff       (20)      433 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)      873 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/test_default_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)     2681 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/test_tokens_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)      840 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/test_version_controller.py
--rw-r--r--   0 kthare10   (503) staff       (20)      809 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/type_util.py
--rw-r--r--   0 kthare10   (503) staff       (20)     3447 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/util.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.288450 fabric-credmgr-1.4.0/fabric_cm/credmgr/test/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/test/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4298 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/test/test_credmgr.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.289659 fabric-credmgr-1.4.0/fabric_cm/credmgr/token/
--rw-r--r--   0 kthare10   (503) staff       (20)        0 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/token/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     7887 2022-12-15 16:24:26.000000 fabric-credmgr-1.4.0/fabric_cm/credmgr/token/fabric_token_encoder.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2023-01-19 19:28:37.293962 fabric-credmgr-1.4.0/fabric_credmgr.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)    17615 2023-01-19 19:28:37.000000 fabric-credmgr-1.4.0/fabric_credmgr.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     3660 2023-01-19 19:28:37.000000 fabric-credmgr-1.4.0/fabric_credmgr.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2023-01-19 19:28:37.000000 fabric-credmgr-1.4.0/fabric_credmgr.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)      100 2023-01-19 19:28:37.000000 fabric-credmgr-1.4.0/fabric_credmgr.egg-info/entry_points.txt
--rw-r--r--   0 kthare10   (503) staff       (20)      164 2023-01-19 19:28:37.000000 fabric-credmgr-1.4.0/fabric_credmgr.egg-info/requires.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       10 2023-01-19 19:28:37.000000 fabric-credmgr-1.4.0/fabric_credmgr.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)      164 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/requirements.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2023-01-19 19:28:37.295787 fabric-credmgr-1.4.0/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)     2543 2022-12-15 15:53:01.000000 fabric-credmgr-1.4.0/setup.py
+-rw-r--r--   0        0        0     1873 2023-06-12 18:34:04.468803 fabric-credmgr-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1495 2023-06-12 18:34:04.468982 fabric-credmgr-1.5.0/Dockerfile
+-rw-r--r--   0        0        0     1071 2023-06-12 18:34:04.469143 fabric-credmgr-1.5.0/LICENSE
+-rw-r--r--   0        0        0    17107 2023-06-12 18:34:04.469373 fabric-credmgr-1.5.0/README.md
+-rw-r--r--   0        0        0      310 2023-06-12 18:34:04.469547 fabric-credmgr-1.5.0/cm-app/.gitignore
+-rw-r--r--   0        0        0      248 2023-06-12 18:34:04.469647 fabric-credmgr-1.5.0/cm-app/Dockerfile
+-rw-r--r--   0        0        0     3359 2023-06-12 18:34:04.469769 fabric-credmgr-1.5.0/cm-app/README.md
+-rwxr-xr-x   0        0        0      510 2023-06-12 18:34:04.469872 fabric-credmgr-1.5.0/cm-app/docker-entrypoint.sh
+-rw-r--r--   0        0        0      982 2023-06-12 18:34:04.470011 fabric-credmgr-1.5.0/cm-app/package.json
+-rw-r--r--   0        0        0   595208 2023-06-12 18:34:04.473293 fabric-credmgr-1.5.0/cm-app/public/fabric.ico
+-rw-r--r--   0        0        0      577 2023-06-12 18:34:04.473469 fabric-credmgr-1.5.0/cm-app/public/index.html
+-rw-r--r--   0        0        0      492 2023-06-12 18:34:04.473564 fabric-credmgr-1.5.0/cm-app/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-06-12 18:34:04.473649 fabric-credmgr-1.5.0/cm-app/public/robots.txt
+-rw-r--r--   0        0        0     1739 2023-06-12 18:34:04.473807 fabric-credmgr-1.5.0/cm-app/src/App.js
+-rw-r--r--   0        0        0      246 2023-06-12 18:34:04.473905 fabric-credmgr-1.5.0/cm-app/src/App.test.js
+-rw-r--r--   0        0        0      166 2023-06-12 18:34:04.474054 fabric-credmgr-1.5.0/cm-app/src/components/Footer.jsx
+-rw-r--r--   0        0        0     1705 2023-06-12 18:34:04.474175 fabric-credmgr-1.5.0/cm-app/src/components/Header.jsx
+-rw-r--r--   0        0        0      552 2023-06-12 18:34:04.474328 fabric-credmgr-1.5.0/cm-app/src/config.json
+-rw-r--r--   0        0        0   595208 2023-06-12 18:34:04.477268 fabric-credmgr-1.5.0/cm-app/src/imgs/fabric-brand.png
+-rw-r--r--   0        0        0      678 2023-06-12 18:34:04.477458 fabric-credmgr-1.5.0/cm-app/src/index.js
+-rw-r--r--   0        0        0     2632 2023-06-12 18:34:04.477575 fabric-credmgr-1.5.0/cm-app/src/logo.svg
+-rw-r--r--   0        0        0    13768 2023-06-12 18:34:04.477789 fabric-credmgr-1.5.0/cm-app/src/pages/CredentialManagerPage.jsx
+-rw-r--r--   0        0        0     1150 2023-06-12 18:34:04.477899 fabric-credmgr-1.5.0/cm-app/src/pages/Home.jsx
+-rw-r--r--   0        0        0      362 2023-06-12 18:34:04.478004 fabric-credmgr-1.5.0/cm-app/src/reportWebVitals.js
+-rw-r--r--   0        0        0      416 2023-06-12 18:34:04.478290 fabric-credmgr-1.5.0/cm-app/src/services/coreApiService.js
+-rw-r--r--   0        0        0      726 2023-06-12 18:34:04.478482 fabric-credmgr-1.5.0/cm-app/src/services/credentialManagerService.js
+-rw-r--r--   0        0        0      468 2023-06-12 18:34:04.478678 fabric-credmgr-1.5.0/cm-app/src/services/externalLinks.json
+-rw-r--r--   0        0        0     1103 2023-06-12 18:34:04.478840 fabric-credmgr-1.5.0/cm-app/src/services/httpService.js
+-rw-r--r--   0        0        0      241 2023-06-12 18:34:04.479042 fabric-credmgr-1.5.0/cm-app/src/setupTests.js
+-rw-r--r--   0        0        0     1060 2023-06-12 18:34:04.479328 fabric-credmgr-1.5.0/cm-app/src/styles/App.scss
+-rw-r--r--   0        0        0     1380 2023-06-12 18:34:04.479518 fabric-credmgr-1.5.0/cm-app/src/styles/custom.scss
+-rw-r--r--   0        0        0      347 2023-06-12 18:34:04.479700 fabric-credmgr-1.5.0/cm-app/src/styles/index.scss
+-rw-r--r--   0        0        0      269 2023-06-12 18:34:04.479974 fabric-credmgr-1.5.0/cm-app/src/utils/checkCmAppType.js
+-rw-r--r--   0        0        0     3189 2023-06-12 18:34:04.480212 fabric-credmgr-1.5.0/config_template
+-rw-r--r--   0        0        0     1465 2023-06-12 18:34:04.480413 fabric-credmgr-1.5.0/docker-compose.yml
+-rw-r--r--   0        0        0       96 2023-06-12 18:34:12.603525 fabric-credmgr-1.5.0/fabric_cm/__init__.py
+-rw-r--r--   0        0        0     2422 2023-06-12 18:34:04.480849 fabric-credmgr-1.5.0/fabric_cm/credmgr/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:34:04.480946 fabric-credmgr-1.5.0/fabric_cm/credmgr/common/__init__.py
+-rw-r--r--   0        0        0     1313 2023-06-12 18:34:04.481289 fabric-credmgr-1.5.0/fabric_cm/credmgr/common/exceptions.py
+-rw-r--r--   0        0        0     1295 2023-06-12 18:34:04.481690 fabric-credmgr-1.5.0/fabric_cm/credmgr/config/__init__.py
+-rw-r--r--   0        0        0     9183 2023-06-12 18:34:04.481946 fabric-credmgr-1.5.0/fabric_cm/credmgr/config/config.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:34:04.482096 fabric-credmgr-1.5.0/fabric_cm/credmgr/credential_managers/__init__.py
+-rw-r--r--   0        0        0     2967 2023-06-12 18:34:04.482345 fabric-credmgr-1.5.0/fabric_cm/credmgr/credential_managers/abstract_credential_manager.py
+-rw-r--r--   0        0        0     9595 2023-06-12 18:34:04.482547 fabric-credmgr-1.5.0/fabric_cm/credmgr/credential_managers/oauth_credmgr.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:34:04.482712 fabric-credmgr-1.5.0/fabric_cm/credmgr/external_apis/__init__.py
+-rw-r--r--   0        0        0     5937 2023-06-12 18:34:04.482852 fabric-credmgr-1.5.0/fabric_cm/credmgr/external_apis/core_api.py
+-rw-r--r--   0        0        0     4814 2023-06-12 18:34:04.482968 fabric-credmgr-1.5.0/fabric_cm/credmgr/external_apis/ldap.py
+-rw-r--r--   0        0        0     1263 2023-06-12 18:34:04.483170 fabric-credmgr-1.5.0/fabric_cm/credmgr/logging/__init__.py
+-rw-r--r--   0        0        0     2724 2023-06-12 18:34:04.483313 fabric-credmgr-1.5.0/fabric_cm/credmgr/logging/log.py
+-rw-r--r--   0        0        0    18587 2023-06-12 18:34:04.483468 fabric-credmgr-1.5.0/fabric_cm/credmgr/openapi.json
+-rw-r--r--   0        0        0     1571 2023-06-12 18:34:04.483664 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/__init__.py
+-rw-r--r--   0        0        0     2210 2023-06-12 18:34:04.483779 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:34:04.483913 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-12 18:34:04.484031 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/controllers/authorization_controller.py
+-rw-r--r--   0        0        0      333 2023-06-12 18:34:04.484130 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/controllers/default_controller.py
+-rw-r--r--   0        0        0     1774 2023-06-12 18:34:04.484311 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/controllers/tokens_controller.py
+-rw-r--r--   0        0        0      295 2023-06-12 18:34:04.484422 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/controllers/version_controller.py
+-rw-r--r--   0        0        0      626 2023-06-12 18:34:04.484532 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/encoder.py
+-rw-r--r--   0        0        0     1910 2023-06-12 18:34:04.484732 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1884 2023-06-12 18:34:04.484850 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     1601 2023-06-12 18:34:04.484963 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/jwks.py
+-rw-r--r--   0        0        0     4628 2023-06-12 18:34:04.485138 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/jwks_keys.py
+-rw-r--r--   0        0        0     1871 2023-06-12 18:34:04.485232 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/request.py
+-rw-r--r--   0        0        0     3881 2023-06-12 18:34:04.485356 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     2454 2023-06-12 18:34:04.485491 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     2860 2023-06-12 18:34:04.485650 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status200_ok_single.py
+-rw-r--r--   0        0        0     1968 2023-06-12 18:34:04.485787 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request.py
+-rw-r--r--   0        0        0     4493 2023-06-12 18:34:04.485884 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     3969 2023-06-12 18:34:04.485980 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     2502 2023-06-12 18:34:04.486114 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     3864 2023-06-12 18:34:04.486205 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden.py
+-rw-r--r--   0        0        0     2451 2023-06-12 18:34:04.486298 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     3831 2023-06-12 18:34:04.486443 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status404_not_found.py
+-rw-r--r--   0        0        0     2436 2023-06-12 18:34:04.486541 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     4218 2023-06-12 18:34:04.486685 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     2625 2023-06-12 18:34:04.486823 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3515 2023-06-12 18:34:04.486933 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/token.py
+-rw-r--r--   0        0        0     3439 2023-06-12 18:34:04.487048 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/tokens.py
+-rw-r--r--   0        0        0     3520 2023-06-12 18:34:04.487186 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/version.py
+-rw-r--r--   0        0        0     2526 2023-06-12 18:34:04.487285 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/version_data.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:34:04.487402 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-12 18:34:04.487499 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/authorization_controller.py
+-rw-r--r--   0        0        0     1558 2023-06-12 18:34:04.487597 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/constants.py
+-rw-r--r--   0        0        0     5429 2023-06-12 18:34:04.487784 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/cors_response.py
+-rw-r--r--   0        0        0     2187 2023-06-12 18:34:04.488025 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/default_controller.py
+-rw-r--r--   0        0        0     6842 2023-06-12 18:34:04.488134 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/tokens_controller.py
+-rw-r--r--   0        0        0     1285 2023-06-12 18:34:04.488253 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/version_controller.py
+-rw-r--r--   0        0        0    13635 2023-06-12 18:34:04.488462 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      433 2023-06-12 18:34:04.488625 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0      873 2023-06-12 18:34:04.488767 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/test/test_default_controller.py
+-rw-r--r--   0        0        0     2681 2023-06-12 18:34:04.488870 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/test/test_tokens_controller.py
+-rw-r--r--   0        0        0      840 2023-06-12 18:34:04.489116 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/test/test_version_controller.py
+-rw-r--r--   0        0        0      809 2023-06-12 18:34:04.489304 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/type_util.py
+-rw-r--r--   0        0        0     3447 2023-06-12 18:34:04.489447 fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/util.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:34:04.489547 fabric-credmgr-1.5.0/fabric_cm/credmgr/test/__init__.py
+-rw-r--r--   0        0        0     4298 2023-06-12 18:34:04.489681 fabric-credmgr-1.5.0/fabric_cm/credmgr/test/test_credmgr.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:34:04.489780 fabric-credmgr-1.5.0/fabric_cm/credmgr/token/__init__.py
+-rw-r--r--   0        0        0     7887 2023-06-12 18:34:04.489882 fabric-credmgr-1.5.0/fabric_cm/credmgr/token/fabric_token_encoder.py
+-rwxr-xr-x   0        0        0     2197 2023-06-12 18:34:04.489994 fabric-credmgr-1.5.0/fabric_cm/credmgr/update_swagger_stub.sh
+-rw-r--r--   0        0        0   279453 2023-06-12 18:34:04.492414 fabric-credmgr-1.5.0/images/credmgr.png
+-rw-r--r--   0        0        0    68431 2023-06-12 18:34:04.493037 fabric-credmgr-1.5.0/images/credmgr2.png
+-rw-r--r--   0        0        0    81311 2023-06-12 18:34:04.493549 fabric-credmgr-1.5.0/images/oidc_client.png
+-rw-r--r--   0        0        0    73988 2023-06-12 18:34:04.494029 fabric-credmgr-1.5.0/images/oidc_client_config.png
+-rw-r--r--   0        0        0   114939 2023-06-12 18:34:04.494683 fabric-credmgr-1.5.0/images/oidc_login.png
+-rw-r--r--   0        0        0   137300 2023-06-12 18:34:04.495575 fabric-credmgr-1.5.0/images/oidc_tokens.png
+-rw-r--r--   0        0        0     9882 2023-06-12 18:34:04.495791 fabric-credmgr-1.5.0/nginx/default.conf
+-rw-r--r--   0        0        0      910 2023-06-12 18:34:04.495911 fabric-credmgr-1.5.0/nginx/nginx.conf
+-rw-r--r--   0        0        0     5711 2023-06-12 18:34:04.496106 fabric-credmgr-1.5.0/oidc-cilogon.md
+-rw-r--r--   0        0        0      981 2023-06-12 18:34:24.574953 fabric-credmgr-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1757 2023-06-12 18:34:04.496392 fabric-credmgr-1.5.0/ssl/chain.pem
+-rw-r--r--   0        0        0     1757 2023-06-12 18:34:04.496492 fabric-credmgr-1.5.0/ssl/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-06-12 18:34:04.496593 fabric-credmgr-1.5.0/ssl/privkey.pem
+-rw-r--r--   0        0        0      800 2023-06-12 18:34:04.496711 fabric-credmgr-1.5.0/ssl/pubkey.pem
+-rw-r--r--   0        0        0       83 2023-06-12 18:34:04.496859 fabric-credmgr-1.5.0/test-requirements.txt
+-rw-r--r--   0        0        0      143 2023-06-12 18:34:04.496967 fabric-credmgr-1.5.0/tox.ini
+-rw-r--r--   0        0        0     3201 2023-06-12 18:34:04.497130 fabric-credmgr-1.5.0/vouch/config_template
+-rw-r--r--   0        0        0    17992 1970-01-01 00:00:00.000000 fabric-credmgr-1.5.0/PKG-INFO
```

### Comparing `fabric-credmgr-1.4.0/LICENSE` & `fabric-credmgr-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/PKG-INFO` & `fabric-credmgr-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: fabric-credmgr
-Version: 1.4.0
-Summary: Fabric Credential Manager API
-Home-page: https://github.com/fabric-testbed/CredentialManager
-Author: Komal Thareja
-Author-email: kthare10@renci.org
-License: MIT
-Keywords: Swagger,Fabric Credential Manager API
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI](https://img.shields.io/pypi/v/fabric-credmgr?style=plastic)](https://pypi.org/project/fabric-credmgr/)
 
 # CredentialManager
 
  ## Table of Contents
 
  - [Overview](#overview)
```

### Comparing `fabric-credmgr-1.4.0/README.md` & `fabric-credmgr-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: fabric-credmgr
+Version: 1.5.0
+Summary: Fabric Credential Manager API
+Keywords: Swagger,Fabric Credential Manager API
+Author-email: Komal Thareja <kthare10@renci.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Dist: requests
+Requires-Dist: requests_oauthlib
+Requires-Dist: connexion
+Requires-Dist: swagger-ui-bundle
+Requires-Dist: python_dateutil
+Requires-Dist: setuptools
+Requires-Dist: ldap3
+Requires-Dist: prometheus_client
+Requires-Dist: waitress
+Requires-Dist: six
+Requires-Dist: cryptography
+Requires-Dist: authlib
+Requires-Dist: fabric_fss_utils==1.5.0
+Project-URL: Home, https://fabric-testbed.net/
+Project-URL: Sources, https://github.com/fabric-testbed/CredentialManager
+
 [![PyPI](https://img.shields.io/pypi/v/fabric-credmgr?style=plastic)](https://pypi.org/project/fabric-credmgr/)
 
 # CredentialManager
 
  ## Table of Contents
 
  - [Overview](#overview)
@@ -441,7 +468,8 @@
       "tag 1",
       "tag 2"
     ]
   },
   "scope": "mf"
 }
 ```
+
```

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/__init__.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/common/exceptions.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/config/__init__.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/config/config.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/config/config.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/credential_managers/abstract_credential_manager.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/credential_managers/abstract_credential_manager.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/credential_managers/oauth_credmgr.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/credential_managers/oauth_credmgr.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/external_apis/core_api.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/external_apis/core_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 # Author Komal Thareja (kthare10@renci.org)
+import datetime
 from typing import Tuple
 
 import requests
 
 from fabric_cm.credmgr.config import CONFIG_OBJ
 from fabric_cm.credmgr.logging import LOG
 
@@ -91,19 +92,28 @@
         if response.status_code != 200:
             raise CoreApiError(f"Core API error occurred status_code: {response.status_code} "
                                f"message: {response.content}")
 
         LOG.debug(f"GET Project Response : {response.json()}")
         projects_res = response.json().get("results")
 
-        if len(projects_res) == 0:
-            raise CoreApiError(f"User is not a member of Project: {project_id}")
-
         projects = []
         for p in projects_res:
+            expires_on = p.get("expires_on")
+            if expires_on is not None:
+                expires_on_dt = datetime.datetime.fromisoformat(expires_on)
+                now = datetime.datetime.now(tz=datetime.timezone.utc)
+                if now > expires_on_dt:
+                    # Do not include the expired project in the token for "all" get slices
+                    if project_id.lower() == "all":
+                        continue
+                    # Fail a request of the token for an expired token
+                    else:
+                        raise CoreApiError(f"Project {p.get('name')} is expired!")
+
             project_memberships = p.get("memberships")
 
             if not project_memberships["is_member"] and not project_memberships["is_creator"] and \
                     not project_memberships["is_owner"]:
                 raise CoreApiError(f"User is not a member of Project: {p.get('uuid')}")
             project = {
                 "name": p.get("name"),
@@ -113,14 +123,17 @@
             # Only pass tags and membership when token is requested for a specific project
             if project_id.lower() != "all":
                 project["tags"] = p.get("tags")
                 project["memberships"] = p.get("memberships")
 
             projects.append(project)
 
+        if len(projects) == 0:
+            raise CoreApiError(f"User is not a member of Project: {project_id}")
+
         # Get User by UUID to get roles (Facility Operator is not Project Specific,
         # so need the roles from people end point)
         url = f"{self.api_server}/people/{uuid}?as_self=true"
         response = s.get(url, verify=ssl_verify)
 
         if response.status_code != 200:
             raise CoreApiError(f"Core API error occurred status_code: {response.status_code} "
```

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/external_apis/ldap.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/external_apis/ldap.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/logging/__init__.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/logging/log.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/logging/log.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/__init__.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/__main__.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 def main():
     """
     Main Entry Point
     """
     log = LOG
     try:
         app = connexion.App(__name__, specification_dir='swagger/')
-        app.app.json_encoder = encoder.JSONEncoder
+        app.json_provider_class = encoder.JSONEncoder
         app.add_api('swagger.yaml',
                     arguments={'title': 'Fabric Credential Manager API'},
                     pythonic_params=True)
         port = CONFIG_OBJ.get_rest_port()
 
         # prometheus server
         prometheus_port = CONFIG_OBJ.get_prometheus_port()
```

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/controllers/tokens_controller.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/controllers/tokens_controller.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/encoder.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/__init__.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/base_model_.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/jwks.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/jwks_keys.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/request.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content_data.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status200_ok_single.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request_errors.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized_errors.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden_errors.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status404_not_found.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status404_not_found_errors.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error_errors.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/token.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/tokens.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/version.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/models/version_data.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/constants.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/constants.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/cors_response.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/cors_response.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/default_controller.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/default_controller.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/tokens_controller.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/tokens_controller.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/response/version_controller.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/response/version_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from fabric_cm.credmgr.swagger_server import received_counter, success_counter, failure_counter
 from fabric_cm.credmgr.swagger_server.models.version import Version
 from fabric_cm.credmgr.swagger_server.models.version_data import VersionData
-from fabric_cm import __VERSION__, __API_REFERENCE__
+from fabric_cm import __version__, __API_REFERENCE__
 from fabric_cm.credmgr.swagger_server.response.constants import HTTP_METHOD_GET, VERSION_URL
 from fabric_cm.credmgr.swagger_server.response.cors_response import cors_500, cors_200
 
 
 def version_get() -> Version:  # noqa: E501
     """version
     Version # noqa: E501
     :rtype: Version
     """
     try:
         received_counter.labels(HTTP_METHOD_GET, VERSION_URL).inc()
         version = VersionData()
         version.reference = __API_REFERENCE__
-        version.version = __VERSION__
+        version.version = __version__
         response = Version()
         response.data = [version]
         response.size = len(response.data)
         response.status = 200
         response.type = 'version'
         success_counter.labels(HTTP_METHOD_GET, VERSION_URL).inc()
         return cors_200(response_body=response)
```

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/swagger/swagger.yaml` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/swagger/swagger.yaml`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/test_default_controller.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/test/test_default_controller.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/test_tokens_controller.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/test/test_tokens_controller.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/test/test_version_controller.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/test/test_version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/type_util.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/type_util.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/swagger_server/util.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/test/test_credmgr.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/test/test_credmgr.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-1.4.0/fabric_cm/credmgr/token/fabric_token_encoder.py` & `fabric-credmgr-1.5.0/fabric_cm/credmgr/token/fabric_token_encoder.py`

 * *Files identical despite different names*

