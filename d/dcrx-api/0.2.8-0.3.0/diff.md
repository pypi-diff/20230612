# Comparing `tmp/dcrx-api-0.2.8.tar.gz` & `tmp/dcrx-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.2.8.tar", last modified: Sun Jun 11 13:58:37 2023, max compression
+gzip compressed data, was "dcrx-api-0.3.0.tar", last modified: Mon Jun 12 07:30:53 2023, max compression
```

## Comparing `dcrx-api-0.2.8.tar` & `dcrx-api-0.3.0.tar`

### file list

```diff
@@ -1,110 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.522446 dcrx-api-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-11 13:58:37.522446 dcrx-api-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.514446 dcrx-api-0.2.8/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.514446 dcrx-api-0.2.8/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.514446 dcrx-api-0.2.8/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.514446 dcrx-api-0.2.8/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/env/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/image_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/remote_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/models/server_memory_limit_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/monitoring/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/base/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.518446 dcrx-api-0.2.8/dcrx_api/services/monitoring/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/cpu/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.522446 dcrx-api-0.2.8/dcrx_api/services/monitoring/memory/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/monitoring/memory/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.522446 dcrx-api-0.2.8/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.522446 dcrx-api-0.2.8/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.522446 dcrx-api-0.2.8/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 13:58:37.514446 dcrx-api-0.2.8/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-11 13:58:37.000000 dcrx-api-0.2.8/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-11 13:58:37.000000 dcrx-api-0.2.8/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 13:58:37.000000 dcrx-api-0.2.8/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-11 13:58:37.000000 dcrx-api-0.2.8/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-11 13:58:37.000000 dcrx-api-0.2.8/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 13:58:37.000000 dcrx-api-0.2.8/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 13:58:37.522446 dcrx-api-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-11 13:58:33.000000 dcrx-api-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/job_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/server_memory_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/registry/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/registry/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/setup.py
```

### Comparing `dcrx-api-0.2.8/LICENSE` & `dcrx-api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/PKG-INFO` & `dcrx-api-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.2.8
+Version: 0.3.0
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,14 +45,16 @@
 
 
 # Getting Started
 
 DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
+DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled.
+
 DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
 
 DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
 
 DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
 
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
@@ -73,19 +75,14 @@
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
 
 DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
-DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Default Docker image registry to push images to.
-
-DOCKER_REGISTRY_USERNAME=test # Default Username to authenticate Docker pushes to the provided registry.
-
-DOCKER_REGISTRY_PASSWORD=test-repo-password # Default Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -109,20 +106,36 @@
 and navigate to `localhost:2277/docs`, where you'll find dcrx-api's OpenAPI documentation.
 
 
 # Authenticating and Building an Image
 
 From here, we'll need to authenticate using the initial user we created above. Open the tab for `/users/login`, and for the `username` and `password` fields enter the username and password of the initial user, then click `Execute`. A `200` status response containg the initial user's username and id should return.
 
+Before creating and pushing any images, we need to create a Registry. Navigate to the `/registry/create` tab. We'll need to provide a `registry_name` (unique shortand reference of our choosing), `registry_uri` (HTTP url to the registry), `registry_user`, and `registry_password:
+
+```json
+{
+  "registry_name": "hello-world",
+  "registry_uri": "https://docker.io/v1/testreg/hello-world",
+  "registry_user": "testuser",
+  "registry_password": "testpassword1*"
+}
+```
+
+Submit the request. DCRX-API will take the information, encrypt the registry password, and store it.
+
 Next navigate to the `/jobs/images/create` tab. As before, we'll need to fill out some data. Go ahead and copy paste the below into the input for the request body:
 
 ```json
 {
-  "name": "hello-world",
+  "name": "testreg/hello-world",
   "tag": "latest",
+  "registry": {
+    "registry_name": "hello-world"
+  },
   "layers": [
     {
       "layer_type": "stage",
       "base": "python",
       "tag": "3.11-slim"
     },
     {
@@ -132,15 +145,15 @@
             "Hello world!"
         ]
     }
   ]
 }
 ```
 
-A dcrx-api image build request requires, at-minimum, a `name`, `tag` and one or more `layer` objects, which will be processed and build in-order of appearance. Note that each layer object almost exactly corresponds to its `dcrx` call. The above corresponds exactly to:
+A dcrx-api image build request requires, at-minimum, a `name`, `tag`, `registry_name`, and one or more `layer` objects, which will be processed and build in-order of appearance. Note that each layer object almost exactly corresponds to its `dcrx` call. The above corresponds exactly to:
 
 ```python
 
 from dcrx import Image
 
 hello_world = Image('hello-world')
 
@@ -149,15 +162,15 @@
     '3.11-slim'
 ).entrypoint([
     'echo',
     'Hello world!'
 ])
 ```
 
-Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in dcrx-api's environmental variables.
+Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in the request.
 
 Note that dcrx-api doesn't wait for the image to be built, instead returning a `JobMetadata` response with a status code of `200`, including the `job_id`. Building images is time-intensive and could potentially bog down a server, so dcrx-api builds and pushes images in the background. We can use the `job_id` of a Job to make further `GET` requests to the `/jobs/images/{job_id}/get` endpoint to monitor and check how our job is progressing. If we need to cancel a job for any reason, we can simple make a `DELETE` request to `/jobs/images/{job_id}/cancel`.
 
 
 # Running the Docker Image
 
 To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
