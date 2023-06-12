# Comparing `tmp/records-mover-1.5.3.tar.gz` & `tmp/records-mover-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "records-mover-1.5.3.tar", last modified: Wed Apr  5 17:57:34 2023, max compression
+gzip compressed data, was "records-mover-1.5.4.tar", last modified: Mon Jun 12 16:22:12 2023, max compression
```

## Comparing `records-mover-1.5.3.tar` & `records-mover-1.5.4.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.718525 records-mover-1.5.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-05 17:56:47.000000 records-mover-1.5.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6805 2023-04-05 17:57:34.718525 records-mover-1.5.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5412 2023-04-05 17:56:47.000000 records-mover-1.5.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.694524 records-mover-1.5.3/records_mover/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.698524 records-mover-1.5.3/records_mover/airflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/airflow/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.698524 records-mover-1.5.3/records_mover/airflow/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      145 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/airflow/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/airflow/hooks/google_cloud_credentials_hook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4410 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/airflow/hooks/records_hook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1048 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/airflow/hooks/sqlalchemy_db_hook.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.698524 records-mover-1.5.3/records_mover/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9608 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/cli/job_config_schema_as_args_parser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.698524 records-mover-1.5.3/records_mover/creds/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/creds/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12137 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/creds/base_creds.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2465 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/creds/creds_via_airflow.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2002 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/creds/creds_via_env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1142 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/creds/creds_via_lastpass.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1452 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/creds/database.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1435 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/creds/lpass.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.698524 records-mover-1.5.3/records_mover/db/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.698524 records-mover-1.5.3/records_mover/db/bigquery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/bigquery/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6809 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/bigquery/bigquery_db_driver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15001 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/bigquery/load_job_config_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8978 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/bigquery/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5146 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/bigquery/unloader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5344 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/connect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/db_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9089 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/driver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1098 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/factory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/loader.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.702524 records-mover-1.5.3/records_mover/db/mysql/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/mysql/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19694 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/mysql/load_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5077 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/mysql/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7515 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/mysql/mysql_db_driver.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.702524 records-mover-1.5.3/records_mover/db/postgres/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.702524 records-mover-1.5.3/records_mover/db/postgres/copy_options/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4471 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2750 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/csv.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12423 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/date_input_style.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/date_output_style.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/mode.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5283 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4044 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/copy_options/types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6168 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4319 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/postgres_db_driver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5453 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/sqlalchemy_postgres_copy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6122 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/postgres/unloader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1847 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/quoting.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.702524 records-mover-1.5.3/records_mover/db/redshift/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/redshift/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8988 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/redshift/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7101 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/redshift/records_copy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6209 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/redshift/records_unload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9423 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/redshift/redshift_db_driver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/redshift/sql.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7973 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/redshift/unloader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/unloader.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.702524 records-mover-1.5.3/records_mover/db/vertica/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1411 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/export_sql.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3991 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/import_sql.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/io_base_wrapper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4182 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/loader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2948 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/records_export_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4357 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/records_import_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6845 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/unloader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5354 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/db/vertica/vertica_db_driver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2787 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/logging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1060 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/mover_types.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.702524 records-mover-1.5.3/records_mover/pandas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/pandas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/py.typed
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.706524 records-mover-1.5.3/records_mover/records/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/base_records_format.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/cli.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.706524 records-mover-1.5.3/records_mover/records/delimited/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1752 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      651 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/compression.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/conversions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3453 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/csv_streamer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4254 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/hint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/hints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12365 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/sniff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2165 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/delimited/validated_records_hints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/deprecated.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1327 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/existing_table_handling.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.706524 records-mover-1.5.3/records_mover/records/job/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/job/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7822 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/job/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/job/mover.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3047 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/job/schema.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/load_plan.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9074 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/mover.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.710524 records-mover-1.5.3/records_mover/records/pandas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/pandas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5700 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/pandas/prep_for_csv.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24256 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/pandas/read_csv_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4304 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/pandas/to_csv_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4518 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/prep.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1779 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/prep_and_load.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2929 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/processing_instructions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2956 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/records.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9287 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/records_directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10672 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/records_format.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3400 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/records_format_file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/records_schema_json_file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/records_schema_sql_file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/records_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/results.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.710524 records-mover-1.5.3/records_mover/records/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/errors.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.710524 records-mover-1.5.3/records_mover/records/schema/field/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14827 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.710524 records-mover-1.5.3/records_mover/records/schema/field/constraints/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/constraints/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9333 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/constraints/constraints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3115 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/constraints/decimal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1797 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/constraints/integer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2471 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/constraints/string.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/field_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/numpy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5427 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/pandas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8181 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/representation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9253 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/sqlalchemy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3093 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/statistics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/field/string_length_generator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.710524 records-mover-1.5.3/records_mover/records/schema/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/schema/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/schema/known_representation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2391 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/schema/pandas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2020 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/schema/schema/sqlalchemy.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.710524 records-mover-1.5.3/records_mover/records/sources/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6459 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2551 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/data_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8399 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/dataframes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2354 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13165 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/factory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8507 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/fileobjs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4468 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/google_sheets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6872 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/table.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/sources/uninferred_fileobjs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      964 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/table.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.714524 records-mover-1.5.3/records_mover/records/targets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7084 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3850 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/data_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1128 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/directory_from_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10310 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/factory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3961 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/fileobj.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5197 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/google_sheets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7462 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/spectrum.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.714524 records-mover-1.5.3/records_mover/records/targets/table/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/table/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/table/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5121 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/table/move_from_dataframes_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3484 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/table/move_from_fileobjs_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3536 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/table/move_from_records_directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2972 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8030 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/targets/table/target.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      483 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/records/unload_plan.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17218 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/session.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.714524 records-mover-1.5.3/records_mover/url/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8203 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3823 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/filesystem.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.714524 records-mover-1.5.3/records_mover/url/gcs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/gcs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/gcs/gcs_directory_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/gcs/gcs_file_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/http.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5278 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/resolver.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.714524 records-mover-1.5.3/records_mover/url/s3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/s3/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      673 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/s3/awscli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3034 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/s3/s3_base_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/s3/s3_directory_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6147 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/s3/s3_file_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      556 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/s3/s3_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      287 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/url/urllib.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.718525 records-mover-1.5.3/records_mover/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1707 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/concat_files.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/json_parameter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7576 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/json_schema.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/json_schema_array_document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/json_schema_document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/lazyprop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1841 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/limits.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2681 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/retry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      724 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/rewound_fileobj.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/utils/structures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-05 17:56:47.000000 records-mover-1.5.3/records_mover/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 17:57:34.698524 records-mover-1.5.3/records_mover.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6805 2023-04-05 17:57:34.000000 records-mover-1.5.3/records_mover.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7542 2023-04-05 17:57:34.000000 records-mover-1.5.3/records_mover.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-05 17:57:34.000000 records-mover-1.5.3/records_mover.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-04-05 17:57:34.000000 records-mover-1.5.3/records_mover.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2828 2023-04-05 17:57:34.000000 records-mover-1.5.3/records_mover.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-04-05 17:57:34.000000 records-mover-1.5.3/records_mover.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-04-05 17:57:34.722525 records-mover-1.5.3/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    11751 2023-04-05 17:56:47.000000 records-mover-1.5.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.122208 records-mover-1.5.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-12 16:22:02.000000 records-mover-1.5.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7002 2023-06-12 16:22:12.122208 records-mover-1.5.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2023-06-12 16:22:02.000000 records-mover-1.5.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.102208 records-mover-1.5.4/records_mover/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1534 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.102208 records-mover-1.5.4/records_mover/airflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/airflow/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.102208 records-mover-1.5.4/records_mover/airflow/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      145 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/airflow/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/airflow/hooks/google_cloud_credentials_hook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4410 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/airflow/hooks/records_hook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1048 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/airflow/hooks/sqlalchemy_db_hook.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.102208 records-mover-1.5.4/records_mover/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10464 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/cli/job_config_schema_as_args_parser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.102208 records-mover-1.5.4/records_mover/creds/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/creds/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12137 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/creds/base_creds.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2465 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/creds/creds_via_airflow.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2002 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/creds/creds_via_env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1142 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/creds/creds_via_lastpass.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1452 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/creds/database.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1435 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/creds/lpass.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.106208 records-mover-1.5.4/records_mover/db/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.106208 records-mover-1.5.4/records_mover/db/bigquery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/bigquery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6809 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/bigquery/bigquery_db_driver.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15001 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/bigquery/load_job_config_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8978 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/bigquery/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5146 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/bigquery/unloader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5254 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/connect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/db_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9089 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/driver.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/factory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4545 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/loader.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.106208 records-mover-1.5.4/records_mover/db/mysql/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/mysql/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19694 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/mysql/load_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5077 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/mysql/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7515 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/mysql/mysql_db_driver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.106208 records-mover-1.5.4/records_mover/db/postgres/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.106208 records-mover-1.5.4/records_mover/db/postgres/copy_options/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4471 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2750 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6487 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/csv.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14773 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/date_input_style.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/date_output_style.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/mode.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5283 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4044 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/copy_options/types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6168 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4319 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/postgres_db_driver.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5453 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/sqlalchemy_postgres_copy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6122 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/postgres/unloader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1847 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/quoting.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.110208 records-mover-1.5.4/records_mover/db/redshift/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/redshift/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8988 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/redshift/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11595 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/redshift/records_copy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6209 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/redshift/records_unload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9423 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/redshift/redshift_db_driver.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/redshift/sql.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7973 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/redshift/unloader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/unloader.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.110208 records-mover-1.5.4/records_mover/db/vertica/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/export_sql.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3991 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/import_sql.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/io_base_wrapper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4182 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/loader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2948 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/records_export_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4357 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/records_import_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6845 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/unloader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5354 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/db/vertica/vertica_db_driver.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2787 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/logging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/mover_types.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.110208 records-mover-1.5.4/records_mover/pandas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/pandas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.110208 records-mover-1.5.4/records_mover/records/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/base_records_format.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5383 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.114208 records-mover-1.5.4/records_mover/records/delimited/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1752 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      651 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/compression.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2798 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/csv_streamer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4254 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/hint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5611 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/hints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12365 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/sniff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2165 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/delimited/validated_records_hints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/deprecated.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1327 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/existing_table_handling.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.114208 records-mover-1.5.4/records_mover/records/job/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/job/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7822 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/job/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/job/mover.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3047 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/job/schema.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/load_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9074 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/mover.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.114208 records-mover-1.5.4/records_mover/records/pandas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/pandas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5714 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/pandas/prep_for_csv.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23611 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/pandas/read_csv_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/pandas/to_csv_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4518 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/prep.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1779 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/prep_and_load.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2929 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/processing_instructions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2956 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/records.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9287 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/records_directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10672 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/records_format.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3400 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/records_format_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/records_schema_json_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/records_schema_sql_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/records_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/results.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.114208 records-mover-1.5.4/records_mover/records/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/errors.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.114208 records-mover-1.5.4/records_mover/records/schema/field/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14827 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.114208 records-mover-1.5.4/records_mover/records/schema/field/constraints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/constraints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9333 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/constraints/constraints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3115 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/constraints/decimal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1797 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/constraints/integer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2471 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/constraints/string.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/field_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/numpy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5427 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8181 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/representation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9253 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/sqlalchemy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3093 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/statistics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/field/string_length_generator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.118208 records-mover-1.5.4/records_mover/records/schema/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/schema/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4048 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/schema/known_representation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2391 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/schema/pandas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2020 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/schema/schema/sqlalchemy.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.118208 records-mover-1.5.4/records_mover/records/sources/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6459 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2551 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/data_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8399 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/dataframes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2354 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13165 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/factory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8507 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/fileobjs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4468 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/google_sheets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6872 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/table.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/sources/uninferred_fileobjs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      964 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/table.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.118208 records-mover-1.5.4/records_mover/records/targets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7084 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3850 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/data_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1128 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/directory_from_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10310 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/factory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3984 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/fileobj.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5197 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/google_sheets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7462 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/spectrum.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.118208 records-mover-1.5.4/records_mover/records/targets/table/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/table/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/table/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5121 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/table/move_from_dataframes_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3484 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/table/move_from_fileobjs_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3536 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/table/move_from_records_directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2972 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8030 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/targets/table/target.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      483 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/records/unload_plan.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17218 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/session.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.118208 records-mover-1.5.4/records_mover/url/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8203 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3823 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/filesystem.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.122208 records-mover-1.5.4/records_mover/url/gcs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/gcs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/gcs/gcs_directory_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/gcs/gcs_file_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/http.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5278 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/resolver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.122208 records-mover-1.5.4/records_mover/url/s3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/s3/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      673 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/s3/awscli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3034 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/s3/s3_base_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/s3/s3_directory_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6147 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/s3/s3_file_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      556 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/s3/s3_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      287 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/url/urllib.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.122208 records-mover-1.5.4/records_mover/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/concat_files.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/json_parameter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7576 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/json_schema.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/json_schema_array_document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/json_schema_document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/lazyprop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1841 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/limits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2681 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/retry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      724 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/rewound_fileobj.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/utils/structures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-06-12 16:22:02.000000 records-mover-1.5.4/records_mover/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-12 16:22:12.102208 records-mover-1.5.4/records_mover.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7002 2023-06-12 16:22:12.000000 records-mover-1.5.4/records_mover.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7542 2023-06-12 16:22:12.000000 records-mover-1.5.4/records_mover.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-12 16:22:12.000000 records-mover-1.5.4/records_mover.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-06-12 16:22:12.000000 records-mover-1.5.4/records_mover.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2828 2023-06-12 16:22:12.000000 records-mover-1.5.4/records_mover.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-06-12 16:22:12.000000 records-mover-1.5.4/records_mover.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2023-06-12 16:22:12.122208 records-mover-1.5.4/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    11751 2023-06-12 16:22:02.000000 records-mover-1.5.4/setup.py
```

### Comparing `records-mover-1.5.3/LICENSE` & `records-mover-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/PKG-INFO` & `records-mover-1.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: records-mover
-Version: 1.5.3
+Version: 1.5.4
 Summary: Library and CLI to move relational data from one place to another - DBs/CSV/gsheets/dataframes/...
 Home-page: UNKNOWN
 Author: Vince Broz
 Author-email: opensource@bluelabs.com
 License: Apache Software License
