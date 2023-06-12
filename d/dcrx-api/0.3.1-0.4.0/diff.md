# Comparing `tmp/dcrx-api-0.3.1.tar.gz` & `tmp/dcrx-api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.3.1.tar", last modified: Mon Jun 12 15:19:28 2023, max compression
+gzip compressed data, was "dcrx-api-0.4.0.tar", last modified: Mon Jun 12 20:42:14 2023, max compression
```

## Comparing `dcrx-api-0.3.1.tar` & `dcrx-api-0.4.0.tar`

### file list

```diff
@@ -1,126 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/image_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/job_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/remote_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/server_limit_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/cpu/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/registry/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/registry/table/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.779478 dcrx-api-0.4.0/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/connection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/models/database_transaction_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/env/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/job_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/models/server_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.787478 dcrx-api-0.4.0/dcrx_api/services/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/registry/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/models/registry_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/registry/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:42:14.783478 dcrx-api-0.4.0/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 20:42:14.000000 dcrx-api-0.4.0/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:42:14.791478 dcrx-api-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-12 20:42:10.000000 dcrx-api-0.4.0/setup.py
```

### Comparing `dcrx-api-0.3.1/LICENSE` & `dcrx-api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/PKG-INFO` & `dcrx-api-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.3.1
+Version: 0.4.0
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,32 +45,38 @@
 
 
 # Getting Started
 
 DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
-DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled.
+DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled. Default is 10 minutes.
 
-DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
+DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error. Default is 50 percent.
 
 DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
 
 DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
 
+DCRX_API_JOB_MAX_PENDING_WAIT=10m # The maximum amount of time a job can remain in PENDING status. Jobs that exceed this threshold are timed out and will fail.
+
+DCRX_API_JOB_MAX_PENDING=100 # The maximum number of pending jobs that a single instance of DCRX-API allows. Default is 100.
+
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
 
 DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION='15m' # Time for JWT authorization token to expire. Default is 15 minutes.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
+DCRX_API_DATABASE_TRANSACTION_RETRIES=3 # Number of times to retry a failed transaction. Default is 3.
+
 DCRX_API_DATABASE_TYPE=sqlite # Type of database to use. Default is sqlite and options are mysql, asyncpg, and sqlite.
 
 DCRX_API_DATABASE_USER=admin # Username used for database connection authentication
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
```

### Comparing `dcrx-api-0.3.1/README.md` & `dcrx-api-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,32 +27,38 @@
 
 
 # Getting Started
 
 DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
-DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled.
+DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled. Default is 10 minutes.
 
-DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
+DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error. Default is 50 percent.
 
 DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
 
 DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
 
+DCRX_API_JOB_MAX_PENDING_WAIT=10m # The maximum amount of time a job can remain in PENDING status. Jobs that exceed this threshold are timed out and will fail.
+
+DCRX_API_JOB_MAX_PENDING=100 # The maximum number of pending jobs that a single instance of DCRX-API allows. Default is 100.
+
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
 
 DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION='15m' # Time for JWT authorization token to expire. Default is 15 minutes.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
+DCRX_API_DATABASE_TRANSACTION_RETRIES=3 # Number of times to retry a failed transaction. Default is 3.
+
 DCRX_API_DATABASE_TYPE=sqlite # Type of database to use. Default is sqlite and options are mysql, asyncpg, and sqlite.
 
 DCRX_API_DATABASE_USER=admin # Username used for database connection authentication
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
```

### Comparing `dcrx-api-0.3.1/dcrx_api/cli/base.py` & `dcrx-api-0.4.0/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/cli/database.py` & `dcrx-api-0.4.0/dcrx_api/cli/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,19 +95,19 @@
     )
 
     await connection.connect()
     await connection.init()
 
     users = await connection.select()
 
-    if len(users) < 1:
+    if users.data is None or len(users.data) < 1:
         await connection.create([
             user
         ])
-    
+
     await auth.close()
     await connection.close()
 
 
 @click.group(help='Commands to migrate or initialize the database.')
 def database():
     pass
```

### Comparing `dcrx-api-0.3.1/dcrx_api/cli/server.py` & `dcrx-api-0.4.0/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/context/manager.py` & `dcrx-api-0.4.0/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/env/env.py` & `dcrx-api-0.4.0/dcrx_api/env/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
     DCRX_API_MAX_MEMORY_PERCENT_USAGE: StrictFloat=50
-    DCRX_API_JOB_TIMEOUT: StrictStr='5s'
+    DCRX_API_JOB_TIMEOUT: StrictStr='10m'
     DCRX_API_JOB_PRUNE_INTERVAL: StrictStr='1s'
-    DCRX_API_JOB_MAX_AGE: StrictStr='1m'
+    DCRX_API_JOB_MAX_AGE: StrictStr='10m'
     DCRX_API_JOB_WORKERS: StrictInt=psutil.cpu_count()
+    DCRX_API_JOB_MAX_PENDING_WAIT: StrictStr='10m'
     DCRX_API_JOB_MAX_PENDING: StrictInt=100
     DCRX_API_JOB_POOL_SIZE: StrictInt=10
     DCRX_API_SECRET_KEY: StrictStr
     DCRX_API_AUTH_ALGORITHM: StrictStr='HS256'
     DCRX_API_TOKEN_EXPIRATION: StrictStr='15m'
+    DCRX_API_DATABASE_TRANSACTION_RETRIES: StrictInt=3
     DCRX_API_DATABASE_TYPE: Optional[StrictStr]='sqlite'
     DCRX_API_DATABASE_USER: Optional[StrictStr]
     DCRX_API_DATABASE_URI: Optional[StrictStr]
     DCRX_API_DATABASE_PORT: Optional[StrictInt]
     DCRX_API_DATABASE_PASSWORD: Optional[StrictStr]
     DCRX_API_DATABASE_NAME: StrictStr='dcrx'
 
@@ -38,19 +40,21 @@
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
             'DCRX_API_MAX_MEMORY_PERCENT_USAGE': float,
             'DCRX_API_JOB_PRUNE_INTERVAL': str,
             'DCRX_API_JOB_TIMEOUT': str,
             'DCRX_API_JOB_MAX_AGE': str,
             'DCRX_API_JOB_WORKERS': int,
+            'DCRX_API_JOB_MAX_PENDING_WAIT': str,
             'DCRX_API_JOB_MAX_PENDING': int,
             'DCRX_API_JOB_POOL_SIZE': int,
             'DCRX_API_SECRET_KEY': str,
             'DCRX_API_AUTH_ALGORITHM': str,
             'DCRX_API_TOKEN_EXPIRATION': str,
+            'DCRX_API_DATABASE_TRANSACTION_RETRIES': int,
             'DCRX_API_DATABASE_TYPE': str,
             'DCRX_API_DATABASE_USER': str,
             'DCRX_API_DATABASE_PASSWORD': str,
             'DCRX_API_DATABASE_NAME': str,
             'DCRX_API_DATABASE_URI': str,
             'DCRX_API_DATABASE_PORT': int
         }