@@ -185,35 +198,7 @@
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
-
-3. Can I push to a registry besides the default? - Yes. New image job requests can be submitted with optional Registry configuration. For example:
-
-```
-{
-  "name": "hello-world",
-  "tag": "latest",
-  "registry": {
-    "registry_url": "https://docker.io/v1/mytest/registry",
-    "registry_user": "DockerUser100",
-    "registry_password": "MyDockerHubToken999*"
-  },
-  "layers": [
-    {
-      "layer_type": "stage",
-      "base": "python",
-      "tag": "3.11-slim"
-    },
-    {
-        "layer_type": "entrypoint",
-        "command": [
-            "echo",
-            "Hello world!"
-        ]
-    }
-  ]
-}
-```
```

### Comparing `dcrx-api-0.2.8/README.md` & `dcrx-api-0.3.0/dcrx_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: dcrx-api
+Version: 0.3.0
+Summary: A RESTful implementation of the DCRX Docker library.
+Home-page: https://github.com/scorbettUM/dcrx-api
+Author: Sean Corbett
+Author-email: sean.corbett@umontana.edu
+Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dcrx-api
 [![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
 [![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
 
 DCRX-API is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! DCRX-API extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
@@ -27,14 +45,16 @@
 
 
 # Getting Started
 
 DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
+DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled.
+
 DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
 
 DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
 
 DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
 
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
@@ -55,19 +75,14 @@
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
 
 DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
-DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Default Docker image registry to push images to.
-
-DOCKER_REGISTRY_USERNAME=test # Default Username to authenticate Docker pushes to the provided registry.
-
-DOCKER_REGISTRY_PASSWORD=test-repo-password # Default Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -91,20 +106,36 @@
 and navigate to `localhost:2277/docs`, where you'll find dcrx-api's OpenAPI documentation.
 
 
 # Authenticating and Building an Image
 
 From here, we'll need to authenticate using the initial user we created above. Open the tab for `/users/login`, and for the `username` and `password` fields enter the username and password of the initial user, then click `Execute`. A `200` status response containg the initial user's username and id should return.
 
+Before creating and pushing any images, we need to create a Registry. Navigate to the `/registry/create` tab. We'll need to provide a `registry_name` (unique shortand reference of our choosing), `registry_uri` (HTTP url to the registry), `registry_user`, and `registry_password:
+
+```json
+{
+  "registry_name": "hello-world",
+  "registry_uri": "https://docker.io/v1/testreg/hello-world",
+  "registry_user": "testuser",
+  "registry_password": "testpassword1*"
+}
+```
+
+Submit the request. DCRX-API will take the information, encrypt the registry password, and store it.
+
 Next navigate to the `/jobs/images/create` tab. As before, we'll need to fill out some data. Go ahead and copy paste the below into the input for the request body:
 
 ```json
 {
-  "name": "hello-world",
+  "name": "testreg/hello-world",
   "tag": "latest",
+  "registry": {
+    "registry_name": "hello-world"
+  },
   "layers": [
     {
       "layer_type": "stage",
       "base": "python",
       "tag": "3.11-slim"
     },
     {
@@ -114,15 +145,15 @@
             "Hello world!"
         ]
     }
   ]
 }
 ```
 
-A dcrx-api image build request requires, at-minimum, a `name`, `tag` and one or more `layer` objects, which will be processed and build in-order of appearance. Note that each layer object almost exactly corresponds to its `dcrx` call. The above corresponds exactly to:
+A dcrx-api image build request requires, at-minimum, a `name`, `tag`, `registry_name`, and one or more `layer` objects, which will be processed and build in-order of appearance. Note that each layer object almost exactly corresponds to its `dcrx` call. The above corresponds exactly to:
 
 ```python
 
 from dcrx import Image
 
 hello_world = Image('hello-world')
 
@@ -131,15 +162,15 @@
     '3.11-slim'
 ).entrypoint([
     'echo',
     'Hello world!'
 ])
 ```
 
-Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in dcrx-api's environmental variables.
+Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in the request.
 
 Note that dcrx-api doesn't wait for the image to be built, instead returning a `JobMetadata` response with a status code of `200`, including the `job_id`. Building images is time-intensive and could potentially bog down a server, so dcrx-api builds and pushes images in the background. We can use the `job_id` of a Job to make further `GET` requests to the `/jobs/images/{job_id}/get` endpoint to monitor and check how our job is progressing. If we need to cancel a job for any reason, we can simple make a `DELETE` request to `/jobs/images/{job_id}/cancel`.
 
 
 # Running the Docker Image
 
 To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
@@ -167,35 +198,7 @@
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
-
-3. Can I push to a registry besides the default? - Yes. New image job requests can be submitted with optional Registry configuration. For example:
-
-```
-{
-  "name": "hello-world",
-  "tag": "latest",
-  "registry": {
-    "registry_url": "https://docker.io/v1/mytest/registry",
-    "registry_user": "DockerUser100",
-    "registry_password": "MyDockerHubToken999*"
-  },
-  "layers": [
-    {
-      "layer_type": "stage",
-      "base": "python",
-      "tag": "3.11-slim"
-    },
-    {
-        "layer_type": "entrypoint",
-        "command": [
-            "echo",
-            "Hello world!"
-        ]
-    }
-  ]
-}
-```
```

### Comparing `dcrx-api-0.2.8/dcrx_api/cli/base.py` & `dcrx-api-0.3.0/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/cli/database.py` & `dcrx-api-0.3.0/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/cli/server.py` & `dcrx-api-0.3.0/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/context/manager.py` & `dcrx-api-0.3.0/dcrx_api/context/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from dcrx_api.services.auth.context import AuthServiceContext
 from dcrx_api.services.jobs.context import JobServiceContext
 from dcrx_api.services.monitoring.context import MonitoringServiceContext
+from dcrx_api.services.registry.context import RegistryConnection
 from dcrx_api.services.users.context import UsersServiceContext
 from typing import Dict, Union, List
 from .types import ContextType
 
 
 class ContextManager:
 
     def __init__(self) -> None:
         self.contexts: Dict[
             ContextType, 
             Union[
                 AuthServiceContext,
                 JobServiceContext, 
                 MonitoringServiceContext,
+                RegistryConnection,
                 UsersServiceContext
             ]
         ] = {}
 
     
     def get(self, context_type: ContextType) -> Union[
         AuthServiceContext,
         JobServiceContext,
         MonitoringServiceContext,
+        RegistryConnection,
         UsersServiceContext,
         None
     ]:
         return self.contexts.get(context_type)
 
     async def initialize(
         self,
         contexts: List[
             Union[
                 AuthServiceContext,
                 JobServiceContext,
                 MonitoringServiceContext,
+                RegistryConnection,
                 UsersServiceContext
             ]
         ]
     ):
         
         for context in contexts:
             await context.initialize()
```

### Comparing `dcrx-api-0.2.8/dcrx_api/database/connection.py` & `dcrx-api-0.3.0/dcrx_api/database/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/env/env.py` & `dcrx-api-0.3.0/dcrx_api/env/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,45 +14,41 @@
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
     DCRX_API_MAX_MEMORY_PERCENT_USAGE: StrictFloat=50
+    DCRX_API_JOB_TIMEOUT: StrictStr='5s'
     DCRX_API_JOB_PRUNE_INTERVAL: StrictStr='1s'
     DCRX_API_JOB_MAX_AGE: StrictStr='1m'
     DCRX_API_JOB_WORKERS: StrictInt=psutil.cpu_count()
     DCRX_API_JOB_POOL_SIZE: StrictInt=10
     DCRX_API_SECRET_KEY: StrictStr
     DCRX_API_AUTH_ALGORITHM: StrictStr='HS256'
     DCRX_API_TOKEN_EXPIRATION: StrictStr='15m'
     DCRX_API_DATABASE_TYPE: Optional[StrictStr]='sqlite'
     DCRX_API_DATABASE_USER: Optional[StrictStr]
     DCRX_API_DATABASE_URI: Optional[StrictStr]
     DCRX_API_DATABASE_PORT: Optional[StrictInt]
     DCRX_API_DATABASE_PASSWORD: Optional[StrictStr]
     DCRX_API_DATABASE_NAME: StrictStr='dcrx'
-    DOCKER_REGISTRY_URI: StrictStr
-    DOCKER_REGISTRY_USERNAME: StrictStr
-    DOCKER_REGISTRY_PASSWORD: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
             'DCRX_API_MAX_MEMORY_PERCENT_USAGE': float,
             'DCRX_API_JOB_PRUNE_INTERVAL': str,
+            'DCRX_API_JOB_TIMEOUT': str,
             'DCRX_API_JOB_MAX_AGE': str,
             'DCRX_API_JOB_WORKERS': int,
             'DCRX_API_JOB_POOL_SIZE': int,
             'DCRX_API_SECRET_KEY': str,
             'DCRX_API_AUTH_ALGORITHM': str,
             'DCRX_API_TOKEN_EXPIRATION': str,
             'DCRX_API_DATABASE_TYPE': str,
             'DCRX_API_DATABASE_USER': str,
             'DCRX_API_DATABASE_PASSWORD': str,
             'DCRX_API_DATABASE_NAME': str,
             'DCRX_API_DATABASE_URI': str,
-            'DCRX_API_DATABASE_PORT': int,
-            'DOCKER_REGISTRY_URI': str,
-            'DOCKER_REGISTRY_USERNAME': str,
-            'DOCKER_REGISTRY_PASSWORD': str
+            'DCRX_API_DATABASE_PORT': int
         }
```

### Comparing `dcrx-api-0.2.8/dcrx_api/env/load_env.py` & `dcrx-api-0.3.0/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/env/time_parser.py` & `dcrx-api-0.3.0/dcrx_api/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/lifespan.py` & `dcrx-api-0.3.0/dcrx_api/lifespan.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 )
 from dcrx_api.services.monitoring.context import (
     CPUMonitor,
     DockerMemoryMonitor,
     MemoryMonitor,
     MonitoringServiceContext
 )
+from dcrx_api.services.registry.context import (
+    RegistryConnection,
+    RegistryServiceContext
+)
 
 from dcrx_api.context.manager import context
 from .env import load_env, Env
 
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
@@ -47,22 +51,28 @@
         docker_memory=DockerMemoryMonitor(
             env,
             job_service_context.queue
         ),
         memory=MemoryMonitor()
     )
 
+    registry_service_context = RegistryServiceContext(
+        env=env,
+        connection=RegistryConnection(env)
+    )
+
     users_service_context = UsersServiceContext(
         env=env,
         connection=UsersConnection(env)
     )
 
     await context.initialize([
         auth_service_context,
         job_service_context,
         monitoring_service_context,
+        registry_service_context,
         users_service_context
     ])
 
     yield
 
     await context.close()
```

### Comparing `dcrx-api-0.2.8/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.3.0/dcrx_api/middleware/auth_middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
     async def dispatch(self, request, call_next):
 
         auth_service_context = context.get(ContextType.AUTH_SERVICE)
         users_service_context = context.get(ContextType.USERS_SERVICE)
 
         allowed_urls = [
+            '/docs',
+            '/openapi.json',
+            '/favicon.ico',
             "/users/login"
         ]
         
         if request.url.path in allowed_urls:
             response = await call_next(request)
             return response
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/auth/manager.py` & `dcrx-api-0.3.0/dcrx_api/services/auth/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
+import base64
 import datetime
 import functools
+from cryptography.fernet import Fernet
 from concurrent.futures import ThreadPoolExecutor
 from dcrx_api.env import Env
 from jose import JWTError, jwt
 from fastapi.security import OAuth2PasswordBearer
 from fastapi.security.utils import get_authorization_scheme_param
 from passlib.context import CryptContext
 from typing import (
@@ -41,26 +43,54 @@
         self.secret_key = env.DCRX_API_SECRET_KEY
         self.auth_algorithm = env.DCRX_API_AUTH_ALGORITHM
         self.token_expiration_time = TimeParser(env.DCRX_API_TOKEN_EXPIRATION).time
 
         self._executor: Union[ThreadPoolExecutor, None] = None
         self._loop: Union[asyncio.AbstractEventLoop, None] = None
 
+        fernet_key = base64.urlsafe_b64encode(
+            self.secret_key.encode().ljust(32)[:32]
+        )
+
+        self._encrypter = Fernet(fernet_key)
+
     async def connect(self):
         self._loop = asyncio.get_event_loop()
         self._executor = ThreadPoolExecutor(max_workers=self.pool_size)
 
     async def encrypt(self, password: str):
         return await self._loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.context.hash,
                 password
             )
         )
