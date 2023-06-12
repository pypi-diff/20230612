# Comparing `tmp/dcrx-api-0.3.0.tar.gz` & `tmp/dcrx-api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-api-0.3.0.tar", last modified: Mon Jun 12 07:30:53 2023, max compression
+gzip compressed data, was "dcrx-api-0.3.1.tar", last modified: Mon Jun 12 15:19:28 2023, max compression
```

## Comparing `dcrx-api-0.3.0.tar` & `dcrx-api-0.3.1.tar`

### file list

```diff
@@ -1,127 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/cli/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/context/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/context/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/connection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/database/table_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/env/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/lifespan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/middleware/auth_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/auth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/authentication_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/auth/models/generated_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/jobs/models/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/build_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/image_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/job_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/job_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/new_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/remote_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/models/server_memory_limit_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/jobs/table/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/base/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/cpu/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.702015 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/docker_memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/registry/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/models/registry_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/registry/table/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_sqlite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/users/models/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/authorized_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/base_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/login_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/updated_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/user_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/models/user_transaction_success_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/dcrx_api/services/users/table/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_mysql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_postgres_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_sqllite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/dcrx_api/services/users/table/users_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:30:53.698015 dcrx-api-0.3.0/dcrx_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 07:30:53.000000 dcrx-api-0.3.0/dcrx_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 07:30:53.706015 dcrx-api-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-12 07:30:40.000000 dcrx-api-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/cli/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/context/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/context/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/database/table_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/env/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/lifespan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/middleware/auth_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api/services/auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/auth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/authentication_failure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/auth/models/generated_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/jobs/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/build_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/image_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/job_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/job_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/new_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/remote_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/models/server_limit_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/jobs/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/base/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/cpu/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.382258 dcrx-api-0.3.1/dcrx_api/services/registry/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/models/registry_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/registry/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_sqlite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/users/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/authorized_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/base_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/login_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/updated_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/user_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/models/user_transaction_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/dcrx_api/services/users/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_mysql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_postgres_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_sqllite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/dcrx_api/services/users/table/users_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:19:28.378257 dcrx-api-0.3.1/dcrx_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 15:19:28.000000 dcrx-api-0.3.1/dcrx_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:19:28.386258 dcrx-api-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-12 15:19:25.000000 dcrx-api-0.3.1/setup.py
```

### Comparing `dcrx-api-0.3.0/LICENSE` & `dcrx-api-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/PKG-INFO` & `dcrx-api-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.3.0/README.md` & `dcrx-api-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/cli/base.py` & `dcrx-api-0.3.1/dcrx_api/cli/base.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/cli/database.py` & `dcrx-api-0.3.1/dcrx_api/cli/database.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/cli/server.py` & `dcrx-api-0.3.1/dcrx_api/cli/server.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/context/manager.py` & `dcrx-api-0.3.1/dcrx_api/context/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/database/connection.py` & `dcrx-api-0.3.1/dcrx_api/database/connection.py`

 * *Files 27% similar despite different names*

```diff
@@ -97,68 +97,100 @@
 
     async def connect(self):
         self.loop = asyncio.get_event_loop()    
 
         if self.engine is None:
             self.setup()
 
-        self.connection = await self.engine.connect()
-
     async def create_table(
         self,
         table: Table
     ):
-        await self.connection.execute(
-            CreateTable(
-                table,
-                if_not_exists=True
-            )
-        )
+        async with self.engine.connect() as connection:
+            try:
+                await connection.execute(
+                    CreateTable(
+                        table,
+                        if_not_exists=True
+                    )
+                )
+
+            except Exception:
+                await connection.rollback()
 
-        await self.connection.commit()
+            await connection.commit()
 
     async def get(
         self, 
         statement: Select
     ) -> List[T]:
