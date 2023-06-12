# Comparing `tmp/fabric-credmgr-client-1.5.0.tar.gz` & `tmp/fabric-credmgr-client-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-credmgr-client-1.5.0.tar", last modified: Mon Jun 12 15:49:14 2023, max compression
+gzip compressed data, was "fabric-credmgr-client-1.5.0rc1.tar", last modified: Thu May 11 18:09:36 2023, max compression
```

## Comparing `fabric-credmgr-client-1.5.0.tar` & `fabric-credmgr-client-1.5.0rc1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.5.0/.gitignore
--rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.5.0/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-05-11 18:03:22.616419 fabric-credmgr-client-1.5.0/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.5.0/.travis.yml
--rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.5.0/LICENSE
--rw-r--r--   0        0        0     4211 2023-05-11 18:03:22.617008 fabric-credmgr-client-1.5.0/README.md
--rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.5.0/docs/DefaultApi.md
--rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.5.0/docs/Jwks.md
--rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.5.0/docs/JwksKeys.md
--rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.5.0/docs/Request.md
--rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.5.0/docs/Status200OkNoContent.md
--rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.5.0/docs/Status200OkNoContentData.md
--rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.5.0/docs/Status200OkSingle.md
--rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.5.0/docs/Status400BadRequest.md
--rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.5.0/docs/Status400BadRequestErrors.md
--rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.5.0/docs/Status401Unauthorized.md
--rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.5.0/docs/Status401UnauthorizedErrors.md
--rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.5.0/docs/Status403Forbidden.md
--rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.5.0/docs/Status403ForbiddenErrors.md
--rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.5.0/docs/Status404NotFound.md
--rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.5.0/docs/Status404NotFoundErrors.md
--rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.5.0/docs/Status500InternalServerError.md
--rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.5.0/docs/Status500InternalServerErrorErrors.md
--rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.5.0/docs/Success.md
--rw-r--r--   0        0        0      403 2023-05-11 18:03:22.619089 fabric-credmgr-client-1.5.0/docs/Token.md
--rw-r--r--   0        0        0      339 2023-05-11 18:03:22.619217 fabric-credmgr-client-1.5.0/docs/Tokens.md
--rw-r--r--   0        0        0     5090 2023-05-11 18:03:22.619366 fabric-credmgr-client-1.5.0/docs/TokensApi.md
--rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.5.0/docs/Version.md
--rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.5.0/docs/VersionApi.md
--rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.5.0/docs/VersionData.md
--rw-r--r--   0        0        0       48 2023-06-12 15:48:47.171764 fabric-credmgr-client-1.5.0/fabric_cm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/__init__.py
--rw-r--r--   0        0        0     6006 2023-05-11 18:03:22.620379 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/credmgr_proxy.py
--rw-r--r--   0        0        0     2545 2023-05-11 18:03:22.620670 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/__init__.py
--rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api/default_api.py
--rw-r--r--   0        0        0    12548 2023-05-11 18:03:22.621635 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api/tokens_api.py
--rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25120 2023-05-11 18:03:22.622136 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api_client.py
--rw-r--r--   0        0        0     7980 2023-05-11 18:03:22.622439 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/configuration.py
--rw-r--r--   0        0        0     2143 2023-05-11 18:03:22.622732 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/jwks.py
--rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
--rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/request.py
--rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     4831 2023-05-11 18:03:22.626321 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/token.py
--rw-r--r--   0        0        0     3394 2023-05-11 18:03:22.626505 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/tokens.py
--rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/version.py
--rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.5.0/git_push.sh
--rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 18:03:22.628116 fabric-credmgr-client-1.5.0/test/__init__.py
--rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.5.0/test/test_default_api.py
--rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.5.0/test/test_jwks.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.5.0/test/test_jwks_keys.py
--rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.5.0/test/test_request.py
--rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.5.0/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.5.0/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.5.0/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.5.0/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.5.0/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.5.0/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.5.0/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.5.0/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.5.0/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.5.0/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.5.0/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.5.0/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.5.0/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.5.0/test/test_token.py
--rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.5.0/test/test_tokens.py
--rw-r--r--   0        0        0     1173 2023-05-11 18:03:22.632206 fabric-credmgr-client-1.5.0/test/test_tokens_api.py
--rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.5.0/test/test_version.py
--rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.5.0/test/test_version_api.py
--rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.5.0/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.5.0/tox.ini
--rw-r--r--   0        0        0     5193 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      794 2023-05-11 18:03:22.615968 fabric-credmgr-client-1.5.0rc1/.gitignore
+-rw-r--r--   0        0        0     1030 2023-05-11 18:03:22.616147 fabric-credmgr-client-1.5.0rc1/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-05-11 18:03:22.616419 fabric-credmgr-client-1.5.0rc1/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-05-11 18:03:22.616544 fabric-credmgr-client-1.5.0rc1/.travis.yml
+-rw-r--r--   0        0        0     1071 2023-05-11 18:03:22.616706 fabric-credmgr-client-1.5.0rc1/LICENSE
+-rw-r--r--   0        0        0     4211 2023-05-11 18:03:22.617008 fabric-credmgr-client-1.5.0rc1/README.md
+-rw-r--r--   0        0        0     1315 2023-05-11 18:03:22.617177 fabric-credmgr-client-1.5.0rc1/docs/DefaultApi.md
+-rw-r--r--   0        0        0      343 2023-05-11 18:03:22.617302 fabric-credmgr-client-1.5.0rc1/docs/Jwks.md
+-rw-r--r--   0        0        0      600 2023-05-11 18:03:22.617403 fabric-credmgr-client-1.5.0rc1/docs/JwksKeys.md
+-rw-r--r--   0        0        0      331 2023-05-11 18:03:22.617518 fabric-credmgr-client-1.5.0rc1/docs/Request.md
+-rw-r--r--   0        0        0      556 2023-05-11 18:03:22.617616 fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContent.md
+-rw-r--r--   0        0        0      404 2023-05-11 18:03:22.617743 fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContentData.md
+-rw-r--r--   0        0        0      434 2023-05-11 18:03:22.617843 fabric-credmgr-client-1.5.0rc1/docs/Status200OkSingle.md
+-rw-r--r--   0        0        0      394 2023-05-11 18:03:22.617940 fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequest.md
+-rw-r--r--   0        0        0      566 2023-05-11 18:03:22.618030 fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequestErrors.md
+-rw-r--r--   0        0        0      560 2023-05-11 18:03:22.618124 fabric-credmgr-client-1.5.0rc1/docs/Status401Unauthorized.md
+-rw-r--r--   0        0        0      409 2023-05-11 18:03:22.618211 fabric-credmgr-client-1.5.0rc1/docs/Status401UnauthorizedErrors.md
+-rw-r--r--   0        0        0      551 2023-05-11 18:03:22.618321 fabric-credmgr-client-1.5.0rc1/docs/Status403Forbidden.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.618447 fabric-credmgr-client-1.5.0rc1/docs/Status403ForbiddenErrors.md
+-rw-r--r--   0        0        0      548 2023-05-11 18:03:22.618553 fabric-credmgr-client-1.5.0rc1/docs/Status404NotFound.md
+-rw-r--r--   0        0        0      402 2023-05-11 18:03:22.618642 fabric-credmgr-client-1.5.0rc1/docs/Status404NotFoundErrors.md
+-rw-r--r--   0        0        0      581 2023-05-11 18:03:22.618726 fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerError.md
+-rw-r--r--   0        0        0      425 2023-05-11 18:03:22.618844 fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerErrorErrors.md
+-rw-r--r--   0        0        0      446 2023-05-11 18:03:22.618969 fabric-credmgr-client-1.5.0rc1/docs/Success.md
+-rw-r--r--   0        0        0      403 2023-05-11 18:03:22.619089 fabric-credmgr-client-1.5.0rc1/docs/Token.md
+-rw-r--r--   0        0        0      339 2023-05-11 18:03:22.619217 fabric-credmgr-client-1.5.0rc1/docs/Tokens.md
+-rw-r--r--   0        0        0     5090 2023-05-11 18:03:22.619366 fabric-credmgr-client-1.5.0rc1/docs/TokensApi.md
+-rw-r--r--   0        0        0      352 2023-05-11 18:03:22.619490 fabric-credmgr-client-1.5.0rc1/docs/Version.md
+-rw-r--r--   0        0        0     1205 2023-05-11 18:03:22.619644 fabric-credmgr-client-1.5.0rc1/docs/VersionApi.md
+-rw-r--r--   0        0        0      346 2023-05-11 18:03:22.619831 fabric-credmgr-client-1.5.0rc1/docs/VersionData.md
+-rw-r--r--   0        0        0       50 2023-05-11 18:06:29.691397 fabric-credmgr-client-1.5.0rc1/fabric_cm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.620222 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/__init__.py
+-rw-r--r--   0        0        0     6006 2023-05-11 18:03:22.620379 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/credmgr_proxy.py
+-rw-r--r--   0        0        0     2545 2023-05-11 18:03:22.620670 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-11 18:03:22.621111 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-11 18:03:22.621312 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/default_api.py
+-rw-r--r--   0        0        0    12548 2023-05-11 18:03:22.621635 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/tokens_api.py
+-rw-r--r--   0        0        0     3755 2023-05-11 18:03:22.621852 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25120 2023-05-11 18:03:22.622136 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api_client.py
+-rw-r--r--   0        0        0     7980 2023-05-11 18:03:22.622439 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2143 2023-05-11 18:03:22.622732 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     2964 2023-05-11 18:03:22.622977 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks.py
+-rw-r--r--   0        0        0     6062 2023-05-11 18:03:22.623162 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py
+-rw-r--r--   0        0        0     3299 2023-05-11 18:03:22.623362 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/request.py
+-rw-r--r--   0        0        0     5011 2023-05-11 18:03:22.623647 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3844 2023-05-11 18:03:22.623886 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     4265 2023-05-11 18:03:22.624053 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3175 2023-05-11 18:03:22.624285 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5783 2023-05-11 18:03:22.624535 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5075 2023-05-11 18:03:22.624762 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3882 2023-05-11 18:03:22.624915 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     5006 2023-05-11 18:03:22.625098 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3843 2023-05-11 18:03:22.625298 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4983 2023-05-11 18:03:22.625479 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3831 2023-05-11 18:03:22.625691 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5236 2023-05-11 18:03:22.625944 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3975 2023-05-11 18:03:22.626141 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     4831 2023-05-11 18:03:22.626321 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/token.py
+-rw-r--r--   0        0        0     3394 2023-05-11 18:03:22.626505 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/tokens.py
+-rw-r--r--   0        0        0     3420 2023-05-11 18:03:22.626788 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3894 2023-05-11 18:03:22.627057 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    13000 2023-05-11 18:03:22.627316 fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-05-11 18:03:22.627539 fabric-credmgr-client-1.5.0rc1/git_push.sh
+-rw-r--r--   0        0        0     1101 2023-05-11 18:07:49.170889 fabric-credmgr-client-1.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 18:03:22.628116 fabric-credmgr-client-1.5.0rc1/test/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-11 18:03:22.628351 fabric-credmgr-client-1.5.0rc1/test/test_default_api.py
+-rw-r--r--   0        0        0      843 2023-05-11 18:03:22.628520 fabric-credmgr-client-1.5.0rc1/test/test_jwks.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.628746 fabric-credmgr-client-1.5.0rc1/test/test_jwks_keys.py
+-rw-r--r--   0        0        0      867 2023-05-11 18:03:22.628966 fabric-credmgr-client-1.5.0rc1/test/test_request.py
+-rw-r--r--   0        0        0      977 2023-05-11 18:03:22.629156 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1011 2023-05-11 18:03:22.629346 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      951 2023-05-11 18:03:22.629517 fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      967 2023-05-11 18:03:22.629752 fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1017 2023-05-11 18:03:22.630042 fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0      981 2023-05-11 18:03:22.630229 fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1031 2023-05-11 18:03:22.630398 fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      975 2023-05-11 18:03:22.630574 fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1025 2023-05-11 18:03:22.630852 fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      969 2023-05-11 18:03:22.631034 fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1019 2023-05-11 18:03:22.631251 fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1059 2023-05-11 18:03:22.631443 fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1109 2023-05-11 18:03:22.631652 fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      869 2023-05-11 18:03:22.631826 fabric-credmgr-client-1.5.0rc1/test/test_token.py
+-rw-r--r--   0        0        0      877 2023-05-11 18:03:22.632046 fabric-credmgr-client-1.5.0rc1/test/test_tokens.py
+-rw-r--r--   0        0        0     1173 2023-05-11 18:03:22.632206 fabric-credmgr-client-1.5.0rc1/test/test_tokens_api.py
+-rw-r--r--   0        0        0      885 2023-05-11 18:03:22.632450 fabric-credmgr-client-1.5.0rc1/test/test_version.py
+-rw-r--r--   0        0        0      816 2023-05-11 18:03:22.632625 fabric-credmgr-client-1.5.0rc1/test/test_version_api.py
+-rw-r--r--   0        0        0      919 2023-05-11 18:03:22.632817 fabric-credmgr-client-1.5.0rc1/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-05-11 18:03:22.632996 fabric-credmgr-client-1.5.0rc1/tox.ini
+-rw-r--r--   0        0        0     5196 1970-01-01 00:00:00.000000 fabric-credmgr-client-1.5.0rc1/PKG-INFO
```

### Comparing `fabric-credmgr-client-1.5.0/.gitignore` & `fabric-credmgr-client-1.5.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/.swagger-codegen-ignore` & `fabric-credmgr-client-1.5.0rc1/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/LICENSE` & `fabric-credmgr-client-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/README.md` & `fabric-credmgr-client-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/DefaultApi.md` & `fabric-credmgr-client-1.5.0rc1/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/JwksKeys.md` & `fabric-credmgr-client-1.5.0rc1/docs/JwksKeys.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/Status200OkNoContent.md` & `fabric-credmgr-client-1.5.0rc1/docs/Status200OkNoContent.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/Status400BadRequestErrors.md` & `fabric-credmgr-client-1.5.0rc1/docs/Status400BadRequestErrors.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/Status401Unauthorized.md` & `fabric-credmgr-client-1.5.0rc1/docs/Status401Unauthorized.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/Status403Forbidden.md` & `fabric-credmgr-client-1.5.0rc1/docs/Status403Forbidden.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/Status404NotFound.md` & `fabric-credmgr-client-1.5.0rc1/docs/Status404NotFound.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/Status500InternalServerError.md` & `fabric-credmgr-client-1.5.0rc1/docs/Status500InternalServerError.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/TokensApi.md` & `fabric-credmgr-client-1.5.0rc1/docs/TokensApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/docs/VersionApi.md` & `fabric-credmgr-client-1.5.0rc1/docs/VersionApi.md`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/credmgr_proxy.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/credmgr_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/__init__.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api/default_api.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api/tokens_api.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api/version_api.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/api_client.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/configuration.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/__init__.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/jwks.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/jwks_keys.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/request.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status404_not_found.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/token.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/tokens.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/version.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/models/version_data.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/fabric_cm/credmgr/swagger_client/rest.py` & `fabric-credmgr-client-1.5.0rc1/fabric_cm/credmgr/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/git_push.sh` & `fabric-credmgr-client-1.5.0rc1/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/pyproject.toml` & `fabric-credmgr-client-1.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_default_api.py` & `fabric-credmgr-client-1.5.0rc1/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_jwks.py` & `fabric-credmgr-client-1.5.0rc1/test/test_jwks.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_jwks_keys.py` & `fabric-credmgr-client-1.5.0rc1/test/test_jwks_keys.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_request.py` & `fabric-credmgr-client-1.5.0rc1/test/test_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status200_ok_no_content.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status200_ok_no_content_data.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status200_ok_single.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status400_bad_request.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status400_bad_request_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status401_unauthorized.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status401_unauthorized_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status403_forbidden.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status403_forbidden_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status404_not_found.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status404_not_found_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status500_internal_server_error.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_status500_internal_server_error_errors.py` & `fabric-credmgr-client-1.5.0rc1/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_token.py` & `fabric-credmgr-client-1.5.0rc1/test/test_token.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_tokens.py` & `fabric-credmgr-client-1.5.0rc1/test/test_tokens.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_tokens_api.py` & `fabric-credmgr-client-1.5.0rc1/test/test_tokens_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_version.py` & `fabric-credmgr-client-1.5.0rc1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_version_api.py` & `fabric-credmgr-client-1.5.0rc1/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/test/test_version_data.py` & `fabric-credmgr-client-1.5.0rc1/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-credmgr-client-1.5.0/PKG-INFO` & `fabric-credmgr-client-1.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-credmgr-client
-Version: 1.5.0
+Version: 1.5.0rc1
 Summary: Fabric Control Framework
 Keywords: Fabric Credential Manager API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