+    
+    async def encrypt_fernet(self, password: str):
+        encrypted_password = await self._loop.run_in_executor(
+            self._executor,
+            functools.partial(
+                self._encrypter.encrypt,
+                password.encode()
+            )
+        )
+
+        return encrypted_password.decode()
+    
+    async def decrypt_fernet(self, password: str):
+        decrypted_password = await self._loop.run_in_executor(
+            self._executor,
+            functools.partial(
+                self._encrypter.decrypt,
+                password.encode()
+            )
+        )
+
+        return decrypted_password.decode()
 
     async def authenticate_user(
         self,
         db_connection: UsersConnection,
         username: str, 
         password: str
     ) -> Union[DBUser, None]:
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/context.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/job.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/job.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import psutil
 import time
 import uuid
 from concurrent.futures import ThreadPoolExecutor
 from docker.models.images import Image as DockerImage
 from dcrx.image import Image, Label
 from dcrx.memory_file import MemoryFile
+from dcrx_api.env.time_parser import TimeParser
+from dcrx_api.services.registry.models import Registry
 from .models import (
     BuildOptions,
     ImageStats,
-    JobMetadata,
-    Registry
+    JobMetadata
 )
 from typing import (
     Union, 
     Optional, 
     Dict, 
     Any,
     List
@@ -29,15 +30,16 @@
 
     def __init__(
         self, 
         connection: JobsConnection,
         image: Image, 
         registry: Registry,
         build_options: Optional[BuildOptions]=None,
-        pool_size: int=psutil.cpu_count()
+        pool_size: int=psutil.cpu_count(),
+        timeout: str='10m',
     ) -> None:
 
         self.job_id = uuid.uuid4()
         self.job_name = image.full_name
 
         self.image = image
         self.registry = registry
@@ -51,43 +53,79 @@
         self._executor = ThreadPoolExecutor(max_workers=pool_size)
         self.loop = asyncio.get_event_loop()
         self.error: Union[Exception, None] = None
         self.connection = connection
 
         self.metadata = JobMetadata(
             id=self.job_id,
+            image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.CREATED.value,
             context=f"Job {self.job_id} created."
         )
 
         dcrx_api_label = Label(
             name='dcrx.api.id',
             value=str(self.job_id)
         )
 
         self.image.layers.insert(1, dcrx_api_label)
+        self.job_pool_size = pool_size
         self.job_image_label = f'{dcrx_api_label.name}={dcrx_api_label.value}'
+        
         self.job_start_time = time.monotonic()
+        self.timeout = TimeParser(timeout).time
+
         self.image_stats = ImageStats()
         self.client_closed = False
 
     async def list(self) -> List[DockerImage]:
         return await self.loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.client.images.list,
                 self.image.name
             )
         )
     
     async def run(self):