-        results = await self.connection.execute(statement)
+        
+        results: List[T] = []
+
+        async with self.engine.connect() as connection:
+            
+            try:
+                results = await connection.execute(statement)
+            
+            except Exception:
+                await connection.rollback()
+
         return [
             row for row in results
-        ]
+        ] 
     
     async def insert_or_update(
         self,
         statements: List[
             Union[Insert, Update]
         ]
     ):
         
-        for statement in statements:
-            await self.connection.execute(statement)
-        
-        await self.connection.commit()
+        async with self.engine.connect() as connection:
+            try:
+                for statement in statements:
+                    await connection.execute(statement)
+
+            except Exception:
+                await connection.rollback()
+            
+
+            await connection.commit()
+
 
     async def delete(
         self,
         statements: List[Delete]
     ):
+        async with self.engine.connect() as connection:
 
-        for statement in statements:
-            await self.connection.execute(statement)
+            try:
+                for statement in statements:
+                    await connection.execute(statement)
+
+            except Exception:
+                await connection.rollback()
         
-        await self.connection.commit()
+            await connection.commit()
 
     async def drop_table(
         self,
         table: Table
     ):
-        await self.connection.execute(
-            DropTable(
-                table,
-                if_exists=True
-            )
-        )
+        async with self.engine.connect() as connection:
+            
+            try:
+                await connection.execute(
+                    DropTable(
+                        table,
+                        if_exists=True
+                    )
+                )
+
+            except Exception:
+                await connection.rollback()
 
-        await self.connection.commit()
+            await connection.commit()
     
     async def close(self):
-        await self.connection.close()
+        if self.connection:
+            await self.connection.close()
```

### Comparing `dcrx-api-0.3.0/dcrx_api/env/env.py` & `dcrx-api-0.3.1/dcrx_api/env/env.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class Env(BaseModel):
     DCRX_API_MAX_MEMORY_PERCENT_USAGE: StrictFloat=50
     DCRX_API_JOB_TIMEOUT: StrictStr='5s'
     DCRX_API_JOB_PRUNE_INTERVAL: StrictStr='1s'
     DCRX_API_JOB_MAX_AGE: StrictStr='1m'
     DCRX_API_JOB_WORKERS: StrictInt=psutil.cpu_count()
+    DCRX_API_JOB_MAX_PENDING: StrictInt=100
     DCRX_API_JOB_POOL_SIZE: StrictInt=10
     DCRX_API_SECRET_KEY: StrictStr
     DCRX_API_AUTH_ALGORITHM: StrictStr='HS256'
     DCRX_API_TOKEN_EXPIRATION: StrictStr='15m'
     DCRX_API_DATABASE_TYPE: Optional[StrictStr]='sqlite'
     DCRX_API_DATABASE_USER: Optional[StrictStr]
     DCRX_API_DATABASE_URI: Optional[StrictStr]
@@ -37,14 +38,15 @@
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
             'DCRX_API_MAX_MEMORY_PERCENT_USAGE': float,
             'DCRX_API_JOB_PRUNE_INTERVAL': str,
             'DCRX_API_JOB_TIMEOUT': str,
             'DCRX_API_JOB_MAX_AGE': str,
             'DCRX_API_JOB_WORKERS': int,
+            'DCRX_API_JOB_MAX_PENDING': int,
             'DCRX_API_JOB_POOL_SIZE': int,
             'DCRX_API_SECRET_KEY': str,
             'DCRX_API_AUTH_ALGORITHM': str,
             'DCRX_API_TOKEN_EXPIRATION': str,
             'DCRX_API_DATABASE_TYPE': str,
             'DCRX_API_DATABASE_USER': str,
             'DCRX_API_DATABASE_PASSWORD': str,
