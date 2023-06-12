# Comparing `tmp/trinsic-sdk-1.9.0.tar.gz` & `tmp/trinsic-sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinsic-sdk-1.9.0.tar", last modified: Fri Feb  3 13:50:59 2023, max compression
+gzip compressed data, was "trinsic-sdk-1.9.1.tar", last modified: Mon Feb  6 13:39:01 2023, max compression
```

## Comparing `trinsic-sdk-1.9.0.tar` & `trinsic-sdk-1.9.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-03 13:50:52.000000 trinsic-sdk-1.9.0/trinsic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/access_management_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/account_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/credential_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/file_management_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/sdk/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/sdk/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/sdk/options/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/sdk/options/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/account/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/account/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/common/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/common/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/filemanagement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/filemanagement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/filemanagement/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/filemanagement/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.310207 trinsic-sdk-1.9.0/trinsic/proto/services/options/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/provider/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/provider/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/trustregistry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/trustregistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/trustregistry/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/trustregistry/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/universalwallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/universalwallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/universalwallet/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/universalwallet/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/templates/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/templates/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/trinsic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/trinsic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/trinsic/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/trinsic/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic/proto/trinsic/services/event/
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/proto/trinsic/services/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/provider_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/security_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/service_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/template_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/trinsic_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/trinsic_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/trustregistry_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-02-03 13:50:34.000000 trinsic-sdk-1.9.0/trinsic/wallet_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:50:59.314207 trinsic-sdk-1.9.0/trinsic_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-03 13:50:59.000000 trinsic-sdk-1.9.0/trinsic_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-02-03 13:50:59.000000 trinsic-sdk-1.9.0/trinsic_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 13:50:59.000000 trinsic-sdk-1.9.0/trinsic_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-03 13:50:59.000000 trinsic-sdk-1.9.0/trinsic_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-03 13:50:59.000000 trinsic-sdk-1.9.0/trinsic_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.911150 trinsic-sdk-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-06 13:39:01.911150 trinsic-sdk-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-06 13:39:01.911150 trinsic-sdk-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-06 13:38:54.000000 trinsic-sdk-1.9.1/trinsic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/access_management_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/account_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/credential_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/file_management_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/sdk/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/sdk/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/sdk/options/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/sdk/options/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/account/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/account/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/common/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/filemanagement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/filemanagement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/filemanagement/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/filemanagement/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/provider/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/provider/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/trustregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/trustregistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/trustregistry/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/trustregistry/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/universalwallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/universalwallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/universalwallet/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/universalwallet/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/templates/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/templates/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/trinsic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/trinsic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/trinsic/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/trinsic/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.907150 trinsic-sdk-1.9.1/trinsic/proto/trinsic/services/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/proto/trinsic/services/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/provider_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/security_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/service_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/template_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/trinsic_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/trinsic_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/trustregistry_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-02-06 13:38:36.000000 trinsic-sdk-1.9.1/trinsic/wallet_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 13:39:01.911150 trinsic-sdk-1.9.1/trinsic_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-06 13:39:01.000000 trinsic-sdk-1.9.1/trinsic_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-02-06 13:39:01.000000 trinsic-sdk-1.9.1/trinsic_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 13:39:01.000000 trinsic-sdk-1.9.1/trinsic_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-06 13:39:01.000000 trinsic-sdk-1.9.1/trinsic_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-06 13:39:01.000000 trinsic-sdk-1.9.1/trinsic_sdk.egg-info/top_level.txt
```

### Comparing `trinsic-sdk-1.9.0/PKG-INFO` & `trinsic-sdk-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinsic-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: Trinsic Services SDK bindings
 Home-page: https://github.com/trinsic-id/okapi/
 Author: Scott Phillips
 Author-email: scott.phillips@trinsic.id
 Project-URL: Bug Tracker, https://github.com/trinsic-id/okapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinsic-sdk-1.9.0/setup.cfg` & `trinsic-sdk-1.9.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trinsic-sdk
-version = 1.9.0
+version = 1.9.1
 author = Scott Phillips
 author_email = scott.phillips@trinsic.id
 description = Trinsic Services SDK bindings
 long_description = file: ./README.md
 long_description_content_type = text/markdown
 url = https://github.com/trinsic-id/okapi/
 project_urls = 
@@ -18,14 +18,15 @@
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	grpclib>=0.4.3rc2
 	betterproto>=2.0.0b4
 	trinsic-okapi>=1.6.0
+	deprecation>=2.1.0
 
 [options.packages.find]
 exclude = tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trinsic-sdk-1.9.0/trinsic/__main__.py` & `trinsic-sdk-1.9.1/trinsic/__main__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/access_management_service.py` & `trinsic-sdk-1.9.1/trinsic/access_management_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/account_service.py` & `trinsic-sdk-1.9.1/trinsic/account_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/credential_service.py` & `trinsic-sdk-1.9.1/trinsic/credential_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/file_management_service.py` & `trinsic-sdk-1.9.1/trinsic/file_management_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/sdk/options/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/sdk/options/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/account/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/account/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/common/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/common/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/filemanagement/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/filemanagement/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/options/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/options/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/provider/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/provider/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/trustregistry/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/trustregistry/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/universalwallet/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/universalwallet/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/templates/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/templates/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/services/verifiablecredentials/v1/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/services/verifiablecredentials/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/proto/trinsic/services/event/__init__.py` & `trinsic-sdk-1.9.1/trinsic/proto/trinsic/services/event/__init__.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/provider_service.py` & `trinsic-sdk-1.9.1/trinsic/provider_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/security_providers.py` & `trinsic-sdk-1.9.1/trinsic/security_providers.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/service_base.py` & `trinsic-sdk-1.9.1/trinsic/service_base.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/template_service.py` & `trinsic-sdk-1.9.1/trinsic/template_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/trinsic_service.py` & `trinsic-sdk-1.9.1/trinsic/trinsic_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/trinsic_util.py` & `trinsic-sdk-1.9.1/trinsic/trinsic_util.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/trustregistry_service.py` & `trinsic-sdk-1.9.1/trinsic/trustregistry_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic/wallet_service.py` & `trinsic-sdk-1.9.1/trinsic/wallet_service.py`

 * *Files identical despite different names*

### Comparing `trinsic-sdk-1.9.0/trinsic_sdk.egg-info/PKG-INFO` & `trinsic-sdk-1.9.1/trinsic_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinsic-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: Trinsic Services SDK bindings
 Home-page: https://github.com/trinsic-id/okapi/
 Author: Scott Phillips
 Author-email: scott.phillips@trinsic.id
 Project-URL: Bug Tracker, https://github.com/trinsic-id/okapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinsic-sdk-1.9.0/trinsic_sdk.egg-info/SOURCES.txt` & `trinsic-sdk-1.9.1/trinsic_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