+        try:
+            await asyncio.wait_for(
+                asyncio.create_task(
+                    self._run(),
+                ),
+                timeout=self.timeout
+            )
         
+        except (asyncio.CancelledError, asyncio.TimeoutError,):
+
+            self.error = Exception(f'Job {self.job_id} timed out')
+
+            self.metadata = JobMetadata(
+                id=self.job_id,
+                image_registry=self.registry.registry_uri,
+                name=self.job_name,
+                image=self.image.name,
+                tag=self.image.tag,
+                status=JobStatus.FAILED.value,
+                context=f'Job timed out.'
+            )
+
+            await self.connection.update([
+                self.metadata
+            ], filters={
+                'id': self.job_id
+            })
+
+            await self.clear()
+            await self.close()
+  
+    async def _run(self):
         await self.connection.create([
             self.metadata
         ])
 
         try:
             await self.login_to_registry()
             await self.assemble_context()
@@ -100,14 +138,15 @@
         await self.clear()
         await self.close()
 
     async def login_to_registry(self):
 
         self.metadata = JobMetadata(
             id=self.job_id,
+            image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.AUTHORIZING.value,
             context=f'Job {self.job_id} authorizing to registry {self.registry.registry_uri}'
         )
 
@@ -128,14 +167,15 @@
             )
         )
 
     async def assemble_context(self):
 
         self.metadata = JobMetadata(
             id=self.job_id,
+            image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.GENERATING.value,
             context=f'Job {self.job_id} generating image {self.image.full_name}'
         )
 
@@ -151,14 +191,15 @@
         )
 
 
     async def build_image(self):
 
         self.metadata = JobMetadata(
             id=self.job_id,
+            image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.BUILDING.value,
             context=f'Job {self.job_id} building image {self.image.full_name}'
         )
 