```

### Comparing `dcrx-api-0.3.0/dcrx_api/env/load_env.py` & `dcrx-api-0.3.1/dcrx_api/env/load_env.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/env/time_parser.py` & `dcrx-api-0.3.1/dcrx_api/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/lifespan.py` & `dcrx-api-0.3.1/dcrx_api/lifespan.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 )
 from dcrx_api.services.users.context import (
     UsersConnection,
     UsersServiceContext
 )
 from dcrx_api.services.monitoring.context import (
     CPUMonitor,
-    DockerMemoryMonitor,
     MemoryMonitor,
     MonitoringServiceContext
 )
 from dcrx_api.services.registry.context import (
     RegistryConnection,
     RegistryServiceContext
 )
@@ -44,18 +43,14 @@
         connection=JobsConnection(env)
     )
 
     monitoring_service_context = MonitoringServiceContext(
         env=env,
         monitor_name='dcrx.main',
         cpu=CPUMonitor(),
-        docker_memory=DockerMemoryMonitor(
-            env,
-            job_service_context.queue
-        ),
         memory=MemoryMonitor()
     )
 
     registry_service_context = RegistryServiceContext(
         env=env,
         connection=RegistryConnection(env)
     )
```

### Comparing `dcrx-api-0.3.0/dcrx_api/middleware/auth_middleware.py` & `dcrx-api-0.3.1/dcrx_api/middleware/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/auth/manager.py` & `dcrx-api-0.3.1/dcrx_api/services/auth/manager.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/connection.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/context.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/job.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,46 @@
         self.job_image_label = f'{dcrx_api_label.name}={dcrx_api_label.value}'
         
         self.job_start_time = time.monotonic()
         self.timeout = TimeParser(timeout).time
 
         self.image_stats = ImageStats()
         self.client_closed = False
+        self.waiter: Union[asyncio.Future, None]=None
 
     async def list(self) -> List[DockerImage]:
         return await self.loop.run_in_executor(
             self._executor,
             functools.partial(
                 self.client.images.list,
                 self.image.name
             )
         )
     
     async def run(self):
+
+
+        if self.waiter:
+            self.metadata = JobMetadata(
+                id=self.job_id,
+                image_registry=self.registry.registry_uri,
+                name=self.job_name,
+                image=self.image.name,
+                tag=self.image.tag,
+                status=JobStatus.PENDING.value,
+                context=f'Job {self.job_id} pending'
+            )
+
+            await self.connection.update([
+                self.metadata
+            ], filters={
+                'id': self.job_id
+            })
+            await self.waiter
+
         try:
             await asyncio.wait_for(
                 asyncio.create_task(
                     self._run(),
                 ),
                 timeout=self.timeout
             )
@@ -118,14 +139,15 @@
                 'id': self.job_id
             })
 
             await self.clear()
             await self.close()
   
     async def _run(self):
+
         await self.connection.create([
             self.metadata
         ])
 
         try:
             await self.login_to_registry()
             await self.assemble_context()