```

### Comparing `dcrx-api-0.3.1/dcrx_api/env/load_env.py` & `dcrx-api-0.4.0/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/env/time_parser.py` & `dcrx-api-0.4.0/dcrx_api/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/lifespan.py` & `dcrx-api-0.4.0/dcrx_api/lifespan.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,23 @@
     env = load_env(Env.types_map())
 
     auth_service_context = AuthServiceContext(
         env=env,
         manager=AuthorizationSessionManager(env)
     )
 
+    jobs_service_connection = JobsConnection(env)
+
     job_service_context = JobServiceContext(
         env=env,
-        queue=JobQueue(env),
-        connection=JobsConnection(env)
+        queue=JobQueue(
+            env,
+            jobs_service_connection
+        ),
+        connection=jobs_service_connection
     )
 
     monitoring_service_context = MonitoringServiceContext(
         env=env,
         monitor_name='dcrx.main',
         cpu=CPUMonitor(),
         memory=MemoryMonitor()
```

### Comparing `dcrx-api-0.3.1/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.4.0/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/auth/manager.py` & `dcrx-api-0.4.0/dcrx_api/services/auth/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,27 +90,27 @@
 
     async def authenticate_user(
         self,
         db_connection: UsersConnection,
         username: str, 
         password: str
     ) -> Union[DBUser, None]:
-        users: List[DBUser] = await db_connection.select(
+        users = await db_connection.select(
             filters={
                 'username': username
             }
         )
 
-        if len(users) < 1:
+        if users.data is None or len(users.data) < 1:
             return AuthResponse(
                 error='User authorization failed',
                 message='Authentication failed'
             )
         
-        user = users.pop()
+        user = users.data.pop()
         
         password_verified = await self._loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.context.verify,
                 password, 
                 user.hashed_password
@@ -224,21 +224,21 @@
 
         except JWTError as validation_error:
             return AuthResponse(
                     error=str(validation_error),
                     message='Authentication failed'
                 )
         
-        users: List[DBUser] = await connection.select(
+        users = await connection.select(
             filters={
                 'username': token_data.username
             }
         )
 
-        if len(users) < 1:
+        if users.data is None or len(users.data) < 1:
             return AuthResponse(
                 error='User authorization failed',
                 message='Authentication failed'
             )
         
         return AuthResponse(
             message='OK'
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.4.0/dcrx_api/services/users/connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,91 @@
 from dcrx_api.database import (
+    ConnectionConfig,
     DatabaseConnection,
-    ConnectionConfig
 )
+from dcrx_api.database.models import DatabaseTransactionResult
 from dcrx_api.env import Env
 from typing import (
     List,
     Dict,
     Any
 )
-from .models import JobMetadata
-from .table import JobsTable
+from .models import DBUser
+from .table import UsersTable
 
 
-class JobsConnection(DatabaseConnection[JobMetadata]):
+class UsersConnection(DatabaseConnection[DBUser]):
 
     def __init__(self, env: Env) -> None:
         super().__init__(
             ConnectionConfig(
                 database_username=env.DCRX_API_DATABASE_USER,
                 database_password=env.DCRX_API_DATABASE_PASSWORD,
                 database_type=env.DCRX_API_DATABASE_TYPE,
                 database_uri=env.DCRX_API_DATABASE_URI,
                 database_port=env.DCRX_API_DATABASE_PORT,
-                database_name=env.DCRX_API_DATABASE_NAME
+                database_name=env.DCRX_API_DATABASE_NAME,
+                database_transaction_retries=env.DCRX_API_DATABASE_TRANSACTION_RETRIES
             )
         )
 
-        self.table: JobsTable[JobMetadata] = JobsTable(
-            'jobs',
+        self.table: UsersTable[DBUser] = UsersTable(
+            'users',
             database_type=self.config.database_type
         )
 
-    async def init(self):
+    async def init(self) -> DatabaseTransactionResult[DBUser]:
         return await self.create_table(self.table.selected.table)
 
     async def select(
         self, 
         filters: Dict[str, Any]={}
-    ):
+    ) -> DatabaseTransactionResult[DBUser]:
         return await self.get(
             self.table.select(
                 filters={
                     name: self.table.selected.types_map.get(
                         name
                     )(value) for name, value in filters.items()
                 }
             )
         )
 
     async def create(
         self, 
-        jobs: List[JobMetadata]
-    ):
+        users: List[DBUser]
+    ) -> DatabaseTransactionResult[DBUser]:
        return await self.insert_or_update(
-           self.table.insert(jobs)
+           self.table.insert(users)
        )
     
     async def update(
         self, 
-        jobs: List[JobMetadata],
+        users: List[DBUser],
         filters: Dict[str, Any]={}
-    ):
+    ) -> DatabaseTransactionResult[DBUser]:
         return await self.insert_or_update(
             self.table.update(
-                jobs,
+                users,
                 filters={
                     name: self.table.selected.types_map.get(
                         name
                     )(value) for name, value in filters.items()
                 }
             )
         )
     
     async def remove(
         self,
         filters: Dict[str, Any]
-    ):
+    ) -> DatabaseTransactionResult[DBUser]:
         return await self.delete([
             self.table.delete({
                 name: self.table.selected.types_map.get(
                     name
                 )(value) for name, value in filters.items()
             })
         ])
     
-    async def drop(self):
+    async def drop(self) -> DatabaseTransactionResult[DBUser]:
         return await self.drop_table(self.table)
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/context.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/job.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/job.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import asyncio
 import docker
 import functools
 import psutil
 import time
 import uuid
 from concurrent.futures import ThreadPoolExecutor
+from docker.errors import (
+    ImageNotFound,
+    APIError
+)
 from docker.models.images import Image as DockerImage
 from dcrx.image import Image, Label
 from dcrx.memory_file import MemoryFile
 from dcrx_api.env.time_parser import TimeParser
 from dcrx_api.services.registry.models import Registry
 from .models import (
     BuildOptions,
     ImageStats,
-    JobMetadata
+    JobMetadata,
+    JobStepResult
 )
 from typing import (
     Union, 
     Optional, 
     Dict, 
     Any,
     List
@@ -32,14 +37,15 @@
         self, 
         connection: JobsConnection,
         image: Image, 
         registry: Registry,
         build_options: Optional[BuildOptions]=None,
         pool_size: int=psutil.cpu_count(),
         timeout: str='10m',
+        wait_timeout: str='10m'
     ) -> None:
 
         self.job_id = uuid.uuid4()
         self.job_name = image.full_name
 
         self.image = image
         self.registry = registry
@@ -72,31 +78,31 @@
 
         self.image.layers.insert(1, dcrx_api_label)
         self.job_pool_size = pool_size
         self.job_image_label = f'{dcrx_api_label.name}={dcrx_api_label.value}'
         
         self.job_start_time = time.monotonic()
         self.timeout = TimeParser(timeout).time
+        self.pending_timeout = TimeParser(wait_timeout).time
 
         self.image_stats = ImageStats()
-        self.client_closed = False
+        self.shutdown = False
         self.waiter: Union[asyncio.Future, None]=None
 
     async def list(self) -> List[DockerImage]:
         return await self.loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.client.images.list,
                 self.image.name
             )
         )
     
     async def run(self):
 