@@ -191,14 +232,15 @@
             size=int(image.attrs.get('Size', 0)/10**6)
         )
         
     async def push_image(self):
 
         self.metadata = JobMetadata(
             id=self.job_id,
+            image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.PUSHING.value,
             context=f'Job {self.job_id} pushing image {self.image.full_name} to registry {self.registry.registry_uri}',
             size=self.image_stats.size
         )
@@ -216,14 +258,26 @@
                 self.image.name,
                 tag=self.image.tag
             )
         )
 
     async def clear(self):
 
+        await self.loop.run_in_executor(
+            self._executor,
+            self.client.api.prune_builds
+        )
+
+        await self.loop.run_in_executor(
+            self._executor,
+            functools.partial(      
+                self.client.api.prune_images
+            )
+        )
+
         for layer in self.image.layers:
             if layer.layer_type == 'stage':
 
                 try:
                     await self.loop.run_in_executor(
                         self._executor,
                         functools.partial(
@@ -249,33 +303,31 @@
 
         await self.loop.run_in_executor(
             self._executor,
             self.image.clear
         )
 
 
-    async def close(
-        self,
-        cancelled: bool=False    
-    ):
+    async def close(self):
 
         if self.error is None:
             status = JobStatus.DONE
             context = f'Job {self.job_id} complete'
 
-        elif cancelled:
+        elif self.metadata.status == JobStatus.CANCELLED.value:
             status = JobStatus.CANCELLED
             context = f'Job {self.job_id} cancelled'
 
         else:
             status = JobStatus.FAILED
             context = str(self.error)
 
         self.metadata = JobMetadata(
             id=self.job_id,
+            image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=status.value,
             context=context,
             size=self.image_stats.size
         )
@@ -283,20 +335,27 @@
 
         await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
-        self._executor.shutdown(cancel_futures=True)
-
         if self.client_closed is False:
-            self.client.close()
+            await self.loop.run_in_executor(
+                None,
+                self.client.close
+            )
             self.client_closed = True
 
         if self.context:
-            self.context.close()
+            await self.loop.run_in_executor(
+                self._executor,
+                self.context.close
+            )
+
+        
+        self._executor.shutdown(cancel_futures=True)
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import asyncio
-import uuid
+import docker
+import functools
+import subprocess
 import time
+import uuid
+from concurrent.futures import ThreadPoolExecutor
 from dcrx_api.env import Env
 from dcrx_api.env.time_parser import TimeParser
-from dcrx.image import Image
 from docker.models.images import Image as DockerImage
-from .models import BuildOptions
-from .models import Registry
 from typing import (
-    Optional, 
     Dict, 
     Union,
     List
 )
 from .job import Job
-from .connection import JobsConnection
 from .models import (
     JobMetadata,
     JobNotFoundException
 )
 from .status import JobStatus
 
 
 class JobQueue:
 
     def __init__(self, env: Env) -> None:
 
         self.pool_size = env.DCRX_API_JOB_WORKERS
 
-        self.registry_uri = env.DOCKER_REGISTRY_URI
-        self.registry_username = env.DOCKER_REGISTRY_USERNAME
-        self.registry_password = env.DOCKER_REGISTRY_PASSWORD
-
         self._jobs: Dict[uuid.UUID, Job] = {}
         self._active: Dict[uuid.UUID, asyncio.Task] = {}
         self.pool_guard = asyncio.Semaphore(
             value=env.DCRX_API_JOB_POOL_SIZE
         )
+        self._executor = ThreadPoolExecutor(max_workers=env.DCRX_API_JOB_WORKERS)
 
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._job_max_age = TimeParser(env.DCRX_API_JOB_MAX_AGE).time
         self._job_prune_interval = TimeParser(env.DCRX_API_JOB_PRUNE_INTERVAL).time
         self._run_cleanup = True
         self.active_images: List[DockerImage] = []
         self.cancelling: List[asyncio.Task] = []
+        self.client = docker.DockerClient(
+            max_pool_size=env.DCRX_API_JOB_WORKERS
+        )
+        self.completed: List[str] = []
+        self.loop = asyncio.get_event_loop()
 
     async def get_active_images(self) -> List[DockerImage]:
 
         active_statuses = [
             'AUTHORIZING',
             'CREATED',
             'GENERATING',
@@ -77,14 +78,29 @@
         self._cleanup_task = asyncio.create_task(
             self._monitor_jobs()
         )
 
     async def _monitor_jobs(self):
         while self._run_cleanup:
 
+            await self.loop.run_in_executor(
+                self._executor,
+                functools.partial(
+                    subprocess.run,
+                    [
+                        "docker",
+                        "system",
+                        "prune",
+                        "-f"
+                    ],
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE
+                )
+            )
+
             self.active_images = await self.get_active_images()
 
             queue_jobs = dict(self._jobs)
             
             for job_id, job in queue_jobs.items():
                 
                 job_elapsed = time.monotonic() - job.job_start_time
@@ -94,55 +110,46 @@
                     self.cancelling.append(
                         asyncio.create_task(
                             self._cancel_task(job)
                         )
                     )
 
                 if job_is_pruneable and job_elapsed > self._job_max_age:
+
+                    images = await self.loop.run_in_executor(
+                        self._executor,
+                        self.client.images.list,
+                        job.image.name
+                    )
+
+                    if len(images) > 0:
+                        await self.loop.run_in_executor(
+                            self._executor,
+                            self.client.images.remove,
+                            job.image.name
+                        )
+
                     del self._jobs[job_id]
 
             
             cancelling_tasks = list(self.cancelling)
             for cancel_task in cancelling_tasks:
                 if cancel_task.done():
                     self.cancelling.remove(cancel_task)
             
             await asyncio.sleep(self._job_prune_interval)
 
     async def _cancel_task(self, job: Job):
-        
-        job.client.close()
+
         job.client_closed = True
 
         await job.clear()
-        await job.close(cancelled=True)
+        await job.close()
 
-    def submit(
-        self,
-        connection: JobsConnection,
-        image: Image, 
-        registry: Optional[Registry]=None,
-        build_options: Optional[BuildOptions]=None
-    ) -> JobMetadata:
-        
-        if registry is None:
-            registry = Registry(
-                registry_uri=self.registry_uri,
-                registry_user=self.registry_username,
-                registry_password=self.registry_password
-                
-            )
-
-        job = Job(
-            connection,
-            image,
-            registry,
-            build_options=build_options,
-            pool_size=self.pool_size
-        )
+    def submit(self, job: Job) -> JobMetadata:
 
         self._jobs[job.job_id] = job
 
         self._active[job.job_id] = asyncio.create_task(
             job.run()
         )
 
@@ -187,14 +194,15 @@
             return JobNotFoundException(
                 job_id=job_id,
                 message=f'Job - {job_id} - not found or is not active.'
             )
         
         cancelled_job.metadata = JobMetadata(
             id=cancelled_job.job_id,
+            image_registry=cancelled_job.registry.registry_uri,
             name=cancelled_job.job_name,
             image=cancelled_job.image.name,
             tag=cancelled_job.image.tag,
             status=JobStatus.CANCELLED.value,
             context=f'Job {cancelled_job.job_id} cancelled.',
             size=cancelled_job.metadata.size
         )
@@ -204,14 +212,23 @@
         return cancelled_job
     
     async def close(self):
 
         self._run_cleanup = False
         await self._cleanup_task
 
+        await self.loop.run_in_executor(
+            self._executor,
+            self.client.close
+        )
+
         for job in self._active.values():
             if not job.done():
                 job.cancel()
 
         for job in self._jobs.values():
-            await job.close()
+            if job.client_closed is False:
+                await job.close()
+
+        self._executor.shutdown(cancel_futures=True)
+
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import sqlalchemy
 import uuid
 from dcrx_api.database.table_types import TableTypes
 
 
-class JobsMySQLTable:
+class JobsSQLiteTable:
 
     def __init__(
         self, 
         jobs_table_name: str
     ) -> None:
         self.table = sqlalchemy.Table(
             jobs_table_name,
             sqlalchemy.MetaData(),
             sqlalchemy.Column(
                 'id', 
-                sqlalchemy.String(36),
+                sqlalchemy.BLOB,
                 primary_key=True,
-                default=uuid.uuid4
+                default=lambda: str(uuid.uuid4()).encode()
+            ),
+            sqlalchemy.Column(
+                'image_registry', 
+                sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'name',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'image',
@@ -42,24 +46,26 @@
                 'size',
                 sqlalchemy.INTEGER
             )
         )
 
         self.columns = {
             'id': self.table.c.id,
+            'image_registry': self.table.c.image_registry,
             'name': self.table.c.name,
             'image': self.table.c.image,
             'tag': self.table.c.tag,
             'status': self.table.c.status,
             'context': self.table.c.context,
             'size': self.table.c.size
         }
 
         self.types_map = {
-            'id': lambda value: str(value),
+            'id': lambda value: str(value).encode(),
+            'image_registry': lambda value: str(value),
             'name': lambda value: str(value),
             'image': lambda value: str(value),
             'tag': lambda value: str(value),
             'status': lambda value: str(value),
             'context': lambda value: str(value),
             'size': lambda value: int(value)
         }
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,18 @@
             sqlalchemy.Column(
                 'id', 
                 UUID(as_uuid=True),
                 primary_key=True,
                 default=uuid.uuid4
             ),
             sqlalchemy.Column(
+                'image_registry', 
+                sqlalchemy.TEXT
+            ),
+            sqlalchemy.Column(
                 'name',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'image',
                 sqlalchemy.TEXT
             ),
@@ -43,24 +47,26 @@
                 'size',
                 sqlalchemy.BIGINT
             )
         )
 
         self.columns = {
             'id': self.table.c.id,
+            'image_registry': self.table.c.image_registry,
             'name': self.table.c.name,
             'image': self.table.c.image,
             'tag': self.table.c.tag,
             'status': self.table.c.status,
             'context': self.table.c.context,
             'size': self.table.c.size
         }
 
         self.types_map = {
             'id': lambda value: uuid.UUID(value),
+            'image_registry': lambda value: str(value),
             'name': lambda value: str(value),
             'image': lambda value: str(value),
             'tag': lambda value: str(value),
             'status': lambda value: str(value),
             'context': lambda value: str(value),
             'size': lambda value: int(value)
         }
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import sqlalchemy
 import uuid
 from dcrx_api.database.table_types import TableTypes
 
 
-class JobsSQLiteTable:
+class JobsMySQLTable:
 
     def __init__(
         self, 
         jobs_table_name: str
     ) -> None:
         self.table = sqlalchemy.Table(
             jobs_table_name,
             sqlalchemy.MetaData(),
             sqlalchemy.Column(
                 'id', 
-                sqlalchemy.BLOB,
+                sqlalchemy.String(36),
                 primary_key=True,
-                default=uuid.uuid4
+                default=lambda: str(uuid.uuid4())
+            ),
+            sqlalchemy.Column(
+                'image_registry', 
+                sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'name',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'image',
@@ -42,24 +46,26 @@
                 'size',
                 sqlalchemy.INTEGER
             )
         )
 
         self.columns = {
             'id': self.table.c.id,
+            'image_registry': self.table.c.image_registry,
             'name': self.table.c.name,
             'image': self.table.c.image,
             'tag': self.table.c.tag,
             'status': self.table.c.status,
             'context': self.table.c.context,
             'size': self.table.c.size
         }
 
         self.types_map = {
-            'id': lambda value: str(value).encode(),
+            'id': lambda value: str(value),
+            'image_registry': lambda value: str(value),
             'name': lambda value: str(value),
             'image': lambda value: str(value),
             'tag': lambda value: str(value),
             'status': lambda value: str(value),
             'context': lambda value: str(value),
             'size': lambda value: int(value)
         }
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/monitoring/base/monitor.py` & `dcrx-api-0.3.0/dcrx_api/services/monitoring/base/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/monitoring/context.py` & `dcrx-api-0.3.0/dcrx_api/services/monitoring/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/monitoring/memory/docker_memory_monitor.py` & `dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/docker_memory_monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/monitoring/memory/monitor.py` & `dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/users/connection.py` & `dcrx-api-0.3.0/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/users/context.py` & `dcrx-api-0.3.0/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/users/service.py` & `dcrx-api-0.3.0/dcrx_api/services/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.3.0/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.table = sqlalchemy.Table(
             users_table_name,
             sqlalchemy.MetaData(),
             sqlalchemy.Column(
                 'id', 
                 sqlalchemy.String(36),
                 primary_key=True,
-                default=uuid.uuid4
+                default=lambda: str(uuid.uuid4)
             ),
             sqlalchemy.Column(
                 'username',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'first_name',
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.3.0/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.3.0/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.table = sqlalchemy.Table(
             users_table_name,
             sqlalchemy.MetaData(),
             sqlalchemy.Column(
                 'id', 
                 sqlalchemy.BLOB,
                 primary_key=True,
-                default=uuid.uuid4
+                default=lambda: str(uuid.uuid4)
             ),
             sqlalchemy.Column(
                 'username',
                 sqlalchemy.TEXT
             ),
             sqlalchemy.Column(
                 'first_name',
```

### Comparing `dcrx-api-0.2.8/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.3.0/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.2.8/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: dcrx-api
-Version: 0.2.8
-Summary: A RESTful implementation of the DCRX Docker library.
-Home-page: https://github.com/scorbettUM/dcrx-api
-Author: Sean Corbett
-Author-email: sean.corbett@umontana.edu
-Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dcrx-api
 [![PyPI version](https://img.shields.io/pypi/v/dcrx-api?color=gre)](https://pypi.org/project/dcrx-api/)
 [![License](https://img.shields.io/github/license/scorbettUM/dcrx-api)](https://github.com/scorbettUM/dcrx-api/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/scorbettUM/dcrx-api/blob/main/CODE_OF_CONDUCT.md)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dcrx-api)](https://pypi.org/project/dcrx-api/)
 
 DCRX-API is a RESTful implementation of the dcrx library, allowing you to create Docker images on request! DCRX-API extends dcrx, providing integrations with the Docker API and dcrx that allow images to be built by making REST requests.
@@ -45,14 +27,16 @@
 
 
 # Getting Started
 
 DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
+DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled.
+
 DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
 
 DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
 
 DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
 
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
@@ -73,19 +57,14 @@
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
 
 DCRX_API_DATABASE_URI=sqlite+aiosqlite:///dcrx # URL/URI of SQL database for storing users and job metadata.
 
 DCRX_API_DATABASE_PORT=3369 # Port of SQL database for storing users and job metadata.
 
-DOCKER_REGISTRY_URI=https://docker.io/v1/myrepo/test-images # Default Docker image registry to push images to.
-
-DOCKER_REGISTRY_USERNAME=test # Default Username to authenticate Docker pushes to the provided registry.
-
-DOCKER_REGISTRY_PASSWORD=test-repo-password # Default Password to authenticate Docker pushes to the provided registry.
 ```
 
 Prior to starting the server, we recommend seeding the database with an initial user. To do so, run the command:
 
 ```bash
 dcrx-api database initialize --username $USERNAME --password $PASSWORD --first-name $FIRST_NAME --last-name $LAST_NAME --email $EMAIL
 ```
@@ -109,20 +88,36 @@
 and navigate to `localhost:2277/docs`, where you'll find dcrx-api's OpenAPI documentation.
 
 
 # Authenticating and Building an Image
 
 From here, we'll need to authenticate using the initial user we created above. Open the tab for `/users/login`, and for the `username` and `password` fields enter the username and password of the initial user, then click `Execute`. A `200` status response containg the initial user's username and id should return.
 
+Before creating and pushing any images, we need to create a Registry. Navigate to the `/registry/create` tab. We'll need to provide a `registry_name` (unique shortand reference of our choosing), `registry_uri` (HTTP url to the registry), `registry_user`, and `registry_password:
+
+```json
+{
+  "registry_name": "hello-world",
+  "registry_uri": "https://docker.io/v1/testreg/hello-world",
+  "registry_user": "testuser",
+  "registry_password": "testpassword1*"
+}
+```
+
+Submit the request. DCRX-API will take the information, encrypt the registry password, and store it.
+
 Next navigate to the `/jobs/images/create` tab. As before, we'll need to fill out some data. Go ahead and copy paste the below into the input for the request body:
 
 ```json
 {
-  "name": "hello-world",
+  "name": "testreg/hello-world",
   "tag": "latest",
+  "registry": {
+    "registry_name": "hello-world"
+  },
   "layers": [
     {
       "layer_type": "stage",
       "base": "python",
       "tag": "3.11-slim"
     },
     {
@@ -132,15 +127,15 @@
             "Hello world!"
         ]
     }
   ]
 }
 ```
 
-A dcrx-api image build request requires, at-minimum, a `name`, `tag` and one or more `layer` objects, which will be processed and build in-order of appearance. Note that each layer object almost exactly corresponds to its `dcrx` call. The above corresponds exactly to:
+A dcrx-api image build request requires, at-minimum, a `name`, `tag`, `registry_name`, and one or more `layer` objects, which will be processed and build in-order of appearance. Note that each layer object almost exactly corresponds to its `dcrx` call. The above corresponds exactly to:
 
 ```python
 
 from dcrx import Image
 
 hello_world = Image('hello-world')
 
@@ -149,15 +144,15 @@
     '3.11-slim'
 ).entrypoint([
     'echo',
     'Hello world!'
 ])
 ```
 
-Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in dcrx-api's environmental variables.
+Go ahead and submit the request via the `Execute` button. This will start a job to build the specified image and push it to the repository specified in the request.
 
 Note that dcrx-api doesn't wait for the image to be built, instead returning a `JobMetadata` response with a status code of `200`, including the `job_id`. Building images is time-intensive and could potentially bog down a server, so dcrx-api builds and pushes images in the background. We can use the `job_id` of a Job to make further `GET` requests to the `/jobs/images/{job_id}/get` endpoint to monitor and check how our job is progressing. If we need to cancel a job for any reason, we can simple make a `DELETE` request to `/jobs/images/{job_id}/cancel`.
 
 
 # Running the Docker Image
 
 To run the Docker image, we recommend first creating a `.env` file with the required environment variables noted above. Then run the image:
@@ -185,35 +180,7 @@
 
 
 # Notes and Gotchas
 
 1. Does dcrx-api require a volume to run? - Yes. While dcrx-api builds images in-memory, Docker still (frustratingly) requires that a physical file be present in the build directory. This means that, if running dcrx-api in Docker or via Kubernetes, you will need to have a volume with the correct permissions mounted.
 
 2. Does the dcrx-api Docker image require root? - Currently yes. The dcrx-api image is based on the latest version of Docker's `dind` image, which runs as and requires root privlidges. We're working on getting the rootless version of `dind` working though!
-
-3. Can I push to a registry besides the default? - Yes. New image job requests can be submitted with optional Registry configuration. For example:
-
-```
-{
-  "name": "hello-world",
-  "tag": "latest",
-  "registry": {
-    "registry_url": "https://docker.io/v1/mytest/registry",
-    "registry_user": "DockerUser100",
-    "registry_password": "MyDockerHubToken999*"
-  },
-  "layers": [
-    {
-      "layer_type": "stage",
-      "base": "python",
-      "tag": "3.11-slim"
-    },
-    {
-        "layer_type": "entrypoint",
-        "command": [
-            "echo",
-            "Hello world!"
-        ]
-    }
-  ]
-}
-```
```

### Comparing `dcrx-api-0.2.8/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.3.0/dcrx_api.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 dcrx_api/services/jobs/service.py
 dcrx_api/services/jobs/status.py
 dcrx_api/services/jobs/models/__init__.py
 dcrx_api/services/jobs/models/build_options.py
 dcrx_api/services/jobs/models/image_stats.py
 dcrx_api/services/jobs/models/job_metadata.py
 dcrx_api/services/jobs/models/job_not_found_exception.py
+dcrx_api/services/jobs/models/job_registry.py
 dcrx_api/services/jobs/models/new_image.py
-dcrx_api/services/jobs/models/registry.py
 dcrx_api/services/jobs/models/remote_add.py
 dcrx_api/services/jobs/models/server_memory_limit_exception.py
 dcrx_api/services/jobs/table/__init__.py
 dcrx_api/services/jobs/table/jobs_mysql_table.py
 dcrx_api/services/jobs/table/jobs_postgres_table.py
 dcrx_api/services/jobs/table/jobs_sqlite_table.py
 dcrx_api/services/jobs/table/jobs_table.py
@@ -63,14 +63,28 @@
 dcrx_api/services/monitoring/base/exceptions.py
 dcrx_api/services/monitoring/base/monitor.py
 dcrx_api/services/monitoring/cpu/__init__.py
 dcrx_api/services/monitoring/cpu/monitor.py
 dcrx_api/services/monitoring/memory/__init__.py
 dcrx_api/services/monitoring/memory/docker_memory_monitor.py
 dcrx_api/services/monitoring/memory/monitor.py
+dcrx_api/services/registry/__init__.py
+dcrx_api/services/registry/connection.py
+dcrx_api/services/registry/context.py
+dcrx_api/services/registry/service.py
+dcrx_api/services/registry/models/__init__.py
+dcrx_api/services/registry/models/registry.py
+dcrx_api/services/registry/models/registry_metadata.py
+dcrx_api/services/registry/models/registry_not_found_exception.py
+dcrx_api/services/registry/models/registry_transaction_success_response.py
+dcrx_api/services/registry/table/__init__.py
+dcrx_api/services/registry/table/registry_mysql_table.py
+dcrx_api/services/registry/table/registry_postgres_table.py
+dcrx_api/services/registry/table/registry_sqlite_table.py
+dcrx_api/services/registry/table/registry_table.py
 dcrx_api/services/users/__init__.py
 dcrx_api/services/users/connection.py
 dcrx_api/services/users/context.py
 dcrx_api/services/users/service.py
 dcrx_api/services/users/models/__init__.py
 dcrx_api/services/users/models/authorized_user.py
 dcrx_api/services/users/models/base_user.py
```

### Comparing `dcrx-api-0.2.8/setup.py` & `dcrx-api-0.3.0/setup.py`

 * *Files identical despite different names*