```

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/models/new_image.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/models/new_image.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/queue.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import asyncio
 import docker
 import functools
 import subprocess
 import time
 import uuid
 from concurrent.futures import ThreadPoolExecutor
+from docker.models.images import Image as DockerImage
+from docker.errors import ImageNotFound
 from dcrx_api.env import Env
 from dcrx_api.env.time_parser import TimeParser
-from docker.models.images import Image as DockerImage
 from typing import (
     Dict, 
     Union,
     List
 )
 from .job import Job
 from .models import (
     JobMetadata,
-    JobNotFoundException
+    JobNotFoundException,
+    ServerLimitException
 )
 from .status import JobStatus
 
 
 class JobQueue:
 
     def __init__(self, env: Env) -> None:
 
         self.pool_size = env.DCRX_API_JOB_WORKERS
 
         self._jobs: Dict[uuid.UUID, Job] = {}
         self._active: Dict[uuid.UUID, asyncio.Task] = {}
-        self.pool_guard = asyncio.Semaphore(
-            value=env.DCRX_API_JOB_POOL_SIZE
-        )
+        self.max_jobs = env.DCRX_API_JOB_POOL_SIZE
+        self.max_pending_jobs = env.DCRX_API_JOB_MAX_PENDING
+
+        self.active_jobs_count = 0
+        self.pending_jobs_count = 0
+        self.pending_jobs: List[Job] = []
+
         self._executor = ThreadPoolExecutor(max_workers=env.DCRX_API_JOB_WORKERS)
 
         self._cleanup_task: Union[asyncio.Task, None] = None
         self._job_max_age = TimeParser(env.DCRX_API_JOB_MAX_AGE).time
         self._job_prune_interval = TimeParser(env.DCRX_API_JOB_PRUNE_INTERVAL).time
         self._run_cleanup = True
         self.active_images: List[DockerImage] = []
@@ -111,26 +117,37 @@
                         asyncio.create_task(
                             self._cancel_task(job)
                         )
                     )
 
                 if job_is_pruneable and job_elapsed > self._job_max_age:
 
+                    self.active_jobs_count -= 1
+                    if len(self.pending_jobs) > 0:
+                        pending_job = self.pending_jobs.pop()
+                        pending_job.waiter.set_result(None)
+                        
+                        self.pending_jobs_count -= 1
+
                     images = await self.loop.run_in_executor(
                         self._executor,
                         self.client.images.list,
                         job.image.name
                     )
 
                     if len(images) > 0:
-                        await self.loop.run_in_executor(
-                            self._executor,
-                            self.client.images.remove,
-                            job.image.name
-                        )
+                        try:
+                            await self.loop.run_in_executor(
+                                self._executor,
+                                self.client.images.remove,
+                                job.image.name
+                            )
+
+                        except ImageNotFound:
+                            pass
 
                     del self._jobs[job_id]
 
             
             cancelling_tasks = list(self.cancelling)
             for cancel_task in cancelling_tasks:
                 if cancel_task.done():
@@ -141,22 +158,39 @@
     async def _cancel_task(self, job: Job):
 
         job.client_closed = True
 
         await job.clear()
         await job.close()
 
-    def submit(self, job: Job) -> JobMetadata:
+    async def submit(self, job: Job) -> JobMetadata:
+
+        if self.active_jobs_count >= self.max_jobs and self.pending_jobs_count < self.max_pending_jobs:
+            job.waiter = asyncio.Future()
+
+        elif self.active_jobs_count >= self.max_jobs:
+            return ServerLimitException(
+                message='Pending jobs quota reached. Please try again later.',
+                limit=self.max_pending_jobs,
+                current=self.pending_jobs_count
+            )
 
         self._jobs[job.job_id] = job
 
         self._active[job.job_id] = asyncio.create_task(
             job.run()
         )
 
+        if job.waiter:
+            self.pending_jobs.append(job)
+            self.pending_jobs_count += 1
+
+        else:
+            self.active_jobs_count += 1
+
         return job.metadata
 
     def get(self, job_id: uuid.UUID) -> Union[JobMetadata, JobNotFoundException]:
         job = self._jobs.get(job_id)
         if job is None:
             return JobNotFoundException(
                 job_id=job_id,
```

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/service.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing import List, Union
 from .job import Job
 from .models import (
     RemoteAdd,
     JobMetadata,
     JobNotFoundException,
     NewImage,
-    ServerMemoryLimitException
+    ServerLimitException
 )
 
 Layer = List[
     Union[
         Add,
         Arg,
         Cmd,
@@ -51,105 +51,114 @@
 
 
 jobs_router = APIRouter()
 
 
 @jobs_router.post(
     "/jobs/images/create",
+    status_code=202,
     responses={
-        400: {
-            'model': ServerMemoryLimitException
-        },
         404: {
             'model': RegistryNotFoundException
-        }
+        },
+        429: {
+            'model': ServerLimitException
+        },
     }
 )
 async def create_job(new_image: NewImage) -> JobMetadata:
 
     job_service_context = context.get(ContextType.JOB_SERVICE)
     monitoring_service_context = context.get(ContextType.MONITORING_SERVICE)
     registry_service_context: RegistryServiceContext = context.get(ContextType.REGISTRY_SERVICE)
     auth_service_context = context.get(ContextType.AUTH_SERVICE)
 
     if monitoring_service_context.exceeded_memory_limit:
-        raise HTTPException(400, detail={
-            "message": "Cannot schedule job - memory limit exceeded.",
+        raise HTTPException(429, detail={
+            "message": "Will not schedule job - memory limit exceeded.",
             "limit": monitoring_service_context.env.DCRX_API_MAX_MEMORY_PERCENT_USAGE,
             "current": monitoring_service_context.get_memory_usage_pct()
         })
+    
+    registries = await registry_service_context.connection.select(
+        filters={
+            'registry_name': new_image.registry.registry_name
+        }
+    )
 
-    async with job_service_context.queue.pool_guard:
-
-        registries = await registry_service_context.connection.select(
-            filters={
-                'registry_name': new_image.registry.registry_name
-            }
-        )
-
-        if len(registries) < 1:
-
-            raise HTTPException(404, detail={
-                "message": "Registry not found."
-            })
-            
-        registry = registries.pop()
+    if len(registries) < 1:
 
-        dcrx_image = Image(
-            new_image.name,
-            tag=new_image.tag
-        )
-
-        layers: Layer = new_image.layers
-
-        for layer in layers:
-
-            if layer.layer_type == 'add':
-                layer = RemoteAdd(
-                    source=layer.source,
-                    destination=layer.destination,
-                    user_id=layer.user_id,
-                    group_id=layer.group_id,
-                    permissions=layer.permissions,
-                    checksum=layer.checksum,
-                    link=layer.link
-                )
-
-            elif layer.layer_type == 'copy':
-                layer = RemoteAdd(
-                    source=layer.source,
-                    destination=layer.destination,
-                    user_id=layer.user_id,
-                    group_id=layer.group_id,
-                    permissions=layer.permissions,
-                    link=layer.link
-                )
-
-            dcrx_image.layers.append(layer)
-
-        decrypted_password = await auth_service_context.manager.decrypt_fernet(
-            registry.registry_password
-        )
-
-        job = Job(
-            job_service_context.connection,
-            dcrx_image,
-            Registry(
-                id=registry.id,
-                registry_name=registry.registry_name,
-                registry_uri=registry.registry_uri,
-                registry_user=registry.registry_user,
-                registry_password=decrypted_password
-            ),
-            build_options=new_image.build_options,
-            pool_size=job_service_context.queue.pool_size,
-            timeout=job_service_context.env.DCRX_API_JOB_TIMEOUT,
-        )
+        raise HTTPException(404, detail={
+            "message": "Registry not found."
+        })
+        
+    registry = registries.pop()
 
-        return job_service_context.queue.submit(job)
+    dcrx_image = Image(
+        new_image.name,
+        tag=new_image.tag
+    )
+
+    layers: Layer = new_image.layers
+
+    for layer in layers:
+
+        if layer.layer_type == 'add':
+            layer = RemoteAdd(
+                source=layer.source,
+                destination=layer.destination,
+                user_id=layer.user_id,
+                group_id=layer.group_id,
+                permissions=layer.permissions,
+                checksum=layer.checksum,
+                link=layer.link
+            )
+
+        elif layer.layer_type == 'copy':
+            layer = RemoteAdd(
+                source=layer.source,
+                destination=layer.destination,
+                user_id=layer.user_id,
+                group_id=layer.group_id,
+                permissions=layer.permissions,
+                link=layer.link
+            )
+
+        dcrx_image.layers.append(layer)
+
+    decrypted_password = await auth_service_context.manager.decrypt_fernet(
+        registry.registry_password
+    )
+
+    job = Job(
+        job_service_context.connection,
+        dcrx_image,
+        Registry(
+            id=registry.id,
+            registry_name=registry.registry_name,
+            registry_uri=registry.registry_uri,
+            registry_user=registry.registry_user,
+            registry_password=decrypted_password
+        ),
+        build_options=new_image.build_options,
+        pool_size=job_service_context.queue.pool_size,
+        timeout=job_service_context.env.DCRX_API_JOB_TIMEOUT,
+    )
+
+    response = await job_service_context.queue.submit(job)
+
+    if isinstance(response, ServerLimitException):
+        raise HTTPException(429, detail={
+            "message": response.message,
+            "limit": response.limit,
+            "current": response.current
+            
+        })
+    
+    return response
 
 
 @jobs_router.get(
     "/jobs/images/{job_id}/get",
     responses={
         404: {
             "model": JobNotFoundException
```

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_mysql_table.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_postgres_table.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_sqlite_table.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/jobs/table/jobs_table.py` & `dcrx-api-0.3.1/dcrx_api/services/jobs/table/jobs_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/monitoring/base/monitor.py` & `dcrx-api-0.3.1/dcrx_api/services/monitoring/base/monitor.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/monitoring/context.py` & `dcrx-api-0.3.1/dcrx_api/services/monitoring/context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 from dcrx_api.context.types import ContextType
 from dcrx_api.env import Env
 from pydantic import (
     BaseModel,
     StrictStr
 )
 from .cpu import CPUMonitor
-from .memory import (
-    DockerMemoryMonitor,
-    MemoryMonitor
-)
+from .memory import MemoryMonitor
 
 
 
 class MonitoringServiceContext(BaseModel):
     env: Env
     monitor_name: StrictStr
     cpu: CPUMonitor
     memory: MemoryMonitor
-    docker_memory: DockerMemoryMonitor
     context_type: ContextType=ContextType.MONITORING_SERVICE
 
     class Config:
         arbitrary_types_allowed = True
 
     @property
     def exceeded_memory_limit(self) -> bool:
         return self.get_memory_usage_pct() > self.env.DCRX_API_MAX_MEMORY_PERCENT_USAGE
 
     def get_memory_usage_pct(self) -> float:
         server_memory_pct = self.memory.get_percent_used(self.monitor_name)
-        docker_memory_pct = self.docker_memory.get_percent_used(self.monitor_name)
-
-        return server_memory_pct + docker_memory_pct
+        return server_memory_pct
 
     async def initialize(self):
         await self.cpu.start_background_monitor(self.monitor_name)
-        await self.docker_memory.start_background_monitor(self.monitor_name)
         await self.memory.start_background_monitor(self.monitor_name)
 
     async def close(self):
         await self.cpu.stop_background_monitor(self.monitor_name)
-        await self.docker_memory.stop_background_monitor(self.monitor_name)
         await self.memory.stop_background_monitor(self.monitor_name)
```

### Comparing `dcrx-api-0.3.0/dcrx_api/services/monitoring/memory/monitor.py` & `dcrx-api-0.3.1/dcrx_api/services/monitoring/memory/monitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import psutil
 from dcrx_api.services.monitoring.base.monitor import BaseMonitor
 
 
 class MemoryMonitor(BaseMonitor):
 
     def __init__(self) -> None:
@@ -10,19 +9,12 @@
         self.total_memory = int(psutil.virtual_memory().total/10**6)
     
     def get_percent_used(self, monitor_name) -> float:
         precentile_usage_metric = f'{monitor_name}_pct_usage'
         return self.active.get(precentile_usage_metric, 0)
 
     def update_monitor(self, monitor_name: str):
-        process = psutil.Process(os.getpid())
-        mem_info = process.memory_info()
 
-        memory_percent_used = int(mem_info.rss/10**6)
-
-        self.active[monitor_name] = memory_percent_used
+        self.active[monitor_name] = int(psutil.virtual_memory().used/10**6)
 
         precentile_usage_metric = f'{monitor_name}_pct_usage'
-        self.active[precentile_usage_metric] = round(
-            memory_percent_used/self.total_memory,
-            3
-        )
+        self.active[precentile_usage_metric] = psutil.virtual_memory().percent
```

### Comparing `dcrx-api-0.3.0/dcrx_api/services/registry/connection.py` & `dcrx-api-0.3.1/dcrx_api/services/registry/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/registry/context.py` & `dcrx-api-0.3.1/dcrx_api/services/registry/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/registry/service.py` & `dcrx-api-0.3.1/dcrx_api/services/registry/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_mysql_table.py` & `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_postgres_table.py` & `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_sqlite_table.py` & `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_sqlite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/registry/table/registry_table.py` & `dcrx-api-0.3.1/dcrx_api/services/registry/table/registry_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/users/connection.py` & `dcrx-api-0.3.1/dcrx_api/services/users/connection.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/users/context.py` & `dcrx-api-0.3.1/dcrx_api/services/users/context.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/users/service.py` & `dcrx-api-0.3.1/dcrx_api/services/users/service.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/users/table/users_mysql_table.py` & `dcrx-api-0.3.1/dcrx_api/services/users/table/users_mysql_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/users/table/users_postgres_table.py` & `dcrx-api-0.3.1/dcrx_api/services/users/table/users_postgres_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/users/table/users_sqllite_table.py` & `dcrx-api-0.3.1/dcrx_api/services/users/table/users_sqllite_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api/services/users/table/users_table.py` & `dcrx-api-0.3.1/dcrx_api/services/users/table/users_table.py`

 * *Files identical despite different names*

### Comparing `dcrx-api-0.3.0/dcrx_api.egg-info/PKG-INFO` & `dcrx-api-0.3.1/dcrx_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: A RESTful implementation of the DCRX Docker library.
 Home-page: https://github.com/scorbettUM/dcrx-api
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops,fastapi
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-api-0.3.0/dcrx_api.egg-info/SOURCES.txt` & `dcrx-api-0.3.1/dcrx_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,29 +47,28 @@
 dcrx_api/services/jobs/models/build_options.py
 dcrx_api/services/jobs/models/image_stats.py
 dcrx_api/services/jobs/models/job_metadata.py
 dcrx_api/services/jobs/models/job_not_found_exception.py
 dcrx_api/services/jobs/models/job_registry.py
 dcrx_api/services/jobs/models/new_image.py
 dcrx_api/services/jobs/models/remote_add.py
-dcrx_api/services/jobs/models/server_memory_limit_exception.py
+dcrx_api/services/jobs/models/server_limit_exception.py
 dcrx_api/services/jobs/table/__init__.py
 dcrx_api/services/jobs/table/jobs_mysql_table.py
 dcrx_api/services/jobs/table/jobs_postgres_table.py
 dcrx_api/services/jobs/table/jobs_sqlite_table.py
 dcrx_api/services/jobs/table/jobs_table.py
 dcrx_api/services/monitoring/__init__.py
 dcrx_api/services/monitoring/context.py
 dcrx_api/services/monitoring/base/__init__.py
 dcrx_api/services/monitoring/base/exceptions.py
 dcrx_api/services/monitoring/base/monitor.py
 dcrx_api/services/monitoring/cpu/__init__.py
 dcrx_api/services/monitoring/cpu/monitor.py
 dcrx_api/services/monitoring/memory/__init__.py
-dcrx_api/services/monitoring/memory/docker_memory_monitor.py
 dcrx_api/services/monitoring/memory/monitor.py
 dcrx_api/services/registry/__init__.py
 dcrx_api/services/registry/connection.py
 dcrx_api/services/registry/context.py
 dcrx_api/services/registry/service.py
 dcrx_api/services/registry/models/__init__.py
 dcrx_api/services/registry/models/registry.py
```

### Comparing `dcrx-api-0.3.0/setup.py` & `dcrx-api-0.3.1/setup.py`

 * *Files identical despite different names*

