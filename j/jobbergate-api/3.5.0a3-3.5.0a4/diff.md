# Comparing `tmp/jobbergate_api-3.5.0a3.tar.gz` & `tmp/jobbergate_api-3.5.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-3.5.0a3.tar", max compression
+gzip compressed data, was "jobbergate_api-3.5.0a4.tar", max compression
```

## Comparing `jobbergate_api-3.5.0a3.tar` & `jobbergate_api-3.5.0a4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1082 2023-05-09 14:04:29.803973 jobbergate_api-3.5.0a3/LICENSE
--rw-r--r--   0        0        0      738 2023-05-09 14:04:29.803973 jobbergate_api-3.5.0a3/README.rst
--rw-r--r--   0        0        0      169 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       41 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/__init__.py
--rw-r--r--   0        0        0     5655 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/application_files.py
--rw-r--r--   0        0        0      234 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/constants.py
--rw-r--r--   0        0        0     9408 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/file_validation.py
--rw-r--r--   0        0        0     1474 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/models.py
--rw-r--r--   0        0        0    14123 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/routers.py
--rw-r--r--   0        0        0     7421 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/schemas.py
--rw-r--r--   0        0        0       40 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0    12157 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/job_script_files.py
--rw-r--r--   0        0        0     1287 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    15623 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     4088 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0       44 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0      529 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     1909 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    12331 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/properties_parser.py
--rw-r--r--   0        0        0    18431 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0    14904 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0      554 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     3621 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/config.py
--rw-r--r--   0        0        0     2466 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     3268 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/main.py
--rw-r--r--   0        0        0     3433 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0       96 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/metadata.py
--rw-r--r--   0        0        0     3470 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/pagination.py
--rw-r--r--   0        0        0     2284 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/s3_manager.py
--rw-r--r--   0        0        0     2166 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/security.py
--rw-r--r--   0        0        0     5580 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/storage.py
--rw-r--r--   0        0        0       40 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/__init__.py
--rw-r--r--   0        0        0       44 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/__init__.py
--rw-r--r--   0        0        0    10634 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_application_files.py
--rw-r--r--   0        0        0     1967 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_file_validation.py
--rw-r--r--   0        0        0    44032 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_routers.py
--rw-r--r--   0        0        0     5180 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_schemas.py
--rw-r--r--   0        0        0     2756 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/conftest.py
--rw-r--r--   0        0        0       42 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     1376 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/conftest.py
--rw-r--r--   0        0        0    11518 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
--rw-r--r--   0        0        0    52389 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_routers.py
--rw-r--r--   0        0        0       46 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0    23970 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
--rw-r--r--   0        0        0    78149 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_routers.py
--rw-r--r--   0        0        0      511 2023-05-09 14:04:29.807973 jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/test_main.py
--rw-r--r--   0        0        0     8900 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/conftest.py
--rw-r--r--   0        0        0     4503 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
--rw-r--r--   0        0        0     3215 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_config.py
--rw-r--r--   0        0        0     4974 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_email_notification.py
--rw-r--r--   0        0        0     3177 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_meta_mapper.py
--rw-r--r--   0        0        0     3959 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_pagination.py
--rw-r--r--   0        0        0     1146 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_s3_manager.py
--rw-r--r--   0        0        0     2718 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_security.py
--rw-r--r--   0        0        0     4512 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_storage.py
--rw-r--r--   0        0        0     2777 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/tests/test_version.py
--rw-r--r--   0        0        0     1102 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/jobbergate_api/version.py
--rw-r--r--   0        0        0     2904 2023-05-09 14:04:29.811973 jobbergate_api-3.5.0a3/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-12 18:40:59.727394 jobbergate_api-3.5.0a4/LICENSE
+-rw-r--r--   0        0        0      738 2023-06-12 18:40:59.727394 jobbergate_api-3.5.0a4/README.rst
+-rw-r--r--   0        0        0      169 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       41 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/__init__.py
+-rw-r--r--   0        0        0     5655 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/application_files.py
+-rw-r--r--   0        0        0      234 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/constants.py
+-rw-r--r--   0        0        0     9408 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/file_validation.py
+-rw-r--r--   0        0        0     1474 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/models.py
+-rw-r--r--   0        0        0    14123 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/routers.py
+-rw-r--r--   0        0        0     7421 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/schemas.py
+-rw-r--r--   0        0        0       40 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    12157 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/job_script_files.py
+-rw-r--r--   0        0        0     1287 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    15623 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     4088 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0       44 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0      529 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     1909 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    12331 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/properties_parser.py
+-rw-r--r--   0        0        0    18431 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0    15946 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0      554 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     3621 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2466 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     3268 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3433 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0       96 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/metadata.py
+-rw-r--r--   0        0        0     3470 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/pagination.py
+-rw-r--r--   0        0        0     2284 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/s3_manager.py
+-rw-r--r--   0        0        0     2166 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/security.py
+-rw-r--r--   0        0        0     5580 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/storage.py
+-rw-r--r--   0        0        0       40 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/__init__.py
+-rw-r--r--   0        0        0    10634 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_application_files.py
+-rw-r--r--   0        0        0     1967 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_file_validation.py
+-rw-r--r--   0        0        0    44032 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_routers.py
+-rw-r--r--   0        0        0     5180 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_schemas.py
+-rw-r--r--   0        0        0     2756 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/conftest.py
+-rw-r--r--   0        0        0       42 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     1376 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/conftest.py
+-rw-r--r--   0        0        0    11518 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
+-rw-r--r--   0        0        0    52389 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_routers.py
+-rw-r--r--   0        0        0       46 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0    24706 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
+-rw-r--r--   0        0        0    78149 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_routers.py
+-rw-r--r--   0        0        0      511 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/test_main.py
+-rw-r--r--   0        0        0     8900 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/conftest.py
+-rw-r--r--   0        0        0     4503 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
+-rw-r--r--   0        0        0     3215 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_config.py
+-rw-r--r--   0        0        0     4974 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_email_notification.py
+-rw-r--r--   0        0        0     3177 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_meta_mapper.py
+-rw-r--r--   0        0        0     3959 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_pagination.py
+-rw-r--r--   0        0        0     1146 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_s3_manager.py
+-rw-r--r--   0        0        0     2718 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_security.py
+-rw-r--r--   0        0        0     4512 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_storage.py
+-rw-r--r--   0        0        0     2777 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_version.py
+-rw-r--r--   0        0        0     1102 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/version.py
+-rw-r--r--   0        0        0     2898 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a4/PKG-INFO
```

### Comparing `jobbergate_api-3.5.0a3/LICENSE` & `jobbergate_api-3.5.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/README.rst` & `jobbergate_api-3.5.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/application_files.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/file_validation.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/models.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/routers.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/applications/schemas.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/job_script_files.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/properties_parser.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 JobSubmission resource schema.
 """
+import re
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, List, Literal, Optional
 
-from pydantic import BaseModel, Extra, Field
+from pydantic import BaseModel, Extra, Field, validator
 
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_submissions.constants import JobSubmissionStatus
 from jobbergate_api.meta_mapper import MetaField, MetaMapper
 
 job_submission_meta_mapper = MetaMapper(
     id=MetaField(
@@ -270,14 +271,34 @@
     time_limit: Optional[str] = Field(description="Step time limit.")
     time_minimum: Optional[int] = Field(description="Minimum run time in minutes.")
     wait_all_nodes: Optional[int] = Field(
         description="Do not begin execution until all nodes are ready for use.", ge=0, le=1
     )
     wckey: Optional[str] = Field(description="Specify wckey to be used with job.")
 
+    @validator("signal", pre=True)
+    def _backward_compatibility_on_signal(cls, value):
+        """
+        Remove the prefix B from signal in order to provide compatibility to legacy jobbergate applications.
+
+        The --signal parameter in Slurm commands allows for the specification of a signal to be sent to a job
+        in case of certain events, in order to trigger a specific behavior. The B syntax in sbatch specifies
+        a signal to be sent only to the job's batch shell, but is not supported by srun or the Slurm rest API,
+        since there is no batch shell to be signalized at runtime.
+
+        Notice the use the R option is possible to allow this job to overlap with a reservation with
+        MaxStartDelay set, so it should be preserved on the original value.
+
+        See test_backward_compatibility_on_signal_parameter for usage examples.
+        """
+        if value:
+            value = re.sub(r"^B:", "", value)
+            value = re.sub(r"^BR:|^RB:", r"R:", value)
+        return value
+
 
 class JobSubmissionCreateRequest(BaseModel):
     """
     Request model for creating JobSubmission instances.
     """
 
     job_submission_name: str
```

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/apps/permissions.py` & `jobbergate_api-3.5.0a4/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/config.py` & `jobbergate_api-3.5.0a4/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/email_notification.py` & `jobbergate_api-3.5.0a4/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/main.py` & `jobbergate_api-3.5.0a4/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/meta_mapper.py` & `jobbergate_api-3.5.0a4/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/pagination.py` & `jobbergate_api-3.5.0a4/jobbergate_api/pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/s3_manager.py` & `jobbergate_api-3.5.0a4/jobbergate_api/s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/security.py` & `jobbergate_api-3.5.0a4/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/storage.py` & `jobbergate_api-3.5.0a4/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_application_files.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_file_validation.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_routers.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/applications/test_schemas.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/conftest.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/conftest.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_scripts/test_routers.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -732,7 +732,29 @@
         jobscript = "#SBATCH --no-requeue\n#SBATCH --requeue"
 
         desired_dict = {"requeue": True}
 
         actual_dict = jobscript_to_dict(jobscript)
 
         assert actual_dict == desired_dict
+
+
+@pytest.mark.parametrize(
+    "input, expected_result",
+    (
+        (None, None),
+        ("USR1@7200", "USR1@7200"),
+        ("B:USR1@7200", "USR1@7200"),
+        ("R:USR1@7200", "R:USR1@7200"),
+        ("RB:USR1@7200", "R:USR1@7200"),
+        ("BR:USR1@7200", "R:USR1@7200"),
+        ("B:BBB", "BBB"),  # a silly case, but let's assert that just the B on the left side is removed
+    ),
+)
+def test_backward_compatibility_on_signal_parameter(input, expected_result):
+    """
+    Test backward compatibility on signal parameter.
+
+    It is expected to remove the 'B' from the prefix while preserving any other, like the 'R'.
+    """
+    actual_result = JobProperties(signal=input).signal
+    assert actual_result == expected_result
```

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/apps/job_submissions/test_routers.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/conftest.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_config.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_email_notification.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_meta_mapper.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_pagination.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_s3_manager.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_security.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_storage.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/tests/test_version.py` & `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/jobbergate_api/version.py` & `jobbergate_api-3.5.0a4/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a3/pyproject.toml` & `jobbergate_api-3.5.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "3.5.0-alpha.3"
+version = "3.5.0a4"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_api-3.5.0a3/PKG-INFO` & `jobbergate_api-3.5.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 3.5.0a3
+Version: 3.5.0a4
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

