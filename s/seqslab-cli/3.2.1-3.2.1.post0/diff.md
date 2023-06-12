# Comparing `tmp/seqslab-cli-3.2.1.tar.gz` & `tmp/seqslab-cli-3.2.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-cli-3.2.1.tar", last modified: Fri May 26 06:05:38 2023, max compression
+gzip compressed data, was "seqslab-cli-3.2.1.post0.tar", last modified: Mon Jun 12 02:43:09 2023, max compression
```

## Comparing `seqslab-cli-3.2.1.tar` & `seqslab-cli-3.2.1.post0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.982665 seqslab-cli-3.2.1/
--rw-r--r--   0 chris      (501) staff       (20)      692 2022-04-15 03:12:06.000000 seqslab-cli-3.2.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       77 2022-04-15 03:12:06.000000 seqslab-cli-3.2.1/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     8762 2023-05-26 06:05:38.983048 seqslab-cli-3.2.1/PKG-INFO
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.912254 seqslab-cli-3.2.1/python/
--rw-r--r--   0 chris      (501) staff       (20)      418 2023-02-24 03:14:45.000000 seqslab-cli-3.2.1/python/requirements.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.920783 seqslab-cli-3.2.1/python/seqslab/
--rw-r--r--   0 chris      (501) staff       (20)     8042 2023-05-26 05:55:52.000000 seqslab-cli-3.2.1/python/seqslab/README.md
--rw-r--r--   0 chris      (501) staff       (20)      786 2023-05-26 06:05:00.000000 seqslab-cli-3.2.1/python/seqslab/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.922980 seqslab-cli-3.2.1/python/seqslab/auth/
--rw-r--r--   0 chris      (501) staff       (20)       79 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/auth/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     4514 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/auth/azuread.py
--rw-r--r--   0 chris      (501) staff       (20)    14275 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/auth/commands.py
--rw-r--r--   0 chris      (501) staff       (20)     1228 2023-02-08 06:39:25.000000 seqslab-cli-3.2.1/python/seqslab/cli.py
--rw-r--r--   0 chris      (501) staff       (20)      728 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/context.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.924236 seqslab-cli-3.2.1/python/seqslab/drs/
--rw-r--r--   0 chris      (501) staff       (20)      228 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.927496 seqslab-cli-3.2.1/python/seqslab/drs/api/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    14655 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/azure.py
--rw-r--r--   0 chris      (501) staff       (20)    14735 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/base.py
--rw-r--r--   0 chris      (501) staff       (20)     1336 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/common.py
--rw-r--r--   0 chris      (501) staff       (20)     5116 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/template.py
--rw-r--r--   0 chris      (501) staff       (20)    37707 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/commands.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.930097 seqslab-cli-3.2.1/python/seqslab/drs/internal/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    20561 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/aiocopy.py
--rw-r--r--   0 chris      (501) staff       (20)     1325 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/common.py
--rw-r--r--   0 chris      (501) staff       (20)     4012 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.931817 seqslab-cli-3.2.1/python/seqslab/drs/storage/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/storage/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    40704 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/storage/azure.py
--rw-r--r--   0 chris      (501) staff       (20)    12838 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/storage/base.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.933606 seqslab-cli-3.2.1/python/seqslab/drs/utils/
--rw-r--r--   0 chris      (501) staff       (20)       81 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/utils/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2075 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/utils/biomimetype.py
--rw-r--r--   0 chris      (501) staff       (20)     3180 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/utils/progressbar.py
--rw-r--r--   0 chris      (501) staff       (20)     2285 2022-07-27 01:18:54.000000 seqslab-cli-3.2.1/python/seqslab/exceptions.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.934960 seqslab-cli-3.2.1/python/seqslab/organization/
--rw-r--r--   0 chris      (501) staff       (20)      271 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2365 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/commands.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.936077 seqslab-cli-3.2.1/python/seqslab/organization/resource/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/resource/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1227 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/resource/base.py
--rw-r--r--   0 chris      (501) staff       (20)     5440 2023-02-24 03:14:45.000000 seqslab-cli-3.2.1/python/seqslab/plugin.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.937241 seqslab-cli-3.2.1/python/seqslab/role/
--rw-r--r--   0 chris      (501) staff       (20)      230 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1275 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/commands.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.938284 seqslab-cli-3.2.1/python/seqslab/role/internal/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/internal/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1324 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/internal/common.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.939974 seqslab-cli-3.2.1/python/seqslab/role/resource/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/resource/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      865 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/resource/azure.py
--rw-r--r--   0 chris      (501) staff       (20)     1286 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/resource/base.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.941161 seqslab-cli-3.2.1/python/seqslab/runsheet/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/runsheet/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     3442 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/runsheet/runsheet.py
--rw-r--r--   0 chris      (501) staff       (20)      452 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/session_logger.py
--rw-r--r--   0 chris      (501) staff       (20)      824 2022-07-27 01:18:54.000000 seqslab-cli-3.2.1/python/seqslab/settings.py
--rw-r--r--   0 chris      (501) staff       (20)     1370 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/statusbar.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.942757 seqslab-cli-3.2.1/python/seqslab/trs/
--rw-r--r--   0 chris      (501) staff       (20)      227 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    20866 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/commands.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.944484 seqslab-cli-3.2.1/python/seqslab/trs/internal/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/internal/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1667 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/internal/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.947924 seqslab-cli-3.2.1/python/seqslab/trs/register/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      940 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/azure.py
--rw-r--r--   0 chris      (501) staff       (20)     9941 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/base.py
--rw-r--r--   0 chris      (501) staff       (20)     1321 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/common.py
--rw-r--r--   0 chris      (501) staff       (20)     7345 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/template.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.950370 seqslab-cli-3.2.1/python/seqslab/trs/resource/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      883 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/azure.py
--rw-r--r--   0 chris      (501) staff       (20)     7267 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/base.py
--rw-r--r--   0 chris      (501) staff       (20)     1346 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/common.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.952213 seqslab-cli-3.2.1/python/seqslab/trs/template/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/template/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     7386 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/template/base.py
--rw-r--r--   0 chris      (501) staff       (20)     2897 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/template/template.py
--rw-r--r--   0 chris      (501) staff       (20)      951 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/usage_logger.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.953539 seqslab-cli-3.2.1/python/seqslab/user/
--rw-r--r--   0 chris      (501) staff       (20)      230 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     6820 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/commands.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.954461 seqslab-cli-3.2.1/python/seqslab/user/internal/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/internal/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1327 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/internal/common.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.961236 seqslab-cli-3.2.1/python/seqslab/user/resource/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/resource/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1743 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/resource/azure.py
--rw-r--r--   0 chris      (501) staff       (20)     4001 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/resource/base.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.965525 seqslab-cli-3.2.1/python/seqslab/wes/
--rw-r--r--   0 chris      (501) staff       (20)      227 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    23184 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/commands.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.967039 seqslab-cli-3.2.1/python/seqslab/wes/internal/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/internal/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1345 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/internal/common.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.970187 seqslab-cli-3.2.1/python/seqslab/wes/resource/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/resource/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      883 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/resource/azure.py
--rw-r--r--   0 chris      (501) staff       (20)    11664 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/resource/base.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.972233 seqslab-cli-3.2.1/python/seqslab/wes/template/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/template/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     3467 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/template/base.py
--rw-r--r--   0 chris      (501) staff       (20)     3234 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/template/template.py
--rw-r--r--   0 chris      (501) staff       (20)     3269 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.974208 seqslab-cli-3.2.1/python/seqslab/workspace/
--rw-r--r--   0 chris      (501) staff       (20)      235 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     7064 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/commands.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.975239 seqslab-cli-3.2.1/python/seqslab/workspace/internal/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/internal/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1336 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/internal/common.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.977268 seqslab-cli-3.2.1/python/seqslab/workspace/resource/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/resource/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      863 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/resource/azure.py
--rw-r--r--   0 chris      (501) staff       (20)     4033 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/resource/base.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.981816 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     8762 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     3385 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       45 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)      429 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-26 05:38:21.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/zip-safe
--rw-r--r--   0 chris      (501) staff       (20)      373 2023-05-26 06:05:38.984138 seqslab-cli-3.2.1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     2182 2023-05-26 05:38:12.000000 seqslab-cli-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.857089 seqslab-cli-3.2.1.post0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/auth/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38488 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.861089 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/role/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.865089 seqslab-cli-3.2.1.post0/python/seqslab/role/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/runsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/runsheet/runsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/session_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/statusbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/trs/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/usage_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/user/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.869089 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/wes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 02:43:09.000000 seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-12 02:43:09.873089 seqslab-cli-3.2.1.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-12 02:42:59.000000 seqslab-cli-3.2.1.post0/setup.py
```

### Comparing `seqslab-cli-3.2.1/LICENSE` & `seqslab-cli-3.2.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/PKG-INFO` & `seqslab-cli-3.2.1.post0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,548 +1,602 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7365 7173  : 2.1.Name: seqs
-00000020: 6c61 622d 636c 690a 5665 7273 696f 6e3a  lab-cli.Version:
-00000030: 2033 2e32 2e31 0a53 756d 6d61 7279 3a20   3.2.1.Summary: 
-00000040: 4174 6765 6e6f 6d69 7820 5365 7173 4c61  Atgenomix SeqsLa
-00000050: 6220 434c 4920 666f 7220 5079 7468 6f6e  b CLI for Python
-00000060: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00000080: 6e6f 6d65 4741 502f 7365 7173 6c61 622d  nomeGAP/seqslab-
-00000090: 636c 690a 4175 7468 6f72 3a20 4a69 612d  cli.Author: Jia-
-000000a0: 596f 7520 4c69 6e0a 4175 7468 6f72 2d65  You Lin.Author-e
-000000b0: 6d61 696c 3a20 6a69 6179 6f75 2e6c 696e  mail: jiayou.lin
-000000c0: 4061 7467 656e 6f6d 6978 2e63 6f6d 0a4c  @atgenomix.com.L
-000000d0: 6963 656e 7365 3a20 4d49 5420 6c69 6365  icense: MIT lice
-000000e0: 6e73 650a 5072 6f6a 6563 742d 5552 4c3a  nse.Project-URL:
-000000f0: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
-00000100: 6874 7470 733a 2f2f 646f 6373 2e61 7467  https://docs.atg
-00000110: 656e 6f6d 6978 2e63 6f6d 2f0a 5072 6f6a  enomix.com/.Proj
-00000120: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
-00000130: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
-00000140: 6875 622e 636f 6d2f 416e 6f6d 6547 4150  hub.com/AnomeGAP
-00000150: 2f73 6571 736c 6162 2d63 6c69 0a43 6c61  /seqslab-cli.Cla
-00000160: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-00000170: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-00000180: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
-00000190: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-000001a0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000001b0: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
-000001c0: 7369 6669 6572 3a20 4f70 6572 6174 696e  sifier: Operatin
-000001d0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000001e0: 6e64 6570 656e 6465 6e74 0a43 6c61 7373  ndependent.Class
-000001f0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000210: 7974 686f 6e0a 436c 6173 7369 6669 6572  ython.Classifier
-00000220: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000230: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000240: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000250: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000270: 6f6e 203a 3a20 332e 390a 5265 7175 6972  on :: 3.9.Requir
-00000280: 6573 2d50 7974 686f 6e3a 203e 3d33 2e38  es-Python: >=3.8
-00000290: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000002a0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000002b0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-000002c0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-000002d0: 3c21 2d2d 2050 524f 4a45 4354 2053 4849  <!-- PROJECT SHI
-000002e0: 454c 4453 202d 2d3e 0a3c 212d 2d0a 2a2a  ELDS -->.<!--.**
-000002f0: 2a20 4927 6d20 7573 696e 6720 6d61 726b  * I'm using mark
-00000300: 646f 776e 2022 7265 6665 7265 6e63 6520  down "reference 
-00000310: 7374 796c 6522 206c 696e 6b73 2066 6f72  style" links for
-00000320: 2072 6561 6461 6269 6c69 7479 2e0a 2a2a   readability..**
-00000330: 2a20 5265 6665 7265 6e63 6520 6c69 6e6b  * Reference link
-00000340: 7320 6172 6520 656e 636c 6f73 6564 2069  s are enclosed i
-00000350: 6e20 6272 6163 6b65 7473 205b 205d 2069  n brackets [ ] i
-00000360: 6e73 7465 6164 206f 6620 7061 7265 6e74  nstead of parent
-00000370: 6865 7365 7320 2820 292e 0a2a 2a2a 2053  heses ( )..*** S
-00000380: 6565 2074 6865 2062 6f74 746f 6d20 6f66  ee the bottom of
-00000390: 2074 6869 7320 646f 6375 6d65 6e74 2066   this document f
-000003a0: 6f72 2074 6865 2064 6563 6c61 7261 7469  or the declarati
-000003b0: 6f6e 206f 6620 7468 6520 7265 6665 7265  on of the refere
-000003c0: 6e63 6520 7661 7269 6162 6c65 730a 2a2a  nce variables.**
-000003d0: 2a20 666f 7220 636f 6e74 7269 6275 746f  * for contributo
-000003e0: 7273 2d75 726c 2c20 666f 726b 732d 7572  rs-url, forks-ur
-000003f0: 6c2c 2065 7463 2e20 5468 6973 2069 7320  l, etc. This is 
-00000400: 616e 206f 7074 696f 6e61 6c2c 2063 6f6e  an optional, con
-00000410: 6369 7365 2073 796e 7461 7820 796f 7520  cise syntax you 
-00000420: 6d61 7920 7573 652e 0a2a 2a2a 2068 7474  may use..*** htt
-00000430: 7073 3a2f 2f77 7777 2e6d 6172 6b64 6f77  ps://www.markdow
-00000440: 6e67 7569 6465 2e6f 7267 2f62 6173 6963  nguide.org/basic
-00000450: 2d73 796e 7461 782f 2372 6566 6572 656e  -syntax/#referen
-00000460: 6365 2d73 7479 6c65 2d6c 696e 6b73 0a2d  ce-style-links.-
-00000470: 2d3e 0a5b 436f 6e74 7269 6275 746f 7273  ->.[Contributors
-00000480: 5d5b 636f 6e74 7269 6275 746f 7273 2d75  ][contributors-u
-00000490: 726c 5d0a 5b53 7461 7267 617a 6572 735d  rl].[Stargazers]
-000004a0: 5b73 7461 7273 2d75 726c 5d0a 5b49 7373  [stars-url].[Iss
-000004b0: 7565 735d 5b69 7373 7565 732d 7572 6c5d  ues][issues-url]
-000004c0: 0a5b 4c69 6365 6e73 655d 5b6c 6963 656e  .[License][licen
-000004d0: 7365 2d75 726c 5d0a 5b21 5b4c 696e 6b65  se-url].[![Linke
-000004e0: 6449 6e5d 5b6c 696e 6b65 6469 6e2d 7368  dIn][linkedin-sh
-000004f0: 6965 6c64 5d5d 5b6c 696e 6b65 6469 6e2d  ield]][linkedin-
-00000500: 7572 6c5d 0a0a 3c21 2d2d 2050 524f 4a45  url]..<!-- PROJE
-00000510: 4354 204c 4f47 4f20 2d2d 3e0a 3c62 7220  CT LOGO -->.<br 
-00000520: 2f3e 0a3c 7020 616c 6967 6e3d 2263 656e  />.<p align="cen
-00000530: 7465 7222 3e0a 2020 3c61 2068 7265 663d  ter">.  <a href=
-00000540: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000550: 636f 6d2f 416e 6f6d 6547 4150 2f73 6571  com/AnomeGAP/seq
-00000560: 736c 6162 2d63 6c69 223e 0a20 2020 203c  slab-cli">.    <
-00000570: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000580: 2f73 7461 7469 632e 7769 7873 7461 7469  /static.wixstati
-00000590: 632e 636f 6d2f 6d65 6469 612f 6637 6136  c.com/media/f7a6
-000005a0: 6135 5f31 6164 3730 6564 3035 6166 3034  a5_1ad70ed05af04
-000005b0: 6437 6562 3435 6565 3565 3264 6633 3437  d7eb45ee5e2df347
-000005c0: 6133 327e 6d76 325f 645f 3432 3636 5f34  a32~mv2_d_4266_4
-000005d0: 3434 395f 735f 345f 322e 6769 6622 2061  449_s_4_2.gif" a
-000005e0: 6c74 3d22 4c6f 676f 2220 7769 6474 683d  lt="Logo" width=
-000005f0: 2238 3022 2068 6569 6768 743d 2238 3022  "80" height="80"
-00000600: 3e0a 2020 3c2f 613e 0a0a 3c68 3220 616c  >.  </a>..<h2 al
-00000610: 6967 6e3d 2263 656e 7465 7222 3e41 7467  ign="center">Atg
-00000620: 656e 6f6d 6978 2053 6571 734c 6162 2056  enomix SeqsLab V
-00000630: 3320 706c 6174 666f 726d 2043 4c49 3c2f  3 platform CLI</
-00000640: 6832 3e0a 0a20 203c 7020 616c 6967 6e3d  h2>..  <p align=
-00000650: 2263 656e 7465 7222 3e0a 2020 2020 436f  "center">.    Co
-00000660: 6d6d 616e 6420 4c69 6e65 2049 6e74 6572  mmand Line Inter
-00000670: 6661 6365 2061 7070 6c69 6361 7469 6f6e  face application
-00000680: 2069 6e20 7468 6520 4174 6765 6e6f 6d69   in the Atgenomi
-00000690: 7820 5365 7173 4c61 6220 706c 6174 666f  x SeqsLab platfo
-000006a0: 726d 2c20 6120 636c 6f75 642d 6669 7273  rm, a cloud-firs
-000006b0: 7420 616e 6420 656e 7465 7270 7269 7365  t and enterprise
-000006c0: 2042 696f 4d65 642d 4954 2069 6e66 7261   BioMed-IT infra
-000006d0: 7374 7275 6374 7572 652e 0a20 2020 203c  structure..    <
-000006e0: 6272 202f 3e0a 2020 2020 3c61 2068 7265  br />.    <a hre
-000006f0: 663d 2268 7474 7073 3a2f 2f64 6f63 732e  f="https://docs.
-00000700: 6174 6765 6e6f 6d69 782e 636f 6d22 3e3c  atgenomix.com"><
-00000710: 7374 726f 6e67 3e45 7870 6c6f 7265 2074  strong>Explore t
-00000720: 6865 2064 6f63 7320 c2bb 3c2f 7374 726f  he docs ..</stro
-00000730: 6e67 3e3c 2f61 3e0a 2020 2020 3c62 7220  ng></a>.    <br 
-00000740: 2f3e 0a20 2020 203c 6272 202f 3e0a 2020  />.    <br />.  
-00000750: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000760: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
-00000770: 6f6d 6547 4150 2f73 6571 736c 6162 2d63  omeGAP/seqslab-c
-00000780: 6c69 2f69 7373 7565 7322 3e52 6570 6f72  li/issues">Repor
-00000790: 7420 4275 673c 2f61 3e0a 2020 2020 c2b7  t Bug</a>.    ..
-000007a0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
-000007b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000007c0: 2f41 6e6f 6d65 4741 502f 7365 7173 6c61  /AnomeGAP/seqsla
-000007d0: 622d 636c 692f 6973 7375 6573 223e 5265  b-cli/issues">Re
-000007e0: 7175 6573 7420 4665 6174 7572 653c 2f61  quest Feature</a
-000007f0: 3e0a 2020 3c2f 703e 0a3c 2f70 3e0a 0a3c  >.  </p>.</p>..<
-00000800: 212d 2d20 5441 424c 4520 4f46 2043 4f4e  !-- TABLE OF CON
-00000810: 5445 4e54 5320 2d2d 3e0a 3c64 6574 6169  TENTS -->.<detai
-00000820: 6c73 206f 7065 6e3d 226f 7065 6e22 3e0a  ls open="open">.
-00000830: 2020 3c73 756d 6d61 7279 3e54 6162 6c65    <summary>Table
-00000840: 206f 6620 436f 6e74 656e 7473 3c2f 7375   of Contents</su
-00000850: 6d6d 6172 793e 0a20 203c 6f6c 3e0a 2020  mmary>.  <ol>.  
-00000860: 2020 3c6c 693e 0a20 2020 2020 203c 6120    <li>.      <a 
-00000870: 6872 6566 3d22 2361 626f 7574 2d74 6865  href="#about-the
-00000880: 2d70 726f 6a65 6374 223e 4162 6f75 7420  -project">About 
-00000890: 5468 6520 5072 6f6a 6563 743c 2f61 3e0a  The Project</a>.
-000008a0: 2020 2020 2020 3c75 6c3e 0a20 2020 2020        <ul>.     
-000008b0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000008c0: 2362 7569 6c74 2d77 6974 6822 3e42 7569  #built-with">Bui
-000008d0: 6c74 2057 6974 683c 2f61 3e3c 2f6c 693e  lt With</a></li>
-000008e0: 0a20 2020 2020 203c 2f75 6c3e 0a20 2020  .      </ul>.   
-000008f0: 203c 2f6c 693e 0a20 2020 203c 6c69 3e0a   </li>.    <li>.
-00000900: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
-00000910: 6765 7474 696e 672d 7374 6172 7465 6422  getting-started"
-00000920: 3e47 6574 7469 6e67 2053 7461 7274 6564  >Getting Started
-00000930: 3c2f 613e 0a20 2020 2020 203c 756c 3e0a  </a>.      <ul>.
-00000940: 2020 2020 2020 2020 3c6c 693e 3c61 2068          <li><a h
-00000950: 7265 663d 2223 7072 6572 6571 7569 7369  ref="#prerequisi
-00000960: 7465 7322 3e50 7265 7265 7175 6973 6974  tes">Prerequisit
-00000970: 6573 3c2f 613e 3c2f 6c69 3e0a 2020 2020  es</a></li>.    
-00000980: 2020 2020 3c6c 693e 3c61 2068 7265 663d      <li><a href=
-00000990: 2223 7275 6e2d 696e 7465 7261 6374 6976  "#run-interactiv
-000009a0: 652d 6d6f 6465 223e 5275 6e20 696e 7465  e-mode">Run inte
-000009b0: 7261 6374 6976 6520 6d6f 6465 3c2f 613e  ractive mode</a>
-000009c0: 3c2f 6c69 3e0a 2020 2020 2020 3c2f 756c  </li>.      </ul
-000009d0: 3e0a 2020 2020 3c2f 6c69 3e0a 2020 2020  >.    </li>.    
-000009e0: 3c6c 693e 3c61 2068 7265 663d 2223 6465  <li><a href="#de
-000009f0: 7665 6c6f 7022 3e44 6576 656c 6f70 3c2f  velop">Develop</
-00000a00: 613e 3c2f 6c69 3e0a 2020 2020 3c6c 693e  a></li>.    <li>
-00000a10: 3c61 2068 7265 663d 2223 726f 6164 6d61  <a href="#roadma
-00000a20: 7022 3e52 6f61 646d 6170 3c2f 613e 3c2f  p">Roadmap</a></
-00000a30: 6c69 3e0a 2020 2020 3c6c 693e 3c61 2068  li>.    <li><a h
-00000a40: 7265 663d 2223 636f 6e74 7269 6275 7469  ref="#contributi
-00000a50: 6e67 223e 436f 6e74 7269 6275 7469 6e67  ng">Contributing
-00000a60: 3c2f 613e 3c2f 6c69 3e0a 2020 2020 3c6c  </a></li>.    <l
-00000a70: 693e 3c61 2068 7265 663d 2223 6c69 6365  i><a href="#lice
-00000a80: 6e73 6522 3e4c 6963 656e 7365 3c2f 613e  nse">License</a>
-00000a90: 3c2f 6c69 3e0a 2020 2020 3c6c 693e 3c61  </li>.    <li><a
-00000aa0: 2068 7265 663d 2223 636f 6e74 6163 7422   href="#contact"
-00000ab0: 3e43 6f6e 7461 6374 3c2f 613e 3c2f 6c69  >Contact</a></li
-00000ac0: 3e0a 2020 2020 3c6c 693e 3c61 2068 7265  >.    <li><a hre
-00000ad0: 663d 2223 6163 6b6e 6f77 6c65 6467 656d  f="#acknowledgem
-00000ae0: 656e 7473 223e 4163 6b6e 6f77 6c65 6467  ents">Acknowledg
-00000af0: 656d 656e 7473 3c2f 613e 3c2f 6c69 3e0a  ements</a></li>.
-00000b00: 2020 3c2f 6f6c 3e0a 3c2f 6465 7461 696c    </ol>.</detail
-00000b10: 733e 0a0a 3c21 2d2d 2041 424f 5554 2054  s>..<!-- ABOUT T
-00000b20: 4845 2050 524f 4a45 4354 202d 2d3e 0a0a  HE PROJECT -->..
-00000b30: 2323 2041 626f 7574 2054 6865 2050 726f  ## About The Pro
-00000b40: 6a65 6374 0a0a 0a53 6571 734c 6162 2043  ject...SeqsLab C
-00000b50: 4c49 2069 7320 7468 6520 6164 7661 6e63  LI is the advanc
-00000b60: 6564 2075 7365 7220 6661 6369 6e67 2069  ed user facing i
-00000b70: 6e74 6572 6661 6365 2074 6f20 696e 7465  nterface to inte
-00000b80: 7261 6374 6976 656c 7920 616e 6420 6175  ractively and au
-00000b90: 746f 6d61 7469 6361 6c6c 7920 6163 6365  tomatically acce
-00000ba0: 7373 2053 6571 734c 6162 2063 6c6f 7564  ss SeqsLab cloud
-00000bb0: 2070 6c61 7466 6f72 6d20 7669 610a 5365   platform via.Se
-00000bc0: 7173 4c61 6220 5245 5354 6675 6c20 4150  qsLab RESTful AP
-00000bd0: 4973 2e20 436f 6d70 6c65 6d65 6e74 6172  Is. Complementar
-00000be0: 7920 7769 7468 2074 6865 2077 6562 2d62  y with the web-b
-00000bf0: 6173 6564 2053 6571 734c 6162 2043 6f6e  ased SeqsLab Con
-00000c00: 736f 6c65 2c20 7468 6520 636f 6d6d 616e  sole, the comman
-00000c10: 6420 6c69 6e65 2061 7070 6c69 6361 7469  d line applicati
-00000c20: 6f6e 2061 6c6c 6f77 7320 6269 6f69 6e66  on allows bioinf
-00000c30: 6f72 6d61 7469 6369 616e 730a 616e 6420  ormaticians.and 
-00000c40: 696e 7665 7374 6967 6174 6f72 7320 746f  investigators to
-00000c50: 2065 6173 696c 7920 6275 696c 6420 6375   easily build cu
-00000c60: 7374 6f6d 2073 6372 6970 7473 2061 6e64  stom scripts and
-00000c70: 2061 7574 6f6d 6174 6520 6f77 6e20 776f   automate own wo
-00000c80: 726b 666c 6f77 7320 706f 7765 7265 6420  rkflows powered 
-00000c90: 6279 2074 6865 2053 6571 734c 6162 2070  by the SeqsLab p
-00000ca0: 6c61 7466 6f72 6d20 696e 6672 6173 7472  latform infrastr
-00000cb0: 7563 7475 7265 0a74 6563 686e 6f6c 6f67  ucture.technolog
-00000cc0: 6965 732e 0a0a 5479 7069 6361 6c20 7573  ies...Typical us
-00000cd0: 6520 6361 7365 733a 0a0a 2a20 4275 696c  e cases:..* Buil
-00000ce0: 6420 6175 746f 6d61 7465 6420 6461 7461  d automated data
-00000cf0: 2070 726f 6475 6374 696f 6e20 7468 6174   production that
-00000d00: 2075 706c 6f61 6473 2061 6e64 2064 6f77   uploads and dow
-00000d10: 6e6c 6f61 6473 2073 6571 7565 6e63 696e  nloads sequencin
-00000d20: 6720 6461 7461 7365 7473 2074 6f2f 6672  g datasets to/fr
-00000d30: 6f6d 2074 6865 2053 6571 734c 6162 2044  om the SeqsLab D
-00000d40: 6174 6120 4875 6220 636c 6f75 6420 7374  ata Hub cloud st
-00000d50: 6f72 6167 652e 0a2a 2053 7562 6d69 7420  orage..* Submit 
-00000d60: 776f 726b 666c 6f77 2072 756e 7320 6f6e  workflow runs on
-00000d70: 2064 656d 616e 6420 7669 6120 5365 7173   demand via Seqs
-00000d80: 4c61 6220 5745 5320 4150 4973 2061 6e64  Lab WES APIs and
-00000d90: 2069 6e74 6567 7261 7465 2077 6974 6820   integrate with 
-00000da0: 6c6f 6361 6c20 646f 776e 7374 7265 616d  local downstream
-00000db0: 2061 6e61 6c79 7369 732e 0a2a 2055 7365   analysis..* Use
-00000dc0: 2061 7320 6175 6469 7420 6c6f 6720 6465   as audit log de
-00000dd0: 7669 6365 2074 6f20 7669 6577 2070 6c61  vice to view pla
-00000de0: 7466 6f72 6d20 7573 6520 6163 7469 7669  tform use activi
-00000df0: 7469 6573 2e0a 0a53 6571 734c 6162 2043  ties...SeqsLab C
-00000e00: 4c49 2073 6861 6c6c 2062 6520 7468 6520  LI shall be the 
-00000e10: 7374 616e 6461 7264 2066 7261 6d65 776f  standard framewo
-00000e20: 726b 2074 6f20 6465 7665 6c6f 7020 636f  rk to develop co
-00000e30: 6d6d 616e 6420 746f 6f6c 6b69 7473 2061  mmand toolkits a
-00000e40: 6e64 2070 726f 7669 6465 2061 7320 7468  nd provide as th
-00000e50: 6520 5365 7173 4c61 6220 706c 6174 666f  e SeqsLab platfo
-00000e60: 726d 2075 7469 6c69 7479 2e0a 0a23 2323  rm utility...###
-00000e70: 2042 7569 6c74 2057 6974 680a 0a53 6571   Built With..Seq
-00000e80: 734c 6162 2043 4c49 2069 7320 6275 696c  sLab CLI is buil
-00000e90: 7420 7769 7468 2074 6865 2066 6f6c 6c6f  t with the follo
-00000ea0: 7769 6e67 206d 616a 6f72 2066 7261 6d65  wing major frame
-00000eb0: 776f 726b 733a 0a0a 2a20 5b53 6571 734c  works:..* [SeqsL
-00000ec0: 6162 2041 5049 735d 2868 7474 7073 3a2f  ab APIs](https:/
-00000ed0: 2f61 7069 2e73 6571 736c 6162 2e6e 6574  /api.seqslab.net
-00000ee0: 2f29 0a2a 205b 5079 7468 6f6e 2d4e 7562  /).* [Python-Nub
-00000ef0: 6961 5d28 6874 7470 733a 2f2f 6769 7468  ia](https://gith
-00000f00: 7562 2e63 6f6d 2f66 6163 6562 6f6f 6b69  ub.com/facebooki
-00000f10: 6e63 7562 6174 6f72 2f70 7974 686f 6e2d  ncubator/python-
-00000f20: 6e75 6269 6129 0a2a 205b 4d53 414c 2050  nubia).* [MSAL P
-00000f30: 7974 686f 6e5d 2868 7474 7073 3a2f 2f6d  ython](https://m
-00000f40: 7361 6c2d 7079 7468 6f6e 2e72 6561 6474  sal-python.readt
-00000f50: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000f60: 6573 742f 290a 2a20 5b41 7a75 7265 2053  est/).* [Azure S
-00000f70: 444b 5d28 6874 7470 733a 2f2f 6769 7468  DK](https://gith
-00000f80: 7562 2e63 6f6d 2f41 7a75 7265 2f61 7a75  ub.com/Azure/azu
-00000f90: 7265 2d73 646b 290a 2a20 5b61 696f 6874  re-sdk).* [aioht
-00000fa0: 7470 5d28 6874 7470 733a 2f2f 646f 6373  tp](https://docs
-00000fb0: 2e61 696f 6874 7470 2e6f 7267 2f65 6e2f  .aiohttp.org/en/
-00000fc0: 7374 6162 6c65 2f69 6e64 6578 2e68 746d  stable/index.htm
-00000fd0: 6c29 0a0a 5365 6375 7269 7479 2069 6e66  l)..Security inf
-00000fe0: 6f72 6d61 7469 6f6e 2070 726f 7465 6374  ormation protect
-00000ff0: 696f 6e20 6973 2073 6563 7572 6564 2061  ion is secured a
-00001000: 6e64 2062 7569 6c74 2077 6974 6820 6120  nd built with a 
-00001010: 7379 7374 656d 206b 6579 7269 6e67 2073  system keyring s
-00001020: 6572 7669 6365 3a0a 0a2a 205b 4b65 7972  ervice:..* [Keyr
-00001030: 696e 675d 2868 7474 7073 3a2f 2f70 7970  ing](https://pyp
-00001040: 692e 6f72 672f 7072 6f6a 6563 742f 6b65  i.org/project/ke
-00001050: 7972 696e 672f 290a 0a3c 212d 2d20 4745  yring/)..<!-- GE
-00001060: 5454 494e 4720 5354 4152 5445 4420 2d2d  TTING STARTED --
-00001070: 3e0a 0a23 2320 4765 7474 696e 6720 5374  >..## Getting St
-00001080: 6172 7465 640a 0a54 6f20 6765 7420 6120  arted..To get a 
-00001090: 6c6f 6361 6c20 636f 7079 2075 7020 616e  local copy up an
-000010a0: 6420 7275 6e6e 696e 672c 2066 6f6c 6c6f  d running, follo
-000010b0: 7720 7468 6573 6520 7369 6d70 6c65 2073  w these simple s
-000010c0: 7465 7073 2e0a 0a23 2323 2050 7265 7265  teps...### Prere
-000010d0: 7175 6973 6974 6573 0a0a 5468 6573 6520  quisites..These 
-000010e0: 7265 636f 6d6d 656e 6465 6420 5b6b 6579  recommended [key
-000010f0: 7269 6e67 5d28 6874 7470 733a 2f2f 7079  ring](https://py
-00001100: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6b  pi.org/project/k
-00001110: 6579 7269 6e67 2f29 2062 6163 6b65 6e64  eyring/) backend
-00001120: 7320 6172 6520 7375 7070 6f72 7465 6420  s are supported 
-00001130: 696e 2074 6869 7320 7061 636b 6167 653a  in this package:
-00001140: 0a0a 2a20 6d61 634f 5320 5b4b 6579 6368  ..* macOS [Keych
-00001150: 6169 6e5d 2868 7474 7073 3a2f 2f65 6e2e  ain](https://en.
-00001160: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-00001170: 6b69 2f4b 6579 6368 6169 6e5f 2532 3873  ki/Keychain_%28s
-00001180: 6f66 7477 6172 6525 3239 290a 2a20 4672  oftware%29).* Fr
-00001190: 6565 6465 736b 746f 7020 5b53 6563 7265  eedesktop [Secre
-000011a0: 7420 5365 7276 6963 655d 2868 7474 703a  t Service](http:
-000011b0: 2f2f 7374 616e 6461 7264 732e 6672 6565  //standards.free
-000011c0: 6465 736b 746f 702e 6f72 672f 7365 6372  desktop.org/secr
-000011d0: 6574 2d73 6572 7669 6365 2f29 2073 7570  et-service/) sup
-000011e0: 706f 7274 7320 6d61 6e79 2044 4520 696e  ports many DE in
-000011f0: 636c 7564 696e 6720 474e 4f4d 4520 280a  cluding GNOME (.
-00001200: 2020 7265 7175 6972 6573 205b 7365 6372    requires [secr
-00001210: 6574 7374 6f72 6167 655d 2868 7474 7073  etstorage](https
-00001220: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
-00001230: 7267 2f70 7970 692f 7365 6372 6574 7374  rg/pypi/secretst
-00001240: 6f72 6167 6529 290a 2a20 4b44 4534 2026  orage)).* KDE4 &
-00001250: 204b 4445 3520 5b4b 5761 6c6c 6574 5d28   KDE5 [KWallet](
-00001260: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00001270: 6564 6961 2e6f 7267 2f77 696b 692f 4b57  edia.org/wiki/KW
-00001280: 616c 6c65 7429 2028 0a20 2072 6571 7569  allet) (.  requi
-00001290: 7265 7320 5b64 6275 735d 2868 7474 7073  res [dbus](https
-000012a0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
-000012b0: 7267 2f70 7970 692f 6462 7573 2d70 7974  rg/pypi/dbus-pyt
-000012c0: 686f 6e29 290a 2a20 5b57 696e 646f 7773  hon)).* [Windows
-000012d0: 2043 7265 6465 6e74 6961 6c20 4c6f 636b   Credential Lock
-000012e0: 6572 5d28 6874 7470 733a 2f2f 646f 6373  er](https://docs
-000012f0: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f65  .microsoft.com/e
-00001300: 6e2d 7573 2f77 696e 646f 7773 2f75 7770  n-us/windows/uwp
-00001310: 2f73 6563 7572 6974 792f 6372 6564 656e  /security/creden
-00001320: 7469 616c 2d6c 6f63 6b65 7229 0a0a 2323  tial-locker)..##
-00001330: 2323 204d 6163 4f53 0a0a 2323 2323 2320  ## MacOS..##### 
-00001340: 466f 7220 4d61 634f 5320 6465 7669 6365  For MacOS device
-00001350: 732c 2079 6f75 2073 686f 756c 6420 6669  s, you should fi
-00001360: 7273 7420 696e 7374 616c 6c20 7468 6520  rst install the 
-00001370: 666f 6c6c 6f77 696e 6720 7061 636b 6167  following packag
-00001380: 6573 3a0a 0a2a 205b 706b 672d 636f 6e66  es:..* [pkg-conf
-00001390: 6967 5d28 6874 7470 733a 2f2f 666f 726d  ig](https://form
-000013a0: 756c 6165 2e62 7265 772e 7368 2f66 6f72  ulae.brew.sh/for
-000013b0: 6d75 6c61 2f70 6b67 2d63 6f6e 6669 6729  mula/pkg-config)
-000013c0: 0a2a 205b 6462 7573 5d28 6874 7470 733a  .* [dbus](https:
-000013d0: 2f2f 666f 726d 756c 6165 2e62 7265 772e  //formulae.brew.
-000013e0: 7368 2f66 6f72 6d75 6c61 2f64 6275 7329  sh/formula/dbus)
-000013f0: 0a2a 205b 676c 6962 5d28 6874 7470 733a  .* [glib](https:
-00001400: 2f2f 666f 726d 756c 6165 2e62 7265 772e  //formulae.brew.
-00001410: 7368 2f66 6f72 6d75 6c61 2f67 6c69 6229  sh/formula/glib)
-00001420: 0a0a 6f72 0a0a 6060 6062 6173 680a 2320  ..or..```bash.# 
-00001430: 696e 7374 616c 6c20 7061 636b 6167 6573  install packages
-00001440: 3a0a 6272 6577 2069 6e73 7461 6c6c 2064  :.brew install d
-00001450: 6275 730a 0a62 7265 7720 696e 7374 616c  bus..brew instal
-00001460: 6c20 706b 672d 636f 6e66 6967 200a 6272  l pkg-config .br
-00001470: 6577 2069 6e73 7461 6c6c 2067 6c69 620a  ew install glib.
-00001480: 0a60 6060 0a0a 5468 6520 666f 6c6c 6f77  .```..The follow
-00001490: 696e 6720 6973 2061 6e20 6578 616d 706c  ing is an exampl
-000014a0: 6520 6f66 2068 6f77 2074 6f20 6c69 7374  e of how to list
-000014b0: 2074 6865 2074 6869 6e67 7320 796f 7520   the things you 
-000014c0: 6e65 6564 2074 6f20 7573 6520 7468 6520  need to use the 
-000014d0: 736f 6674 7761 7265 2061 6e64 2068 6f77  software and how
-000014e0: 2074 6f20 696e 7374 616c 6c20 7468 656d   to install them
-000014f0: 2e0a 0a2a 2055 7369 6e67 204b 6579 7269  ...* Using Keyri
-00001500: 6e67 206f 6e20 6865 6164 6c65 7373 204c  ng on headless L
-00001510: 696e 7578 2073 7973 7465 6d73 2069 6e20  inux systems in 
-00001520: 6120 446f 636b 6572 2063 6f6e 7461 696e  a Docker contain
-00001530: 6572 0a0a 2020 4368 6563 6b20 6f75 7420  er..  Check out 
-00001540: 5b4b 6579 7269 6e67 5d28 6874 7470 733a  [Keyring](https:
-00001550: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00001560: 6374 2f6b 6579 7269 6e67 2f29 2066 6f72  ct/keyring/) for
-00001570: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00001580: 686f 7720 746f 2075 7365 204b 6579 7269  how to use Keyri
-00001590: 6e67 206f 6e20 6120 6865 6164 6c65 7373  ng on a headless
-000015a0: 204c 696e 7578 2073 7973 7465 6d20 6173   Linux system as
-000015b0: 2077 656c 6c20 6173 2069 6e20 6120 446f   well as in a Do
-000015c0: 636b 6572 0a20 2063 6f6e 7461 696e 6572  cker.  container
-000015d0: 2e0a 0a2a 2050 7974 686f 6e20 5665 7273  ...* Python Vers
-000015e0: 696f 6e20 332e 382b 0a2a 2050 7974 686f  ion 3.8+.* Pytho
-000015f0: 6e20 7669 7274 7561 6c20 656e 7669 726f  n virtual enviro
-00001600: 6e6d 656e 740a 0a20 2060 6060 6261 7368  nment..  ```bash
-00001610: 0a20 2070 6970 3320 696e 7374 616c 6c20  .  pip3 install 
-00001620: 7365 7173 6c61 622d 636c 690a 2020 6060  seqslab-cli.  ``
-00001630: 600a 0a23 2323 2052 756e 2069 6e74 6572  `..### Run inter
-00001640: 6163 7469 7665 206d 6f64 650a 0a2a 2044  active mode..* D
-00001650: 6973 706c 6179 2061 7661 696c 6162 6c65  isplay available
-00001660: 2063 6f6d 6d61 6e64 730a 2020 6060 6062   commands.  ```b
-00001670: 6173 680a 2020 7365 7173 6c61 623e 2068  ash.  seqslab> h
-00001680: 656c 700a 2020 6060 600a 0a23 2323 2052  elp.  ```..### R
-00001690: 756e 206e 6f6e 2d69 6e74 6572 6163 7469  un non-interacti
-000016a0: 7665 206d 6f64 650a 0a54 6865 206e 6f6e  ve mode..The non
-000016b0: 2d69 6e74 6572 6163 7469 7665 206d 6f64  -interactive mod
-000016c0: 6520 776f 726b 7320 6578 6163 746c 7920  e works exactly 
-000016d0: 6c69 6b65 2061 6e79 2074 7261 6469 7469  like any traditi
-000016e0: 6f6e 616c 204c 696e 7578 2d62 6173 6564  onal Linux-based
-000016f0: 2063 6f6d 6d61 6e64 206c 696e 6520 7574   command line ut
-00001700: 696c 6974 792e 0a0a 2323 2320 4175 7468  ility...### Auth
-00001710: 656e 7469 6361 7465 2077 6974 6820 5365  enticate with Se
-00001720: 7173 4c61 6220 4150 490a 0a2a 2053 6574  qsLab API..* Set
-00001730: 2070 6c61 7466 6f72 6d20 6261 636b 656e   platform backen
-00001740: 6420 746f 2075 7365 2077 6865 6e20 6c61  d to use when la
-00001750: 756e 6368 696e 6720 5365 7173 4c61 6220  unching SeqsLab 
-00001760: 434c 492e 2054 6865 2064 6566 6175 6c74  CLI. The default
-00001770: 2076 616c 7565 2069 7320 2261 7a75 7265   value is "azure
-00001780: 222e 0a0a 2020 6060 6062 6173 680a 2020  "...  ```bash.  
-00001790: 7365 7173 6c61 6220 2d2d 6261 636b 656e  seqslab --backen
-000017a0: 6420 617a 7572 650a 2020 6060 600a 0a2a  d azure.  ```..*
-000017b0: 2053 696e 676c 6520 636f 6d6d 616e 6420   Single command 
-000017c0: 746f 2073 6967 6e20 696e 2074 6f20 5365  to sign in to Se
-000017d0: 7173 4c61 6220 4150 4920 616e 6420 6f62  qsLab API and ob
-000017e0: 7461 696e 2041 5049 2074 6f6b 656e 732e  tain API tokens.
-000017f0: 2042 7920 6465 6661 756c 742c 2073 6967   By default, sig
-00001800: 6e69 6e20 636f 6d6d 616e 6420 7573 6573  nin command uses
-00001810: 2064 6576 6963 6520 636f 6465 2066 6c6f   device code flo
-00001820: 7720 666f 720a 2020 6272 6f77 7365 726c  w for.  browserl
-00001830: 6573 7320 7379 7374 656d 2e0a 0a20 2060  ess system...  `
-00001840: 6060 6261 7368 0a20 2061 7574 6820 7369  ``bash.  auth si
-00001850: 676e 696e 0a20 2060 6060 0a0a 2020 5365  gnin.  ```..  Se
-00001860: 7420 6064 6576 6963 652d 636f 6465 6020  t `device-code` 
-00001870: 6172 6775 6d65 6e74 2074 6f20 5472 7565  argument to True
-00001880: 2066 6f72 2064 6576 6963 6520 6175 7468   for device auth
-00001890: 6f72 697a 6174 696f 6e20 6772 616e 7420  orization grant 
-000018a0: 666c 6f77 2e20 4279 2064 6566 6175 6c74  flow. By default
-000018b0: 2c20 7369 676e 696e 2075 7365 7320 7468  , signin uses th
-000018c0: 6520 6175 7468 2063 6f64 6520 666c 6f77  e auth code flow
-000018d0: 2e0a 0a20 2060 6060 6261 7368 0a20 2061  ...  ```bash.  a
-000018e0: 7574 6820 7369 676e 696e 2064 6576 6963  uth signin devic
-000018f0: 652d 636f 6465 3d54 7275 650a 2020 6060  e-code=True.  ``
-00001900: 600a 0a2a 2047 6574 2041 5049 2061 6363  `..* Get API acc
-00001910: 6573 7320 746f 6b65 6e20 746f 2069 6e74  ess token to int
-00001920: 6572 6163 7420 7769 7468 2053 6571 734c  eract with SeqsL
-00001930: 6162 2041 5049 2061 7070 7320 696e 2079  ab API apps in y
-00001940: 6f75 7220 636f 6d6d 616e 6473 2e0a 0a20  our commands... 
-00001950: 2060 6060 7079 7468 6f6e 0a20 2066 726f   ```python.  fro
-00001960: 6d20 7365 7173 6c61 622e 6175 7468 2e63  m seqslab.auth.c
-00001970: 6f6d 6d61 6e64 7320 696d 706f 7274 2041  ommands import A
-00001980: 7574 680a 2020 0a20 2074 6f6b 656e 203d  uth.  .  token =
-00001990: 2041 7574 682e 6765 745f 746f 6b65 6e28   Auth.get_token(
-000019a0: 290a 2020 6163 6365 7373 203d 2074 6f6b  ).  access = tok
-000019b0: 656e 2e67 6574 2822 746f 6b65 6e73 2229  en.get("tokens")
-000019c0: 2e67 6574 2822 6163 6365 7373 2229 0a20  .get("access"). 
-000019d0: 2023 2075 7365 2074 6f6b 656e 2069 6e20   # use token in 
-000019e0: 796f 7572 2072 6571 7565 7374 2068 6561  your request hea
-000019f0: 6465 722c 2065 783a 2041 7574 686f 7269  der, ex: Authori
-00001a00: 7a61 7469 6f6e 3a20 4265 6172 6572 207b  zation: Bearer {
-00001a10: 6163 6365 7373 7d0a 2020 6174 7472 7320  access}.  attrs 
-00001a20: 3d20 746f 6b65 6e2e 6765 7428 2261 7474  = token.get("att
-00001a30: 7273 2229 0a20 2023 2061 7474 7273 2069  rs").  # attrs i
-00001a40: 7320 6120 6469 6374 696f 6e61 7279 2063  s a dictionary c
-00001a50: 6f6e 7461 696e 696e 6720 7468 6520 696e  ontaining the in
-00001a60: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-00001a70: 7468 6520 7369 676e 696e 672d 696e 2075  the signing-in u
-00001a80: 7365 722e 0a20 2060 6060 0a0a 2020 6041  ser..  ```..  `A
-00001a90: 7574 682e 6765 745f 746f 6b65 6e28 2960  uth.get_token()`
-00001aa0: 2077 696c 6c20 6175 746f 6d61 7469 6361   will automatica
-00001ab0: 6c6c 7920 7265 6672 6573 6820 7468 6520  lly refresh the 
-00001ac0: 6163 6365 7373 2074 6f6b 656e 2069 6620  access token if 
-00001ad0: 6578 7069 7265 642e 2057 6865 6e20 7265  expired. When re
-00001ae0: 6672 6573 6820 746f 6b65 6e20 6578 7069  fresh token expi
-00001af0: 7265 732c 2074 6865 2066 756e 6374 696f  res, the functio
-00001b00: 6e0a 2020 7265 7475 726e 7320 4e6f 6e65  n.  returns None
-00001b10: 2069 6620 7573 6572 7320 6e65 6564 2074   if users need t
-00001b20: 6f20 7369 676e 2062 6163 6b20 696e 2074  o sign back in t
-00001b30: 6f20 5365 7173 4c61 6220 4150 492e 0a0a  o SeqsLab API...
-00001b40: 2020 5468 6520 746f 6b65 6e73 2061 7265    The tokens are
-00001b50: 2070 6572 7369 7374 656e 746c 7920 6361   persistently ca
-00001b60: 6368 6564 2069 6e20 7468 6520 7379 7374  ched in the syst
-00001b70: 656d 2d73 7570 706f 7274 6564 2073 6563  em-supported sec
-00001b80: 7265 7420 7365 7276 6963 652c 2073 7563  ret service, suc
-00001b90: 6820 6173 2046 7265 6564 6573 6b74 6f70  h as Freedesktop
-00001ba0: 2053 6563 7265 7420 5365 7276 6963 6520   Secret Service 
-00001bb0: 616e 640a 2020 6d61 634f 5320 4b65 7963  and.  macOS Keyc
-00001bc0: 6861 696e 2e20 4173 2061 2072 6573 756c  hain. As a resul
-00001bd0: 742c 2074 6865 2076 616c 6964 2061 6363  t, the valid acc
-00001be0: 6573 7320 746f 6b65 6e20 6361 6e20 6265  ess token can be
-00001bf0: 2075 7365 6420 6163 726f 7373 206d 756c   used across mul
-00001c00: 7469 706c 6520 434c 4920 7365 7373 696f  tiple CLI sessio
-00001c10: 6e73 2e0a 0a3c 212d 2d20 524f 4144 4d41  ns...<!-- ROADMA
-00001c20: 5020 2d2d 3e0a 0a23 2320 526f 6164 6d61  P -->..## Roadma
-00001c30: 700a 0a53 6565 2074 6865 205b 6f70 656e  p..See the [open
-00001c40: 2069 7373 7565 735d 2868 7474 7073 3a2f   issues](https:/
-00001c50: 2f67 6974 6875 622e 636f 6d2f 416e 6f6d  /github.com/Anom
-00001c60: 6547 4150 2f73 6571 736c 6162 2d63 6c69  eGAP/seqslab-cli
-00001c70: 2f69 7373 7565 7329 2066 6f72 2061 206c  /issues) for a l
-00001c80: 6973 7420 6f66 2070 726f 706f 7365 6420  ist of proposed 
-00001c90: 6665 6174 7572 6573 2028 616e 6420 6b6e  features (and kn
-00001ca0: 6f77 6e20 6973 7375 6573 290a 2e0a 0a0a  own issues).....
-00001cb0: 0a3c 212d 2d20 434f 4e54 5249 4255 5449  .<!-- CONTRIBUTI
-00001cc0: 4e47 202d 2d3e 0a0a 2323 2043 6f6e 7472  NG -->..## Contr
-00001cd0: 6962 7574 696e 670a 0a57 6520 646f 6e27  ibuting..We don'
-00001ce0: 7420 6375 7272 656e 746c 7920 6f70 656e  t currently open
-00001cf0: 2074 6f20 7468 6520 636f 6d6d 756e 6974   to the communit
-00001d00: 7920 666f 7220 636f 6e74 7269 6275 7469  y for contributi
-00001d10: 6f6e 2c20 6275 7420 7769 6c6c 2069 6e20  on, but will in 
-00001d20: 7468 6520 6675 7475 7265 2e0a 0a0a 3c21  the future....<!
-00001d30: 2d2d 204c 4943 454e 5345 202d 2d3e 0a0a  -- LICENSE -->..
-00001d40: 2323 204c 6963 656e 7365 0a0a 5365 6520  ## License..See 
-00001d50: 604c 4943 454e 5345 6020 666f 7220 6d6f  `LICENSE` for mo
-00001d60: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0a  re information..
-00001d70: 0a0a 0a3c 212d 2d20 434f 4e54 4143 5420  ...<!-- CONTACT 
-00001d80: 2d2d 3e0a 0a23 2320 436f 6e74 6163 740a  -->..## Contact.
-00001d90: 0a41 6c6c 656e 2043 6861 6e67 202d 205b  .Allen Chang - [
-00001da0: 4c69 6e6b 6564 496e 5d28 6874 7470 733a  LinkedIn](https:
-00001db0: 2f2f 7777 772e 6c69 6e6b 6564 696e 2e63  //www.linkedin.c
-00001dc0: 6f6d 2f69 6e2f 616c 6c65 6e2d 6368 616e  om/in/allen-chan
-00001dd0: 672f 2920 2d20 616c 6c65 6e2e 6368 616e  g/) - allen.chan
-00001de0: 6740 6174 6765 6e6f 6d69 782e 636f 6d0a  g@atgenomix.com.
-00001df0: 0a50 726f 6a65 6374 204c 696e 6b3a 205b  .Project Link: [
-00001e00: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001e10: 6f6d 2f61 7467 656e 6f6d 6978 5d28 6874  om/atgenomix](ht
-00001e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001e30: 2f61 7467 656e 6f6d 6978 290a 0a0a 0a3c  /atgenomix)....<
-00001e40: 212d 2d20 4143 4b4e 4f57 4c45 4447 454d  !-- ACKNOWLEDGEM
-00001e50: 454e 5453 202d 2d3e 0a0a 2323 2041 636b  ENTS -->..## Ack
-00001e60: 6e6f 776c 6564 6765 6d65 6e74 730a 0a2a  nowledgements..*
-00001e70: 205b 4661 6365 626f 6f6b 2049 6e63 7562   [Facebook Incub
-00001e80: 6174 6f72 5d28 6874 7470 733a 2f2f 6769  ator](https://gi
-00001e90: 7468 7562 2e63 6f6d 2f66 6163 6562 6f6f  thub.com/faceboo
-00001ea0: 6b69 6e63 7562 6174 6f72 290a 2a20 5b4d  kincubator).* [M
-00001eb0: 6963 726f 736f 6674 2069 6465 6e74 6974  icrosoft identit
-00001ec0: 7920 706c 6174 666f 726d 5d28 6874 7470  y platform](http
-00001ed0: 733a 2f2f 646f 6373 2e6d 6963 726f 736f  s://docs.microso
-00001ee0: 6674 2e63 6f6d 2f65 6e2d 7573 2f61 7a75  ft.com/en-us/azu
-00001ef0: 7265 2f61 6374 6976 652d 6469 7265 6374  re/active-direct
-00001f00: 6f72 792f 6465 7665 6c6f 702f 6163 7469  ory/develop/acti
-00001f10: 7665 2d64 6972 6563 746f 7279 2d76 322d  ve-directory-v2-
-00001f20: 7072 6f74 6f63 6f6c 7329 0a2a 205b 4741  protocols).* [GA
-00001f30: 3447 485d 2868 7474 7073 3a2f 2f77 7777  4GH](https://www
-00001f40: 2e67 6134 6768 2e6f 7267 2f29 0a2a 205b  .ga4gh.org/).* [
-00001f50: 4265 7374 2d52 4541 444d 452d 5465 6d70  Best-README-Temp
-00001f60: 6c61 7465 5d28 6874 7470 733a 2f2f 6769  late](https://gi
-00001f70: 7468 7562 2e63 6f6d 2f6f 7468 6e65 696c  thub.com/othneil
-00001f80: 6472 6577 2f42 6573 742d 5245 4144 4d45  drew/Best-README
-00001f90: 2d54 656d 706c 6174 6529 0a0a 3c21 2d2d  -Template)..<!--
-00001fa0: 204d 4152 4b44 4f57 4e20 4c49 4e4b 5320   MARKDOWN LINKS 
-00001fb0: 2620 494d 4147 4553 202d 2d3e 0a3c 212d  & IMAGES -->.<!-
-00001fc0: 2d20 6874 7470 733a 2f2f 7777 772e 6d61  - https://www.ma
-00001fd0: 726b 646f 776e 6775 6964 652e 6f72 672f  rkdownguide.org/
-00001fe0: 6261 7369 632d 7379 6e74 6178 2f23 7265  basic-syntax/#re
-00001ff0: 6665 7265 6e63 652d 7374 796c 652d 6c69  ference-style-li
-00002000: 6e6b 7320 2d2d 3e0a 0a5b 636f 6e74 7269  nks -->..[contri
-00002010: 6275 746f 7273 2d75 726c 5d3a 2068 7474  butors-url]: htt
-00002020: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002030: 416e 6f6d 6547 4150 2f73 6571 736c 6162  AnomeGAP/seqslab
-00002040: 2d63 6c69 2f67 7261 7068 732f 636f 6e74  -cli/graphs/cont
-00002050: 7269 6275 746f 7273 0a0a 5b73 7461 7273  ributors..[stars
-00002060: 2d75 726c 5d3a 2068 7474 7073 3a2f 2f67  -url]: https://g
-00002070: 6974 6875 622e 636f 6d2f 416e 6f6d 6547  ithub.com/AnomeG
-00002080: 4150 2f73 6571 736c 6162 2d63 6c69 2f73  AP/seqslab-cli/s
-00002090: 7461 7267 617a 6572 730a 0a5b 6973 7375  targazers..[issu
-000020a0: 6573 2d75 726c 5d3a 2068 7474 7073 3a2f  es-url]: https:/
-000020b0: 2f67 6974 6875 622e 636f 6d2f 416e 6f6d  /github.com/Anom
-000020c0: 6547 4150 2f73 6571 736c 6162 2d63 6c69  eGAP/seqslab-cli
-000020d0: 2f69 7373 7565 730a 0a5b 6c69 6365 6e73  /issues..[licens
-000020e0: 652d 7572 6c5d 3a20 6874 7470 733a 2f2f  e-url]: https://
-000020f0: 6769 7468 7562 2e63 6f6d 2f41 6e6f 6d65  github.com/Anome
-00002100: 4741 502f 7365 7173 6c61 622d 636c 692f  GAP/seqslab-cli/
-00002110: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
-00002120: 452e 7478 740a 0a5b 6c69 6e6b 6564 696e  E.txt..[linkedin
-00002130: 2d73 6869 656c 645d 3a20 6874 7470 733a  -shield]: https:
-00002140: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00002150: 2f62 6164 6765 2f2d 4c69 6e6b 6564 496e  /badge/-LinkedIn
-00002160: 2d62 6c61 636b 2e73 7667 3f73 7479 6c65  -black.svg?style
-00002170: 3d66 6f72 2d74 6865 2d62 6164 6765 266c  =for-the-badge&l
-00002180: 6f67 6f3d 6c69 6e6b 6564 696e 2663 6f6c  ogo=linkedin&col
-00002190: 6f72 423d 3535 350a 0a5b 6c69 6e6b 6564  orB=555..[linked
-000021a0: 696e 2d75 726c 5d3a 2068 7474 7073 3a2f  in-url]: https:/
-000021b0: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
-000021c0: 6d2f 636f 6d70 616e 792f 6174 6765 6e6f  m/company/atgeno
-000021d0: 6d69 780a 0a5b 7072 6f64 7563 742d 7363  mix..[product-sc
-000021e0: 7265 656e 7368 6f74 5d3a 2068 7474 7073  reenshot]: https
-000021f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
-00002200: 6f6d 6547 4150 2f73 6571 736c 6162 2d63  omeGAP/seqslab-c
-00002210: 6c69 2f62 6c6f 622f 6d61 696e 2f41 7467  li/blob/main/Atg
-00002220: 656e 6f6d 6978 2532 3053 6571 734c 6162  enomix%20SeqsLab
-00002230: 2532 3056 332e 706e 670a                 %20V3.png.
+00000000: 3c21 2d2d 2050 524f 4a45 4354 2053 4849  <!-- PROJECT SHI
+00000010: 454c 4453 202d 2d3e 0a3c 212d 2d0a 2a2a  ELDS -->.<!--.**
+00000020: 2a20 4927 6d20 7573 696e 6720 6d61 726b  * I'm using mark
+00000030: 646f 776e 2022 7265 6665 7265 6e63 6520  down "reference 
+00000040: 7374 796c 6522 206c 696e 6b73 2066 6f72  style" links for
+00000050: 2072 6561 6461 6269 6c69 7479 2e0a 2a2a   readability..**
+00000060: 2a20 5265 6665 7265 6e63 6520 6c69 6e6b  * Reference link
+00000070: 7320 6172 6520 656e 636c 6f73 6564 2069  s are enclosed i
+00000080: 6e20 6272 6163 6b65 7473 205b 205d 2069  n brackets [ ] i
+00000090: 6e73 7465 6164 206f 6620 7061 7265 6e74  nstead of parent
+000000a0: 6865 7365 7320 2820 292e 0a2a 2a2a 2053  heses ( )..*** S
+000000b0: 6565 2074 6865 2062 6f74 746f 6d20 6f66  ee the bottom of
+000000c0: 2074 6869 7320 646f 6375 6d65 6e74 2066   this document f
+000000d0: 6f72 2074 6865 2064 6563 6c61 7261 7469  or the declarati
+000000e0: 6f6e 206f 6620 7468 6520 7265 6665 7265  on of the refere
+000000f0: 6e63 6520 7661 7269 6162 6c65 730a 2a2a  nce variables.**
+00000100: 2a20 666f 7220 636f 6e74 7269 6275 746f  * for contributo
+00000110: 7273 2d75 726c 2c20 666f 726b 732d 7572  rs-url, forks-ur
+00000120: 6c2c 2065 7463 2e20 5468 6973 2069 7320  l, etc. This is 
+00000130: 616e 206f 7074 696f 6e61 6c2c 2063 6f6e  an optional, con
+00000140: 6369 7365 2073 796e 7461 7820 796f 7520  cise syntax you 
+00000150: 6d61 7920 7573 652e 0a2a 2a2a 2068 7474  may use..*** htt
+00000160: 7073 3a2f 2f77 7777 2e6d 6172 6b64 6f77  ps://www.markdow
+00000170: 6e67 7569 6465 2e6f 7267 2f62 6173 6963  nguide.org/basic
+00000180: 2d73 796e 7461 782f 2372 6566 6572 656e  -syntax/#referen
+00000190: 6365 2d73 7479 6c65 2d6c 696e 6b73 0a2d  ce-style-links.-
+000001a0: 2d3e 0a5b 436f 6e74 7269 6275 746f 7273  ->.[Contributors
+000001b0: 5d5b 636f 6e74 7269 6275 746f 7273 2d75  ][contributors-u
+000001c0: 726c 5d0a 5b53 7461 7267 617a 6572 735d  rl].[Stargazers]
+000001d0: 5b73 7461 7273 2d75 726c 5d0a 5b49 7373  [stars-url].[Iss
+000001e0: 7565 735d 5b69 7373 7565 732d 7572 6c5d  ues][issues-url]
+000001f0: 0a5b 4c69 6365 6e73 655d 5b6c 6963 656e  .[License][licen
+00000200: 7365 2d75 726c 5d0a 5b21 5b4c 696e 6b65  se-url].[![Linke
+00000210: 6449 6e5d 5b6c 696e 6b65 6469 6e2d 7368  dIn][linkedin-sh
+00000220: 6965 6c64 5d5d 5b6c 696e 6b65 6469 6e2d  ield]][linkedin-
+00000230: 7572 6c5d 0a0a 3c21 2d2d 2050 524f 4a45  url]..<!-- PROJE
+00000240: 4354 204c 4f47 4f20 2d2d 3e0a 3c62 7220  CT LOGO -->.<br 
+00000250: 2f3e 0a3c 7020 616c 6967 6e3d 2263 656e  />.<p align="cen
+00000260: 7465 7222 3e0a 2020 3c61 2068 7265 663d  ter">.  <a href=
+00000270: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000280: 636f 6d2f 416e 6f6d 6547 4150 2f73 6571  com/AnomeGAP/seq
+00000290: 736c 6162 2d63 6c69 223e 0a20 2020 203c  slab-cli">.    <
+000002a0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000002b0: 2f73 7461 7469 632e 7769 7873 7461 7469  /static.wixstati
+000002c0: 632e 636f 6d2f 6d65 6469 612f 6637 6136  c.com/media/f7a6
+000002d0: 6135 5f31 6164 3730 6564 3035 6166 3034  a5_1ad70ed05af04
+000002e0: 6437 6562 3435 6565 3565 3264 6633 3437  d7eb45ee5e2df347
+000002f0: 6133 327e 6d76 325f 645f 3432 3636 5f34  a32~mv2_d_4266_4
+00000300: 3434 395f 735f 345f 322e 6769 6622 2061  449_s_4_2.gif" a
+00000310: 6c74 3d22 4c6f 676f 2220 7769 6474 683d  lt="Logo" width=
+00000320: 2238 3022 2068 6569 6768 743d 2238 3022  "80" height="80"
+00000330: 3e0a 2020 3c2f 613e 0a0a 3c68 3220 616c  >.  </a>..<h2 al
+00000340: 6967 6e3d 2263 656e 7465 7222 3e41 7467  ign="center">Atg
+00000350: 656e 6f6d 6978 2053 6571 734c 6162 2056  enomix SeqsLab V
+00000360: 3320 434c 493c 2f68 323e 0a3c 2f70 3e0a  3 CLI</h2>.</p>.
+00000370: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000380: 223e 0a20 2043 6f6d 6d61 6e64 2d6c 696e  ">.  Command-lin
+00000390: 6520 696e 7465 7266 6163 6520 6f66 2041  e interface of A
+000003a0: 7467 656e 6f6d 6978 2053 6571 734c 6162  tgenomix SeqsLab
+000003b0: 2c20 6120 636c 6f75 642d 6e61 7469 7665  , a cloud-native
+000003c0: 2062 696f 6d65 6469 6361 6c20 696e 666f   biomedical info
+000003d0: 726d 6174 6963 7320 2842 696f 4d65 6420  rmatics (BioMed 
+000003e0: 4954 2920 706c 6174 666f 726d 0a20 203c  IT) platform.  <
+000003f0: 6272 202f 3e0a 2020 3c61 2068 7265 663d  br />.  <a href=
+00000400: 2268 7474 7073 3a2f 2f64 6f63 732e 6174  "https://docs.at
+00000410: 6765 6e6f 6d69 782e 636f 6d22 3e3c 7374  genomix.com"><st
+00000420: 726f 6e67 3e45 7870 6c6f 7265 2074 6865  rong>Explore the
+00000430: 2064 6f63 7320 c2bb 3c2f 7374 726f 6e67   docs ..</strong
+00000440: 3e3c 2f61 3e0a 2020 3c62 7220 2f3e 0a20  ></a>.  <br />. 
+00000450: 203c 6272 202f 3e0a 2020 3c61 2068 7265   <br />.  <a hre
+00000460: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000470: 622e 636f 6d2f 416e 6f6d 6547 4150 2f73  b.com/AnomeGAP/s
+00000480: 6571 736c 6162 2d63 6c69 2f69 7373 7565  eqslab-cli/issue
+00000490: 7322 3e52 6570 6f72 7420 6973 7375 653c  s">Report issue<
+000004a0: 2f61 3e0a 2020 c2b7 0a20 203c 6120 6872  /a>.  ...  <a hr
+000004b0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000004c0: 7562 2e63 6f6d 2f41 6e6f 6d65 4741 502f  ub.com/AnomeGAP/
+000004d0: 7365 7173 6c61 622d 636c 692f 6973 7375  seqslab-cli/issu
+000004e0: 6573 223e 5265 7175 6573 7420 6665 6174  es">Request feat
+000004f0: 7572 653c 2f61 3e0a 3c2f 703e 0a0a 3c21  ure</a>.</p>..<!
+00000500: 2d2d 2054 4142 4c45 204f 4620 434f 4e54  -- TABLE OF CONT
+00000510: 454e 5453 202d 2d3e 0a3c 6465 7461 696c  ENTS -->.<detail
+00000520: 7320 6f70 656e 3d22 6f70 656e 223e 0a20  s open="open">. 
+00000530: 203c 7375 6d6d 6172 793e 5461 626c 6520   <summary>Table 
+00000540: 6f66 2043 6f6e 7465 6e74 733c 2f73 756d  of Contents</sum
+00000550: 6d61 7279 3e0a 2020 3c6f 6c3e 0a20 2020  mary>.  <ol>.   
+00000560: 203c 6c69 3e0a 2020 2020 2020 3c61 2068   <li>.      <a h
+00000570: 7265 663d 2223 6f76 6572 7669 6577 223e  ref="#overview">
+00000580: 4f76 6572 7669 6577 3c2f 613e 0a20 2020  Overview</a>.   
+00000590: 2020 203c 756c 3e0a 2020 2020 2020 2020     <ul>.        
+000005a0: 3c6c 693e 3c61 2068 7265 663d 2223 756e  <li><a href="#un
+000005b0: 6465 726c 7969 6e67 2d74 6563 686e 6f6c  derlying-technol
+000005c0: 6f67 7922 3e55 6e64 6572 6c79 696e 6720  ogy">Underlying 
+000005d0: 5465 6368 6e6f 6c6f 6779 3c2f 613e 3c2f  Technology</a></
+000005e0: 6c69 3e0a 2020 2020 2020 3c2f 756c 3e0a  li>.      </ul>.
+000005f0: 2020 2020 3c2f 6c69 3e0a 2020 2020 3c6c      </li>.    <l
+00000600: 693e 0a20 2020 2020 203c 6120 6872 6566  i>.      <a href
+00000610: 3d22 2367 6574 7469 6e67 2d73 7461 7274  ="#getting-start
+00000620: 6564 223e 4765 7474 696e 6720 5374 6172  ed">Getting Star
+00000630: 7465 643c 2f61 3e0a 2020 2020 2020 3c75  ted</a>.      <u
+00000640: 6c3e 0a20 2020 2020 2020 203c 6c69 3e3c  l>.        <li><
+00000650: 6120 6872 6566 3d22 2370 7265 7265 7175  a href="#prerequ
+00000660: 6973 6974 6573 223e 5072 6572 6571 7569  isites">Prerequi
+00000670: 7369 7465 733c 2f61 3e3c 2f6c 693e 0a20  sites</a></li>. 
+00000680: 2020 2020 2020 203c 6c69 3e3c 6120 6872         <li><a hr
+00000690: 6566 3d22 2369 6e74 6572 6163 7469 7665  ef="#interactive
+000006a0: 2d6d 6f64 6522 3e49 6e74 6572 6163 7469  -mode">Interacti
+000006b0: 7665 204d 6f64 653c 2f61 3e3c 2f6c 693e  ve Mode</a></li>
+000006c0: 0a20 2020 2020 2020 203c 6c69 3e3c 6120  .        <li><a 
+000006d0: 6872 6566 3d22 2363 6c69 2d6d 6f64 6522  href="#cli-mode"
+000006e0: 3e43 4c49 204d 6f64 653c 2f61 3e3c 2f6c  >CLI Mode</a></l
+000006f0: 693e 0a20 2020 2020 203c 2f75 6c3e 0a20  i>.      </ul>. 
+00000700: 2020 203c 2f6c 693e 0a20 2020 203c 6c69     </li>.    <li
+00000710: 3e0a 2020 2020 2020 3c61 2068 7265 663d  >.      <a href=
+00000720: 2223 6465 7665 6c6f 706d 656e 7422 3e44  "#development">D
+00000730: 6576 656c 6f70 6d65 6e74 3c2f 613e 0a20  evelopment</a>. 
+00000740: 2020 2020 203c 756c 3e0a 2020 2020 2020       <ul>.      
+00000750: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
+00000760: 6175 7468 656e 7469 6361 7469 6f6e 2d77  authentication-w
+00000770: 6974 682d 7468 652d 7365 7173 6c61 622d  ith-the-seqslab-
+00000780: 6170 6922 3e41 7574 6865 6e74 6963 6174  api">Authenticat
+00000790: 696f 6e20 7769 7468 2074 6865 2053 6571  ion with the Seq
+000007a0: 734c 6162 2041 5049 3c2f 613e 3c2f 6c69  sLab API</a></li
+000007b0: 3e0a 2020 2020 2020 3c2f 756c 3e0a 2020  >.      </ul>.  
+000007c0: 2020 3c2f 6c69 3e0a 2020 2020 3c6c 693e    </li>.    <li>
+000007d0: 3c61 2068 7265 663d 2223 726f 6164 6d61  <a href="#roadma
+000007e0: 7022 3e52 6f61 646d 6170 3c2f 613e 3c2f  p">Roadmap</a></
+000007f0: 6c69 3e0a 2020 2020 3c6c 693e 3c61 2068  li>.    <li><a h
+00000800: 7265 663d 2223 636f 6e74 7269 6275 7469  ref="#contributi
+00000810: 6e67 223e 436f 6e74 7269 6275 7469 6e67  ng">Contributing
+00000820: 3c2f 613e 3c2f 6c69 3e0a 2020 2020 3c6c  </a></li>.    <l
+00000830: 693e 3c61 2068 7265 663d 2223 6c69 6365  i><a href="#lice
+00000840: 6e73 6522 3e4c 6963 656e 7365 3c2f 613e  nse">License</a>
+00000850: 3c2f 6c69 3e0a 2020 2020 3c6c 693e 3c61  </li>.    <li><a
+00000860: 2068 7265 663d 2223 636f 6e74 6163 7422   href="#contact"
+00000870: 3e43 6f6e 7461 6374 3c2f 613e 3c2f 6c69  >Contact</a></li
+00000880: 3e0a 2020 2020 3c6c 693e 3c61 2068 7265  >.    <li><a hre
+00000890: 663d 2223 6163 6b6e 6f77 6c65 6467 656d  f="#acknowledgem
+000008a0: 656e 7473 223e 4163 6b6e 6f77 6c65 6467  ents">Acknowledg
+000008b0: 656d 656e 7473 3c2f 613e 3c2f 6c69 3e0a  ements</a></li>.
+000008c0: 2020 3c2f 6f6c 3e0a 3c2f 6465 7461 696c    </ol>.</detail
+000008d0: 733e 0a0a 2323 204f 7665 7276 6965 770a  s>..## Overview.
+000008e0: 0a21 5b50 726f 6475 6374 2053 6372 6565  .![Product Scree
+000008f0: 6e20 5368 6f74 5d28 6874 7470 733a 2f2f  n Shot](https://
+00000900: 6769 7468 7562 2e63 6f6d 2f41 6e6f 6d65  github.com/Anome
+00000910: 4741 502f 7365 7173 6c61 622d 636c 692f  GAP/seqslab-cli/
+00000920: 626c 6f62 2f6d 6169 6e2f 4174 6765 6e6f  blob/main/Atgeno
+00000930: 6d69 7825 3230 5365 7173 4c61 6225 3230  mix%20SeqsLab%20
+00000940: 5633 2e70 6e67 290a 0a57 6f72 6b69 6e67  V3.png)..Working
+00000950: 2061 6c6f 6e67 7369 6465 2074 6865 2077   alongside the w
+00000960: 6562 2d62 6173 6564 2053 6571 734c 6162  eb-based SeqsLab
+00000970: 2043 6f6e 736f 6c65 2c20 7468 6520 434c   Console, the CL
+00000980: 4920 656e 6162 6c65 7320 6269 6f69 6e66  I enables bioinf
+00000990: 6f72 6d61 7469 6369 616e 7320 746f 2065  ormaticians to e
+000009a0: 6173 696c 7920 6275 696c 6420 6375 7374  asily build cust
+000009b0: 6f6d 2073 6372 6970 7473 2061 6e64 2061  om scripts and a
+000009c0: 7574 6f6d 6174 6520 776f 726b 666c 6f77  utomate workflow
+000009d0: 7320 6f6e 2053 6571 734c 6162 2e0a 0a43  s on SeqsLab...C
+000009e0: 6f6d 6d6f 6e20 7573 6520 6361 7365 7320  ommon use cases 
+000009f0: 666f 7220 7468 6520 434c 4920 696e 636c  for the CLI incl
+00000a00: 7564 6520 7468 6520 666f 6c6c 6f77 696e  ude the followin
+00000a10: 673a 0a0a 2a20 4175 746f 6d61 7465 2070  g:..* Automate p
+00000a20: 726f 6365 7373 696e 6720 6f66 2073 6571  rocessing of seq
+00000a30: 7565 6e63 696e 6720 6461 7461 2c20 696e  uencing data, in
+00000a40: 636c 7564 696e 6720 7570 6c6f 6164 696e  cluding uploadin
+00000a50: 6720 616e 6420 646f 776e 6c6f 6164 696e  g and downloadin
+00000a60: 6720 6f66 2064 6174 6173 6574 7320 746f  g of datasets to
+00000a70: 2f66 726f 6d20 7468 6520 5365 7173 4c61  /from the SeqsLa
+00000a80: 6220 4461 7461 2048 7562 0a2a 2053 7562  b Data Hub.* Sub
+00000a90: 6d69 7420 776f 726b 666c 6f77 2072 756e  mit workflow run
+00000aa0: 2072 6571 7565 7374 7320 6f6e 2064 656d   requests on dem
+00000ab0: 616e 6420 7669 6120 5365 7173 4c61 6220  and via SeqsLab 
+00000ac0: 576f 726b 666c 6f77 2045 7865 6375 7469  Workflow Executi
+00000ad0: 6f6e 2053 6572 7669 6365 2028 5745 5329  on Service (WES)
+00000ae0: 2041 5049 732c 2061 6e64 2069 6e74 6567   APIs, and integ
+00000af0: 7261 7465 2077 6974 6820 6c6f 6361 6c20  rate with local 
+00000b00: 646f 776e 7374 7265 616d 2061 6e61 6c79  downstream analy
+00000b10: 7369 7320 746f 6f6c 730a 2a20 5669 6577  sis tools.* View
+00000b20: 2072 6563 6f72 6473 206f 6620 706c 6174   records of plat
+00000b30: 666f 726d 2061 6374 6976 6974 6965 7320  form activities 
+00000b40: 666f 7220 6175 6469 7469 6e67 2070 7572  for auditing pur
+00000b50: 706f 7365 730a 0a23 2323 2055 6e64 6572  poses..### Under
+00000b60: 6c79 696e 6720 5465 6368 6e6f 6c6f 6779  lying Technology
+00000b70: 0a0a 5468 6520 5365 7173 4c61 6220 434c  ..The SeqsLab CL
+00000b80: 4920 6973 2062 7569 6c74 2075 7369 6e67  I is built using
+00000b90: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+00000ba0: 0a2a 205b 5365 7173 4c61 6220 4150 4973  .* [SeqsLab APIs
+00000bb0: 5d28 6874 7470 733a 2f2f 6170 692e 7365  ](https://api.se
+00000bc0: 7173 6c61 622e 6e65 742f 290a 2a20 5b50  qslab.net/).* [P
+00000bd0: 7974 686f 6e2d 4e75 6269 615d 2868 7474  ython-Nubia](htt
+00000be0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000bf0: 6661 6365 626f 6f6b 696e 6375 6261 746f  facebookincubato
+00000c00: 722f 7079 7468 6f6e 2d6e 7562 6961 290a  r/python-nubia).
+00000c10: 2a20 5b4d 5341 4c20 5079 7468 6f6e 5d28  * [MSAL Python](
+00000c20: 6874 7470 733a 2f2f 6d73 616c 2d70 7974  https://msal-pyt
+00000c30: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
+00000c40: 696f 2f65 6e2f 6c61 7465 7374 2f29 0a2a  io/en/latest/).*
+00000c50: 205b 417a 7572 6520 5344 4b5d 2868 7474   [Azure SDK](htt
+00000c60: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000c70: 417a 7572 652f 617a 7572 652d 7364 6b29  Azure/azure-sdk)
+00000c80: 0a2a 205b 6169 6f68 7474 705d 2868 7474  .* [aiohttp](htt
+00000c90: 7073 3a2f 2f64 6f63 732e 6169 6f68 7474  ps://docs.aiohtt
+00000ca0: 702e 6f72 672f 656e 2f73 7461 626c 652f  p.org/en/stable/
+00000cb0: 696e 6465 782e 6874 6d6c 290a 0a2a 2a4e  index.html)..**N
+00000cc0: 6f74 652a 2a3a 2054 6865 206d 6563 6861  ote**: The mecha
+00000cd0: 6e69 736d 7320 666f 7220 7365 6375 7265  nisms for secure
+00000ce0: 2069 6e66 6f72 6d61 7469 6f6e 2073 746f   information sto
+00000cf0: 7261 6765 2061 7265 2062 7569 6c74 2061  rage are built a
+00000d00: 726f 756e 6420 6120 5b6b 6579 7269 6e67  round a [keyring
+00000d10: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
+00000d20: 7267 2f70 726f 6a65 6374 2f6b 6579 7269  rg/project/keyri
+00000d30: 6e67 2f29 2073 6572 7669 6365 2e0a 0a23  ng/) service...#
+00000d40: 2320 4765 7474 696e 6720 5374 6172 7465  # Getting Starte
+00000d50: 640a 0a23 2323 2050 7265 7265 7175 6973  d..### Prerequis
+00000d60: 6974 6573 0a0a 2a20 5079 7468 6f6e 2033  ites..* Python 3
+00000d70: 2e38 206f 7220 6c61 7465 720a 0a2a 2041  .8 or later..* A
+00000d80: 2050 7974 686f 6e20 7669 7274 7561 6c20   Python virtual 
+00000d90: 656e 7669 726f 6e6d 656e 740a 0a20 2049  environment..  I
+00000da0: 6e73 7461 6c6c 2074 6865 2053 6571 734c  nstall the SeqsL
+00000db0: 6162 2043 4c49 2e0a 2020 6060 6062 6173  ab CLI..  ```bas
+00000dc0: 680a 2020 7069 7033 2069 6e73 7461 6c6c  h.  pip3 install
+00000dd0: 2073 6571 736c 6162 2d63 6c69 0a20 2060   seqslab-cli.  `
+00000de0: 6060 0a2a 2041 206b 6579 7269 6e67 2062  ``.* A keyring b
+00000df0: 6163 6b65 6e64 0a0a 2020 5468 6520 5365  ackend..  The Se
+00000e00: 7173 4c61 6220 434c 4920 7375 7070 6f72  qsLab CLI suppor
+00000e10: 7473 2074 6865 2066 6f6c 6c6f 7769 6e67  ts the following
+00000e20: 206b 6579 7269 6e67 2062 6163 6b65 6e64   keyring backend
+00000e30: 733a 0a0a 2020 2a20 6d61 634f 5320 5b4b  s:..  * macOS [K
+00000e40: 6579 6368 6169 6e5d 2868 7474 7073 3a2f  eychain](https:/
+00000e50: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00000e60: 672f 7769 6b69 2f4b 6579 6368 6169 6e5f  g/wiki/Keychain_
+00000e70: 2532 3873 6f66 7477 6172 6525 3239 290a  %28software%29).
+00000e80: 2020 2a20 4672 6565 6465 736b 746f 7020    * Freedesktop 
+00000e90: 5b53 6563 7265 7420 5365 7276 6963 655d  [Secret Service]
+00000ea0: 2868 7474 703a 2f2f 7374 616e 6461 7264  (http://standard
+00000eb0: 732e 6672 6565 6465 736b 746f 702e 6f72  s.freedesktop.or
+00000ec0: 672f 7365 6372 6574 2d73 6572 7669 6365  g/secret-service
+00000ed0: 2f29 2028 7265 7175 6972 6573 205b 7365  /) (requires [se
+00000ee0: 6372 6574 7374 6f72 6167 655d 2868 7474  cretstorage](htt
+00000ef0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
+00000f00: 2e6f 7267 2f70 7970 692f 7365 6372 6574  .org/pypi/secret
+00000f10: 7374 6f72 6167 6529 290a 2020 2a20 4b44  storage)).  * KD
+00000f20: 4534 2026 204b 4445 3520 5b4b 5761 6c6c  E4 & KDE5 [KWall
+00000f30: 6574 5d28 6874 7470 733a 2f2f 656e 2e77  et](https://en.w
+00000f40: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00000f50: 692f 4b57 616c 6c65 7429 2028 7265 7175  i/KWallet) (requ
+00000f60: 6972 6573 205b 6462 7573 5d28 6874 7470  ires [dbus](http
+00000f70: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+00000f80: 6f72 672f 7079 7069 2f64 6275 732d 7079  org/pypi/dbus-py
+00000f90: 7468 6f6e 2929 0a20 202a 205b 5769 6e64  thon)).  * [Wind
+00000fa0: 6f77 7320 4372 6564 656e 7469 616c 204c  ows Credential L
+00000fb0: 6f63 6b65 725d 2868 7474 7073 3a2f 2f64  ocker](https://d
+00000fc0: 6f63 732e 6d69 6372 6f73 6f66 742e 636f  ocs.microsoft.co
+00000fd0: 6d2f 656e 2d75 732f 7769 6e64 6f77 732f  m/en-us/windows/
+00000fe0: 7577 702f 7365 6375 7269 7479 2f63 7265  uwp/security/cre
+00000ff0: 6465 6e74 6961 6c2d 6c6f 636b 6572 290a  dential-locker).
+00001000: 0a20 202a 2a4e 6f74 652a 2a3a 2053 6565  .  **Note**: See
+00001010: 2074 6865 205b 5079 7468 6f6e 206b 6579   the [Python key
+00001020: 7269 6e67 206c 6962 7261 7279 2064 6f63  ring library doc
+00001030: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+00001040: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00001050: 6a65 6374 2f6b 6579 7269 6e67 2f29 2066  ject/keyring/) f
+00001060: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00001070: 696f 6e20 6162 6f75 7420 7573 696e 6720  ion about using 
+00001080: 6b65 7972 696e 6720 6f6e 2061 2068 6561  keyring on a hea
+00001090: 646c 6573 7320 4c69 6e75 7820 7379 7374  dless Linux syst
+000010a0: 656d 2069 6e20 6120 446f 636b 6572 2063  em in a Docker c
+000010b0: 6f6e 7461 696e 6572 2e0a 0a2a 2028 6d61  ontainer...* (ma
+000010c0: 634f 5320 6465 7669 6365 7329 2054 6865  cOS devices) The
+000010d0: 2066 6f6c 6c6f 7769 6e67 2070 6163 6b61   following packa
+000010e0: 6765 733a 0a0a 2020 2a20 5b70 6b67 2d63  ges:..  * [pkg-c
+000010f0: 6f6e 6669 675d 2868 7474 7073 3a2f 2f66  onfig](https://f
+00001100: 6f72 6d75 6c61 652e 6272 6577 2e73 682f  ormulae.brew.sh/
+00001110: 666f 726d 756c 612f 706b 672d 636f 6e66  formula/pkg-conf
+00001120: 6967 290a 2020 2a20 5b64 6275 735d 2868  ig).  * [dbus](h
+00001130: 7474 7073 3a2f 2f66 6f72 6d75 6c61 652e  ttps://formulae.
+00001140: 6272 6577 2e73 682f 666f 726d 756c 612f  brew.sh/formula/
+00001150: 6462 7573 290a 2020 2a20 5b67 6c69 625d  dbus).  * [glib]
+00001160: 2868 7474 7073 3a2f 2f66 6f72 6d75 6c61  (https://formula
+00001170: 652e 6272 6577 2e73 682f 666f 726d 756c  e.brew.sh/formul
+00001180: 612f 676c 6962 290a 0a20 2059 6f75 2063  a/glib)..  You c
+00001190: 616e 2069 6e73 7461 6c6c 2074 6865 2072  an install the r
+000011a0: 6571 7569 7265 6420 7061 636b 6167 6573  equired packages
+000011b0: 2075 7369 6e67 2048 6f6d 6562 7265 772e   using Homebrew.
+000011c0: 0a20 2060 6060 6261 7368 0a20 2023 2069  .  ```bash.  # i
+000011d0: 6e73 7461 6c6c 2070 6163 6b61 6765 733a  nstall packages:
+000011e0: 0a20 2062 7265 7720 696e 7374 616c 6c20  .  brew install 
+000011f0: 6462 7573 0a20 2062 7265 7720 696e 7374  dbus.  brew inst
+00001200: 616c 6c20 706b 672d 636f 6e66 6967 200a  all pkg-config .
+00001210: 2020 6272 6577 2069 6e73 7461 6c6c 2067    brew install g
+00001220: 6c69 620a 2020 6060 600a 0a23 2323 2049  lib.  ```..### I
+00001230: 6e74 6572 6163 7469 7665 204d 6f64 650a  nteractive Mode.
+00001240: 0a54 6869 7320 6d6f 6465 2070 726f 7669  .This mode provi
+00001250: 6465 7320 6669 7368 2d73 7479 6c65 2061  des fish-style a
+00001260: 7574 6f2d 636f 6d70 6c65 7469 6f6e 2066  uto-completion f
+00001270: 756e 6374 696f 6e61 6c69 7479 2074 6861  unctionality tha
+00001280: 7420 6973 2075 7365 722d 6672 6965 6e64  t is user-friend
+00001290: 6c79 2c20 6573 7065 6369 616c 6c79 2066  ly, especially f
+000012a0: 6f72 2062 6567 696e 6e65 7273 2e0a 0a2a  or beginners...*
+000012b0: 2052 756e 2069 6e74 6572 6163 7469 7665   Run interactive
+000012c0: 206d 6f64 652e 0a20 2060 6060 6261 7368   mode..  ```bash
+000012d0: 0a20 2076 6972 7475 616c 656e 7620 2e76  .  virtualenv .v
+000012e0: 656e 760a 2020 736f 7572 6365 202e 7665  env.  source .ve
+000012f0: 6e76 2f62 696e 2f61 6374 6976 6174 650a  nv/bin/activate.
+00001300: 2020 6578 706f 7274 2050 5954 484f 4e50    export PYTHONP
+00001310: 4154 483d 2428 7077 6429 0a20 2070 7974  ATH=$(pwd).  pyt
+00001320: 686f 6e33 2073 6571 736c 6162 2f63 6c69  hon3 seqslab/cli
+00001330: 2e70 790a 2020 6060 600a 0a2a 2044 6973  .py.  ```..* Dis
+00001340: 706c 6179 2074 6865 2061 7661 696c 6162  play the availab
+00001350: 6c65 2063 6f6d 6d61 6e64 732e 0a20 2060  le commands..  `
+00001360: 6060 6261 7368 0a20 2073 6571 736c 6162  ``bash.  seqslab
+00001370: 3e20 6865 6c70 0a20 2060 6060 0a0a 2323  > help.  ```..##
+00001380: 2320 434c 4920 4d6f 6465 0a0a 496e 2074  # CLI Mode..In t
+00001390: 6869 7320 6d6f 6465 2c20 7468 6520 5365  his mode, the Se
+000013a0: 7173 4c61 6220 434c 4920 776f 726b 7320  qsLab CLI works 
+000013b0: 6578 6163 746c 7920 6c69 6b65 2061 6e79  exactly like any
+000013c0: 2074 7261 6469 7469 6f6e 616c 204c 696e   traditional Lin
+000013d0: 7578 2d62 6173 6564 2063 6f6d 6d61 6e64  ux-based command
+000013e0: 2d6c 696e 6520 7574 696c 6974 792e 0a0a  -line utility...
+000013f0: 2323 2044 6576 656c 6f70 6d65 6e74 0a0a  ## Development..
+00001400: 436f 6d6d 616e 6473 2061 7265 2064 6566  Commands are def
+00001410: 696e 6564 2061 7320 6e6f 726d 616c 2050  ined as normal P
+00001420: 7974 686f 6e20 6675 6e63 7469 6f6e 7320  ython functions 
+00001430: 7769 7468 2060 4063 6f6d 6d61 6e64 6020  with `@command` 
+00001440: 616e 6420 6040 6172 6775 6d65 6e74 6020  and `@argument` 
+00001450: 6465 636f 7261 746f 7273 2e20 5375 7065  decorators. Supe
+00001460: 7220 636f 6d6d 616e 6473 2061 7265 2069  r commands are i
+00001470: 6d70 6c65 6d65 6e74 6564 2061 7320 5079  mplemented as Py
+00001480: 7468 6f6e 2063 6c61 7373 206f 626a 6563  thon class objec
+00001490: 7473 2c20 616e 6420 696e 7374 616e 6365  ts, and instance
+000014a0: 206d 6574 686f 6473 2064 6563 6f72 6174   methods decorat
+000014b0: 6564 2077 6974 6820 6040 636f 6d6d 616e  ed with `@comman
+000014c0: 6460 2061 7265 2073 7562 2d63 6f6d 6d61  d` are sub-comma
+000014d0: 6e64 732e 2049 6e20 6e6f 6e2d 696e 7465  nds. In non-inte
+000014e0: 7261 6374 6976 6520 6d6f 6465 2c20 796f  ractive mode, yo
+000014f0: 7520 6361 6e20 7365 7420 6040 636f 6d6d  u can set `@comm
+00001500: 616e 6460 2d64 6563 6f72 6174 6564 2066  and`-decorated f
+00001510: 756e 6374 696f 6e73 2074 6f20 7265 7475  unctions to retu
+00001520: 726e 2061 6e20 6069 6e74 602c 2077 6869  rn an `int`, whi
+00001530: 6368 2069 7320 7573 6564 2061 7320 7468  ch is used as th
+00001540: 6520 4c69 6e75 7820 7265 7475 726e 2063  e Linux return c
+00001550: 6f64 652e 0a0a 4279 2064 6566 6175 6c74  ode...By default
+00001560: 2c20 7468 6520 6672 616d 6577 6f72 6b20  , the framework 
+00001570: 6c6f 6164 7320 636f 6d6d 616e 6473 2066  loads commands f
+00001580: 726f 6d20 7468 6520 6070 7974 686f 6e2f  rom the `python/
+00001590: 7365 7173 6c61 622f 636f 6d6d 616e 6473  seqslab/commands
+000015a0: 6020 6d6f 6475 6c65 2064 6972 6563 746f  ` module directo
+000015b0: 7279 2e20 4174 6765 6e6f 6d69 7820 7265  ry. Atgenomix re
+000015c0: 636f 6d6d 656e 6473 2069 6d70 6c65 6d65  commends impleme
+000015d0: 6e74 696e 6720 796f 7572 2070 726f 6772  nting your progr
+000015e0: 616d 2073 7472 7563 7475 7265 2075 6e64  am structure und
+000015f0: 6572 2074 6865 2060 636f 6d6d 616e 6473  er the `commands
+00001600: 6020 6469 7265 6374 6f72 792e 0a0a 6060  ` directory...``
+00001610: 6070 7974 686f 6e0a 0a66 726f 6d20 7465  `python..from te
+00001620: 726d 636f 6c6f 7220 696d 706f 7274 2063  rmcolor import c
+00001630: 7072 696e 740a 6672 6f6d 206e 7562 6961  print.from nubia
+00001640: 2069 6d70 6f72 7420 6172 6775 6d65 6e74   import argument
+00001650: 2c20 636f 6d6d 616e 640a 4063 6f6d 6d61  , command.@comma
+00001660: 6e64 2822 6865 6c6c 6f22 290a 4061 7267  nd("hello").@arg
+00001670: 756d 656e 7428 226e 616d 6522 2c20 7479  ument("name", ty
+00001680: 7065 3d73 7472 2c20 706f 7369 7469 6f6e  pe=str, position
+00001690: 616c 3d54 7275 652c 2064 6573 6372 6970  al=True, descrip
+000016a0: 7469 6f6e 3d22 596f 7572 206e 616d 6522  tion="Your name"
+000016b0: 2920 0a64 6566 2068 656c 6c6f 286e 616d  ) .def hello(nam
+000016c0: 653a 2073 7472 2920 2d3e 2069 6e74 3a0a  e: str) -> int:.
+000016d0: 2020 2020 2222 220a 2020 2020 636f 6d6d      """.    comm
+000016e0: 616e 6420 6865 6c70 2c20 6f72 2074 6865  and help, or the
+000016f0: 2063 6f6d 6d61 6e64 2077 6f6e 2774 2062   command won't b
+00001700: 6520 6c6f 6164 6564 2e0a 2020 2020 2222  e loaded..    ""
+00001710: 220a 2020 2020 6370 7269 6e74 2866 2248  ".    cprint(f"H
+00001720: 656c 6c6f 207b 6e61 6d65 7d21 222c 2022  ello {name}!", "
+00001730: 6772 6565 6e22 290a 2020 2020 7265 7475  green").    retu
+00001740: 726e 2030 0a40 636f 6d6d 616e 640a 636c  rn 0.@command.cl
+00001750: 6173 7320 5375 7065 7243 6f6d 6d61 6e64  ass SuperCommand
+00001760: 3a0a 2020 2222 2273 7570 6572 2d63 6f6d  :.  """super-com
+00001770: 6d61 6e64 2063 6f6d 6d61 6e64 2068 656c  mand command hel
+00001780: 7022 2222 0a0a 2020 6465 6620 5f5f 696e  p"""..  def __in
+00001790: 6974 5f5f 2873 656c 6629 3a0a 2020 2020  it__(self):.    
+000017a0: 7365 6c66 2e5f 7368 6172 6564 203d 2022  self._shared = "
+000017b0: 7368 6172 6564 2076 6172 6961 626c 6520  shared variable 
+000017c0: 7661 6c75 6522 0a0a 2020 4070 726f 7065  value"..  @prope
+000017d0: 7274 790a 2020 6465 6620 7368 6172 6564  rty.  def shared
+000017e0: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
+000017f0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00001800: 7368 6172 6564 0a20 2020 200a 2020 4063  shared.    .  @c
+00001810: 6f6d 6d61 6e64 2861 6c69 6173 6573 3d5b  ommand(aliases=[
+00001820: 2265 6368 6f22 5d29 0a20 2040 6172 6775  "echo"]).  @argu
+00001830: 6d65 6e74 2822 6669 7273 7422 2c0a 2020  ment("first",.  
+00001840: 2020 2020 2020 2020 2020 7479 7065 3d73            type=s
+00001850: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00001860: 706f 7369 7469 6f6e 616c 3d46 616c 7365  positional=False
+00001870: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00001880: 7363 7269 7074 696f 6e3d 2266 6972 7374  scription="first
+00001890: 6e61 6d65 222c 0a20 2020 2020 2020 2020  name",.         
+000018a0: 2020 2061 6c69 6173 6573 3d5b 2266 225d     aliases=["f"]
+000018b0: 290a 2020 4061 7267 756d 656e 7428 226c  ).  @argument("l
+000018c0: 6173 7422 2c0a 2020 2020 2020 2020 2020  ast",.          
+000018d0: 2020 7479 7065 3d73 7472 2c0a 2020 2020    type=str,.    
+000018e0: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
+000018f0: 616c 3d46 616c 7365 2c0a 2020 2020 2020  al=False,.      
+00001900: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00001910: 6e3d 226c 6173 746e 616d 6522 2c0a 2020  n="lastname",.  
+00001920: 2020 2020 2020 2020 2020 616c 6961 7365            aliase
+00001930: 733d 5b22 6c22 5d29 0a20 2064 6566 2063  s=["l"]).  def c
+00001940: 7072 696e 7428 7365 6c66 2c20 6669 7273  print(self, firs
+00001950: 743a 2073 7472 2c20 6c61 7374 3a20 7374  t: str, last: st
+00001960: 7229 202d 3e20 696e 743a 0a20 2020 2020  r) -> int:.     
+00001970: 2022 2222 0a20 2020 2020 2073 7562 2d63   """.      sub-c
+00001980: 6f6d 6d61 6e64 2068 656c 7020 6d65 7373  ommand help mess
+00001990: 6167 652e 0a20 2020 2020 2022 2222 0a20  age..      """. 
+000019a0: 2020 2020 2063 7072 696e 7428 6622 7b66       cprint(f"{f
+000019b0: 6972 7374 7d20 7b6c 6173 747d 222c 2022  irst} {last}", "
+000019c0: 7265 6422 290a 2020 2020 2020 7265 7475  red").      retu
+000019d0: 726e 2030 0a60 6060 0a0a 2323 2320 4175  rn 0.```..### Au
+000019e0: 7468 656e 7469 6361 7469 6f6e 2077 6974  thentication wit
+000019f0: 6820 7468 6520 5365 7173 4c61 6220 4150  h the SeqsLab AP
+00001a00: 490a 0a52 6567 6172 646c 6573 7320 6f66  I..Regardless of
+00001a10: 2074 6865 206d 6f64 6520 2869 6e74 6572   the mode (inter
+00001a20: 6163 7469 7665 206f 7220 6e6f 6e2d 696e  active or non-in
+00001a30: 7465 7261 6374 6976 6529 2074 6861 7420  teractive) that 
+00001a40: 796f 7520 696e 7465 6e64 2074 6f20 7573  you intend to us
+00001a50: 652c 2079 6f75 206d 7573 7420 7369 676e  e, you must sign
+00001a60: 2069 6e20 746f 2061 7574 6865 6e74 6963   in to authentic
+00001a70: 6174 6520 7468 6520 7365 7373 696f 6e2e  ate the session.
+00001a80: 2054 6865 2053 6571 734c 6162 2043 4c49   The SeqsLab CLI
+00001a90: 2066 6f6c 6c6f 7773 2074 6865 204f 4175   follows the OAu
+00001aa0: 7468 2032 2e30 2044 6576 6963 6520 4175  th 2.0 Device Au
+00001ab0: 7468 6f72 697a 6174 696f 6e20 4772 616e  thorization Gran
+00001ac0: 7420 2865 7874 6572 6e61 6c20 5552 4c29  t (external URL)
+00001ad0: 2070 726f 6365 7373 2e0a 0a2a 2053 7065   process...* Spe
+00001ae0: 6369 6679 2074 6865 2070 6c61 7466 6f72  cify the platfor
+00001af0: 6d20 6261 636b 656e 6420 746f 2062 6520  m backend to be 
+00001b00: 7573 6564 2077 6865 6e20 6c61 756e 6368  used when launch
+00001b10: 696e 6720 7468 6520 5365 7173 4c61 6220  ing the SeqsLab 
+00001b20: 434c 492e 2054 6865 2064 6566 6175 6c74  CLI. The default
+00001b30: 2076 616c 7565 2069 7320 6061 7a75 7265   value is `azure
+00001b40: 602e 0a0a 2020 6060 6062 6173 680a 2020  `...  ```bash.  
+00001b50: 7365 7173 6c61 6220 2d2d 6261 636b 656e  seqslab --backen
+00001b60: 6420 617a 7572 650a 2020 6060 600a 0a2a  d azure.  ```..*
+00001b70: 2053 6967 6e20 696e 2074 6f20 7468 6520   Sign in to the 
+00001b80: 5365 7173 4c61 6220 4150 4920 616e 6420  SeqsLab API and 
+00001b90: 6f62 7461 696e 2041 5049 2074 6f6b 656e  obtain API token
+00001ba0: 7320 7769 7468 2061 2073 696e 676c 6520  s with a single 
+00001bb0: 636f 6d6d 616e 642e 2042 7920 6465 6661  command. By defa
+00001bc0: 756c 742c 2074 6865 2073 6967 6e2d 696e  ult, the sign-in
+00001bd0: 2063 6f6d 6d61 6e64 2075 7365 7320 7468   command uses th
+00001be0: 6520 4465 7669 6365 2043 6f64 6520 466c  e Device Code Fl
+00001bf0: 6f77 2066 6f72 2062 726f 7773 6572 6c65  ow for browserle
+00001c00: 7373 2073 7973 7465 6d73 2e0a 0a20 2060  ss systems...  `
+00001c10: 6060 6261 7368 0a20 2061 7574 6820 7369  ``bash.  auth si
+00001c20: 676e 696e 0a20 2060 6060 0a0a 2020 5365  gnin.  ```..  Se
+00001c30: 7420 7468 6520 6465 7669 6365 2d63 6f64  t the device-cod
+00001c40: 6520 6172 6775 6d65 6e74 2074 6f20 6054  e argument to `T
+00001c50: 7275 6560 2e20 4279 2064 6566 6175 6c74  rue`. By default
+00001c60: 2c20 7468 6520 7369 676e 2d69 6e20 7072  , the sign-in pr
+00001c70: 6f63 6573 7320 7573 6573 2074 6865 2041  ocess uses the A
+00001c80: 7574 686f 7269 7a61 7469 6f6e 2043 6f64  uthorization Cod
+00001c90: 6520 466c 6f77 2e0a 0a20 2060 6060 6261  e Flow...  ```ba
+00001ca0: 7368 0a20 2061 7574 6820 7369 676e 696e  sh.  auth signin
+00001cb0: 2064 6576 6963 652d 636f 6465 3d54 7275   device-code=Tru
+00001cc0: 650a 2020 6060 600a 0a2a 204f 6274 6169  e.  ```..* Obtai
+00001cd0: 6e20 616e 2041 5049 2061 6363 6573 7320  n an API access 
+00001ce0: 746f 6b65 6e20 666f 7220 696e 7465 7261  token for intera
+00001cf0: 6374 696e 6720 7769 7468 2053 6571 734c  cting with SeqsL
+00001d00: 6162 2041 5049 2061 7070 732e 0a0a 2020  ab API apps...  
+00001d10: 6060 6070 7974 686f 6e0a 2020 6672 6f6d  ```python.  from
+00001d20: 2073 6571 736c 6162 2e61 7574 682e 636f   seqslab.auth.co
+00001d30: 6d6d 616e 6473 2069 6d70 6f72 7420 4175  mmands import Au
+00001d40: 7468 0a20 200a 2020 746f 6b65 6e20 3d20  th.  .  token = 
+00001d50: 4175 7468 2e67 6574 5f74 6f6b 656e 2829  Auth.get_token()
+00001d60: 0a20 2061 6363 6573 7320 3d20 746f 6b65  .  access = toke
+00001d70: 6e2e 6765 7428 2274 6f6b 656e 7322 292e  n.get("tokens").
+00001d80: 6765 7428 2261 6363 6573 7322 290a 2020  get("access").  
+00001d90: 2320 7573 6520 746f 6b65 6e20 696e 2079  # use token in y
+00001da0: 6f75 7220 7265 7175 6573 7420 6865 6164  our request head
+00001db0: 6572 2c20 6578 3a20 4175 7468 6f72 697a  er, ex: Authoriz
+00001dc0: 6174 696f 6e3a 2042 6561 7265 7220 7b61  ation: Bearer {a
+00001dd0: 6363 6573 737d 0a20 2061 7474 7273 203d  ccess}.  attrs =
+00001de0: 2074 6f6b 656e 2e67 6574 2822 6174 7472   token.get("attr
+00001df0: 7322 290a 2020 2320 6174 7472 7320 6973  s").  # attrs is
+00001e00: 2061 2064 6963 7469 6f6e 6172 7920 636f   a dictionary co
+00001e10: 6e74 6169 6e69 6e67 2074 6865 2069 6e66  ntaining the inf
+00001e20: 6f72 6d61 7469 6f6e 2061 626f 7574 2074  ormation about t
+00001e30: 6865 2073 6967 6e69 6e67 2d69 6e20 7573  he signing-in us
+00001e40: 6572 2e0a 2020 6060 600a 0a20 2060 4175  er..  ```..  `Au
+00001e50: 7468 2e67 6574 5f74 6f6b 656e 2829 6020  th.get_token()` 
+00001e60: 6175 746f 6d61 7469 6361 6c6c 7920 7265  automatically re
+00001e70: 6672 6573 6865 7320 7468 6520 6163 6365  freshes the acce
+00001e80: 7373 2074 6f6b 656e 2075 706f 6e20 6578  ss token upon ex
+00001e90: 7069 7261 7469 6f6e 2e20 5768 656e 2075  piration. When u
+00001ea0: 7365 7273 2061 7474 656d 7074 2074 6f20  sers attempt to 
+00001eb0: 7369 676e 2069 6e20 746f 2074 6865 2053  sign in to the S
+00001ec0: 6571 734c 6162 2041 5049 2062 6566 6f72  eqsLab API befor
+00001ed0: 6520 6120 6e65 7720 6163 6365 7373 2074  e a new access t
+00001ee0: 6f6b 656e 2069 7320 6765 6e65 7261 7465  oken is generate
+00001ef0: 642c 2074 6865 2066 756e 6374 696f 6e20  d, the function 
+00001f00: 7265 7475 726e 7320 604e 6f6e 6560 2e0a  returns `None`..
+00001f10: 0a20 2041 6363 6573 7320 746f 6b65 6e73  .  Access tokens
+00001f20: 2061 7265 2070 6572 7369 7374 656e 746c   are persistentl
+00001f30: 7920 6361 6368 6564 2069 6e20 7468 6520  y cached in the 
+00001f40: 7379 7374 656d 2d73 7570 706f 7274 6564  system-supported
+00001f50: 2073 6563 7265 7420 7365 7276 6963 652c   secret service,
+00001f60: 2073 7563 6820 6173 2046 7265 6564 6573   such as Freedes
+00001f70: 6b74 6f70 2053 6563 7265 7420 5365 7276  ktop Secret Serv
+00001f80: 6963 6520 616e 6420 6d61 634f 5320 4b65  ice and macOS Ke
+00001f90: 7963 6861 696e 2e20 4173 2061 2072 6573  ychain. As a res
+00001fa0: 756c 742c 2076 616c 6964 2061 6363 6573  ult, valid acces
+00001fb0: 7320 746f 6b65 6e73 2063 616e 2062 6520  s tokens can be 
+00001fc0: 7573 6564 2061 6372 6f73 7320 6d75 6c74  used across mult
+00001fd0: 6970 6c65 2053 6571 734c 6162 2043 4c49  iple SeqsLab CLI
+00001fe0: 2073 6573 7369 6f6e 732e 0a0a 2323 2052   sessions...## R
+00001ff0: 6f61 646d 6170 0a0a 5365 6520 7468 6520  oadmap..See the 
+00002000: 5b6c 6973 745d 2868 7474 7073 3a2f 2f67  [list](https://g
+00002010: 6974 6875 622e 636f 6d2f 416e 6f6d 6547  ithub.com/AnomeG
+00002020: 4150 2f73 6571 736c 6162 2d63 6c69 2f69  AP/seqslab-cli/i
+00002030: 7373 7565 7329 206f 6620 7072 6f70 6f73  ssues) of propos
+00002040: 6564 2066 6561 7475 7265 7320 616e 6420  ed features and 
+00002050: 6b6e 6f77 6e20 6973 7375 6573 2e0a 0a23  known issues...#
+00002060: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00002070: 5468 6520 7265 706f 7369 746f 7279 2063  The repository c
+00002080: 7572 7265 6e74 6c79 2064 6f65 7320 6e6f  urrently does no
+00002090: 7420 6163 6365 7074 2063 6f6e 7472 6962  t accept contrib
+000020a0: 7574 696f 6e73 2062 7574 2077 696c 6c20  utions but will 
+000020b0: 6576 656e 7475 616c 6c79 2062 6520 6f70  eventually be op
+000020c0: 656e 6564 2074 6f20 7468 6520 636f 6d6d  ened to the comm
+000020d0: 756e 6974 792e 0a0a 2323 204c 6963 656e  unity...## Licen
+000020e0: 7365 0a0a 5365 6520 604c 6963 656e 7365  se..See `License
+000020f0: 602e 0a0a 2323 2043 6f6e 7461 6374 200a  `...## Contact .
+00002100: 0a4d 6169 6e20 636f 6e74 6163 743a 205b  .Main contact: [
+00002110: 416c 6c65 6e20 4368 616e 675d 2868 7474  Allen Chang](htt
+00002120: 7073 3a2f 2f77 7777 2e6c 696e 6b65 6469  ps://www.linkedi
+00002130: 6e2e 636f 6d2f 696e 2f61 6c6c 656e 2d63  n.com/in/allen-c
+00002140: 6861 6e67 2f29 200a 0a45 6d61 696c 3a20  hang/) ..Email: 
+00002150: 616c 6c65 6e2e 6368 616e 6740 6174 6765  allen.chang@atge
+00002160: 6e6f 6d69 782e 636f 6d0a 0a50 726f 6a65  nomix.com..Proje
+00002170: 6374 2072 6570 6f73 6974 6f72 793a 205b  ct repository: [
+00002180: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002190: 6f6d 2f61 7467 656e 6f6d 6978 5d28 6874  om/atgenomix](ht
+000021a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000021b0: 2f61 7467 656e 6f6d 6978 290a 0a23 2320  /atgenomix)..## 
+000021c0: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
+000021d0: 0a0a 2a20 5b46 6163 6562 6f6f 6b20 496e  ..* [Facebook In
+000021e0: 6375 6261 746f 725d 2868 7474 7073 3a2f  cubator](https:/
+000021f0: 2f67 6974 6875 622e 636f 6d2f 6661 6365  /github.com/face
+00002200: 626f 6f6b 696e 6375 6261 746f 7229 0a2a  bookincubator).*
+00002210: 205b 4d69 6372 6f73 6f66 7420 6964 656e   [Microsoft iden
+00002220: 7469 7479 2070 6c61 7466 6f72 6d5d 2868  tity platform](h
+00002230: 7474 7073 3a2f 2f64 6f63 732e 6d69 6372  ttps://docs.micr
+00002240: 6f73 6f66 742e 636f 6d2f 656e 2d75 732f  osoft.com/en-us/
+00002250: 617a 7572 652f 6163 7469 7665 2d64 6972  azure/active-dir
+00002260: 6563 746f 7279 2f64 6576 656c 6f70 2f61  ectory/develop/a
+00002270: 6374 6976 652d 6469 7265 6374 6f72 792d  ctive-directory-
+00002280: 7632 2d70 726f 746f 636f 6c73 290a 2a20  v2-protocols).* 
+00002290: 5b47 4134 4748 5d28 6874 7470 733a 2f2f  [GA4GH](https://
+000022a0: 7777 772e 6761 3467 682e 6f72 672f 290a  www.ga4gh.org/).
+000022b0: 2a20 5b42 6573 742d 5245 4144 4d45 2d54  * [Best-README-T
+000022c0: 656d 706c 6174 655d 2868 7474 7073 3a2f  emplate](https:/
+000022d0: 2f67 6974 6875 622e 636f 6d2f 6f74 686e  /github.com/othn
+000022e0: 6569 6c64 7265 772f 4265 7374 2d52 4541  eildrew/Best-REA
+000022f0: 444d 452d 5465 6d70 6c61 7465 290a 0a3c  DME-Template)..<
+00002300: 212d 2d20 4d41 524b 444f 574e 204c 494e  !-- MARKDOWN LIN
+00002310: 4b53 2026 2049 4d41 4745 5320 2d2d 3e0a  KS & IMAGES -->.
+00002320: 3c21 2d2d 2068 7474 7073 3a2f 2f77 7777  <!-- https://www
+00002330: 2e6d 6172 6b64 6f77 6e67 7569 6465 2e6f  .markdownguide.o
+00002340: 7267 2f62 6173 6963 2d73 796e 7461 782f  rg/basic-syntax/
+00002350: 2372 6566 6572 656e 6365 2d73 7479 6c65  #reference-style
+00002360: 2d6c 696e 6b73 202d 2d3e 0a0a 5b63 6f6e  -links -->..[con
+00002370: 7472 6962 7574 6f72 732d 7572 6c5d 3a20  tributors-url]: 
+00002380: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002390: 6f6d 2f41 6e6f 6d65 4741 502f 7365 7173  om/AnomeGAP/seqs
+000023a0: 6c61 622d 636c 692f 6772 6170 6873 2f63  lab-cli/graphs/c
+000023b0: 6f6e 7472 6962 7574 6f72 730a 0a5b 7374  ontributors..[st
+000023c0: 6172 732d 7572 6c5d 3a20 6874 7470 733a  ars-url]: https:
+000023d0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6e6f  //github.com/Ano
+000023e0: 6d65 4741 502f 7365 7173 6c61 622d 636c  meGAP/seqslab-cl
+000023f0: 692f 7374 6172 6761 7a65 7273 0a0a 5b69  i/stargazers..[i
+00002400: 7373 7565 732d 7572 6c5d 3a20 6874 7470  ssues-url]: http
+00002410: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00002420: 6e6f 6d65 4741 502f 7365 7173 6c61 622d  nomeGAP/seqslab-
+00002430: 636c 692f 6973 7375 6573 0a0a 5b6c 6963  cli/issues..[lic
+00002440: 656e 7365 2d75 726c 5d3a 2068 7474 7073  ense-url]: https
+00002450: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
+00002460: 6f6d 6547 4150 2f73 6571 736c 6162 2d63  omeGAP/seqslab-c
+00002470: 6c69 2f62 6c6f 622f 6d61 696e 2f4c 4943  li/blob/main/LIC
+00002480: 454e 5345 2e74 7874 0a0a 5b6c 696e 6b65  ENSE.txt..[linke
+00002490: 6469 6e2d 7368 6965 6c64 5d3a 2068 7474  din-shield]: htt
+000024a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000024b0: 2e69 6f2f 6261 6467 652f 2d4c 696e 6b65  .io/badge/-Linke
+000024c0: 6449 6e2d 626c 6163 6b2e 7376 673f 7374  dIn-black.svg?st
+000024d0: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+000024e0: 6526 6c6f 676f 3d6c 696e 6b65 6469 6e26  e&logo=linkedin&
+000024f0: 636f 6c6f 7242 3d35 3535 0a0a 5b6c 696e  colorB=555..[lin
+00002500: 6b65 6469 6e2d 7572 6c5d 3a20 6874 7470  kedin-url]: http
+00002510: 733a 2f2f 7777 772e 6c69 6e6b 6564 696e  s://www.linkedin
+00002520: 2e63 6f6d 2f63 6f6d 7061 6e79 2f61 7467  .com/company/atg
+00002530: 656e 6f6d 6978 0a0a 5b70 726f 6475 6374  enomix..[product
+00002540: 2d73 6372 6565 6e73 686f 745d 3a20 6874  -screenshot]: ht
+00002550: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002560: 2f41 6e6f 6d65 4741 502f 7365 7173 6c61  /AnomeGAP/seqsla
+00002570: 622d 636c 692f 626c 6f62 2f6d 6169 6e2f  b-cli/blob/main/
+00002580: 4174 6765 6e6f 6d69 7825 3230 5365 7173  Atgenomix%20Seqs
+00002590: 4c61 6225 3230 5633 2e70 6e67 0a         Lab%20V3.png.
```

### Comparing `seqslab-cli-3.2.1/python/seqslab/__init__.py` & `seqslab-cli-3.2.1.post0/python/seqslab/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 name = "seqslab"
 
 __all__ = [
 
 ]
 
 
-__version__ = "3.2.1"
+__version__ = "3.2.1.post0"
 
 LOGGING = {
     "DIR_PATH": "/var/log/seqslab"
 }
```

### Comparing `seqslab-cli-3.2.1/python/seqslab/auth/azuread.py` & `seqslab-cli-3.2.1.post0/python/seqslab/auth/azuread.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/auth/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/auth/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/cli.py` & `seqslab-cli-3.2.1.post0/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/context.py` & `seqslab-cli-3.2.1.post0/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/api/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/api/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/api/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/api/template.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/api/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,37 +580,52 @@
             }]
 
         results = backend.create_drsobjects(drs_type='bundle', payloads=payloads)
 
         return results
 
     @command(aliases=["clean"])
+    @argument("ids",
+              type=List[str],
+              positional=False,
+              description="Specify the IDs of the DRS object that you want to delete "
+                          "(optional).")
     @argument("names",
               type=List[str],
               positional=False,
-              description="Generate a list of DRS object names "
+              description="Specify the names of the DRS object that you want to delete "
                           "(optional).")
     @argument("tags",
               type=List[str],
               positional=False,
-              description="Specify the label of the DRS object that you want to delete "
+              description="Specify the labels of the DRS object that you want to delete "
                           "(optional).")
+    @argument("backend_resource",
+              type=str,
+              positional=False,
+              description="Specify whether or not you want to delete the associated computing resources (default = true, optional).",
+              aliases=["purge"],
+              choices=['true', 'false'])
     def delete(
             self,
+            ids: List[str] = [],
             tags: List[str] = [],
             names: List[str] = [],
+            backend_resource: str = "true"
     ) -> int:
         """
-        Delete DRS objects either by name or by tag.
+        Delete DRS objects by DRS id, by DRS name or by DRS tag.
         """
-        if not names and not tags:
-            cprint("Either give names or tags to do DRS query", "red")
+        if not ids and not names and not tags:
+            cprint("Must specify one of the ids, names or tags to identify DRS objects for deletion", "red")
             return errno.ENOENT
 
-        asyncio.run(utils.drs_delete(names, tags))
+        resps = asyncio.run(utils.drs_delete(ids, names, tags, query_opts=f"?backend_content={backend_resource}"))
+        for r in resps:
+            print(r)
 
         return 0
 
     @command
     @argument("names",
               type=List[str],
               positional=False,
```

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/internal/aiocopy.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/aiocopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,20 @@
     def checksum(checksum, type):
         return {
             "checksum": checksum,
             "type": type
         }
 
     @staticmethod
-    def access_method(access_methods_type, access_tier, dst, region, Authorization=None):
+    def access_method(access_methods_type, access_tier, dst, region):
         return {
             "type": access_methods_type,
             "access_url": {
                 "url": dst,
-                "headers": {"Authorization": Authorization}
+                "headers": {}
             },
             "access_tier": access_tier,
             "region": region
         }
 
     def __str__(self):
         return json.dumps(
```

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/internal/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/internal/utils.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/internal/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,17 +66,19 @@
 @async_exception_handler
 async def drs_crud(drs_id: str, method: str, **kwargs) -> dict:
     try:
         token = BaseAuth.get_token().get("tokens").get("access")
     except KeyError:
         raise KeyError(f"No tokens, Please signin first!")
 
+    query_opts = kwargs.get("query_opts", None)
+    url = os.path.join(DRS_OBJECT_URL, drs_id, query_opts) if query_opts else os.path.join(DRS_OBJECT_URL, drs_id)
     async with RetryClient(client_session=ClientSession(raise_for_status=False),
                            retry_options=RandomRetry(attempts=3)).request(
-            method=method, url=os.path.join(DRS_OBJECT_URL, drs_id), proxy=kwargs.get("proxy", None),
+            method=method, url=url, proxy=kwargs.get("proxy", None),
             headers={"Authorization": f"Bearer {token}"},
     ) as response:
         resp = await response.content.read()
     return json.loads(resp) if len(resp) else None
 
 
 @async_exception_handler
@@ -98,18 +100,18 @@
     if not res.get('objects'):
         return False
     else:
         return True
 
 
 @async_exception_handler
-async def drs_delete(names: List[str], labels: List[str], **kwargs):
+async def drs_delete(ids: List[str], names: List[str], labels: List[str], **kwargs):
     search = [drs_search(names=names, labels=[]), drs_search(names=[], labels=labels)]
     resps = await asyncio.gather(*search, return_exceptions=False)
-    drs_ids = [ob.get('id') for res in resps for ob in res.get('objects')]
+    drs_ids = list(set([ob.get('id') for res in resps for ob in res.get('objects')] + ids))
     if not drs_ids:
         cprint(f'No object to be delete')
     else:
         cprint(f'drs to be delete {drs_ids}')
     delete = [drs_crud(drs, "delete", **kwargs) for drs in drs_ids]
     resps_delete = await asyncio.gather(*delete, return_exceptions=False)
     return resps_delete
```

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/storage/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/storage/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/storage/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/utils/biomimetype.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/biomimetype.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/drs/utils/progressbar.py` & `seqslab-cli-3.2.1.post0/python/seqslab/drs/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/exceptions.py` & `seqslab-cli-3.2.1.post0/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/organization/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/organization/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/organization/resource/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/organization/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/plugin.py` & `seqslab-cli-3.2.1.post0/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/role/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/role/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/role/internal/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/role/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/role/resource/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/role/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/role/resource/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/role/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/runsheet/runsheet.py` & `seqslab-cli-3.2.1.post0/python/seqslab/runsheet/runsheet.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/settings.py` & `seqslab-cli-3.2.1.post0/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/statusbar.py` & `seqslab-cli-3.2.1.post0/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/internal/utils.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/register/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/register/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/register/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/register/template.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/register/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/resource/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/resource/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/resource/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/template/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/trs/template/template.py` & `seqslab-cli-3.2.1.post0/python/seqslab/trs/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/usage_logger.py` & `seqslab-cli-3.2.1.post0/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/user/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/user/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/user/internal/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/user/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/user/resource/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/user/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/user/resource/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/user/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/wes/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/wes/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/wes/internal/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/wes/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/wes/resource/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/wes/resource/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/wes/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/wes/template/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/wes/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/wes/template/template.py` & `seqslab-cli-3.2.1.post0/python/seqslab/wes/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/wes/utils.py` & `seqslab-cli-3.2.1.post0/python/seqslab/wes/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/workspace/commands.py` & `seqslab-cli-3.2.1.post0/python/seqslab/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/workspace/internal/common.py` & `seqslab-cli-3.2.1.post0/python/seqslab/workspace/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/workspace/resource/azure.py` & `seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab/workspace/resource/base.py` & `seqslab-cli-3.2.1.post0/python/seqslab/workspace/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.1/python/seqslab_cli.egg-info/SOURCES.txt` & `seqslab-cli-3.2.1.post0/python/seqslab_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 MANIFEST.in
+README.md
+requirements.txt
 setup.cfg
 setup.py
-python/requirements.txt
-python/seqslab/README.md
 python/seqslab/__init__.py
 python/seqslab/cli.py
 python/seqslab/context.py
 python/seqslab/exceptions.py
 python/seqslab/plugin.py
 python/seqslab/session_logger.py
 python/seqslab/settings.py
```

### Comparing `seqslab-cli-3.2.1/setup.py` & `seqslab-cli-3.2.1.post0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,63 +15,64 @@
 }
 
 
 def get_requirement():
     requirements = [    # dependency list
         'pip>=22.0.4'
     ]
-    with open(os.path.join(setup_file_loc, 'python/requirements.txt'), 'r') as f:
+    with open(os.path.join(setup_file_loc, 'requirements.txt'), 'r') as f:
         ori_req = f.read().splitlines()
     requirements.extend(ori_req)
     return requirements
 
+
 def get_version(package):
     """
     Return package version as listed in `__version__` in `init.py`.
     """
     init_py = open(os.path.join(setup_file_loc, package, '__init__.py')).read()
     return re.search("^__version__ = ['\"]([^'\"]+)['\"]", init_py, re.MULTILINE).group(1)
 
 
 def readme():
-    path = os.path.join(setup_file_loc, 'python/seqslab', 'README.md')
+    path = os.path.join(setup_file_loc, 'README.md')
     with open(path, "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name='seqslab-cli',
     version=get_version('python/seqslab'),
-    author="Jia-You Lin",
-    author_email='jiayou.lin@atgenomix.com',
-
+    author="Allen Chang",
+    author_email="allen.chang@atgenomix.com",
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         # https://pypi.org/pypi?%3Aaction=list_classifiers
     ],
-    description="Atgenomix SeqsLab CLI for Python",
+    description="Atgenomix SeqsLab Command Line Tool",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/AnomeGAP/seqslab-cli",
     license="MIT license",
-
     packages=find_packages(where='python'),
     package_dir={'': 'python'},
 
     include_package_data=True,
     install_requires=get_requirement(),
     extras_require=extras_require,
     python_requires='>=3.8',
     zip_safe=True,
-
+    data_files=[
+        ('', ['requirements.txt', ])
+    ],
     entry_points={
         'console_scripts': [
             'seqslab = seqslab.cli:main',
             # setting console scripts, you can call seqslab to run cmd
         ],
     }
```