-
         if self.waiter:
             self.metadata = JobMetadata(
                 id=self.job_id,
                 image_registry=self.registry.registry_uri,
                 name=self.job_name,
                 image=self.image.name,
                 tag=self.image.tag,
@@ -105,136 +111,187 @@
             )
 
             await self.connection.update([
                 self.metadata
             ], filters={
                 'id': self.job_id
             })
-            await self.waiter
+
+            try:
+                await asyncio.wait_for(
+                    self.waiter,
+                    timeout=self.pending_timeout
+                )
+
+            except (asyncio.CancelledError, asyncio.TimeoutError,):
+                await self.cancel()
+                return 
 
         try:
             await asyncio.wait_for(
                 asyncio.create_task(
                     self._run(),
                 ),
                 timeout=self.timeout
             )
         
         except (asyncio.CancelledError, asyncio.TimeoutError,):
+            await self.cancel()
 
-            self.error = Exception(f'Job {self.job_id} timed out')
-
-            self.metadata = JobMetadata(
-                id=self.job_id,
-                image_registry=self.registry.registry_uri,
-                name=self.job_name,
-                image=self.image.name,
-                tag=self.image.tag,
-                status=JobStatus.FAILED.value,
-                context=f'Job timed out.'
-            )
-
-            await self.connection.update([
-                self.metadata
-            ], filters={
-                'id': self.job_id
-            })
 
-            await self.clear()
-            await self.close()
-  
-    async def _run(self):
+    async def _run(self) -> JobStepResult:
 
