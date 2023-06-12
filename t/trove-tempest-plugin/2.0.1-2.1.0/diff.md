# Comparing `tmp/trove_tempest_plugin-2.0.1.tar.gz` & `tmp/trove_tempest_plugin-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove_tempest_plugin-2.0.1.tar", last modified: Thu Mar  9 10:33:46 2023, max compression
+gzip compressed data, was "trove_tempest_plugin-2.1.0.tar", last modified: Mon Jun 12 13:56:26 2023, max compression
```

## Comparing `trove_tempest_plugin-2.0.1.tar` & `trove_tempest_plugin-2.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.625681 trove_tempest_plugin-2.0.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2023-03-09 10:33:46.625681 trove_tempest_plugin-2.0.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.617681 trove_tempest_plugin-2.0.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.617681 trove_tempest_plugin-2.0.1/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2683 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.613681 trove_tempest_plugin-2.0.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.617681 trove_tempest_plugin-2.0.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/releasenotes/notes/drop-py-2-7-c3f42fa06d0485d9.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.617681 trove_tempest_plugin-2.0.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.621681 trove_tempest_plugin-2.0.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.621681 trove_tempest_plugin-2.0.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9275 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2023-03-09 10:33:46.625681 trove_tempest_plugin-2.0.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/tempest_blacklist.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.621681 trove_tempest_plugin-2.0.1/trove_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.621681 trove_tempest_plugin-2.0.1/trove_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4075 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/services/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.621681 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29475 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.625681 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7597 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5289 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10586 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10079 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_replication.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_update_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6361 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_backup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10589 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_instance_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_instance_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_instance_update_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7289 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_replication.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3277 2023-03-09 10:33:24.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 10:33:46.621681 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2023-03-09 10:33:46.000000 trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.401929 trove_tempest_plugin-2.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3638 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2751 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2023-06-12 13:56:26.401929 trove_tempest_plugin-2.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.393929 trove_tempest_plugin-2.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.393929 trove_tempest_plugin-2.1.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2683 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.389929 trove_tempest_plugin-2.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.393929 trove_tempest_plugin-2.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/releasenotes/notes/drop-py-2-7-c3f42fa06d0485d9.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.393929 trove_tempest_plugin-2.1.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.393929 trove_tempest_plugin-2.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.393929 trove_tempest_plugin-2.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9275 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2023-06-12 13:56:26.401929 trove_tempest_plugin-2.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/tempest_blacklist.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.393929 trove_tempest_plugin-2.1.0/trove_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.397929 trove_tempest_plugin-2.1.0/trove_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4075 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/services/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.397929 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29475 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.401929 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7597 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5289 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10586 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10079 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_replication.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_update_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6361 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_backup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10589 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_instance_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_instance_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_instance_update_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7289 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_replication.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3277 2023-06-12 13:55:57.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-12 13:56:26.397929 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2023-06-12 13:56:26.000000 trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/top_level.txt
```

### Comparing `trove_tempest_plugin-2.0.1/.zuul.yaml` & `trove_tempest_plugin-2.1.0/.zuul.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -55,19 +55,26 @@
     timeout: 10800
     description: |
       This job is for testing on py3 which is Ussuri onwards.
     required-projects: &base_required_projects
       - openstack/trove
       - openstack/trove-tempest-plugin
       - openstack/tempest
-    irrelevant-files:
+    irrelevant-files: &base_irrelevant_files
       - ^.*\.rst$
+      - ^api-ref/.*$
       - ^doc/.*$
       - ^etc/.*$
       - ^releasenotes/.*$
+      - ^test-requirements.txt$
+      - ^tox.ini$
+      - ^LICENSE$
+      - ^contrib/
+      - ^zuul\.d/
+      - ^\..+
     vars: &base_vars
       tox_envlist: all
       tempest_concurrency: 1
       devstack_localrc:
         TEMPEST_PLUGINS: /opt/stack/trove-tempest-plugin
         USE_PYTHON3: true
         Q_AGENT: openvswitch
@@ -113,9 +120,10 @@
       tempest_test_blacklist: '{{ ansible_user_dir }}/{{ zuul.projects["opendev.org/openstack/trove-tempest-plugin"].src_dir }}/tempest_blacklist.txt'
 
 - job:
     name: trove-tempest-ipv6-only
     parent: devstack-tempest-ipv6
     description: |
       Trove devstack tempest tests job for IPv6-only deployment
+    irrelevant-files: *base_irrelevant_files
     required-projects: *base_required_projects
     vars: *base_vars
```

### Comparing `trove_tempest_plugin-2.0.1/AUTHORS` & `trove_tempest_plugin-2.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/CONTRIBUTING.rst` & `trove_tempest_plugin-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/ChangeLog` & `trove_tempest_plugin-2.1.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+2.1.0
+-----
+
+* Ignore files for trove-tempest-ipv6 job
+
 2.0.1
 -----
 
 * Fixing tests with tox 4.2.6
 
 2.0.0
 -----
```

### Comparing `trove_tempest_plugin-2.0.1/LICENSE` & `trove_tempest_plugin-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/PKG-INFO` & `trove_tempest_plugin-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: trove_tempest_plugin
-Version: 2.0.1
+Version: 2.1.0
 Summary: Tempest plugin for Trove project
 Home-page: https://docs.openstack.org/trove/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ====================
         Trove Tempest Plugin
```

### Comparing `trove_tempest_plugin-2.0.1/doc/source/conf.py` & `trove_tempest_plugin-2.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/doc/source/index.rst` & `trove_tempest_plugin-2.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/releasenotes/source/conf.py` & `trove_tempest_plugin-2.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/requirements.txt` & `trove_tempest_plugin-2.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/setup.cfg` & `trove_tempest_plugin-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/setup.py` & `trove_tempest_plugin-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/tox.ini` & `trove_tempest_plugin-2.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/config.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/plugin.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/services/client.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/services/client.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/base.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/constants.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/constants.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/exceptions.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/exceptions.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_actions.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_actions.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_backup.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_backup.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_basic.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_basic.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_replication.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_replication.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/base_update_access.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/base_update_access.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_backup.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_backup.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_instance_actions.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_instance_actions.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_instance_basic.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_instance_basic.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_instance_update_access.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_instance_update_access.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/scenario/test_replication.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/scenario/test_replication.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin/tests/utils.py` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin/tests/utils.py`

 * *Files identical despite different names*

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/PKG-INFO` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: trove-tempest-plugin
-Version: 2.0.1
+Version: 2.1.0
 Summary: Tempest plugin for Trove project
 Home-page: https://docs.openstack.org/trove/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ====================
         Trove Tempest Plugin
```

### Comparing `trove_tempest_plugin-2.0.1/trove_tempest_plugin.egg-info/SOURCES.txt` & `trove_tempest_plugin-2.1.0/trove_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