-Download-URL: https://github.com/bluelabsio/records-mover/tarball/1.5.3
+Download-URL: https://github.com/bluelabsio/records-mover/tarball/1.5.4
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database :: Front-Ends
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -42,14 +42,16 @@
 
 <img
  src="https://raw.githubusercontent.com/bluelabsio/records-mover/master/docs/records-mover-horizontal.png"
  alt="Records Mover">
 
 [![Documentation Status](https://readthedocs.org/projects/records-mover/badge/?version=latest)](https://records-mover.readthedocs.io/en/latest/?badge=latest)
 
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/bluelabsio/records-mover/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/bluelabsio/records-mover/tree/main)
+
 Records mover is a command-line tool and Python library you can
 use to move relational data from one place to another.
 
 Relational data here means anything roughly "rectangular" - with
 columns and rows.  For example, it supports reading and writing from:
 
 * Databases, including using native high-speed methods of
```

### Comparing `records-mover-1.5.3/README.md` & `records-mover-1.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 <img
  src="https://raw.githubusercontent.com/bluelabsio/records-mover/master/docs/records-mover-horizontal.png"
  alt="Records Mover">
 
 [![Documentation Status](https://readthedocs.org/projects/records-mover/badge/?version=latest)](https://records-mover.readthedocs.io/en/latest/?badge=latest)
 
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/bluelabsio/records-mover/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/bluelabsio/records-mover/tree/main)
+
 Records mover is a command-line tool and Python library you can
 use to move relational data from one place to another.
 
 Relational data here means anything roughly "rectangular" - with
 columns and rows.  For example, it supports reading and writing from:
 
 * Databases, including using native high-speed methods of
```

### Comparing `records-mover-1.5.3/records_mover/__init__.py` & `records-mover-1.5.4/records_mover/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/airflow/hooks/google_cloud_credentials_hook.py` & `records-mover-1.5.4/records_mover/airflow/hooks/google_cloud_credentials_hook.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/airflow/hooks/records_hook.py` & `records-mover-1.5.4/records_mover/airflow/hooks/records_hook.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/airflow/hooks/sqlalchemy_db_hook.py` & `records-mover-1.5.4/records_mover/airflow/hooks/sqlalchemy_db_hook.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/cli/job_config_schema_as_args_parser.py` & `records-mover-1.5.4/records_mover/cli/job_config_schema_as_args_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,131 +56,157 @@
             return key
         return prefix + '.' + key
 
     def configure_from_properties(self,
                                   properties: JsonSchema,
                                   required_keys: Iterable[str],
                                   prefix: str = '') -> None:
+        self.required_keys = required_keys
         for naked_key, raw_value in properties.items():
             if not isinstance(raw_value, dict):
                 raise TypeError(f"Did not understand [{raw_value}] in [{properties}]")
             value: Dict[str, object] = raw_value
             key = self.add_to_prefix(prefix, naked_key)
             self.configure_from_single_property(key, value, required_keys, properties)
 
     def configure_from_single_property(self,
                                        key: str,
                                        value: Dict[str, object],
                                        required_keys: Iterable[str],
                                        properties: JsonSchema) -> None:
-        arg_name = key
-        # For consistency with other args, we map dashes to underscores in the CLI args
-        formatted_key_name = key.replace('-', '_')
         kwargs: ArgParseArgument = {}
-        if key in required_keys:
-            # use a positional argument if it's required
-            arg_name = key
-        else:
-            # use a --parameter=value argument if it's optional
-            arg_name = "--" + formatted_key_name
-            kwargs['required'] = False
+        arg_name = self.get_arg_name(key, value)
 
-            # When the formatted_key_name differs from key, this will make sure that the arg
-            # parser is storing the value in a place that matches the actual schema
+        if not self.is_key_required(key):
+            kwargs['required'] = False
+            # When the formatted_key_name differs from key, this will make sure
+            # that the arg parser is storing the value in a place that matches
+            # the actual schema
             kwargs['dest'] = key
 
         if 'default' in value:
             kwargs['default'] = value['default']
 
         if 'description' in value:
             kwargs['help'] = str(value['description'])
 
         if 'enum' in value:
-            enum_values: Iterable[Any] = value['enum']  # type: ignore
-            non_none_values: Iterable[Any] = [v for v in enum_values if v is not None]
-            kwargs['choices'] = non_none_values
-            if None in enum_values:
-                # add an arg that maps to 'None' for this key
-                no_arg_kwargs: ArgParseArgument = {}
-                # if --no_foo is specified, set foo variable to None
-                split_key_name = formatted_key_name.split('.')
-                no_arg_arg_name = '--' + '.'.join([*split_key_name[:-1],
-                                                   'no_' + split_key_name[-1]])
-                no_arg_kwargs['action'] = 'store_const'
-                no_arg_kwargs['const'] = ARG_VALUE_WAS_NONE
-                no_arg_kwargs['dest'] = key
-                no_arg_kwargs['required'] = False
-                self.arg_parser.add_argument(no_arg_arg_name, **no_arg_kwargs)
-
+            self.add_enum_arg(key, arg_name, value, kwargs)
         elif 'type' in value and value['type'] == 'string':
             kwargs['type'] = str
+            self.arg_parser.add_argument(arg_name, **kwargs)
         elif 'type' in value and value['type'] == 'integer':
             kwargs['type'] = int
+            self.arg_parser.add_argument(arg_name, **kwargs)
         elif 'type' in value and value['type'] == 'array':
-            items = value['items']
-            if not isinstance(items, dict):
-                raise TypeError(f"Did not understand [{items}] in [{properties}]")
-            item_type = items['type']
-            if not isinstance(item_type, str):
-                raise TypeError(f"Did not understand [{item_type}] in [{properties}]")
-            if item_type == 'string':
-                kwargs['type'] = str
-            elif item_type == 'integer':
-                kwargs['type'] = int
-            else:
-                raise NotImplementedError("Teach me how to handle array item "
-                                          f"type of {item_type}")
-            kwargs['nargs'] = '*'
+            self.add_array_arg(key, arg_name, value, kwargs, properties)
         elif 'type' in value and value['type'] == 'object':
-            # Recurse and handle nested dicts
-            sub_properties = value['properties']
-            if not isinstance(sub_properties, dict):
-                raise TypeError(f"Did not understand [{sub_properties}] in [{properties}]")
-            required_subkeys: List[str] = []
-            if key in required_keys:
-                required_subkeys = [
-                    self.add_to_prefix(key, partial_subkey)
-                    for partial_subkey
-                    in value.get('required', [])  # type: ignore
-                ]
-            self.configure_from_properties(sub_properties, required_subkeys, prefix=key)
-            return  # no immediate argument to add
+            self.add_object_arg(key, arg_name, value, kwargs, properties)
         elif 'type' in value and value['type'] == 'boolean':
-            # https://stackoverflow.com/questions/9183936/boolean-argument-for-script
-            if 'default' in value:
-                if value['default'] is True:
-                    # if --no_foo is specified, set foo variable to False
-                    arg_name = "--no_" + formatted_key_name
-                    kwargs['action'] = 'store_false'
-                else:
-                    kwargs['action'] = 'store_true'
-            else:
-                if key in required_keys:
-                    raise NotImplementedError("Teach me how to handle a required boolean "
-                                              "with no default")
-                else:
-                    # the regular --foo will set this to True:
-                    kwargs['action'] = 'store_const'
-                    # store_true sets a default, so we use store_const
-                    kwargs['const'] = True
-
-                    # and we'll add an arg that maps to False for this key:
-                    false_arg_kwargs: ArgParseArgument = {}
-                    # if --no_foo is specified, set foo variable to False
-                    split_key_name = formatted_key_name.split('.')
-                    false_arg_arg_name = '--' + '.'.join([*split_key_name[:-1],
-                                                          'no_' + split_key_name[-1]])
-                    false_arg_kwargs['action'] = 'store_const'
-                    false_arg_kwargs['const'] = False
-                    false_arg_kwargs['dest'] = key
-                    false_arg_kwargs['required'] = False
-                    self.arg_parser.add_argument(false_arg_arg_name, **false_arg_kwargs)
+            self.add_bool_arg(key, arg_name, value, kwargs)
         else:
             raise Exception("Did not know how to handle key " + key +
                             " and value " + str(value))
+
+    # For consistency with other args, we map dashes to underscores in the
+    # CLI args
+    def formatted_key_name(self, key: str) -> str:
+        return key.replace('-', '_')
+
+    def is_key_required(self, key: str) -> bool:
+        return key in self.required_keys
+
+    def get_arg_name(self, key: str, value: Dict[str, object]) -> str:
+        if self.is_key_required(key):
+            return key  # why is this not formatted_key_name?
+
+        if value.get('type') == 'boolean' and value.get('default') is True:
+            return '--no_' + self.formatted_key_name(key)
+        else:
+            return "--" + self.formatted_key_name(key)
+
+    def add_enum_arg(self, key, arg_name, value, kwargs):
+        enum_values: Iterable[Any] = value['enum']  # type: ignore
+        non_none_values: Iterable[Any] = [v for v in enum_values if v is not None]
+        kwargs['choices'] = non_none_values
+        if None in enum_values:
+            # add an arg that maps to 'None' for this key
+            no_arg_kwargs: ArgParseArgument = {}
+            # if --no_foo is specified, set foo variable to None
+            split_key_name = self.formatted_key_name(key).split('.')
+            no_arg_arg_name = '--' + '.'.join([*split_key_name[:-1],
+                                               'no_' + split_key_name[-1]])
+            no_arg_kwargs['action'] = 'store_const'
+            no_arg_kwargs['const'] = ARG_VALUE_WAS_NONE
+            no_arg_kwargs['dest'] = key
+            no_arg_kwargs['required'] = False
+            self.arg_parser.add_argument(no_arg_arg_name, **no_arg_kwargs)
+        self.arg_parser.add_argument(arg_name, **kwargs)
+
+    def add_array_arg(self, key, arg_name, value, kwargs, props):
+        items = value['items']
+        if not isinstance(items, dict):
+            raise TypeError(f"Did not understand [{items}] in [{props}]")
+        item_type = items['type']
+        if not isinstance(item_type, str):
+            raise TypeError(f"Did not understand [{item_type}] in [{props}]")
+        if item_type == 'string':
+            kwargs['type'] = str
+        elif item_type == 'integer':
+            kwargs['type'] = int
+        else:
+            raise NotImplementedError("Teach me how to handle array item "
+                                      f"type of {item_type}")
+        kwargs['nargs'] = '*'
+        self.arg_parser.add_argument(arg_name, **kwargs)
+
+    def add_object_arg(self, key, arg_name, value, kwargs, props):
+        # Recurse and handle nested dicts
+        sub_properties = value['properties']
+        if not isinstance(sub_properties, dict):
+            raise TypeError(f"Did not understand [{sub_properties}] in [{props}]")
+        required_subkeys: List[str] = []
+        if self.is_key_required(key):
+            required_subkeys = [
+                self.add_to_prefix(key, partial_subkey)
+                for partial_subkey
+                in value.get('required', [])
+            ]
+        sub_config = JobConfigSchemaAsArgsParser(self.config_json_schema, self.arg_parser)
+        sub_config.configure_from_properties(sub_properties, required_subkeys, prefix=key)
+
+    def add_bool_arg(self, key, arg_name, value, kwargs):
+        # https://stackoverflow.com/questions/9183936/boolean-argument-for-script
+        if 'default' in value:
+            if value['default'] is True:
+                # if --no_foo is specified, set foo variable to False
+                kwargs['action'] = 'store_false'
+            else:
+                kwargs['action'] = 'store_true'
+        else:
+            if self.is_key_required(key):
+                raise NotImplementedError("Teach me how to handle a required boolean "
+                                          "with no default")
+            else:
+                # the regular --foo will set this to True:
+                kwargs['action'] = 'store_const'
+                # store_true sets a default, so we use store_const
+                kwargs['const'] = True
+
+                # and we'll add an arg that maps to False for this key:
+                false_arg_kwargs: ArgParseArgument = {}
+                # if --no_foo is specified, set foo variable to False
+                split_key_name = self.formatted_key_name(key).split('.')
+                false_arg_arg_name = '--' + '.'.join([*split_key_name[:-1],
+                                                      'no_' + split_key_name[-1]])
+                false_arg_kwargs['action'] = 'store_const'
+                false_arg_kwargs['const'] = False
+                false_arg_kwargs['dest'] = key
+                false_arg_kwargs['required'] = False
+                self.arg_parser.add_argument(false_arg_arg_name, **false_arg_kwargs)
         self.arg_parser.add_argument(arg_name, **kwargs)
 
     def configure_arg_parser(self) -> None:
         schema = self.config_json_schema
         if schema['type'] == 'object':
             props = schema['properties']
             if not isinstance(props, dict):
```

### Comparing `records-mover-1.5.3/records_mover/creds/base_creds.py` & `records-mover-1.5.4/records_mover/creds/base_creds.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/creds/creds_via_airflow.py` & `records-mover-1.5.4/records_mover/creds/creds_via_airflow.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/creds/creds_via_env.py` & `records-mover-1.5.4/records_mover/creds/creds_via_env.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/creds/creds_via_lastpass.py` & `records-mover-1.5.4/records_mover/creds/creds_via_lastpass.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/creds/database.py` & `records-mover-1.5.4/records_mover/creds/database.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/creds/lpass.py` & `records-mover-1.5.4/records_mover/creds/lpass.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/bigquery/bigquery_db_driver.py` & `records-mover-1.5.4/records_mover/db/bigquery/bigquery_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/bigquery/load_job_config_options.py` & `records-mover-1.5.4/records_mover/db/bigquery/load_job_config_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/bigquery/loader.py` & `records-mover-1.5.4/records_mover/db/bigquery/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/bigquery/unloader.py` & `records-mover-1.5.4/records_mover/db/bigquery/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/connect.py` & `records-mover-1.5.4/records_mover/db/connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,21 +109,22 @@
     elif driver == 'bigquery':
         if 'bq_service_account_json' in db_facts:
             raise NotImplementedError("pybigquery does not support providing credentials info "
                                       "(service account JSON) directly")
 
         return create_bigquery_sqlalchemy_url(db_facts)
     else:
-        return sa.engine.url.URL(drivername=driver,
-                                 username=username,
-                                 password=db_facts['password'],
-                                 host=db_facts['host'],
-                                 port=db_facts['port'],
-                                 database=db_facts['database'],
-                                 query=query_for_type.get(db_type))
+        return sa.engine.url.URL.create(  # type: ignore
+            drivername=driver,
+            username=username,
+            password=db_facts['password'],
+            host=db_facts['host'],
+            port=db_facts['port'],
+            database=db_facts['database'],
+            query=query_for_type.get(db_type))
 
 
 def engine_from_lpass_entry(lpass_entry_name: str) -> sa.engine.Engine:
     db_facts = db_facts_from_lpass(lpass_entry_name)
     return engine_from_db_facts(db_facts)
```

### Comparing `records-mover-1.5.3/records_mover/db/db_type.py` & `records-mover-1.5.4/records_mover/db/db_type.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/driver.py` & `records-mover-1.5.4/records_mover/db/driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/factory.py` & `records-mover-1.5.4/records_mover/db/factory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/loader.py` & `records-mover-1.5.4/records_mover/db/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/mysql/load_options.py` & `records-mover-1.5.4/records_mover/db/mysql/load_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/mysql/loader.py` & `records-mover-1.5.4/records_mover/db/mysql/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/mysql/mysql_db_driver.py` & `records-mover-1.5.4/records_mover/db/mysql/mysql_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/copy_options/__init__.py` & `records-mover-1.5.4/records_mover/db/postgres/copy_options/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/copy_options/common.py` & `records-mover-1.5.4/records_mover/db/postgres/copy_options/common.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/copy_options/csv.py` & `records-mover-1.5.4/records_mover/db/postgres/copy_options/csv.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/copy_options/date_input_style.py` & `records-mover-1.5.4/records_mover/db/postgres/copy_options/date_input_style.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,14 @@
 from .types import DateOrderStyle
 
 
 def determine_input_date_order_style(unhandled_hints: Set[str],
                                      hints: ValidatedRecordsHints,
                                      fail_if_cant_handle_hint: bool) ->\
         Optional[DateOrderStyle]:
-    date_order_style: Optional[DateOrderStyle] = None
-
-    def upgrade_date_order_style(style: DateOrderStyle, hint_name: str) -> None:
-        nonlocal date_order_style
-        if date_order_style not in (None, style):
-            cant_handle_hint(fail_if_cant_handle_hint, hint_name, hints)
-        else:
-            date_order_style = style
-            quiet_remove(unhandled_hints, hint_name)
 
     # https://www.postgresql.org/docs/9.5/datatype-datetime.html#DATATYPE-DATETIME-INPUT
 
     # "Date and time input is accepted in almost any reasonable
     # format, including ISO 8601, SQL-compatible, traditional
     # POSTGRES, and others. For some formats, ordering of day, month,
     # and year in date input is ambiguous and there is support for
@@ -36,346 +27,381 @@
     #  DateStyle
     # -----------
     #  ISO, MDY
     # (1 row)
     #
     # postgres=#
 
-    datetimeformattz = hints.datetimeformattz
-
-    # datetimeformattz: Valid values: "YYYY-MM-DD HH:MI:SSOF",
-    # "YYYY-MM-DD HH:MI:SS", "YYYY-MM-DD HH24:MI:SSOF", "YYYY-MM-DD
-    # HH24:MI:SSOF", "MM/DD/YY HH24:MI". See Redshift docs for more
-    # information (note that HH: is equivalent to HH24: and that if
-    # you don't provide an offset (OF), times are assumed to be in
-    # UTC).
-
-    # Default value is "YYYY-MM-DD HH:MI:SSOF".
-
-    #
-    # To get a postgres database to test these cases with:
-    #
-    # cd tests/integration
-    # ./itest shell
-    # db dockerized-postgres
-    if datetimeformattz in ['YYYY-MM-DD HH:MI:SSOF',
-                            'YYYY-MM-DD HH24:MI:SSOF']:
-        #
-        #  postgres=# select timestamptz '2020-01-01 23:01:01-10';
-        #        timestamptz
-        #  ------------------------
-        #   2020-01-02 09:01:01+00
-        #  (1 row)
-        #
-        #  postgres=#
-
-        # Any DateStyle will do as this is unambiguous
-        quiet_remove(unhandled_hints, 'datetimeformattz')
-    elif datetimeformattz == 'YYYY-MM-DD HH:MI:SS':
-        #
-        #
-        #  postgres=# select timestamptz '2020-01-01 23:01:01';
-        #        timestamptz
-        #  ------------------------
-        #   2020-01-01 23:01:01+00
-        #  (1 row)
-        #
-        #  postgres=#
-
-        # Any DateStyle will do as this is unambiguous
-        quiet_remove(unhandled_hints, 'datetimeformattz')
-    elif datetimeformattz == "MM/DD/YY HH24:MI":
-        # "MM/DD/YY HH24:MI"
-        #
-        #  postgres=# select timestamptz '01/02/2999 23:01';
-        #        timestamptz
-        #  ------------------------
-        #   2999-01-02 23:01:00+00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('MDY', 'datetimeformattz')
-    elif datetimeformattz == 'DD-MM-YY HH:MI:SSOF':
-        #  postgres=# select timestamptz '02-01-2999 23:01:01-10';
-        #        timestamptz
-        #  ------------------------
-        #   2999-02-02 09:01:01+00
-        #  (1 row)
-        #
-        upgrade_date_order_style('DMY', 'datetimeformattz')
-    elif datetimeformattz == 'DD/MM/YY HH:MI:SSOF':
-        #  postgres=# select timestamptz '02/01/99 23:01:01-10';
-        #        timestamptz
-        #  ------------------------
-        #   1999-02-02 09:01:01+00
-        #  (1 row)
-        #
-        upgrade_date_order_style('DMY', 'datetimeformattz')
-    elif datetimeformattz == 'DD-MM-YYYY HH:MI:SSOF':
-        #  postgres=# select timestamptz '02-01-1999 23:01:01-10';
-        #        timestamptz
-        #  ------------------------
-        #   1999-02-02 09:01:01+00
-        #  (1 row)
-        #
-        upgrade_date_order_style('DMY', 'datetimeformattz')
-    elif datetimeformattz == 'MM/DD/YY HH:MI:SSOF':
-        #  postgres=# select timestamptz '01/02/99 23:01:01-10';
-        #        timestamptz
-        #  ------------------------
-        #   1999-01-03 09:01:01+00
-        #  (1 row)
-        #
-        upgrade_date_order_style('MDY', 'datetimeformattz')
-    elif datetimeformattz == 'MM-DD-YYYY HH:MI:SSOF':
-        #  postgres=# select timestamptz '01-02-1999 23:01:01-10';
-        #        timestamptz
-        #  ------------------------
-        #   1999-01-03 09:01:01+00
-        #  (1 row)
-        #
-        upgrade_date_order_style('MDY', 'datetimeformattz')
-    else:
-        cant_handle_hint(fail_if_cant_handle_hint, 'datetimeformattz', hints)
-
-    # datetimeformat: Valid values: "YYYY-MM-DD HH24:MI:SS",
-    # "YYYY-MM-DD HH12:MI AM", "MM/DD/YY HH24:MI". See Redshift docs
-    # for more information.
+    handler = DateInputStyleHandler(
+        unhandled_hints, hints, fail_if_cant_handle_hint)
 
-    datetimeformat = hints.datetimeformat
+    return handler.date_order_style
 
-    if datetimeformat in ("YYYY-MM-DD HH24:MI:SS",
-                          "YYYY-MM-DD HH:MI:SS"):
-        #
-        #  postgres=# select timestamp '2020-01-02 15:13:12';
-        #        timestamp
-        #  ---------------------
-        #   2020-01-02 15:13:12
-        #  (1 row)
-        #
-        #  postgres=#
-
-        # Any DateStyle will do as this is unambiguous
-        quiet_remove(unhandled_hints, 'datetimeformat')
-    elif datetimeformat == "YYYY-MM-DD HH12:MI AM":
-        # "YYYY-MM-DD HH12:MI AM"
-        #
-        #  postgres=# select timestamp '2020-01-02 1:13 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-01-02 13:13:00
-        #  (1 row)
-        #
-        #  postgres=#
-
-        # Any DateStyle will do as this is unambiguous
-        quiet_remove(unhandled_hints, 'datetimeformat')
-    elif datetimeformat == "MM/DD/YY HH24:MI":
-        #  postgres=# select timestamp '01/02/20 15:23';
-        #        timestamp
-        #  ---------------------
-        #   2020-01-02 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
 
-        upgrade_date_order_style('MDY', 'datetimeformat')
-    elif datetimeformat == 'DD-MM-YY HH12:MI AM':
-        #  postgres=# select timestamp '02-01-20 3:23 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-02-01 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('DMY', 'datetimeformat')
-    elif datetimeformat == 'DD/MM/YY HH12:MI AM':
-        #  postgres=# select timestamp '02/01/20 3:23 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-02-01 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('DMY', 'datetimeformat')
-    elif datetimeformat == 'DD-MM-YYYY HH12:MI AM':
-        #  postgres=# select timestamp '02-01-2020 3:23 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-02-01 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('DMY', 'datetimeformat')
-    elif datetimeformat == 'MM-DD-YY HH12:MI AM':
-        #  postgres=# select timestamp '02-01-20 3:23 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-02-01 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('MDY', 'datetimeformat')
-    elif datetimeformat == 'MM/DD/YY HH12:MI AM':
-        #  postgres=# select timestamp '02/01/20 3:23 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-02-01 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('MDY', 'datetimeformat')
-    elif datetimeformat == 'MM-DD-YYYY HH12:MI AM':
-        #  postgres=# select timestamp '01-02-2020 3:23 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-01-02 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('MDY', 'datetimeformat')
-    elif datetimeformat == 'MM-DD-YYYY HH:MI:SS':
-        #  postgres=# select timestamp '01-02-2020 3:23 PM';
-        #        timestamp
-        #  ---------------------
-        #   2020-01-02 15:23:00
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('MDY', 'datetimeformat')
-    else:
-        cant_handle_hint(fail_if_cant_handle_hint, 'datetimeformat', hints)
+class DateInputStyleHandler():
+    def __init__(self,
+                 unhandled_hints: Set[str],
+                 hints: ValidatedRecordsHints,
+                 fail_if_cant_handle_hint: bool):
+
+        self.unhandled_hints = unhandled_hints
+        self.hints = hints
+        self.fail_if_cant_handle_hint = fail_if_cant_handle_hint
+        self.date_order_style: Optional[DateOrderStyle] = None
+
+        self.process_hint_datetimeformattz()
+        self.process_hint_datetimeformat()
+        self.process_hint_timeonlyformat()
+        self.process_hint_dateformat()
+
+    def upgrade_date_order_style(self, style: DateOrderStyle, hint_name: str) -> None:
+        if self.date_order_style not in (None, style):
+            cant_handle_hint(self.fail_if_cant_handle_hint, hint_name, self.hints)
+        else:
+            self.date_order_style = style
+            quiet_remove(self.unhandled_hints, hint_name)
 
-    timeonlyformat = hints.timeonlyformat
+    def process_hint_datetimeformattz(self):
+        datetimeformattz = self.hints.datetimeformattz
 
-    # timeonlyformat: Valid values: "HH12:MI AM" (e.g., "1:00 PM"),
-    # "HH24:MI:SS" (e.g., "13:00:00")
+        # datetimeformattz: Valid values: "YYYY-MM-DD HH:MI:SSOF",
+        # "YYYY-MM-DD HH:MI:SS", "YYYY-MM-DD HH24:MI:SSOF", "YYYY-MM-DD
+        # HH24:MI:SSOF", "MM/DD/YY HH24:MI". See Redshift docs for more
+        # information (note that HH: is equivalent to HH24: and that if
+        # you don't provide an offset (OF), times are assumed to be in
+        # UTC).
+
+        # Default value is "YYYY-MM-DD HH:MI:SSOF".
+
+        #
+        # To get a postgres database to test these cases with:
+        #
+        # cd tests/integration
+        # ./itest shell
+        # db dockerized-postgres
+        if datetimeformattz in ['YYYY-MM-DD HH:MI:SSOF',
+                                'YYYY-MM-DD HH24:MI:SSOF']:
+            #
+            #  postgres=# select timestamptz '2020-01-01 23:01:01-10';
+            #        timestamptz
+            #  ------------------------
+            #   2020-01-02 09:01:01+00
+            #  (1 row)
+            #
+            #  postgres=#
+
+            # Any DateStyle will do as this is unambiguous
+            quiet_remove(self.unhandled_hints, 'datetimeformattz')
+        elif datetimeformattz == 'YYYY-MM-DD HH:MI:SS':
+            #
+            #
+            #  postgres=# select timestamptz '2020-01-01 23:01:01';
+            #        timestamptz
+            #  ------------------------
+            #   2020-01-01 23:01:01+00
+            #  (1 row)
+            #
+            #  postgres=#
+
+            # Any DateStyle will do as this is unambiguous
+            quiet_remove(self.unhandled_hints, 'datetimeformattz')
+        elif datetimeformattz == "MM/DD/YY HH24:MI":
+            # "MM/DD/YY HH24:MI"
+            #
+            #  postgres=# select timestamptz '01/02/2999 23:01';
+            #        timestamptz
+            #  ------------------------
+            #   2999-01-02 23:01:00+00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('MDY', 'datetimeformattz')
+        elif datetimeformattz == 'DD-MM-YY HH:MI:SSOF':
+            #  postgres=# select timestamptz '02-01-2999 23:01:01-10';
+            #        timestamptz
+            #  ------------------------
+            #   2999-02-02 09:01:01+00
+            #  (1 row)
+            #
+            self.upgrade_date_order_style('DMY', 'datetimeformattz')
+        elif datetimeformattz == 'DD/MM/YY HH:MI:SSOF':
+            #  postgres=# select timestamptz '02/01/99 23:01:01-10';
+            #        timestamptz
+            #  ------------------------
+            #   1999-02-02 09:01:01+00
+            #  (1 row)
+            #
+            self.upgrade_date_order_style('DMY', 'datetimeformattz')
+        elif datetimeformattz == 'DD-MM-YYYY HH:MI:SSOF':
+            #  postgres=# select timestamptz '02-01-1999 23:01:01-10';
+            #        timestamptz
+            #  ------------------------
+            #   1999-02-02 09:01:01+00
+            #  (1 row)
+            #
+            self.upgrade_date_order_style('DMY', 'datetimeformattz')
+        elif datetimeformattz == 'MM/DD/YY HH:MI:SSOF':
+            #  postgres=# select timestamptz '01/02/99 23:01:01-10';
+            #        timestamptz
+            #  ------------------------
+            #   1999-01-03 09:01:01+00
+            #  (1 row)
+            #
+            self.upgrade_date_order_style('MDY', 'datetimeformattz')
+        elif datetimeformattz == 'MM-DD-YYYY HH:MI:SSOF':
+            #  postgres=# select timestamptz '01-02-1999 23:01:01-10';
+            #        timestamptz
+            #  ------------------------
+            #   1999-01-03 09:01:01+00
+            #  (1 row)
+            #
+            self.upgrade_date_order_style('MDY', 'datetimeformattz')
+        else:
+            cant_handle_hint(self.fail_if_cant_handle_hint,
+                             'datetimeformattz', self.hints)
 
-    if timeonlyformat == "HH12:MI AM":
-        # "HH12:MI AM" (e.g., "1:00 PM"),
-        #
-        #  postgres=# select time '1:00 PM';
-        #     time
-        #  ----------
-        #   13:00:00
-        #  (1 row)
-        #
-        #  postgres=#
+    def process_hint_datetimeformat(self):
+        # datetimeformat: Valid values: "YYYY-MM-DD HH24:MI:SS",
+        # "YYYY-MM-DD HH12:MI AM", "MM/DD/YY HH24:MI". See Redshift docs
+        # for more information.
+
+        datetimeformat = self.hints.datetimeformat
+
+        if datetimeformat in ("YYYY-MM-DD HH24:MI:SS",
+                              "YYYY-MM-DD HH:MI:SS"):
+            #
+            #  postgres=# select timestamp '2020-01-02 15:13:12';
+            #        timestamp
+            #  ---------------------
+            #   2020-01-02 15:13:12
+            #  (1 row)
+            #
+            #  postgres=#
+
+            # Any DateStyle will do as this is unambiguous
+            quiet_remove(self.unhandled_hints, 'datetimeformat')
+        elif datetimeformat == "YYYY-MM-DD HH12:MI AM":
+            # "YYYY-MM-DD HH12:MI AM"
+            #
+            #  postgres=# select timestamp '2020-01-02 1:13 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-01-02 13:13:00
+            #  (1 row)
+            #
+            #  postgres=#
+
+            # Any DateStyle will do as this is unambiguous
+            quiet_remove(self.unhandled_hints, 'datetimeformat')
+        elif datetimeformat == "MM/DD/YY HH24:MI":
+            #  postgres=# select timestamp '01/02/20 15:23';
+            #        timestamp
+            #  ---------------------
+            #   2020-01-02 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+
+            self.upgrade_date_order_style('MDY', 'datetimeformat')
+        elif datetimeformat == 'DD-MM-YY HH12:MI AM':
+            #  postgres=# select timestamp '02-01-20 3:23 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-02-01 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('DMY', 'datetimeformat')
+        elif datetimeformat == 'DD/MM/YY HH12:MI AM':
+            #  postgres=# select timestamp '02/01/20 3:23 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-02-01 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('DMY', 'datetimeformat')
+        elif datetimeformat == 'DD-MM-YYYY HH12:MI AM':
+            #  postgres=# select timestamp '02-01-2020 3:23 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-02-01 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('DMY', 'datetimeformat')
+        elif datetimeformat == 'MM-DD-YY HH12:MI AM':
+            #  postgres=# select timestamp '02-01-20 3:23 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-02-01 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('MDY', 'datetimeformat')
+        elif datetimeformat == 'MM/DD/YY HH12:MI AM':
+            #  postgres=# select timestamp '02/01/20 3:23 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-02-01 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('MDY', 'datetimeformat')
+        elif datetimeformat == 'MM-DD-YYYY HH12:MI AM':
+            #  postgres=# select timestamp '01-02-2020 3:23 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-01-02 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('MDY', 'datetimeformat')
+        elif datetimeformat == 'MM-DD-YYYY HH:MI:SS':
+            #  postgres=# select timestamp '01-02-2020 3:23 PM';
+            #        timestamp
+            #  ---------------------
+            #   2020-01-02 15:23:00
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('MDY', 'datetimeformat')
+        else:
+            cant_handle_hint(self.fail_if_cant_handle_hint,
+                             'datetimeformat', self.hints)
 
-        # Supported!
-        quiet_remove(unhandled_hints, 'timeonlyformat')
-    elif timeonlyformat == "HH24:MI:SS":
+    def process_hint_timeonlyformat(self):
+        timeonlyformat = self.hints.timeonlyformat
 
+        # timeonlyformat: Valid values: "HH12:MI AM" (e.g., "1:00 PM"),
         # "HH24:MI:SS" (e.g., "13:00:00")
-        #
-        #  postgres=# select time '13:00:00';
-        #     time
-        #  ----------
-        #   13:00:00
-        #  (1 row)
-        #
-        #  postgres=#
 
-        # Supported!
-        quiet_remove(unhandled_hints, 'timeonlyformat')
-    elif timeonlyformat == "HH:MI:SS":
-        #  postgres=# select time '13:00:00';
-        #     time
-        #  ----------
-        #   13:00:00
-        #  (1 row)
-        #
-        #  postgres=#
-        quiet_remove(unhandled_hints, 'timeonlyformat')
-    elif timeonlyformat == "HH24:MI":
+        if timeonlyformat == "HH12:MI AM":
+            # "HH12:MI AM" (e.g., "1:00 PM"),
+            #
+            #  postgres=# select time '1:00 PM';
+            #     time
+            #  ----------
+            #   13:00:00
+            #  (1 row)
+            #
+            #  postgres=#
+
+            # Supported!
+            quiet_remove(self.unhandled_hints, 'timeonlyformat')
+        elif timeonlyformat == "HH24:MI:SS":
+
+            # "HH24:MI:SS" (e.g., "13:00:00")
+            #
+            #  postgres=# select time '13:00:00';
+            #     time
+            #  ----------
+            #   13:00:00
+            #  (1 row)
+            #
+            #  postgres=#
+
+            # Supported!
+            quiet_remove(self.unhandled_hints, 'timeonlyformat')
+        elif timeonlyformat == "HH:MI:SS":
+            #  postgres=# select time '13:00:00';
+            #     time
+            #  ----------
+            #   13:00:00
+            #  (1 row)
+            #
+            #  postgres=#
+            quiet_remove(self.unhandled_hints, 'timeonlyformat')
+        elif timeonlyformat == "HH24:MI":
+
+            # "HH24:MI" (e.g., "13:00")
+            #
+            #  postgres=# select time '13:00';
+            #     time
+            #  ----------
+            #   13:00:00
+            #  (1 row)
+            #
+            #  postgres=#
 
-        # "HH24:MI" (e.g., "13:00")
-        #
-        #  postgres=# select time '13:00';
-        #     time
-        #  ----------
-        #   13:00:00
-        #  (1 row)
-        #
-        #  postgres=#
+            # Supported!
+            quiet_remove(self.unhandled_hints, 'timeonlyformat')
+        else:
+            cant_handle_hint(self.fail_if_cant_handle_hint, 'timeonlyformat', self.hints)
 
-        # Supported!
-        quiet_remove(unhandled_hints, 'timeonlyformat')
-    else:
-        cant_handle_hint(fail_if_cant_handle_hint, 'timeonlyformat', hints)
-
-    # dateformat: Valid values: null, "YYYY-MM-DD", "MM-DD-YYYY", "DD-MM-YYYY", "MM/DD/YY".
-    dateformat = hints.dateformat
-
-    if dateformat == "YYYY-MM-DD":
-        #  postgres=# select date '1999-01-02';
-        #      date
-        #  ------------
-        #   1999-01-02
-        #  (1 row)
-        #
-        #  postgres=#
-        # Any DateStyle will do as this is unambiguous
-        quiet_remove(unhandled_hints, 'dateformat')
-    elif dateformat == "MM-DD-YYYY":
-        # "MM-DD-YYYY"
-        #
-        #  postgres=# select date '01-02-1999';
-        #      date
-        #  ------------
-        #   1999-01-02
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('MDY', 'dateformat')
-    elif dateformat == "DD-MM-YYYY":
-        # "DD-MM-YYYY" - not supported by default, need to switch to
-        # DMY:
-        #
-        #  postgres=# select date '02-01-1999';
-        #      date
-        #  ------------
-        #   1999-02-01
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('DMY', 'dateformat')
-    elif dateformat == "DD-MM-YY":
-        #  postgres=# select date '02-01-99';
-        #      date
-        #  ------------
-        #   1999-02-01
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('DMY', 'dateformat')
-    elif dateformat == "MM/DD/YY":
-        # "MM/DD/YY".
-        #
-        #  postgres=# select date '01/02/99';
-        #      date
-        #  ------------
-        #   1999-01-02
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('MDY', 'dateformat')
-    elif dateformat == "DD/MM/YY":
-        #  postgres=# select date '02/01/99';
-        #      date
-        #  ------------
-        #   1999-02-01
-        #  (1 row)
-        #
-        #  postgres=#
-        upgrade_date_order_style('DMY', 'dateformat')
-    elif dateformat is None:
-        # null implies that that date format is unknown, and that the
-        # implementation SHOULD generate using their default value and
-        # parse permissively.
-
-        # ...which is what Postgres does!
-        quiet_remove(unhandled_hints, 'dateformat')
-    else:
-        cant_handle_hint(fail_if_cant_handle_hint, 'dateformat', hints)
+    def process_hint_dateformat(self):
+        # dateformat: Valid values:
+        # null, "YYYY-MM-DD", "MM-DD-YYYY", "DD-MM-YYYY", "MM/DD/YY".
+        dateformat = self.hints.dateformat
+
+        if dateformat == "YYYY-MM-DD":
+            #  postgres=# select date '1999-01-02';
+            #      date
+            #  ------------
+            #   1999-01-02
+            #  (1 row)
+            #
+            #  postgres=#
+            # Any DateStyle will do as this is unambiguous
+            quiet_remove(self.unhandled_hints, 'dateformat')
+        elif dateformat == "MM-DD-YYYY":
+            # "MM-DD-YYYY"
+            #
+            #  postgres=# select date '01-02-1999';
+            #      date
+            #  ------------
+            #   1999-01-02
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('MDY', 'dateformat')
+        elif dateformat == "DD-MM-YYYY":
+            # "DD-MM-YYYY" - not supported by default, need to switch to
+            # DMY:
+            #
+            #  postgres=# select date '02-01-1999';
+            #      date
+            #  ------------
+            #   1999-02-01
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('DMY', 'dateformat')
+        elif dateformat == "DD-MM-YY":
+            #  postgres=# select date '02-01-99';
+            #      date
+            #  ------------
+            #   1999-02-01
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('DMY', 'dateformat')
+        elif dateformat == "MM/DD/YY":
+            # "MM/DD/YY".
+            #
+            #  postgres=# select date '01/02/99';
+            #      date
+            #  ------------
+            #   1999-01-02
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('MDY', 'dateformat')
+        elif dateformat == "DD/MM/YY":
+            #  postgres=# select date '02/01/99';
+            #      date
+            #  ------------
+            #   1999-02-01
+            #  (1 row)
+            #
+            #  postgres=#
+            self.upgrade_date_order_style('DMY', 'dateformat')
+        elif dateformat is None:
+            # null implies that that date format is unknown, and that the
+            # implementation SHOULD generate using their default value and
+            # parse permissively.
 
-    return date_order_style
+            # ...which is what Postgres does!
+            quiet_remove(self.unhandled_hints, 'dateformat')
+        else:
+            cant_handle_hint(self.fail_if_cant_handle_hint,
+                             'dateformat', self.hints)
```

### Comparing `records-mover-1.5.3/records_mover/db/postgres/copy_options/date_output_style.py` & `records-mover-1.5.4/records_mover/db/postgres/copy_options/date_output_style.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/copy_options/text.py` & `records-mover-1.5.4/records_mover/db/postgres/copy_options/text.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/copy_options/types.py` & `records-mover-1.5.4/records_mover/db/postgres/copy_options/types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/loader.py` & `records-mover-1.5.4/records_mover/db/postgres/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/postgres_db_driver.py` & `records-mover-1.5.4/records_mover/db/postgres/postgres_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/sqlalchemy_postgres_copy.py` & `records-mover-1.5.4/records_mover/db/postgres/sqlalchemy_postgres_copy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/postgres/unloader.py` & `records-mover-1.5.4/records_mover/db/postgres/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/quoting.py` & `records-mover-1.5.4/records_mover/db/quoting.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/redshift/loader.py` & `records-mover-1.5.4/records_mover/db/redshift/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/redshift/records_unload.py` & `records-mover-1.5.4/records_mover/db/redshift/records_unload.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/redshift/redshift_db_driver.py` & `records-mover-1.5.4/records_mover/db/redshift/redshift_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/redshift/sql.py` & `records-mover-1.5.4/records_mover/db/redshift/sql.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/redshift/unloader.py` & `records-mover-1.5.4/records_mover/db/redshift/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/unloader.py` & `records-mover-1.5.4/records_mover/db/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/vertica/export_sql.py` & `records-mover-1.5.4/records_mover/db/vertica/export_sql.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/vertica/import_sql.py` & `records-mover-1.5.4/records_mover/db/vertica/import_sql.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/vertica/loader.py` & `records-mover-1.5.4/records_mover/db/vertica/loader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/vertica/records_export_options.py` & `records-mover-1.5.4/records_mover/db/vertica/records_export_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/vertica/records_import_options.py` & `records-mover-1.5.4/records_mover/db/vertica/records_import_options.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/vertica/unloader.py` & `records-mover-1.5.4/records_mover/db/vertica/unloader.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/db/vertica/vertica_db_driver.py` & `records-mover-1.5.4/records_mover/db/vertica/vertica_db_driver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/logging.py` & `records-mover-1.5.4/records_mover/logging.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/mover_types.py` & `records-mover-1.5.4/records_mover/mover_types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/pandas/__init__.py` & `records-mover-1.5.4/records_mover/pandas/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,11 +25,12 @@
     # Some spreadsheets will drop a trailing ',' after the
     # last column in the header with actual content when
     # exporting to CSV, leaving you with an empty column.
     # Pandas helpfully names this empty column for you as
     # "unnamed: 1", or maybe "Unnamed: 1" (not sure why/when
     # that differs).  Let's clean those up.
     for column in df:
-        if column.startswith('Unnamed: ') or column.startswith('unnamed: '):
-            if not df[column].notnull().any():
-                df = df.drop(column, axis=1)
+        if type(column) == str:
+            if column.startswith('Unnamed: ') or column.startswith('unnamed: '):
+                if not df[column].notnull().any():
+                    df = df.drop(column, axis=1)
     return df
```

### Comparing `records-mover-1.5.3/records_mover/records/__init__.py` & `records-mover-1.5.4/records_mover/records/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/base_records_format.py` & `records-mover-1.5.4/records_mover/records/base_records_format.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/cli.py` & `records-mover-1.5.4/records_mover/records/cli.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/__init__.py` & `records-mover-1.5.4/records_mover/records/delimited/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/compression.py` & `records-mover-1.5.4/records_mover/records/delimited/compression.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/conversions.py` & `records-mover-1.5.4/records_mover/records/delimited/conversions.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/csv_streamer.py` & `records-mover-1.5.4/records_mover/records/delimited/csv_streamer.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,26 +40,14 @@
         'encoding': python_encoding_from_hint.get(encoding_hint, encoding_hint),
         'header': header,
         'compression': pandas_compression_from_hint[compression_hint],
         'escapechar': hints.get('escape'),
         'iterator': True,
         'engine': 'python'
     }
-    if header is None:
-        # Pandas only accepts the prefix argument (which makes for
-        # tidier column names when otherwise not provided) when the
-        # header is explicitly marked as missing, not when it's
-        # available or even when we ask Pandas to infer it.  Bummer,
-        # as this means that when Pandas infers that there's no
-        # header, the column names will end up different than folks
-        # explicitly tell records mover that there is no header.
-        #
-        # https://github.com/pandas-dev/pandas/issues/27394
-        # https://github.com/pandas-dev/pandas/pull/31383
-        kwargs['prefix'] = 'untitled_'
     if 'quoting' in hints:
         quoting = hints['quoting']
         kwargs['quoting'] = pandas_quoting_from_hint[quoting]
     # The streaming code from pandas demands a text stream if we're
     # dealing with an uncompressed CSV file, and a binary stream
     # if we're dealing with compressed file.
     if isinstance(filepath_or_buffer, str):
```

### Comparing `records-mover-1.5.3/records_mover/records/delimited/hint.py` & `records-mover-1.5.4/records_mover/records/delimited/hint.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/hints.py` & `records-mover-1.5.4/records_mover/records/delimited/hints.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/sniff.py` & `records-mover-1.5.4/records_mover/records/delimited/sniff.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/types.py` & `records-mover-1.5.4/records_mover/records/delimited/types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/utils.py` & `records-mover-1.5.4/records_mover/records/delimited/utils.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/delimited/validated_records_hints.py` & `records-mover-1.5.4/records_mover/records/delimited/validated_records_hints.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/deprecated.py` & `records-mover-1.5.4/records_mover/records/deprecated.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/existing_table_handling.py` & `records-mover-1.5.4/records_mover/records/existing_table_handling.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/job/config.py` & `records-mover-1.5.4/records_mover/records/job/config.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/job/mover.py` & `records-mover-1.5.4/records_mover/records/job/mover.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/job/schema.py` & `records-mover-1.5.4/records_mover/records/job/schema.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/mover.py` & `records-mover-1.5.4/records_mover/records/mover.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/pandas/__init__.py` & `records-mover-1.5.4/records_mover/records/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/pandas/prep_for_csv.py` & `records-mover-1.5.4/records_mover/records/pandas/prep_for_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,9 +106,9 @@
     for index, field in enumerate(remaining_fields):
         series = formatted_df.iloc[:, index]
         formatted_series = _convert_series_or_index(series,
                                                     field,
                                                     records_format,
                                                     processing_instructions)
         if formatted_series is not None:
-            formatted_df.iloc[:, index] = formatted_series
+            formatted_df[formatted_df.columns[index]] = formatted_series
     return formatted_df
```

### Comparing `records-mover-1.5.3/records_mover/records/pandas/read_csv_options.py` & `records-mover-1.5.4/records_mover/records/pandas/read_csv_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from ...utils import quiet_remove
 from ..delimited import cant_handle_hint
 from ..processing_instructions import ProcessingInstructions
 from ..records_format import DelimitedRecordsFormat
 from records_mover.records.schema import RecordsSchema
 import logging
 from typing import Set, Dict, Any
+from packaging import version
+import pandas as pd
 
 
 logger = logging.getLogger(__name__)
 
 # flake8: noqa: C901
 def pandas_read_csv_options(records_format: DelimitedRecordsFormat,
                             records_schema: RecordsSchema,
@@ -143,37 +145,14 @@
     #
     # If the parsed data only contains one column then return a Series.
     #
     # (better to keep a standard format, no matter how many columsn)
     #
 
     #
-    # prefix : str, optional
-    #
-    # Prefix to add to column numbers when no header, e.g. ‘X’ for X0, X1,
-    #
-
-    #
-    # Not sure this actually does anything - when loading a CSV format
-    # file with an empty final column name - e.g.,
-    # tests/integration/resources/delimited-csv-with-header.csv - the
-    # column still comes out as 'unnamed: 11'ead as 'untitled_11'.
-    #
-    # Leaving this in case a future version of Pandas behaves
-    # better.
-    #
-    if pandas_options['header'] is None:
-        # Pandas only accepts the prefix argument when the
-        # header is marked as missing.
-        #
-        # https://github.com/pandas-dev/pandas/issues/27394
-        # https://github.com/pandas-dev/pandas/pull/31383
-        pandas_options['prefix'] = 'untitled_'
-
-    #
     # mangle_dupe_cols : bool, default True
     #
     # Duplicate columns will be specified as ‘X’, ‘X.1’, …’X.N’,
     # rather than ‘X’…’X’. Passing in False will cause data to be
     # overwritten if there are duplicate names in the columns.
     #
 
@@ -518,15 +497,18 @@
 
     #
     # lineterminator : str (length 1), optional
     #
     # Character to break file into lines. Only valid with C parser.
     #
     if non_standard_record_terminator:
-        pandas_options['lineterminator'] = hints.record_terminator
+        if version.parse(pd.__version__) >= version.parse('1.5.0'):
+            pandas_options['lineterminator'] = hints.record_terminator
+        else:
+            pandas_options['line_terminator'] = hints.record_terminator
     quiet_remove(unhandled_hints, 'record-terminator')
 
     #
     # quotechar : str (length 1), optional
     #
     # The character used to denote the start and end of a quoted
     # item. Quoted items can include the delimiter and it will be
@@ -626,33 +608,31 @@
     # Deprecated since version 0.21.0: This argument will be removed
     # and will always convert to MultiIndex
     #
 
     # (deprecated, so not supplying)
 
     #
-    # error_bad_lines : bool, default True
+    # on_bad_lines : string default 'error'
     #
     # Lines with too many fields (e.g. a csv line with too many
     # commas) will by default cause an exception to be raised, and no
     # DataFrame will be returned. If False, then these “bad lines”
     # will dropped from the DataFrame that is returned.
     #
 
-    pandas_options['error_bad_lines'] = processing_instructions.fail_if_row_invalid
+    pandas_options['on_bad_lines'] = 'error' if processing_instructions.fail_if_row_invalid else 'warn'
 
     #
-    # warn_bad_lines : bool, default True
+    #  
     #
-    # If error_bad_lines is False, and warn_bad_lines is True, a
+    # If processing_instructions.fail_if_row_invalid is False, a
     # warning for each “bad line” will be output.
     #
 
-    pandas_options['warn_bad_lines'] = True
-
     #
     # delim_whitespace : bool, default False
     #
     # Specifies whether or not whitespace (e.g. ' ' or ' ') will be
     # used as the sep. Equivalent to setting sep='\s+'. If this option
     # is set to True, nothing should be passed in for the delimiter
     # parameter.
```

### Comparing `records-mover-1.5.3/records_mover/records/pandas/to_csv_options.py` & `records-mover-1.5.4/records_mover/records/pandas/to_csv_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from ...utils import quiet_remove
 from ..delimited import cant_handle_hint
 from ..processing_instructions import ProcessingInstructions
 from ..records_format import DelimitedRecordsFormat
 from records_mover.mover_types import _assert_never
 import logging
 from typing import Set, Dict
+from packaging import version
+import pandas as pd
 
 
 logger = logging.getLogger(__name__)
 
 
 def pandas_to_csv_options(records_format: DelimitedRecordsFormat,
                           unhandled_hints: Set[str],
@@ -107,11 +109,14 @@
     # .to_csv() call.
     quiet_remove(unhandled_hints, 'timeonlyformat')
     quiet_remove(unhandled_hints, 'dateformat')
 
     pandas_options['sep'] = hints.field_delimiter
     quiet_remove(unhandled_hints, 'field-delimiter')
 
-    pandas_options['line_terminator'] = hints.record_terminator
+    if version.parse(pd.__version__) >= version.parse('1.5.0'):
+        pandas_options['lineterminator'] = hints.record_terminator
+    else:
+        pandas_options['line_terminator'] = hints.record_terminator
     quiet_remove(unhandled_hints, 'record-terminator')
 
     return pandas_options
```

### Comparing `records-mover-1.5.3/records_mover/records/prep.py` & `records-mover-1.5.4/records_mover/records/prep.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/prep_and_load.py` & `records-mover-1.5.4/records_mover/records/prep_and_load.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/processing_instructions.py` & `records-mover-1.5.4/records_mover/records/processing_instructions.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/records.py` & `records-mover-1.5.4/records_mover/records/records.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/records_directory.py` & `records-mover-1.5.4/records_mover/records/records_directory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/records_format.py` & `records-mover-1.5.4/records_mover/records/records_format.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/records_format_file.py` & `records-mover-1.5.4/records_mover/records/records_format_file.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/records_schema_json_file.py` & `records-mover-1.5.4/records_mover/records/records_schema_json_file.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/records_types.py` & `records-mover-1.5.4/records_mover/records/records_types.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/results.py` & `records-mover-1.5.4/records_mover/records/results.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/__init__.py` & `records-mover-1.5.4/records_mover/records/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/__init__.py` & `records-mover-1.5.4/records_mover/records/schema/field/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/constraints/constraints.py` & `records-mover-1.5.4/records_mover/records/schema/field/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/constraints/decimal.py` & `records-mover-1.5.4/records_mover/records/schema/field/constraints/decimal.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/constraints/integer.py` & `records-mover-1.5.4/records_mover/records/schema/field/constraints/integer.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/constraints/string.py` & `records-mover-1.5.4/records_mover/records/schema/field/constraints/string.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/numpy.py` & `records-mover-1.5.4/records_mover/records/schema/field/numpy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/pandas.py` & `records-mover-1.5.4/records_mover/records/schema/field/pandas.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/representation.py` & `records-mover-1.5.4/records_mover/records/schema/field/representation.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/sqlalchemy.py` & `records-mover-1.5.4/records_mover/records/schema/field/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/statistics.py` & `records-mover-1.5.4/records_mover/records/schema/field/statistics.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/field/string_length_generator.py` & `records-mover-1.5.4/records_mover/records/schema/field/string_length_generator.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/schema/__init__.py` & `records-mover-1.5.4/records_mover/records/schema/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/schema/known_representation.py` & `records-mover-1.5.4/records_mover/records/schema/schema/known_representation.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/schema/pandas.py` & `records-mover-1.5.4/records_mover/records/schema/schema/pandas.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/schema/schema/sqlalchemy.py` & `records-mover-1.5.4/records_mover/records/schema/schema/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/base.py` & `records-mover-1.5.4/records_mover/records/sources/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/data_url.py` & `records-mover-1.5.4/records_mover/records/sources/data_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/dataframes.py` & `records-mover-1.5.4/records_mover/records/sources/dataframes.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/directory.py` & `records-mover-1.5.4/records_mover/records/sources/directory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/factory.py` & `records-mover-1.5.4/records_mover/records/sources/factory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/fileobjs.py` & `records-mover-1.5.4/records_mover/records/sources/fileobjs.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/google_sheets.py` & `records-mover-1.5.4/records_mover/records/sources/google_sheets.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/table.py` & `records-mover-1.5.4/records_mover/records/sources/table.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/sources/uninferred_fileobjs.py` & `records-mover-1.5.4/records_mover/records/sources/uninferred_fileobjs.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/table.py` & `records-mover-1.5.4/records_mover/records/table.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/base.py` & `records-mover-1.5.4/records_mover/records/targets/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/data_url.py` & `records-mover-1.5.4/records_mover/records/targets/data_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/directory_from_url.py` & `records-mover-1.5.4/records_mover/records/targets/directory_from_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/factory.py` & `records-mover-1.5.4/records_mover/records/targets/factory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/fileobj.py` & `records-mover-1.5.4/records_mover/records/targets/fileobj.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,14 +70,14 @@
         # (bleh).  Instead, if compression is set, write to a temp
         # file first.
         if self.records_format.hints['compression'] is None:
             text_fileobj = io.TextIOWrapper(self.fileobj, encoding=encoding)
             move_count = write_dfs(text_fileobj)
             text_fileobj.detach()
         else:
-            with NamedTemporaryFile(prefix='mover_fileobj_target') as output_file:
+            with NamedTemporaryFile(prefix='mover_fileobj_target') as output_file: # noqa
                 move_count = write_dfs(output_file.name)
                 with open(output_file.name, "rb") as output_fileobj:
-                    copyfileobj(output_fileobj, self.fileobj)
+                    copyfileobj(output_fileobj, self.fileobj)  # type: ignore
 
         logger.info('CSV file written')
         return MoveResult(output_urls=None, move_count=move_count)
```

### Comparing `records-mover-1.5.3/records_mover/records/targets/google_sheets.py` & `records-mover-1.5.4/records_mover/records/targets/google_sheets.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/spectrum.py` & `records-mover-1.5.4/records_mover/records/targets/spectrum.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/table/base.py` & `records-mover-1.5.4/records_mover/records/targets/table/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/table/move_from_dataframes_source.py` & `records-mover-1.5.4/records_mover/records/targets/table/move_from_dataframes_source.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/table/move_from_fileobjs_source.py` & `records-mover-1.5.4/records_mover/records/targets/table/move_from_fileobjs_source.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/table/move_from_records_directory.py` & `records-mover-1.5.4/records_mover/records/targets/table/move_from_records_directory.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py` & `records-mover-1.5.4/records_mover/records/targets/table/move_from_temp_loc_after_filling_it.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/records/targets/table/target.py` & `records-mover-1.5.4/records_mover/records/targets/table/target.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/session.py` & `records-mover-1.5.4/records_mover/session.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/base.py` & `records-mover-1.5.4/records_mover/url/base.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/filesystem.py` & `records-mover-1.5.4/records_mover/url/filesystem.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/gcs/gcs_directory_url.py` & `records-mover-1.5.4/records_mover/url/gcs/gcs_directory_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/gcs/gcs_file_url.py` & `records-mover-1.5.4/records_mover/url/gcs/gcs_file_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/resolver.py` & `records-mover-1.5.4/records_mover/url/resolver.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/s3/awscli.py` & `records-mover-1.5.4/records_mover/url/s3/awscli.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/s3/s3_base_url.py` & `records-mover-1.5.4/records_mover/url/s3/s3_base_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/s3/s3_directory_url.py` & `records-mover-1.5.4/records_mover/url/s3/s3_directory_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/s3/s3_file_url.py` & `records-mover-1.5.4/records_mover/url/s3/s3_file_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/url/s3/s3_url.py` & `records-mover-1.5.4/records_mover/url/s3/s3_url.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/__init__.py` & `records-mover-1.5.4/records_mover/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/concat_files.py` & `records-mover-1.5.4/records_mover/utils/concat_files.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/json_schema.py` & `records-mover-1.5.4/records_mover/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/json_schema_array_document.py` & `records-mover-1.5.4/records_mover/utils/json_schema_array_document.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/json_schema_document.py` & `records-mover-1.5.4/records_mover/utils/json_schema_document.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/lazyprop.py` & `records-mover-1.5.4/records_mover/utils/lazyprop.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/limits.py` & `records-mover-1.5.4/records_mover/utils/limits.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/retry.py` & `records-mover-1.5.4/records_mover/utils/retry.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/rewound_fileobj.py` & `records-mover-1.5.4/records_mover/utils/rewound_fileobj.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover/utils/structures.py` & `records-mover-1.5.4/records_mover/utils/structures.py`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover.egg-info/PKG-INFO` & `records-mover-1.5.4/records_mover.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: records-mover
-Version: 1.5.3
+Version: 1.5.4
 Summary: Library and CLI to move relational data from one place to another - DBs/CSV/gsheets/dataframes/...
 Home-page: UNKNOWN
 Author: Vince Broz
 Author-email: opensource@bluelabs.com
 License: Apache Software License
-Download-URL: https://github.com/bluelabsio/records-mover/tarball/1.5.3
+Download-URL: https://github.com/bluelabsio/records-mover/tarball/1.5.4
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database :: Front-Ends
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -42,14 +42,16 @@
 
 <img
  src="https://raw.githubusercontent.com/bluelabsio/records-mover/master/docs/records-mover-horizontal.png"
  alt="Records Mover">
 
 [![Documentation Status](https://readthedocs.org/projects/records-mover/badge/?version=latest)](https://records-mover.readthedocs.io/en/latest/?badge=latest)
 
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/bluelabsio/records-mover/tree/main.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/bluelabsio/records-mover/tree/main)
+
 Records mover is a command-line tool and Python library you can
 use to move relational data from one place to another.
 
 Relational data here means anything roughly "rectangular" - with
 columns and rows.  For example, it supports reading and writing from:
 
 * Databases, including using native high-speed methods of
```

### Comparing `records-mover-1.5.3/records_mover.egg-info/SOURCES.txt` & `records-mover-1.5.4/records_mover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/records_mover.egg-info/requires.txt` & `records-mover-1.5.4/records_mover.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 sqlalchemy<2.0,>=1.4
 
 [mysql]
 pymysql
 sqlalchemy<2.0,>=1.4
 
 [pandas]
-pandas<2,>=1.1.5
+pandas<2,>=1.3.5
 
 [parquet]
 pyarrow
 
 [postgres-binary]
 psycopg2-binary
 sqlalchemy<2.0,>=1.4
@@ -174,14 +174,14 @@
 pymysql
 sqlalchemy<2.0,>=1.4
 awscli<2,>=1
 boto<3,>=2
 boto3
 s3-concat<0.2,>=0.1.7
 smart_open>=2
-pandas<2,>=1.1.5
+pandas<2,>=1.3.5
 google-cloud-storage
 smart_open>=2
 
 [vertica]
 sqlalchemy-vertica-python<0.6,>=0.5.5
 sqlalchemy<2.0,>=1.4
```

### Comparing `records-mover-1.5.3/setup.cfg` & `records-mover-1.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `records-mover-1.5.3/setup.py` & `records-mover-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 ] + google_api_client_dependencies
 
 parquet_dependencies = [
     'pyarrow'
 ]
 
 pandas_dependencies = [
-    'pandas>=1.1.5,<2',
+    'pandas>=1.3.5,<2',
 ]
 
 mysql_dependencies = [
     'pymysql'
 ] + db_dependencies
 
 redshift_dependencies_base = [
```