-        await self.connection.create([
+        response = await self.connection.create([
             self.metadata
         ])
 
+        if response.error:
+            self.error = response.error
+            return JobStepResult(
+                message='Failed to connect to database',
+                error=self.error
+            )
+        
+        job_step_result = JobStepResult(
+            message='Job successfully initialized'
+        )
+
         try:
-            await self.login_to_registry()
-            await self.assemble_context()
-            await self.build_image()
-            await self.push_image()
+            job_step_result = await self.login_to_registry()
+            job_step_result = await self.assemble_context()
+            job_step_result = await self.build_image()
+            job_step_result = await self.push_image()
 
         except Exception as job_exception:
             self.error = job_exception
+            job_step_result = JobStepResult(
+                message='Job failed',
+                error=str(job_exception)
+            )
+
+        return job_step_result
+    
+    async def cancel(self):
+        self.error = Exception(f'Job {self.job_id} timed out')
+
+        self.metadata = JobMetadata(
+            id=self.job_id,
+            image_registry=self.registry.registry_uri,
+            name=self.job_name,
+            image=self.image.name,
+            tag=self.image.tag,
+            status=JobStatus.FAILED.value,
+            context=f'Job timed out.'
+        )
 
-        await self.clear()
-        await self.close()
+        await self.connection.update([
+            self.metadata
+        ], filters={
+            'id': self.job_id
+        })
 
-    async def login_to_registry(self):
+    async def login_to_registry(self) -> JobStepResult:
 
         self.metadata = JobMetadata(
             id=self.job_id,
             image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.AUTHORIZING.value,
             context=f'Job {self.job_id} authorizing to registry {self.registry.registry_uri}'
         )
 
-        await self.connection.update([
+        response = await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
+        if response.error:
+            self.error = response.error
+            return JobStepResult(
+                message='Job metadata update failed',
+                error=response.error
+            )
+
         await self.loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.client.api.login,
                 self.registry.registry_user,
                 password=self.registry.registry_password,
                 registry=self.registry.registry_uri,
                 reauth=True
             )
         )
 
-    async def assemble_context(self):
+        return JobStepResult(
+            message='Registry login succeeded'
+        )
+
+    async def assemble_context(self) -> JobStepResult:
 
         self.metadata = JobMetadata(
             id=self.job_id,
             image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.GENERATING.value,
             context=f'Job {self.job_id} generating image {self.image.full_name}'
         )
 
-        await self.connection.update([
+        response = await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
+        if response.error:
+            self.error = response.error
+            return JobStepResult(
+                message='Job metadata update failed',
+                error=response.error
+            )
+
         self.context = await self.loop.run_in_executor(
             self._executor,
             self.image.to_context
         )
 
+        return JobStepResult(
+            message='DCRX image successfully assembled'
+        )
 
-    async def build_image(self):
+    async def build_image(self) -> JobStepResult:
 
         self.metadata = JobMetadata(
             id=self.job_id,
             image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.BUILDING.value,
             context=f'Job {self.job_id} building image {self.image.full_name}'
         )
 
-        await self.connection.update([
+        response = await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
+        if response.error:
+            self.error = response.error
+            return JobStepResult(
+                message='Job metadata update failed',
+                error=response.error
+            )
+
         build_options: Dict[str, Any] = {}
 
         if self.build_options:
             build_options = self.build_options.dict()
 
         image_result = await self.loop.run_in_executor(
             self._executor,
@@ -249,91 +306,66 @@
             )   
         )
 
         image, _ = image_result 
         self.image_stats = ImageStats(
             size=int(image.attrs.get('Size', 0)/10**6)
         )
+
+        return JobStepResult(
+            message='Docker image successfully built'
+        )
         
-    async def push_image(self):
+    async def push_image(self) -> JobStepResult:
 
         self.metadata = JobMetadata(
             id=self.job_id,
             image_registry=self.registry.registry_uri,
             name=self.job_name,
             image=self.image.name,
             tag=self.image.tag,
             status=JobStatus.PUSHING.value,
             context=f'Job {self.job_id} pushing image {self.image.full_name} to registry {self.registry.registry_uri}',
             size=self.image_stats.size
         )
 
-        await self.connection.update([
+        response = await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
+        if response.error:
+            self.error = response.error
+            return JobStepResult(
+                message='Job metadata update failed',
+                error=response.error
+            )
+
         await self.loop.run_in_executor(
             self._executor,
             functools.partial(        
                 self.client.images.push,
                 self.image.name,
                 tag=self.image.tag
             )
         )
 
-    async def clear(self):
-
-        await self.loop.run_in_executor(
-            self._executor,
-            self.client.api.prune_builds
+        return JobStepResult(
+            message='Docker image successfully pushed'
         )
 
-        await self.loop.run_in_executor(
-            self._executor,
-            functools.partial(      
-                self.client.api.prune_images
-            )
-        )
-
-        for layer in self.image.layers:
-            if layer.layer_type == 'stage':
-
-                try:
-                    await self.loop.run_in_executor(
-                        self._executor,
-                        functools.partial(
-                            self.client.images.remove,
-                            f'{layer.base}:{layer.tag}'
-                        )
-                    )
-                
-                except Exception:
-                    pass
-
-        try:
-            await self.loop.run_in_executor(
-                self._executor,
-                functools.partial(
-                    self.client.images.remove,
-                    self.image.full_name
-                )
-            )
-
-        except Exception:
-            pass
 
-        await self.loop.run_in_executor(
-            self._executor,
-            self.image.clear
-        )
+    async def close(self):
 
+        self.shutdown = True
+        if self._executor and self._executor._shutdown:
+            self._executor = None
 
-    async def close(self):
+        await self._clear()
 
         if self.error is None:
             status = JobStatus.DONE
             context = f'Job {self.job_id} complete'
 
         elif self.metadata.status == JobStatus.CANCELLED.value:
             status = JobStatus.CANCELLED
@@ -357,27 +389,71 @@
 
         await self.connection.update([
             self.metadata
         ], filters={
             'id': self.job_id
         })
 
-        if self.client_closed is False:
-            await self.loop.run_in_executor(
-                None,
-                self.client.close
-            )
-            self.client_closed = True
+        await self.loop.run_in_executor(
+            None,
+            self.client.close
+        )
 
         if self.context:
             await self.loop.run_in_executor(
                 self._executor,
                 self.context.close
             )
 
+        if self._executor:
+            self._executor.shutdown(cancel_futures=True)
         
-        self._executor.shutdown(cancel_futures=True)
+    async def _clear(self):
+
+        try:
+            await self.loop.run_in_executor(
+                self._executor,
+                self.client.api.prune_builds
+            )
+
+            await self.loop.run_in_executor(
+                self._executor,
+                functools.partial(      
+                    self.client.api.prune_images
+                )
+            )
         
+        except APIError:
+            pass
+
+        for layer in self.image.layers:
+            if layer.layer_type == 'stage':
+
+                try:
+                    await self.loop.run_in_executor(
+                        self._executor,
+                        functools.partial(
+                            self.client.images.remove,
+                            f'{layer.base}:{layer.tag}'
+                        )
+                    )
+                
+                except ImageNotFound:
+                    pass
 
+        try:
+            await self.loop.run_in_executor(
+                self._executor,
+                functools.partial(
+                    self.client.images.remove,
+                    self.image.full_name
+                )
+            )
 
+        except ImageNotFound:
+            pass
 
+        await self.loop.run_in_executor(
+            self._executor,
+            self.image.clear
+        )
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,50 +10,58 @@
 from dcrx_api.env import Env
 from dcrx_api.env.time_parser import TimeParser
 from typing import (
     Dict, 
     Union,
     List
 )
+from .connection import JobsConnection
 from .job import Job
 from .models import (
     JobMetadata,
     JobNotFoundException,
     ServerLimitException
 )
 from .status import JobStatus
 
 
 class JobQueue:
 
-    def __init__(self, env: Env) -> None:
+    def __init__(
+        self, 
+        env: Env,
+        connection: JobsConnection
+    ) -> None:
 
         self.pool_size = env.DCRX_API_JOB_WORKERS
 
+        self._connection = connection
         self._jobs: Dict[uuid.UUID, Job] = {}
         self._active: Dict[uuid.UUID, asyncio.Task] = {}
         self.max_jobs = env.DCRX_API_JOB_POOL_SIZE
         self.max_pending_jobs = env.DCRX_API_JOB_MAX_PENDING
 
         self.active_jobs_count = 0
         self.pending_jobs_count = 0
-        self.pending_jobs: List[Job] = []
+        self.running_jobs = asyncio.Queue(maxsize=self.max_jobs)
+        self.pending_jobs = asyncio.Queue(maxsize=self.max_pending_jobs)
+
+        self.completed: List[asyncio.Task] = []
 
         self._executor = ThreadPoolExecutor(max_workers=env.DCRX_API_JOB_WORKERS)
 
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._job_max_age = TimeParser(env.DCRX_API_JOB_MAX_AGE).time
         self._job_prune_interval = TimeParser(env.DCRX_API_JOB_PRUNE_INTERVAL).time
         self._run_cleanup = True
         self.active_images: List[DockerImage] = []
-        self.cancelling: List[asyncio.Task] = []
         self.client = docker.DockerClient(
             max_pool_size=env.DCRX_API_JOB_WORKERS
         )
-        self.completed: List[str] = []
+
         self.loop = asyncio.get_event_loop()
 
     async def get_active_images(self) -> List[DockerImage]:
 
         active_statuses = [
             'AUTHORIZING',
             'CREATED',
@@ -102,36 +110,31 @@
                     stderr=subprocess.PIPE
                 )
             )
 
             self.active_images = await self.get_active_images()
 
             queue_jobs = dict(self._jobs)
+
+            pruneable_statuses = ['DONE', 'CANCELLED', 'FAILED']
             
             for job_id, job in queue_jobs.items():
                 
                 job_elapsed = time.monotonic() - job.job_start_time
-                job_is_pruneable = job.metadata.status in ['DONE', 'CANCELLED', 'FAILED']
+                job_is_pruneable = job.metadata.status in pruneable_statuses
 
-                if job.metadata.status == 'CANCELLED':
-                    self.cancelling.append(
+                if job.metadata.status in pruneable_statuses:
+                    self.completed.append(
                         asyncio.create_task(
-                            self._cancel_task(job)
+                            job.close()
                         )
                     )
 
                 if job_is_pruneable and job_elapsed > self._job_max_age:
 
-                    self.active_jobs_count -= 1
-                    if len(self.pending_jobs) > 0:
-                        pending_job = self.pending_jobs.pop()
-                        pending_job.waiter.set_result(None)
-                        
-                        self.pending_jobs_count -= 1
-
                     images = await self.loop.run_in_executor(
                         self._executor,
                         self.client.images.list,
                         job.image.name
                     )
 
                     if len(images) > 0:
@@ -144,52 +147,71 @@
 
                         except ImageNotFound:
                             pass
 
                     del self._jobs[job_id]
 
             
-            cancelling_tasks = list(self.cancelling)
-            for cancel_task in cancelling_tasks:
-                if cancel_task.done():
-                    self.cancelling.remove(cancel_task)
-            
-            await asyncio.sleep(self._job_prune_interval)
+            for _ in range(self.active_jobs_count):
+                job: Job = await self.running_jobs.get()
+                job_is_pruneable = job.metadata.status in pruneable_statuses
+
+                if job_is_pruneable is False:
+                    await self.running_jobs.put(job)
+
+                elif self.pending_jobs_count > 0:
+                    await self.running_jobs.put(
+                        await self.pending_jobs.get()
+                    )
+
+                    self.active_jobs_count = self.running_jobs.qsize()
+                    self.pending_jobs_count = self.pending_jobs.qsize()
+
+            for _ in range(self.pending_jobs_count):
+                job: Job = await self.pending_jobs.get()
+                job_is_pruneable = job.metadata.status in pruneable_statuses
 
-    async def _cancel_task(self, job: Job):
+                if job_is_pruneable is False:
+                    await self.pending_jobs.put(job)
 
-        job.client_closed = True
+            self.pending_jobs_count = self.pending_jobs.qsize()
 
-        await job.clear()
-        await job.close()
+
+            self.active_jobs_count = self.running_jobs.qsize()
+            
+            completed_tasks = list(self.completed)
+            for completed_task in completed_tasks:
+                if completed_task.done():
+                    self.completed.remove(completed_task)
+            
+            await asyncio.sleep(self._job_prune_interval)
 
     async def submit(self, job: Job) -> JobMetadata:
 
         if self.active_jobs_count >= self.max_jobs and self.pending_jobs_count < self.max_pending_jobs:
             job.waiter = asyncio.Future()
+            await self.pending_jobs.put(job)
+            self.pending_jobs_count = self.pending_jobs.qsize()
 
         elif self.active_jobs_count >= self.max_jobs:
             return ServerLimitException(
                 message='Pending jobs quota reached. Please try again later.',
                 limit=self.max_pending_jobs,
                 current=self.pending_jobs_count
             )
-
-        self._jobs[job.job_id] = job
-
+        
+        else:
+            await self.running_jobs.put(job)
+            self.active_jobs_count = self.running_jobs.qsize()
+        
         self._active[job.job_id] = asyncio.create_task(
             job.run()
         )
 
-        if job.waiter:
-            self.pending_jobs.append(job)
-            self.pending_jobs_count += 1
-
-        else:
-            self.active_jobs_count += 1
+        self._jobs[job.job_id] = job
 
         return job.metadata
 
     def get(self, job_id: uuid.UUID) -> Union[JobMetadata, JobNotFoundException]:
         job = self._jobs.get(job_id)
         if job is None:
             return JobNotFoundException(
@@ -251,18 +273,38 @@
         await self._cleanup_task
 
         await self.loop.run_in_executor(
             self._executor,
             self.client.close
         )
 
-        for job in self._active.values():
-            if not job.done():
-                job.cancel()
-
-        for job in self._jobs.values():
-            if job.client_closed is False:
-                await job.close()
+        cancel_jobs: List[Job] = []
+        for _ in range(self.pending_jobs_count):
+            job: Job = await self.pending_jobs.get()
+            if job.shutdown is False:
+                cancel_jobs.append(job)
+
+            await asyncio.gather(*[
+                asyncio.create_task(
+                    job.close()
+                ) for job in cancel_jobs
+            ])
+
+        cancel_jobs: List[Job] = []
+        for _ in range(self.active_jobs_count):
+            job: Job = await self.running_jobs.get()
+            if job.shutdown is False:
+                cancel_jobs.append(job)
+            
+            await asyncio.gather(*[
+                asyncio.create_task(
+                    job.close()
+                ) for job in cancel_jobs
+            ])
+        
+        for job_task in self._active.values():
+            if not job_task.done():
+                job_task.cancel()
 
-        self._executor.shutdown(cancel_futures=True)
+        self._executor.shutdown()
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/service.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import uuid
 from dcrx import Image
 from dcrx_api.context.manager import context, ContextType
+from dcrx_api.database.models import DatabaseTransactionResult
 from dcrx_api.services.registry.context import RegistryServiceContext
 from dcrx_api.services.registry.models import Registry, RegistryNotFoundException
 from fastapi import APIRouter, HTTPException
 from dcrx.layers import (
     Add,
     Arg,
     Cmd,
@@ -59,14 +60,17 @@
     responses={
         404: {
             'model': RegistryNotFoundException
         },
         429: {
             'model': ServerLimitException
         },
+        500: {
+            "model": DatabaseTransactionResult
+        }
     }
 )
 async def create_job(new_image: NewImage) -> JobMetadata:
 
     job_service_context = context.get(ContextType.JOB_SERVICE)
     monitoring_service_context = context.get(ContextType.MONITORING_SERVICE)
     registry_service_context: RegistryServiceContext = context.get(ContextType.REGISTRY_SERVICE)
@@ -75,27 +79,32 @@
     if monitoring_service_context.exceeded_memory_limit:
         raise HTTPException(429, detail={
             "message": "Will not schedule job - memory limit exceeded.",
             "limit": monitoring_service_context.env.DCRX_API_MAX_MEMORY_PERCENT_USAGE,
             "current": monitoring_service_context.get_memory_usage_pct()
         })
     
-    registries = await registry_service_context.connection.select(
+    response = await registry_service_context.connection.select(
         filters={
             'registry_name': new_image.registry.registry_name
         }
     )
 
-    if len(registries) < 1:
-
+    if response.data is None or len(response.data) < 1:
         raise HTTPException(404, detail={
             "message": "Registry not found."
         })
+    
+    elif response.error:
+        raise HTTPException(500, detail={
+            "message": response.message,
+            "error": response.error
+        })
         
-    registry = registries.pop()
+    registry = response.data.pop()
 
     dcrx_image = Image(
         new_image.name,
         tag=new_image.tag
     )
 
     layers: Layer = new_image.layers
@@ -138,14 +147,15 @@
             registry_uri=registry.registry_uri,
             registry_user=registry.registry_user,
             registry_password=decrypted_password
         ),
         build_options=new_image.build_options,
         pool_size=job_service_context.queue.pool_size,
         timeout=job_service_context.env.DCRX_API_JOB_TIMEOUT,
+        wait_timeout=job_service_context.env.DCRX_API_JOB_MAX_PENDING_WAIT
     )
 
     response = await job_service_context.queue.submit(job)
 
     if isinstance(response, ServerLimitException):
         raise HTTPException(429, detail={
             "message": response.message,
@@ -158,37 +168,46 @@
 
 
 @jobs_router.get(
     "/jobs/images/{job_id}/get",
     responses={
         404: {
             "model": JobNotFoundException
+        },
+        500: {
+            "model": DatabaseTransactionResult
         }
     }
 )
 async def get_job(job_id: str) -> JobMetadata:
 
     job_service_context = context.get(ContextType.JOB_SERVICE)
 
     retrieved_job = job_service_context.queue.get(
         uuid.UUID(job_id)
     )
 
     if isinstance(retrieved_job, JobNotFoundException):
 
-        retrieved_jobs = await job_service_context.connection.select(
+        response = await job_service_context.connection.select(
             filters={
                 'id': job_id
             }
         )
 
-        if len(retrieved_jobs) < 1:
+        if response.data is None or len(response.data) < 1:
             raise HTTPException(404, detail=retrieved_job.message)
         
-        job = retrieved_jobs.pop()
+        elif response.error:
+            raise HTTPException(500, detail={
+                "message": response.message,
+                "error": response.error
+            })
+        
+        job = response.data.pop()
 
         retrieved_job = JobMetadata(
             id=job.id,
             image_registry=job.image_registry,
             name=job.name,
             image=job.image,
             tag=job.tag,
@@ -201,14 +220,17 @@
 
 
 @jobs_router.delete(
     "/jobs/images/{job_id}/cancel",
     responses={
         404: {
             "model": JobNotFoundException
+        },
+        500: {
+            "model": DatabaseTransactionResult
         }
     }
 )
 async def cancel_job(job_id: str) -> JobMetadata:
 
     job_service_context = context.get(ContextType.JOB_SERVICE)
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,50 +12,50 @@
     Any,
     Union,
     Callable,
     Optional,
     TypeVar,
     Generic
 )
-from .jobs_mysql_table import JobsMySQLTable
-from .jobs_postgres_table import JobsPostgresTable
-from .jobs_sqlite_table import JobsSQLiteTable
+from .registry_mysql_table import RegistryMySQLTable
+from .registry_postgres_table import RegistryPostgresTable
+from .registry_sqlite_table import RegistrySQLiteTable
 
 M = TypeVar('M', bound=BaseModel)
 
-class JobsTable(Generic[M]):
+class RegistryTable(Generic[M]):
 
     def __init__(
         self,
         users_table_name: str,
         database_type: Literal["mysql", "postgres", "sqlite"]="sqlite"
     ) -> None:
         self._table_types: Dict[
             Literal["mysql", "postgres", "sqlite"],
             Callable[
                 [str],
                 Union[
-                    JobsMySQLTable,
-                    JobsPostgresTable,
-                    JobsSQLiteTable
+                    RegistryMySQLTable,
+                    RegistryPostgresTable,
+                    RegistrySQLiteTable
                 ]
             ]
         ] = {
-            'mysql': lambda table_name: JobsMySQLTable(table_name),
-            'postgres': lambda table_name: JobsPostgresTable(table_name),
-            'sqlite': lambda table_name: JobsSQLiteTable(table_name)
+            'mysql': lambda table_name: RegistryMySQLTable(table_name),
+            'postgres': lambda table_name: RegistryPostgresTable(table_name),
+            'sqlite': lambda table_name: RegistrySQLiteTable(table_name)
         }
 
         self.selected: Union[
-            JobsMySQLTable,
-            JobsPostgresTable,
-            JobsSQLiteTable
+            RegistryMySQLTable,
+            RegistryPostgresTable,
+            RegistrySQLiteTable
         ] = self._table_types.get(
             database_type,
-            JobsMySQLTable
+            RegistryMySQLTable
         )(users_table_name)
 
     def select(
         self, 
         filters: Optional[Dict[str, Any]]={}
     ) -> Select:
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/monitoring/base/monitor.py` & `dcrx-api-0.4.0/dcrx_api/services/monitoring/base/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/monitoring/context.py` & `dcrx-api-0.4.0/dcrx_api/services/monitoring/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/monitor.py` & `dcrx-api-0.4.0/dcrx_api/services/monitoring/memory/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/registry/connection.py` & `dcrx-api-0.4.0/dcrx_api/services/registry/connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dcrx_api.database import (
     DatabaseConnection,
     ConnectionConfig
 )
+from dcrx_api.database.models import DatabaseTransactionResult
 from dcrx_api.env import Env
 from typing import (
     List,
     Dict,
     Any
 )
 from .models import Registry
@@ -18,72 +19,73 @@
         super().__init__(
             ConnectionConfig(
                 database_username=env.DCRX_API_DATABASE_USER,
                 database_password=env.DCRX_API_DATABASE_PASSWORD,
                 database_type=env.DCRX_API_DATABASE_TYPE,
                 database_uri=env.DCRX_API_DATABASE_URI,
                 database_port=env.DCRX_API_DATABASE_PORT,
-                database_name=env.DCRX_API_DATABASE_NAME
+                database_name=env.DCRX_API_DATABASE_NAME,
+                database_transaction_retries=env.DCRX_API_DATABASE_TRANSACTION_RETRIES
             )
         )
 
         self.table: RegistryTable[Registry] = RegistryTable(
             'registries',
             database_type=self.config.database_type
         )
 
-    async def init(self):
+    async def init(self) -> DatabaseTransactionResult[Registry]:
         return await self.create_table(self.table.selected.table)
 
     async def select(
         self, 
         filters: Dict[str, Any]={}
-    ):
+    ) -> DatabaseTransactionResult[Registry]:
         return await self.get(
             self.table.select(
                 filters={
                     name: self.table.selected.types_map.get(
                         name
                     )(value) for name, value in filters.items()
                 }
             )
         )
 
     async def create(
         self, 
         registries: List[Registry]
-    ):
+    ) -> DatabaseTransactionResult[Registry]:
        return await self.insert_or_update(
            self.table.insert(registries)
        )
     
     async def update(
         self, 
         registries: List[Registry],
         filters: Dict[str, Any]={}
-    ):
+    ) -> DatabaseTransactionResult[Registry]:
         return await self.insert_or_update(
             self.table.update(
                 registries,
                 filters={
                     name: self.table.selected.types_map.get(
                         name
                     )(value) for name, value in filters.items()
                 }
             )
         )
     
     async def remove(
         self,
         filters: Dict[str, Any]
-    ):
+    ) -> DatabaseTransactionResult[Registry]:
         return await self.delete([
             self.table.delete({
                 name: self.table.selected.types_map.get(
                     name
                 )(value) for name, value in filters.items()
             })
         ])
     
-    async def drop(self):
+    async def drop(self) -> DatabaseTransactionResult[Registry]:
         return await self.drop_table(self.table)
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/registry/context.py` & `dcrx-api-0.4.0/dcrx_api/services/registry/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/registry/service.py` & `dcrx-api-0.4.0/dcrx_api/services/registry/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import uuid
 from dcrx_api.services.auth.models import AuthenticationFailureException
 from dcrx_api.context.manager import context, ContextType
+from dcrx_api.database.models import DatabaseTransactionResult
 from fastapi import APIRouter, HTTPException
 from typing import Literal
 from .context import RegistryServiceContext
 from .models import (
     RegistryMetadata,
     RegistryNotFoundException,
     Registry,
@@ -18,14 +19,17 @@
     '/registry/{registry_id_or_name}/get',
     responses={
         401: {
             "model": AuthenticationFailureException
         },
         404: {
             "model": RegistryNotFoundException
+        },
+        500: {
+            "model": DatabaseTransactionResult
         }
     }
 )
 async def get_registry(
     registry_id_or_name: str, 
     match_by: Literal["id", "registry_uri"]="id"
 ) -> RegistryTransactionSuccessResponse:
@@ -37,105 +41,138 @@
     }
 
     if match_by == 'registry_uri':
         filters = {
             'registry_uri': registry_id_or_name
         }
 
-    registries = await registry_service_context.connection.select(
+    response = await registry_service_context.connection.select(
         filters=filters
     )
 
-    if len(registries) < 1:
+    if len(response.data) < 1:
         raise HTTPException(404, detail=f'Registry {registry_id_or_name} not found.')
     
-    registry = registries.pop()
+    elif response.error:
+        raise HTTPException(500, detail={
+            "message": response.message,
+            "error": response.error
+        })
+    
+    registry = response.data.pop()
     
     return RegistryTransactionSuccessResponse(
         id=registry.id,
         registry_name=registry.registry_name,
     )
 
 
 @registry_router.post(
     '/registry/create',
     status_code=201,
     responses={
         401: {
             "model": AuthenticationFailureException
+        },
+        500: {
+            "model": DatabaseTransactionResult
         }
     }
 )
 async def create_registry(registry: RegistryMetadata) -> RegistryTransactionSuccessResponse:
 
     registry_service_context: RegistryServiceContext = context.get(ContextType.REGISTRY_SERVICE)
     auth_service_context = context.get(ContextType.AUTH_SERVICE)
 
     hashed_password = await auth_service_context.manager.encrypt_fernet(
         registry.registry_password
     )
 
     new_registry_id = uuid.uuid4()
-    await registry_service_context.connection.create([
+    response = await registry_service_context.connection.create([
         Registry(
             id=new_registry_id,
             registry_name=registry.registry_name,
             registry_uri=registry.registry_uri,
             registry_user=registry.registry_user,
             registry_password=hashed_password
         )
     ])
 
+    if response.error:
+        raise HTTPException(500, detail={
+            "message": response.message,
+            "error": response.error
+        })
+
     return RegistryTransactionSuccessResponse(
         id=new_registry_id,
         registry_name=registry.registry_name,
         message='Successfully created'
     )
 
 
 @registry_router.put(
     '/registry/update',
     status_code=202,
     responses={
         401: {
             "model": AuthenticationFailureException
+        },
+        500: {
+            "model": DatabaseTransactionResult
         }
     }
 )
 async def update_registry(registry: Registry) -> RegistryTransactionSuccessResponse:
 
     registry_service_context: RegistryServiceContext = context.get(ContextType.REGISTRY_SERVICE)
 
-    await registry_service_context.connection.update([
+    response = await registry_service_context.connection.update([
         registry
     ])
 
+    if response.error:
+        raise HTTPException(500, detail={
+            "message": response.message,
+            "error": response.error
+        })
+
     return RegistryTransactionSuccessResponse(
         id=registry.id,
         registry_name=registry.registry_name,
         message='Successfully updated'
     )
 
 
 @registry_router.delete(
     '/registry/{registry_id}/delete',
     status_code=200,
     responses={
         401: {
             "model": AuthenticationFailureException
+        },
+        500: {
+            "model": DatabaseTransactionResult
         }
     }
 )
 async def delete_registry(registry_id: str) -> RegistryTransactionSuccessResponse:
 
     registry_service_context: RegistryServiceContext = context.get(ContextType.REGISTRY_SERVICE)
 
-    await registry_service_context.connection.remove(
+    response = await registry_service_context.connection.remove(
         filters={
             'id': registry_id
         }
     )
 
+    if response.error:
+        raise HTTPException(500, detail={
+            "message": response.message,
+            "error": response.error
+        })
+
     return RegistryTransactionSuccessResponse(
         id=registry_id,
         message='Successfully deleted'
     )
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_mysql_table.py` & `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_postgres_table.py` & `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_sqlite_table.py` & `dcrx-api-0.4.0/dcrx_api/services/registry/table/registry_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_table.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,68 +10,82 @@
     Dict, 
     List,
     Any,
     Union,
     Callable,
     Optional,
     TypeVar,
-    Generic
+    Generic,
+    Tuple
 )
-from .registry_mysql_table import RegistryMySQLTable
-from .registry_postgres_table import RegistryPostgresTable
-from .registry_sqlite_table import RegistrySQLiteTable
+from .jobs_mysql_table import JobsMySQLTable
+from .jobs_postgres_table import JobsPostgresTable
+from .jobs_sqlite_table import JobsSQLiteTable
 
 M = TypeVar('M', bound=BaseModel)
 
-class RegistryTable(Generic[M]):
+class JobsTable(Generic[M]):
 
     def __init__(
         self,
         users_table_name: str,
         database_type: Literal["mysql", "postgres", "sqlite"]="sqlite"
     ) -> None:
         self._table_types: Dict[
             Literal["mysql", "postgres", "sqlite"],
             Callable[
                 [str],
                 Union[
-                    RegistryMySQLTable,
-                    RegistryPostgresTable,
-                    RegistrySQLiteTable
+                    JobsMySQLTable,
+                    JobsPostgresTable,
+                    JobsSQLiteTable
                 ]
             ]
         ] = {
-            'mysql': lambda table_name: RegistryMySQLTable(table_name),
-            'postgres': lambda table_name: RegistryPostgresTable(table_name),
-            'sqlite': lambda table_name: RegistrySQLiteTable(table_name)
+            'mysql': lambda table_name: JobsMySQLTable(table_name),
+            'postgres': lambda table_name: JobsPostgresTable(table_name),
+            'sqlite': lambda table_name: JobsSQLiteTable(table_name)
         }
 
         self.selected: Union[
-            RegistryMySQLTable,
-            RegistryPostgresTable,
-            RegistrySQLiteTable
+            JobsMySQLTable,
+            JobsPostgresTable,
+            JobsSQLiteTable
         ] = self._table_types.get(
             database_type,
-            RegistryMySQLTable
+            JobsMySQLTable
         )(users_table_name)
 
     def select(
         self, 
-        filters: Optional[Dict[str, Any]]={}
+        filters: Optional[Dict[str, Union[Any, Tuple[Any, ...]]]]={}
     ) -> Select:
 
         select_clause: Select = self.selected.table.select()
 
         if filters:
-            for field_name, value in filters.items():
-                select_clause = select_clause.where(
-                    self.selected.columns.get(field_name) == self.selected.types_map.get(
-                        field_name
-                    )(value)
-                )
+            for field_name, values in filters.items():
+
+                if isinstance(values, tuple):
+                    select_clause = select_clause.where(
+                        self.selected.columns.get(field_name).in_(
+                            tuple([
+                                self.selected.types_map.get(
+                                    field_name
+                                )(value) for value in values
+                            ])
+                        ))
+
+                else:
+
+                    select_clause = select_clause.where(
+                        self.selected.columns.get(field_name) == self.selected.types_map.get(
+                            field_name
+                        )(values)
+                    )
 
         return select_clause
     
     def insert(
         self,
         jobs: List[M]
     ) -> List[Insert]:
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/users/connection.py` & `dcrx-api-0.4.0/dcrx_api/services/jobs/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 from dcrx_api.database import (
     DatabaseConnection,
     ConnectionConfig
 )
+from dcrx_api.database.models import DatabaseTransactionResult
 from dcrx_api.env import Env
 from typing import (
     List,
     Dict,
-    Any
+    Any,
+    Union,
+    Tuple
 )
-from .models import DBUser
-from .table import UsersTable
+from .models import JobMetadata
+from .status import JobStatus
+from .table import JobsTable
 
 
-class UsersConnection(DatabaseConnection[DBUser]):
+class JobsConnection(DatabaseConnection[JobMetadata]):
 
     def __init__(self, env: Env) -> None:
         super().__init__(
             ConnectionConfig(
                 database_username=env.DCRX_API_DATABASE_USER,
                 database_password=env.DCRX_API_DATABASE_PASSWORD,
                 database_type=env.DCRX_API_DATABASE_TYPE,
                 database_uri=env.DCRX_API_DATABASE_URI,
                 database_port=env.DCRX_API_DATABASE_PORT,
-                database_name=env.DCRX_API_DATABASE_NAME
+                database_name=env.DCRX_API_DATABASE_NAME,
+                database_transaction_retries=env.DCRX_API_DATABASE_TRANSACTION_RETRIES
             )
         )
 
-        self.table: UsersTable[DBUser] = UsersTable(
-            'users',
+        self.table: JobsTable[JobMetadata] = JobsTable(
+            'jobs',
             database_type=self.config.database_type
         )
 
-    async def init(self):
+    async def init(self) -> DatabaseTransactionResult[JobMetadata]:
         return await self.create_table(self.table.selected.table)
 
     async def select(
         self, 
-        filters: Dict[str, Any]={}
-    ):
+        filters: Dict[str, Union[Any, Tuple[Any, ...]]]={}
+    ) -> DatabaseTransactionResult[JobMetadata]:
         return await self.get(
             self.table.select(
-                filters={
-                    name: self.table.selected.types_map.get(
-                        name
-                    )(value) for name, value in filters.items()
-                }
+                filters=filters
             )
         )
-
+    
     async def create(
         self, 
-        users: List[DBUser]
-    ):
+        jobs: List[JobMetadata]
+    ) -> DatabaseTransactionResult[JobMetadata]:
        return await self.insert_or_update(
-           self.table.insert(users)
+           self.table.insert(jobs)
        )
     
     async def update(
         self, 
-        users: List[DBUser],
+        jobs: List[JobMetadata],
         filters: Dict[str, Any]={}
-    ):
+    ) -> DatabaseTransactionResult[JobMetadata]:
         return await self.insert_or_update(
             self.table.update(
-                users,
+                jobs,
                 filters={
                     name: self.table.selected.types_map.get(
                         name
                     )(value) for name, value in filters.items()
                 }
             )
         )
     
     async def remove(
         self,
         filters: Dict[str, Any]
-    ):
+    ) -> DatabaseTransactionResult[JobMetadata]:
         return await self.delete([
             self.table.delete({
                 name: self.table.selected.types_map.get(
                     name
                 )(value) for name, value in filters.items()
             })
         ])
     
-    async def drop(self):
+    async def drop(self) -> DatabaseTransactionResult[JobMetadata]:
         return await self.drop_table(self.table)
```

### Comparing `dcrx-api-0.3.1/dcrx_api/services/users/context.py` & `dcrx-api-0.4.0/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.4.0/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.4.0/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.4.0/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.4.0/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.1/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.4.0/dcrx_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.3.1
+Version: 0.4.0
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -45,32 +45,38 @@
 
 
 # Getting Started
 
 DCRX-API requires a slew of environmental variables in order to run correctly. These include:
 
 ```
-DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled.
+DCRX_API_JOB_TIMEOUT=10m # The maximum amount of time before an image build + push job times out and is cancelled. Default is 10 minutes.
 
-DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error.
+DCRX_API_MAX_MEMORY_PERCENT_USAGE=50 # The percent of system memory DCRX-API and Docker image builds created by DCRX-API can use. If exceeded, new jobs will be rejected and requests will return a 400 error. Default is 50 percent.
 
 DCRX_API_JOB_PRUNE_INTERVAL='1s' # How often dcrx-api checks for done, failed, or cancelled jobs to remove from in-memory storage.
 
 DCRX_API_JOB_MAX_AGE='1m'= # Time before done, failed, or cancelled jobs are pruned from in-memory storage.
 
+DCRX_API_JOB_MAX_PENDING_WAIT=10m # The maximum amount of time a job can remain in PENDING status. Jobs that exceed this threshold are timed out and will fail.
+
+DCRX_API_JOB_MAX_PENDING=100 # The maximum number of pending jobs that a single instance of DCRX-API allows. Default is 100.
+
 DCRX_API_JOB_POOL_SIZE=10 # Maximum number of concurrent builds. Default is 10.
 
 DCRX_API_JOB_WORKERS=4 # Number of workers to use per-job. Default is the number os OS threads.
 
 DCRX_API_TOKEN_EXPIRATION='15m' # Time for JWT authorization token to expire. Default is 15 minutes.
 
 DCRX_API_SECRET_KEY=testingthis # Initial secret used to hash user passwords.
 
 DCRX_API_AUTH_ALGORITHM=HS256 # Algorithm to use for hashing user passwords.
 
+DCRX_API_DATABASE_TRANSACTION_RETRIES=3 # Number of times to retry a failed transaction. Default is 3.
+
 DCRX_API_DATABASE_TYPE=sqlite # Type of database to use. Default is sqlite and options are mysql, asyncpg, and sqlite.
 
 DCRX_API_DATABASE_USER=admin # Username used for database connection authentication
 
 DCRX_API_DATABASE_PASSWORD=test1234 # Password used for database connection authentrication
 
 DCRX_API_DATABASE_NAME=dcrx # Name of database to use for storing users. Default is dcrx.
```

### Comparing `dcrx-api-0.3.1/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.4.0/dcrx_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 dcrx_api/context/__init__.py
 dcrx_api/context/manager.py
 dcrx_api/context/types.py
 dcrx_api/database/__init__.py
 dcrx_api/database/connection.py
 dcrx_api/database/connection_config.py
 dcrx_api/database/table_types.py
+dcrx_api/database/models/__init__.py
+dcrx_api/database/models/database_transaction_result.py
 dcrx_api/env/__init__.py
 dcrx_api/env/env.py
 dcrx_api/env/load_env.py
 dcrx_api/env/time_parser.py
 dcrx_api/middleware/__init__.py
 dcrx_api/middleware/auth_middleware.py
 dcrx_api/services/__init__.py
@@ -45,14 +47,15 @@
 dcrx_api/services/jobs/status.py
 dcrx_api/services/jobs/models/__init__.py
 dcrx_api/services/jobs/models/build_options.py
 dcrx_api/services/jobs/models/image_stats.py
 dcrx_api/services/jobs/models/job_metadata.py
 dcrx_api/services/jobs/models/job_not_found_exception.py
 dcrx_api/services/jobs/models/job_registry.py
+dcrx_api/services/jobs/models/job_step_result.py
 dcrx_api/services/jobs/models/new_image.py
 dcrx_api/services/jobs/models/remote_add.py
 dcrx_api/services/jobs/models/server_limit_exception.py
 dcrx_api/services/jobs/table/__init__.py
 dcrx_api/services/jobs/table/jobs_mysql_table.py
 dcrx_api/services/jobs/table/jobs_postgres_table.py
 dcrx_api/services/jobs/table/jobs_sqlite_table.py
```

### Comparing `dcrx-api-0.3.1/setup.py` & `dcrx-api-0.4.0/setup.py`

 * *Files identical despite different names*

