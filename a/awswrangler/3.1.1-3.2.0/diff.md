# Comparing `tmp/awswrangler-3.1.1.tar.gz` & `tmp/awswrangler-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awswrangler-3.1.1.tar", max compression
+gzip compressed data, was "awswrangler-3.2.0.tar", max compression
```

## Comparing `awswrangler-3.1.1.tar` & `awswrangler-3.2.0.tar`

### file list

```diff
@@ -1,145 +1,153 @@
--rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.1.1/LICENSE.txt
--rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.1.1/NOTICE.txt
--rw-r--r--   0        0        0    19946 2023-05-16 00:05:56.635964 awswrangler-3.1.1/README.md
--rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.1.1/THIRD_PARTY.txt
--rw-r--r--   0        0        0     1405 2023-04-21 16:06:31.383067 awswrangler-3.1.1/awswrangler/__init__.py
--rw-r--r--   0        0        0      276 2023-05-16 00:05:56.636826 awswrangler-3.1.1/awswrangler/__metadata__.py
--rw-r--r--   0        0        0     4359 2023-04-25 15:43:59.617624 awswrangler-3.1.1/awswrangler/_arrow.py
--rw-r--r--   0        0        0    27916 2023-05-02 21:22:41.635980 awswrangler-3.1.1/awswrangler/_config.py
--rw-r--r--   0        0        0    31116 2023-04-25 15:43:59.618486 awswrangler-3.1.1/awswrangler/_data_types.py
--rw-r--r--   0        0        0    13202 2023-05-02 20:57:29.199914 awswrangler-3.1.1/awswrangler/_databases.py
--rw-r--r--   0        0        0     6169 2023-04-21 16:06:31.387129 awswrangler-3.1.1/awswrangler/_distributed.py
--rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.1.1/awswrangler/_executor.py
--rw-r--r--   0        0        0     6211 2023-04-21 16:06:31.388148 awswrangler-3.1.1/awswrangler/_sql_formatter.py
--rw-r--r--   0        0        0    28878 2023-04-25 15:43:59.619218 awswrangler-3.1.1/awswrangler/_utils.py
--rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.1.1/awswrangler/annotations.py
--rw-r--r--   0        0        0     1190 2023-05-05 17:01:05.124627 awswrangler-3.1.1/awswrangler/athena/__init__.py
--rw-r--r--   0        0        0     9301 2023-04-21 16:06:31.390689 awswrangler-3.1.1/awswrangler/athena/_cache.py
--rw-r--r--   0        0        0     9681 2023-05-05 17:01:05.124758 awswrangler-3.1.1/awswrangler/athena/_executions.py
--rw-r--r--   0        0        0     2148 2023-05-05 17:01:05.124846 awswrangler-3.1.1/awswrangler/athena/_executions.pyi
--rw-r--r--   0        0        0    54600 2023-05-16 00:05:56.637451 awswrangler-3.1.1/awswrangler/athena/_read.py
--rw-r--r--   0        0        0    11526 2023-05-05 17:01:05.125558 awswrangler-3.1.1/awswrangler/athena/_read.pyi
--rw-r--r--   0        0        0    41939 2023-05-05 17:01:05.126045 awswrangler-3.1.1/awswrangler/athena/_utils.py
--rw-r--r--   0        0        0     7073 2023-05-05 17:01:05.126400 awswrangler-3.1.1/awswrangler/athena/_write_iceberg.py
--rw-r--r--   0        0        0     2414 2023-01-17 17:33:17.175478 awswrangler-3.1.1/awswrangler/catalog/__init__.py
--rw-r--r--   0        0        0    14077 2023-04-21 16:06:31.392981 awswrangler-3.1.1/awswrangler/catalog/_add.py
--rw-r--r--   0        0        0    50455 2023-04-21 16:06:31.393727 awswrangler-3.1.1/awswrangler/catalog/_create.py
--rw-r--r--   0        0        0    11466 2023-04-21 16:06:31.393962 awswrangler-3.1.1/awswrangler/catalog/_definitions.py
--rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.1.1/awswrangler/catalog/_delete.py
--rw-r--r--   0        0        0    36053 2023-04-21 16:06:31.395286 awswrangler-3.1.1/awswrangler/catalog/_get.py
--rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.1.1/awswrangler/catalog/_utils.py
--rw-r--r--   0        0        0     1199 2022-08-02 16:44:38.863657 awswrangler-3.1.1/awswrangler/chime.py
--rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.1.1/awswrangler/cloudwatch.py
--rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.1.1/awswrangler/data_api/__init__.py
--rw-r--r--   0        0        0     2841 2023-04-21 16:06:31.396849 awswrangler-3.1.1/awswrangler/data_api/_connector.py
--rw-r--r--   0        0        0     5723 2023-04-21 16:06:31.397250 awswrangler-3.1.1/awswrangler/data_api/rds.py
--rw-r--r--   0        0        0     9547 2023-04-21 16:06:31.397699 awswrangler-3.1.1/awswrangler/data_api/redshift.py
--rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.1.1/awswrangler/data_quality/__init__.py
--rw-r--r--   0        0        0    13403 2023-04-21 16:06:31.398627 awswrangler-3.1.1/awswrangler/data_quality/_create.py
--rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.1.1/awswrangler/data_quality/_get.py
--rw-r--r--   0        0        0     6550 2023-04-21 16:06:31.399880 awswrangler-3.1.1/awswrangler/data_quality/_utils.py
--rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.1.1/awswrangler/distributed/__init__.py
--rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.1.1/awswrangler/distributed/ray/__init__.py
--rw-r--r--   0        0        0     6256 2023-04-21 16:06:31.400358 awswrangler-3.1.1/awswrangler/distributed/ray/_core.py
--rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.1.1/awswrangler/distributed/ray/_core.pyi
--rw-r--r--   0        0        0     2121 2023-04-21 16:06:31.400948 awswrangler-3.1.1/awswrangler/distributed/ray/_executor.py
--rw-r--r--   0        0        0     4239 2023-05-10 17:40:59.248347 awswrangler-3.1.1/awswrangler/distributed/ray/_register.py
--rw-r--r--   0        0        0     2443 2023-04-21 16:06:31.401571 awswrangler-3.1.1/awswrangler/distributed/ray/_utils.py
--rw-r--r--   0        0        0     1013 2023-04-21 16:06:31.401685 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-21 16:06:31.401968 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
--rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
--rw-r--r--   0        0        0     3323 2023-05-05 18:06:21.358459 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
--rw-r--r--   0        0        0    18476 2023-05-15 20:31:05.631250 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
--rw-r--r--   0        0        0     8991 2023-05-15 23:11:38.901422 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
--rw-r--r--   0        0        0     5896 2023-05-01 20:36:12.635110 awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
--rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.1.1/awswrangler/distributed/ray/modin/__init__.py
--rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.1.1/awswrangler/distributed/ray/modin/_core.py
--rw-r--r--   0        0        0      929 2023-04-21 16:06:31.403611 awswrangler-3.1.1/awswrangler/distributed/ray/modin/_data_types.py
--rw-r--r--   0        0        0     4126 2023-04-25 15:43:59.620007 awswrangler-3.1.1/awswrangler/distributed/ray/modin/_utils.py
--rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/__init__.py
--rw-r--r--   0        0        0     1912 2023-05-15 18:43:51.641408 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py
--rw-r--r--   0        0        0     5507 2023-04-21 16:06:31.404564 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_text.py
--rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py
--rw-r--r--   0        0        0     3065 2023-04-21 16:06:31.405385 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py
--rw-r--r--   0        0        0     5479 2023-05-15 20:31:05.633385 awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_text.py
--rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.1.1/awswrangler/distributed/ray/s3/__init__.py
--rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.1.1/awswrangler/distributed/ray/s3/_list.py
--rw-r--r--   0        0        0     1005 2023-04-21 16:06:31.406314 awswrangler-3.1.1/awswrangler/distributed/ray/s3/_read_parquet.py
--rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.1.1/awswrangler/dynamodb/__init__.py
--rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.1.1/awswrangler/dynamodb/_delete.py
--rw-r--r--   0        0        0    24958 2023-05-05 17:01:05.126808 awswrangler-3.1.1/awswrangler/dynamodb/_read.py
--rw-r--r--   0        0        0     9045 2023-05-05 17:01:05.126904 awswrangler-3.1.1/awswrangler/dynamodb/_read.pyi
--rw-r--r--   0        0        0     6978 2023-05-05 17:01:05.127213 awswrangler-3.1.1/awswrangler/dynamodb/_utils.py
--rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.1.1/awswrangler/dynamodb/_write.py
--rw-r--r--   0        0        0    44390 2023-05-05 17:01:05.127643 awswrangler-3.1.1/awswrangler/emr.py
--rw-r--r--   0        0        0     2756 2023-05-02 21:22:41.637450 awswrangler-3.1.1/awswrangler/exceptions.py
--rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.1.1/awswrangler/lakeformation/__init__.py
--rw-r--r--   0        0        0    10941 2023-04-21 16:06:31.410840 awswrangler-3.1.1/awswrangler/lakeformation/_read.py
--rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.1.1/awswrangler/lakeformation/_utils.py
--rw-r--r--   0        0        0    20293 2023-05-15 23:11:38.902130 awswrangler-3.1.1/awswrangler/mysql.py
--rw-r--r--   0        0        0      570 2023-05-02 21:22:41.638164 awswrangler-3.1.1/awswrangler/neptune/__init__.py
--rw-r--r--   0        0        0    12730 2023-05-15 20:31:18.255917 awswrangler-3.1.1/awswrangler/neptune/_client.py
--rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.1.1/awswrangler/neptune/_gremlin_init.py
--rw-r--r--   0        0        0     2685 2023-05-15 20:31:18.256245 awswrangler-3.1.1/awswrangler/neptune/_gremlin_parser.py
--rw-r--r--   0        0        0    22208 2023-05-15 20:31:18.256641 awswrangler-3.1.1/awswrangler/neptune/_neptune.py
--rw-r--r--   0        0        0     3748 2023-04-21 16:06:31.413536 awswrangler-3.1.1/awswrangler/neptune/_utils.py
--rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.1.1/awswrangler/opensearch/__init__.py
--rw-r--r--   0        0        0     6480 2023-05-15 20:31:18.256995 awswrangler-3.1.1/awswrangler/opensearch/_read.py
--rw-r--r--   0        0        0    13764 2023-05-15 20:31:18.257329 awswrangler-3.1.1/awswrangler/opensearch/_utils.py
--rw-r--r--   0        0        0    21509 2023-05-15 20:31:18.257745 awswrangler-3.1.1/awswrangler/opensearch/_write.py
--rw-r--r--   0        0        0    20931 2023-05-15 23:11:38.903127 awswrangler-3.1.1/awswrangler/oracle.py
--rw-r--r--   0        0        0     1595 2023-05-15 23:11:28.066397 awswrangler-3.1.1/awswrangler/pandas/__init__.py
--rw-r--r--   0        0        0    20629 2023-05-15 23:11:38.904222 awswrangler-3.1.1/awswrangler/postgresql.py
--rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.1.1/awswrangler/py.typed
--rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.1.1/awswrangler/quicksight/__init__.py
--rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.1.1/awswrangler/quicksight/_cancel.py
--rw-r--r--   0        0        0    15508 2023-05-15 22:16:43.536525 awswrangler-3.1.1/awswrangler/quicksight/_create.py
--rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.1.1/awswrangler/quicksight/_delete.py
--rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.1.1/awswrangler/quicksight/_describe.py
--rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.1.1/awswrangler/quicksight/_get_list.py
--rw-r--r--   0        0        0     1929 2023-05-15 22:16:43.536932 awswrangler-3.1.1/awswrangler/quicksight/_utils.py
--rw-r--r--   0        0        0      440 2023-05-10 17:40:59.251591 awswrangler-3.1.1/awswrangler/redshift/__init__.py
--rw-r--r--   0        0        0     8809 2023-05-15 20:31:18.259025 awswrangler-3.1.1/awswrangler/redshift/_connect.py
--rw-r--r--   0        0        0    18905 2023-05-15 20:31:18.259447 awswrangler-3.1.1/awswrangler/redshift/_read.py
--rw-r--r--   0        0        0     6086 2023-05-10 17:40:59.251990 awswrangler-3.1.1/awswrangler/redshift/_read.pyi
--rw-r--r--   0        0        0    15681 2023-05-15 20:31:18.259784 awswrangler-3.1.1/awswrangler/redshift/_utils.py
--rw-r--r--   0        0        0    28318 2023-05-15 20:31:18.260094 awswrangler-3.1.1/awswrangler/redshift/_write.py
--rw-r--r--   0        0        0     1789 2023-05-02 21:22:41.642687 awswrangler-3.1.1/awswrangler/s3/__init__.py
--rw-r--r--   0        0        0    10594 2023-04-21 16:06:31.421145 awswrangler-3.1.1/awswrangler/s3/_copy.py
--rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.1.1/awswrangler/s3/_delete.py
--rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.1.1/awswrangler/s3/_describe.py
--rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.1.1/awswrangler/s3/_download.py
--rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.1.1/awswrangler/s3/_fs.py
--rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.1.1/awswrangler/s3/_list.py
--rw-r--r--   0        0        0     3970 2023-04-21 16:06:31.423979 awswrangler-3.1.1/awswrangler/s3/_list.pyi
--rw-r--r--   0        0        0     5342 2023-04-21 16:06:31.424139 awswrangler-3.1.1/awswrangler/s3/_read.py
--rw-r--r--   0        0        0     3471 2023-05-02 21:22:41.643295 awswrangler-3.1.1/awswrangler/s3/_read_deltalake.py
--rw-r--r--   0        0        0     3277 2023-05-15 20:31:18.260401 awswrangler-3.1.1/awswrangler/s3/_read_excel.py
--rw-r--r--   0        0        0    36296 2023-05-16 00:05:56.638034 awswrangler-3.1.1/awswrangler/s3/_read_parquet.py
--rw-r--r--   0        0        0     9380 2023-05-05 17:01:05.128332 awswrangler-3.1.1/awswrangler/s3/_read_parquet.pyi
--rw-r--r--   0        0        0    26728 2023-05-16 00:05:56.638491 awswrangler-3.1.1/awswrangler/s3/_read_text.py
--rw-r--r--   0        0        0     7577 2023-05-05 17:01:05.129193 awswrangler-3.1.1/awswrangler/s3/_read_text.pyi
--rw-r--r--   0        0        0     4108 2023-04-21 16:06:31.426375 awswrangler-3.1.1/awswrangler/s3/_read_text_core.py
--rw-r--r--   0        0        0    11991 2023-05-02 21:22:41.644182 awswrangler-3.1.1/awswrangler/s3/_select.py
--rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.1.1/awswrangler/s3/_upload.py
--rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.1.1/awswrangler/s3/_wait.py
--rw-r--r--   0        0        0     4715 2023-04-21 16:06:31.428073 awswrangler-3.1.1/awswrangler/s3/_write.py
--rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.1.1/awswrangler/s3/_write_concurrent.py
--rw-r--r--   0        0        0    12694 2023-04-21 16:06:31.428881 awswrangler-3.1.1/awswrangler/s3/_write_dataset.py
--rw-r--r--   0        0        0     4087 2023-05-02 21:22:41.644400 awswrangler-3.1.1/awswrangler/s3/_write_deltalake.py
--rw-r--r--   0        0        0     3196 2023-05-15 20:31:18.260647 awswrangler-3.1.1/awswrangler/s3/_write_excel.py
--rw-r--r--   0        0        0    43262 2023-05-16 00:05:56.639011 awswrangler-3.1.1/awswrangler/s3/_write_parquet.py
--rw-r--r--   0        0        0    48588 2023-05-16 00:05:56.639505 awswrangler-3.1.1/awswrangler/s3/_write_text.py
--rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.1.1/awswrangler/secretsmanager.py
--rw-r--r--   0        0        0    17975 2023-05-15 23:11:38.908565 awswrangler-3.1.1/awswrangler/sqlserver.py
--rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.1.1/awswrangler/sts.py
--rw-r--r--   0        0        0      644 2023-05-10 17:40:59.253502 awswrangler-3.1.1/awswrangler/timestream/__init__.py
--rw-r--r--   0        0        0     4512 2023-05-10 17:40:59.255448 awswrangler-3.1.1/awswrangler/timestream/_create.py
--rw-r--r--   0        0        0     2491 2023-05-10 17:40:59.255770 awswrangler-3.1.1/awswrangler/timestream/_delete.py
--rw-r--r--   0        0        0     2603 2023-05-15 23:11:38.909361 awswrangler-3.1.1/awswrangler/timestream/_list.py
--rw-r--r--   0        0        0     5881 2023-05-10 17:40:59.256502 awswrangler-3.1.1/awswrangler/timestream/_read.py
--rw-r--r--   0        0        0      722 2023-05-10 17:40:59.256775 awswrangler-3.1.1/awswrangler/timestream/_read.pyi
--rw-r--r--   0        0        0    26397 2023-05-15 20:31:05.639995 awswrangler-3.1.1/awswrangler/timestream/_write.py
--rw-r--r--   0        0        0     8983 2023-05-02 21:22:41.646552 awswrangler-3.1.1/awswrangler/typing.py
--rw-r--r--   0        0        0     4806 2023-05-16 00:05:56.640136 awswrangler-3.1.1/pyproject.toml
--rw-r--r--   0        0        0    22585 1970-01-01 00:00:00.000000 awswrangler-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.2.0/LICENSE.txt
+-rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.2.0/NOTICE.txt
+-rw-r--r--   0        0        0    19946 2023-06-12 13:30:35.513945 awswrangler-3.2.0/README.md
+-rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.2.0/THIRD_PARTY.txt
+-rw-r--r--   0        0        0     1445 2023-05-31 14:40:28.389961 awswrangler-3.2.0/awswrangler/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-12 13:30:35.514884 awswrangler-3.2.0/awswrangler/__metadata__.py
+-rw-r--r--   0        0        0     4351 2023-06-01 19:20:47.696084 awswrangler-3.2.0/awswrangler/_arrow.py
+-rw-r--r--   0        0        0    28922 2023-05-31 14:40:28.390662 awswrangler-3.2.0/awswrangler/_config.py
+-rw-r--r--   0        0        0    32498 2023-05-30 21:03:56.362052 awswrangler-3.2.0/awswrangler/_data_types.py
+-rw-r--r--   0        0        0    13918 2023-05-30 20:11:08.955818 awswrangler-3.2.0/awswrangler/_databases.py
+-rw-r--r--   0        0        0     6254 2023-06-01 18:11:15.743108 awswrangler-3.2.0/awswrangler/_distributed.py
+-rw-r--r--   0        0        0     2063 2023-04-21 16:06:31.388005 awswrangler-3.2.0/awswrangler/_executor.py
+-rw-r--r--   0        0        0     5780 2023-06-08 17:37:13.335354 awswrangler-3.2.0/awswrangler/_sql_formatter.py
+-rw-r--r--   0        0        0    29441 2023-06-07 15:18:15.457609 awswrangler-3.2.0/awswrangler/_utils.py
+-rw-r--r--   0        0        0     1701 2023-04-21 16:06:31.390428 awswrangler-3.2.0/awswrangler/annotations.py
+-rw-r--r--   0        0        0     1329 2023-06-12 13:31:06.245746 awswrangler-3.2.0/awswrangler/athena/__init__.py
+-rw-r--r--   0        0        0     9602 2023-05-26 14:00:36.361829 awswrangler-3.2.0/awswrangler/athena/_cache.py
+-rw-r--r--   0        0        0     9681 2023-06-12 13:31:06.246845 awswrangler-3.2.0/awswrangler/athena/_executions.py
+-rw-r--r--   0        0        0     2148 2023-06-12 13:31:06.247439 awswrangler-3.2.0/awswrangler/athena/_executions.pyi
+-rw-r--r--   0        0        0    57298 2023-06-12 13:31:06.248210 awswrangler-3.2.0/awswrangler/athena/_read.py
+-rw-r--r--   0        0        0    12408 2023-06-12 13:31:06.248740 awswrangler-3.2.0/awswrangler/athena/_read.pyi
+-rw-r--r--   0        0        0     8661 2023-06-06 15:33:48.272209 awswrangler-3.2.0/awswrangler/athena/_spark.py
+-rw-r--r--   0        0        0    42079 2023-06-12 13:31:06.249301 awswrangler-3.2.0/awswrangler/athena/_utils.py
+-rw-r--r--   0        0        0     8398 2023-06-05 15:24:55.446413 awswrangler-3.2.0/awswrangler/athena/_write_iceberg.py
+-rw-r--r--   0        0        0     2531 2023-06-08 16:04:13.943426 awswrangler-3.2.0/awswrangler/catalog/__init__.py
+-rw-r--r--   0        0        0    17109 2023-06-08 16:04:13.943922 awswrangler-3.2.0/awswrangler/catalog/_add.py
+-rw-r--r--   0        0        0    60168 2023-06-08 16:04:13.944729 awswrangler-3.2.0/awswrangler/catalog/_create.py
+-rw-r--r--   0        0        0    14525 2023-06-08 16:04:13.945212 awswrangler-3.2.0/awswrangler/catalog/_definitions.py
+-rw-r--r--   0        0        0     8236 2023-04-21 16:06:31.394534 awswrangler-3.2.0/awswrangler/catalog/_delete.py
+-rw-r--r--   0        0        0    36053 2023-05-26 15:59:19.165550 awswrangler-3.2.0/awswrangler/catalog/_get.py
+-rw-r--r--   0        0        0    11233 2023-04-21 16:06:31.395700 awswrangler-3.2.0/awswrangler/catalog/_utils.py
+-rw-r--r--   0        0        0     1199 2023-06-07 15:18:15.458044 awswrangler-3.2.0/awswrangler/chime.py
+-rw-r--r--   0        0        0    16592 2023-04-21 16:06:31.396720 awswrangler-3.2.0/awswrangler/cloudwatch.py
+-rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.2.0/awswrangler/data_api/__init__.py
+-rw-r--r--   0        0        0     5367 2023-05-30 20:11:08.961643 awswrangler-3.2.0/awswrangler/data_api/_connector.py
+-rw-r--r--   0        0        0    16265 2023-06-08 16:04:13.945849 awswrangler-3.2.0/awswrangler/data_api/rds.py
+-rw-r--r--   0        0        0    11152 2023-05-30 20:11:08.962941 awswrangler-3.2.0/awswrangler/data_api/redshift.py
+-rw-r--r--   0        0        0      377 2023-01-17 17:33:17.179381 awswrangler-3.2.0/awswrangler/data_quality/__init__.py
+-rw-r--r--   0        0        0    13403 2023-05-24 14:22:08.634079 awswrangler-3.2.0/awswrangler/data_quality/_create.py
+-rw-r--r--   0        0        0     1404 2023-04-21 16:06:31.398990 awswrangler-3.2.0/awswrangler/data_quality/_get.py
+-rw-r--r--   0        0        0     6762 2023-06-02 15:24:52.109779 awswrangler-3.2.0/awswrangler/data_quality/_utils.py
+-rw-r--r--   0        0        0       26 2023-04-21 16:06:31.399991 awswrangler-3.2.0/awswrangler/distributed/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-21 16:06:31.400247 awswrangler-3.2.0/awswrangler/distributed/ray/__init__.py
+-rw-r--r--   0        0        0     6334 2023-05-31 17:49:00.586004 awswrangler-3.2.0/awswrangler/distributed/ray/_core.py
+-rw-r--r--   0        0        0      931 2023-04-21 16:06:31.400648 awswrangler-3.2.0/awswrangler/distributed/ray/_core.pyi
+-rw-r--r--   0        0        0     2121 2023-04-21 16:06:31.400948 awswrangler-3.2.0/awswrangler/distributed/ray/_executor.py
+-rw-r--r--   0        0        0     4971 2023-06-08 16:04:13.946455 awswrangler-3.2.0/awswrangler/distributed/ray/_register.py
+-rw-r--r--   0        0        0     2443 2023-04-21 16:06:31.401571 awswrangler-3.2.0/awswrangler/distributed/ray/_utils.py
+-rw-r--r--   0        0        0     1131 2023-06-08 16:04:13.946930 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-21 16:06:31.401968 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
+-rw-r--r--   0        0        0     1273 2023-04-21 16:06:31.402074 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
+-rw-r--r--   0        0        0     1999 2023-06-08 16:04:13.947209 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_orc_datasource.py
+-rw-r--r--   0        0        0     3323 2023-05-05 18:06:21.358459 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
+-rw-r--r--   0        0        0    19699 2023-06-09 14:50:38.346223 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
+-rw-r--r--   0        0        0     9016 2023-06-02 15:24:52.110526 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
+-rw-r--r--   0        0        0     5896 2023-05-01 20:36:12.635110 awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
+-rw-r--r--   0        0        0      135 2023-04-21 16:06:31.402995 awswrangler-3.2.0/awswrangler/distributed/ray/modin/__init__.py
+-rw-r--r--   0        0        0     2524 2023-04-21 16:06:31.403517 awswrangler-3.2.0/awswrangler/distributed/ray/modin/_core.py
+-rw-r--r--   0        0        0      929 2023-06-12 14:16:31.031863 awswrangler-3.2.0/awswrangler/distributed/ray/modin/_data_types.py
+-rw-r--r--   0        0        0     4126 2023-05-24 14:22:08.637288 awswrangler-3.2.0/awswrangler/distributed/ray/modin/_utils.py
+-rw-r--r--   0        0        0       27 2023-04-21 16:06:31.403997 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/__init__.py
+-rw-r--r--   0        0        0     1484 2023-06-08 16:04:13.947578 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_orc.py
+-rw-r--r--   0        0        0     1871 2023-05-31 17:49:00.586748 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py
+-rw-r--r--   0        0        0     5507 2023-05-31 17:49:00.587331 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_text.py
+-rw-r--r--   0        0        0     7306 2023-04-21 16:06:31.405287 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py
+-rw-r--r--   0        0        0     3043 2023-06-08 16:04:13.947746 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_orc.py
+-rw-r--r--   0        0        0     3065 2023-06-05 20:19:19.920635 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py
+-rw-r--r--   0        0        0     5479 2023-05-24 14:22:08.637884 awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_text.py
+-rw-r--r--   0        0        0       21 2023-04-21 16:06:31.405975 awswrangler-3.2.0/awswrangler/distributed/ray/s3/__init__.py
+-rw-r--r--   0        0        0     2413 2023-04-21 16:06:31.406055 awswrangler-3.2.0/awswrangler/distributed/ray/s3/_list.py
+-rw-r--r--   0        0        0      850 2023-06-08 16:04:13.947913 awswrangler-3.2.0/awswrangler/distributed/ray/s3/_read_orc.py
+-rw-r--r--   0        0        0     1005 2023-05-24 14:22:08.638085 awswrangler-3.2.0/awswrangler/distributed/ray/s3/_read_parquet.py
+-rw-r--r--   0        0        0      484 2023-05-04 22:03:58.498637 awswrangler-3.2.0/awswrangler/dynamodb/__init__.py
+-rw-r--r--   0        0        0     1545 2023-04-21 16:06:31.406985 awswrangler-3.2.0/awswrangler/dynamodb/_delete.py
+-rw-r--r--   0        0        0    25553 2023-05-25 19:44:59.410205 awswrangler-3.2.0/awswrangler/dynamodb/_read.py
+-rw-r--r--   0        0        0     9612 2023-05-25 19:44:59.410735 awswrangler-3.2.0/awswrangler/dynamodb/_read.pyi
+-rw-r--r--   0        0        0     6918 2023-05-31 14:40:28.392193 awswrangler-3.2.0/awswrangler/dynamodb/_utils.py
+-rw-r--r--   0        0        0     8406 2023-04-21 16:06:31.408377 awswrangler-3.2.0/awswrangler/dynamodb/_write.py
+-rw-r--r--   0        0        0    44390 2023-05-30 21:03:56.363883 awswrangler-3.2.0/awswrangler/emr.py
+-rw-r--r--   0        0        0    10247 2023-05-31 14:40:28.392544 awswrangler-3.2.0/awswrangler/emr_serverless.py
+-rw-r--r--   0        0        0     2977 2023-06-06 15:33:48.272648 awswrangler-3.2.0/awswrangler/exceptions.py
+-rw-r--r--   0        0        0      682 2023-04-13 20:06:09.276287 awswrangler-3.2.0/awswrangler/lakeformation/__init__.py
+-rw-r--r--   0        0        0    12069 2023-06-01 18:11:15.749542 awswrangler-3.2.0/awswrangler/lakeformation/_read.py
+-rw-r--r--   0        0        0    13151 2023-04-21 16:06:31.411661 awswrangler-3.2.0/awswrangler/lakeformation/_utils.py
+-rw-r--r--   0        0        0    21739 2023-06-07 15:18:11.152506 awswrangler-3.2.0/awswrangler/mysql.py
+-rw-r--r--   0        0        0      673 2023-05-26 16:02:45.896496 awswrangler-3.2.0/awswrangler/neptune/__init__.py
+-rw-r--r--   0        0        0    16117 2023-05-30 20:11:08.965837 awswrangler-3.2.0/awswrangler/neptune/_client.py
+-rw-r--r--   0        0        0      923 2023-04-21 16:06:31.412767 awswrangler-3.2.0/awswrangler/neptune/_gremlin_init.py
+-rw-r--r--   0        0        0     2708 2023-05-30 20:11:08.966466 awswrangler-3.2.0/awswrangler/neptune/_gremlin_parser.py
+-rw-r--r--   0        0        0    25013 2023-05-30 20:11:08.967071 awswrangler-3.2.0/awswrangler/neptune/_neptune.py
+-rw-r--r--   0        0        0     3752 2023-05-26 16:02:45.898491 awswrangler-3.2.0/awswrangler/neptune/_utils.py
+-rw-r--r--   0        0        0      502 2023-01-30 20:05:15.832378 awswrangler-3.2.0/awswrangler/opensearch/__init__.py
+-rw-r--r--   0        0        0     6480 2023-05-25 19:45:07.454333 awswrangler-3.2.0/awswrangler/opensearch/_read.py
+-rw-r--r--   0        0        0    13764 2023-05-25 19:45:07.455041 awswrangler-3.2.0/awswrangler/opensearch/_utils.py
+-rw-r--r--   0        0        0    23823 2023-06-01 18:11:15.750105 awswrangler-3.2.0/awswrangler/opensearch/_write.py
+-rw-r--r--   0        0        0    22400 2023-05-30 20:11:08.968627 awswrangler-3.2.0/awswrangler/oracle.py
+-rw-r--r--   0        0        0     1282 2023-05-31 19:28:36.904170 awswrangler-3.2.0/awswrangler/pandas/__init__.py
+-rw-r--r--   0        0        0    22222 2023-05-25 19:45:07.457161 awswrangler-3.2.0/awswrangler/postgresql.py
+-rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.2.0/awswrangler/py.typed
+-rw-r--r--   0        0        0     2219 2023-01-17 17:33:17.208660 awswrangler-3.2.0/awswrangler/quicksight/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-21 16:06:31.416913 awswrangler-3.2.0/awswrangler/quicksight/_cancel.py
+-rw-r--r--   0        0        0    19228 2023-05-24 14:22:08.643001 awswrangler-3.2.0/awswrangler/quicksight/_create.py
+-rw-r--r--   0        0        0    11710 2023-04-21 16:06:31.417954 awswrangler-3.2.0/awswrangler/quicksight/_delete.py
+-rw-r--r--   0        0        0     8660 2023-04-21 16:06:31.418387 awswrangler-3.2.0/awswrangler/quicksight/_describe.py
+-rw-r--r--   0        0        0    23657 2023-05-15 14:19:50.276077 awswrangler-3.2.0/awswrangler/quicksight/_get_list.py
+-rw-r--r--   0        0        0     2096 2023-05-24 14:22:08.643693 awswrangler-3.2.0/awswrangler/quicksight/_utils.py
+-rw-r--r--   0        0        0      440 2023-05-24 14:22:08.643793 awswrangler-3.2.0/awswrangler/redshift/__init__.py
+-rw-r--r--   0        0        0     8809 2023-05-25 19:45:07.457727 awswrangler-3.2.0/awswrangler/redshift/_connect.py
+-rw-r--r--   0        0        0    20832 2023-05-25 19:45:07.458325 awswrangler-3.2.0/awswrangler/redshift/_read.py
+-rw-r--r--   0        0        0     6716 2023-05-25 19:44:59.414763 awswrangler-3.2.0/awswrangler/redshift/_read.pyi
+-rw-r--r--   0        0        0    15681 2023-06-08 16:02:36.685888 awswrangler-3.2.0/awswrangler/redshift/_utils.py
+-rw-r--r--   0        0        0    28318 2023-05-25 19:45:07.459429 awswrangler-3.2.0/awswrangler/redshift/_write.py
+-rw-r--r--   0        0        0     2008 2023-06-08 16:04:13.948537 awswrangler-3.2.0/awswrangler/s3/__init__.py
+-rw-r--r--   0        0        0    10594 2023-05-24 14:22:08.646591 awswrangler-3.2.0/awswrangler/s3/_copy.py
+-rw-r--r--   0        0        0     5289 2023-04-21 16:06:31.421784 awswrangler-3.2.0/awswrangler/s3/_delete.py
+-rw-r--r--   0        0        0     9327 2023-04-21 16:06:31.422180 awswrangler-3.2.0/awswrangler/s3/_describe.py
+-rw-r--r--   0        0        0     2633 2023-01-30 20:05:15.841405 awswrangler-3.2.0/awswrangler/s3/_download.py
+-rw-r--r--   0        0        0    23146 2023-04-21 16:06:31.422841 awswrangler-3.2.0/awswrangler/s3/_fs.py
+-rw-r--r--   0        0        0    15683 2023-04-21 16:06:31.423159 awswrangler-3.2.0/awswrangler/s3/_list.py
+-rw-r--r--   0        0        0     4158 2023-05-25 19:44:59.415563 awswrangler-3.2.0/awswrangler/s3/_list.pyi
+-rw-r--r--   0        0        0    15344 2023-06-08 16:04:13.949787 awswrangler-3.2.0/awswrangler/s3/_read.py
+-rw-r--r--   0        0        0     4167 2023-06-02 15:24:52.111207 awswrangler-3.2.0/awswrangler/s3/_read_deltalake.py
+-rw-r--r--   0        0        0     3277 2023-05-25 19:45:07.459896 awswrangler-3.2.0/awswrangler/s3/_read_excel.py
+-rw-r--r--   0        0        0    23253 2023-06-08 16:04:13.950493 awswrangler-3.2.0/awswrangler/s3/_read_orc.py
+-rw-r--r--   0        0        0    33869 2023-06-12 13:30:35.516197 awswrangler-3.2.0/awswrangler/s3/_read_parquet.py
+-rw-r--r--   0        0        0    10040 2023-06-12 13:30:35.516790 awswrangler-3.2.0/awswrangler/s3/_read_parquet.pyi
+-rw-r--r--   0        0        0    27928 2023-06-12 13:30:35.517277 awswrangler-3.2.0/awswrangler/s3/_read_text.py
+-rw-r--r--   0        0        0     7993 2023-05-25 19:44:59.418542 awswrangler-3.2.0/awswrangler/s3/_read_text.pyi
+-rw-r--r--   0        0        0     4108 2023-05-22 20:51:56.860472 awswrangler-3.2.0/awswrangler/s3/_read_text_core.py
+-rw-r--r--   0        0        0    12569 2023-05-25 19:44:59.419017 awswrangler-3.2.0/awswrangler/s3/_select.py
+-rw-r--r--   0        0        0     2465 2023-04-21 16:06:31.426801 awswrangler-3.2.0/awswrangler/s3/_upload.py
+-rw-r--r--   0        0        0     6205 2023-04-21 16:06:31.427634 awswrangler-3.2.0/awswrangler/s3/_wait.py
+-rw-r--r--   0        0        0    18407 2023-06-08 16:04:13.952552 awswrangler-3.2.0/awswrangler/s3/_write.py
+-rw-r--r--   0        0        0     1840 2023-04-21 16:06:31.428436 awswrangler-3.2.0/awswrangler/s3/_write_concurrent.py
+-rw-r--r--   0        0        0    12740 2023-05-30 20:11:08.971499 awswrangler-3.2.0/awswrangler/s3/_write_dataset.py
+-rw-r--r--   0        0        0     4144 2023-06-02 15:24:52.111757 awswrangler-3.2.0/awswrangler/s3/_write_deltalake.py
+-rw-r--r--   0        0        0     3196 2023-05-25 19:45:07.460376 awswrangler-3.2.0/awswrangler/s3/_write_excel.py
+-rw-r--r--   0        0        0    26674 2023-06-08 16:04:13.953259 awswrangler-3.2.0/awswrangler/s3/_write_orc.py
+-rw-r--r--   0        0        0    39437 2023-06-12 13:30:35.518029 awswrangler-3.2.0/awswrangler/s3/_write_parquet.py
+-rw-r--r--   0        0        0    48588 2023-06-12 13:30:35.518732 awswrangler-3.2.0/awswrangler/s3/_write_text.py
+-rw-r--r--   0        0        0     2018 2023-04-21 16:06:31.431108 awswrangler-3.2.0/awswrangler/secretsmanager.py
+-rw-r--r--   0        0        0    19421 2023-05-25 19:45:07.461036 awswrangler-3.2.0/awswrangler/sqlserver.py
+-rw-r--r--   0        0        0     1853 2023-04-21 16:06:31.432014 awswrangler-3.2.0/awswrangler/sts.py
+-rw-r--r--   0        0        0      727 2023-05-25 19:44:59.420093 awswrangler-3.2.0/awswrangler/timestream/__init__.py
+-rw-r--r--   0        0        0     4512 2023-05-24 14:22:08.650822 awswrangler-3.2.0/awswrangler/timestream/_create.py
+-rw-r--r--   0        0        0     2491 2023-05-24 14:22:08.651071 awswrangler-3.2.0/awswrangler/timestream/_delete.py
+-rw-r--r--   0        0        0     2603 2023-05-24 14:22:08.651315 awswrangler-3.2.0/awswrangler/timestream/_list.py
+-rw-r--r--   0        0        0    16998 2023-05-30 21:03:56.364637 awswrangler-3.2.0/awswrangler/timestream/_read.py
+-rw-r--r--   0        0        0     1910 2023-05-25 19:44:59.421306 awswrangler-3.2.0/awswrangler/timestream/_read.pyi
+-rw-r--r--   0        0        0    26397 2023-05-24 14:22:08.652414 awswrangler-3.2.0/awswrangler/timestream/_write.py
+-rw-r--r--   0        0        0     9355 2023-06-08 16:04:13.954640 awswrangler-3.2.0/awswrangler/typing.py
+-rw-r--r--   0        0        0     4847 2023-06-12 15:27:53.371623 awswrangler-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    22585 1970-01-01 00:00:00.000000 awswrangler-3.2.0/PKG-INFO
```

### Comparing `awswrangler-3.1.1/LICENSE.txt` & `awswrangler-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/README.md` & `awswrangler-3.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.1.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/3.2.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
@@ -95,33 +95,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -154,39 +154,39 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#distributed-ray)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

### Comparing `awswrangler-3.1.1/THIRD_PARTY.txt` & `awswrangler-3.2.0/THIRD_PARTY.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/__init__.py` & `awswrangler-3.2.0/awswrangler/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     catalog,
     chime,
     cloudwatch,
     data_api,
     data_quality,
     dynamodb,
     emr,
+    emr_serverless,
     exceptions,
     lakeformation,
     mysql,
     neptune,
     opensearch,
     oracle,
     postgresql,
@@ -32,22 +33,23 @@
     timestream,
     typing,
 )
 from awswrangler.__metadata__ import __description__, __license__, __title__, __version__  # noqa
 from awswrangler._config import config  # noqa
 from awswrangler._distributed import EngineEnum, MemoryFormatEnum, engine, memory_format  # noqa
 
-engine.initialize()
+engine.register()
 
 __all__ = [
     "athena",
     "catalog",
     "chime",
     "cloudwatch",
     "emr",
+    "emr_serverless",
     "data_api",
     "data_quality",
     "dynamodb",
     "exceptions",
     "opensearch",
     "oracle",
     "quicksight",
```

### Comparing `awswrangler-3.1.1/awswrangler/_arrow.py` & `awswrangler-3.2.0/awswrangler/_arrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def _extract_partitions_from_path(path_root: str, path: str) -> Dict[str, str]:
     path_root = path_root if path_root.endswith("/") else f"{path_root}/"
     if path_root not in path:
         raise Exception(f"Object {path} is not under the root path ({path_root}).")
     path_wo_filename: str = path.rpartition("/")[0] + "/"
     path_wo_prefix: str = path_wo_filename.replace(f"{path_root}/", "")
-    dirs: Tuple[str, ...] = tuple(x for x in path_wo_prefix.split("/") if (x != "") and (x.count("=") > 0))
+    dirs: Tuple[str, ...] = tuple(x for x in path_wo_prefix.split("/") if x and (x.count("=") > 0))
     if not dirs:
         return {}
     values_tups = cast(Tuple[Tuple[str, str]], tuple(tuple(x.split("=", maxsplit=1)[:2]) for x in dirs))
     values_dics: Dict[str, str] = dict(values_tups)
     return values_dics
```

### Comparing `awswrangler-3.1.1/awswrangler/_config.py` & `awswrangler-3.2.0/awswrangler/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import os
 from functools import wraps
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Type, TypeVar, Union, cast
 
 import botocore.config
 import pandas as pd
+from typing_extensions import Literal
 
 from awswrangler import exceptions
 from awswrangler.typing import AthenaCacheSettings
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
@@ -40,18 +41,20 @@
     "max_remote_cache_entries": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
     "max_local_cache_entries": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
     "athena_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "cloudwatch_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "lakeformation_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "neptune_load_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "timestream_batch_load_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
+    "emr_serverless_job_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "s3_block_size": _ConfigArg(dtype=int, nullable=False, enforced=True),
     "workgroup": _ConfigArg(dtype=str, nullable=False, enforced=True),
     "chunksize": _ConfigArg(dtype=int, nullable=False, enforced=True),
     "suppress_warnings": _ConfigArg(dtype=bool, nullable=False, default=False, loaded=True),
+    "dtype_backend": _ConfigArg(dtype=str, nullable=True),
     # Endpoints URLs
     "s3_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "athena_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "sts_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "glue_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "redshift_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "kms_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
@@ -372,14 +375,23 @@
         return cast(float, self["timestream_batch_load_wait_polling_delay"])
 
     @timestream_batch_load_wait_polling_delay.setter
     def timestream_batch_load_wait_polling_delay(self, value: float) -> None:
         self._set_config_value(key="timestream_batch_load_wait_polling_delay", value=value)
 
     @property
+    def emr_serverless_job_wait_polling_delay(self) -> float:
+        """Property emr_serverless_job_wait_polling_delay."""
+        return cast(float, self["emr_serverless_job_wait_polling_delay"])
+
+    @emr_serverless_job_wait_polling_delay.setter
+    def emr_serverless_job_wait_polling_delay(self, value: float) -> None:
+        self._set_config_value(key="emr_serverless_job_wait_polling_delay", value=value)
+
+    @property
     def s3_block_size(self) -> int:
         """Property s3_block_size."""
         return cast(int, self["s3_block_size"])
 
     @s3_block_size.setter
     def s3_block_size(self, value: int) -> None:
         self._set_config_value(key="s3_block_size", value=value)
@@ -408,14 +420,23 @@
         return cast(bool, self["suppress_warnings"])
 
     @suppress_warnings.setter
     def suppress_warnings(self, value: bool) -> None:
         self._set_config_value(key="suppress_warnings", value=value)
 
     @property
+    def dtype_backend(self) -> Literal["numpy_nullable", "pyarrow", None]:
+        """Property dtype_backend."""
+        return cast(Literal["numpy_nullable", "pyarrow", None], self["dtype_backend"])
+
+    @dtype_backend.setter
+    def dtype_backend(self, value: Literal["numpy_nullable", "pyarrow", None]) -> None:
+        self._set_config_value(key="dtype_backend", value=value)
+
+    @property
     def s3_endpoint_url(self) -> Optional[str]:
         """Property s3_endpoint_url."""
         return cast(Optional[str], self["s3_endpoint_url"])
 
     @s3_endpoint_url.setter
     def s3_endpoint_url(self, value: Optional[str]) -> None:
         self._set_config_value(key="s3_endpoint_url", value=value)
```

### Comparing `awswrangler-3.1.1/awswrangler/_data_types.py` & `awswrangler-3.2.0/awswrangler/_data_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -338,41 +338,41 @@
         )
     if dtype.startswith("map") is True:
         parts: List[str] = _split_map(s=orig_dtype[4:-1])
         return pa.map_(athena2pyarrow(parts[0]), athena2pyarrow(parts[1]))
     raise exceptions.UnsupportedType(f"Unsupported Athena type: {dtype}")
 
 
-def athena2pandas(dtype: str) -> str:  # pylint: disable=too-many-branches,too-many-return-statements
+def athena2pandas(dtype: str, dtype_backend: Optional[str] = None) -> str:  # pylint: disable=too-many-return-statements
     """Athena to Pandas data types conversion."""
     dtype = dtype.lower()
     if dtype == "tinyint":
-        return "Int8"
+        return "Int8" if dtype_backend != "pyarrow" else "int8[pyarrow]"
     if dtype == "smallint":
-        return "Int16"
+        return "Int16" if dtype_backend != "pyarrow" else "int16[pyarrow]"
     if dtype in ("int", "integer"):
-        return "Int32"
+        return "Int32" if dtype_backend != "pyarrow" else "int32[pyarrow]"
     if dtype == "bigint":
-        return "Int64"
+        return "Int64" if dtype_backend != "pyarrow" else "int64[pyarrow]"
     if dtype in ("float", "real"):
-        return "float32"
+        return "float32" if dtype_backend != "pyarrow" else "double[pyarrow]"
     if dtype == "double":
-        return "float64"
+        return "float64" if dtype_backend != "pyarrow" else "double[pyarrow]"
     if dtype == "boolean":
-        return "boolean"
+        return "boolean" if dtype_backend != "pyarrow" else "bool[pyarrow]"
     if (dtype == "string") or dtype.startswith("char") or dtype.startswith("varchar"):
-        return "string"
+        return "string" if dtype_backend != "pyarrow" else "string[pyarrow]"
     if dtype in ("timestamp", "timestamp with time zone"):
-        return "datetime64"
+        return "datetime64" if dtype_backend != "pyarrow" else "date64[pyarrow]"
     if dtype == "date":
-        return "date"
+        return "date" if dtype_backend != "pyarrow" else "date32[pyarrow]"
     if dtype.startswith("decimal"):
-        return "decimal"
+        return "decimal" if dtype_backend != "pyarrow" else "double[pyarrow]"
     if dtype in ("binary", "varbinary"):
-        return "bytes"
+        return "bytes" if dtype_backend != "pyarrow" else "binary[pyarrow]"
     if dtype in ("array", "row", "map"):
         return "object"
     raise exceptions.UnsupportedType(f"Unsupported Athena type: {dtype}")
 
 
 def athena2quicksight(dtype: str) -> str:  # pylint: disable=too-many-branches,too-many-return-statements
     """Athena to Quicksight data types conversion."""
@@ -461,42 +461,58 @@
     if pa.types.is_boolean(dtype):
         return pd.BooleanDtype()
     if pa.types.is_string(dtype):
         return pd.StringDtype()
     return None
 
 
+def pyarrow2pyarrow_backed_pandas_extension(  # pylint: disable=too-many-branches,too-many-return-statements
+    dtype: pa.DataType,
+) -> Optional[pd.api.extensions.ExtensionDtype]:
+    """Pyarrow to Pandas PyArrow-backed data types conversion."""
+    return pd.ArrowDtype(dtype)
+
+
+def get_pyarrow2pandas_type_mapper(
+    dtype_backend: Optional[str] = None,
+) -> Callable[[pa.DataType], Optional[pd.api.extensions.ExtensionDtype]]:
+    if dtype_backend == "pyarrow":
+        return pyarrow2pyarrow_backed_pandas_extension
+
+    return pyarrow2pandas_extension
+
+
 @engine.dispatch_on_engine
 def pyarrow_types_from_pandas(  # pylint: disable=too-many-branches,too-many-statements
     df: pd.DataFrame, index: bool, ignore_cols: Optional[List[str]] = None, index_left: bool = False
 ) -> Dict[str, pa.DataType]:
     """Extract the related Pyarrow data types from any Pandas DataFrame."""
     # Handle exception data types (e.g. Int64, Int32, string)
     ignore_cols = [] if ignore_cols is None else ignore_cols
     cols: List[str] = []
     cols_dtypes: Dict[str, Optional[pa.DataType]] = {}
     for name, dtype in df.dtypes.to_dict().items():
-        dtype = str(dtype)
+        dtype_str = str(dtype)
         if name in ignore_cols:
             cols_dtypes[name] = None
-        elif dtype == "Int8":
+        elif dtype_str == "Int8":
             cols_dtypes[name] = pa.int8()
-        elif dtype == "Int16":
+        elif dtype_str == "Int16":
             cols_dtypes[name] = pa.int16()
-        elif dtype == "Int32":
+        elif dtype_str == "Int32":
             cols_dtypes[name] = pa.int32()
-        elif dtype == "Int64":
+        elif dtype_str == "Int64":
             cols_dtypes[name] = pa.int64()
-        elif dtype == "float32":
+        elif dtype_str == "float32":
             cols_dtypes[name] = pa.float32()
-        elif dtype == "float64":
+        elif dtype_str == "float64":
             cols_dtypes[name] = pa.float64()
-        elif dtype == "string":
+        elif dtype_str == "string":
             cols_dtypes[name] = pa.string()
-        elif dtype == "boolean":
+        elif dtype_str == "boolean":
             cols_dtypes[name] = pa.bool_()
         else:
             cols.append(name)
 
     # Filling cols_dtypes
     for col in cols:
         _logger.debug("Inferring PyArrow type from column: %s", col)
@@ -546,22 +562,24 @@
     # Filling schema
     columns_types: Dict[str, pa.DataType]
     columns_types = {n: cols_dtypes[n] for n in sorted_cols}
     _logger.debug("columns_types: %s", columns_types)
     return columns_types
 
 
-def pyarrow2pandas_defaults(use_threads: Union[bool, int], kwargs: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
+def pyarrow2pandas_defaults(
+    use_threads: Union[bool, int], kwargs: Optional[Dict[str, Any]] = None, dtype_backend: Optional[str] = None
+) -> Dict[str, Any]:
     """Return Pyarrow to Pandas default dictionary arguments."""
     default_kwargs = {
         "use_threads": use_threads,
         "split_blocks": True,
         "self_destruct": True,
         "ignore_metadata": False,
-        "types_mapper": pyarrow2pandas_extension,
+        "types_mapper": get_pyarrow2pandas_type_mapper(dtype_backend),
     }
     if kwargs:
         default_kwargs.update(kwargs)
     return default_kwargs
 
 
 def process_not_inferred_dtype(ex: pa.ArrowInvalid) -> pa.DataType:
@@ -681,25 +699,27 @@
     partitions_types: Optional[Dict[str, str]] = None
     if partitions is not None:
         partitions_types = {p.name: pyarrow2athena(p.dictionary.type, ignore_null=ignore_null) for p in partitions}
     _logger.debug("partitions_types: %s", partitions_types)
     return columns_types, partitions_types
 
 
-def cast_pandas_with_athena_types(df: pd.DataFrame, dtype: Dict[str, str]) -> pd.DataFrame:
+def cast_pandas_with_athena_types(
+    df: pd.DataFrame, dtype: Dict[str, str], dtype_backend: Optional[str] = None
+) -> pd.DataFrame:
     """Cast columns in a Pandas DataFrame."""
     mutability_ensured: bool = False
     for col, athena_type in dtype.items():
         if (
             (col in df.columns)
             and (athena_type.startswith("array") is False)
             and (athena_type.startswith("struct") is False)
             and (athena_type.startswith("map") is False)
         ):
-            desired_type: str = athena2pandas(dtype=athena_type)
+            desired_type: str = athena2pandas(dtype=athena_type, dtype_backend=dtype_backend)
             current_type: str = _normalize_pandas_dtype_name(dtype=str(df[col].dtypes))
             if desired_type != current_type:  # Needs conversion
                 _logger.debug("current_type: %s -> desired_type: %s", current_type, desired_type)
                 if mutability_ensured is False:
                     df = _arrow.ensure_df_is_mutable(df=df)
                     mutability_ensured = True
                 _cast_pandas_column(df=df, col=col, current_type=current_type, desired_type=desired_type)
```

### Comparing `awswrangler-3.1.1/awswrangler/_databases.py` & `awswrangler-3.2.0/awswrangler/_databases.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import importlib.util
 import logging
 import ssl
 from typing import Any, Dict, Generator, Iterator, List, NamedTuple, Optional, Tuple, Union, cast, overload
 
 import boto3
 import pyarrow as pa
+from typing_extensions import Literal
 
 import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions, oracle, secretsmanager
 from awswrangler.catalog import get_connection
 
 _oracledb_found = importlib.util.find_spec("oracledb")
 
@@ -149,20 +150,21 @@
 def _records2df(
     records: List[Tuple[Any]],
     cols_names: List[str],
     index: Optional[Union[str, List[str]]],
     safe: bool,
     dtype: Optional[Dict[str, pa.DataType]],
     timestamp_as_object: bool,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"],
 ) -> pd.DataFrame:
     arrays: List[pa.Array] = []
     for col_values, col_name in zip(tuple(zip(*records)), cols_names):  # Transposing
         if (dtype is None) or (col_name not in dtype):
             if _oracledb_found:
-                col_values = oracle.handle_oracle_objects(col_values, col_name)
+                col_values = oracle.handle_oracle_objects(col_values, col_name)  # ruff: noqa: PLW2901
             try:
                 array: pa.Array = pa.array(obj=col_values, safe=safe)  # Creating Arrow array
             except pa.ArrowInvalid as ex:
                 array = _data_types.process_not_inferred_array(ex, values=col_values)  # Creating Arrow array
         else:
             try:
                 if _oracledb_found:
@@ -179,15 +181,15 @@
         table = pa.Table.from_arrays(arrays=arrays, names=cols_names)  # Creating arrow Table
         df = table.to_pandas(  # Creating Pandas DataFrame
             use_threads=True,
             split_blocks=True,
             self_destruct=True,
             integer_object_nulls=False,
             date_as_object=True,
-            types_mapper=_data_types.pyarrow2pandas_extension,
+            types_mapper=_data_types.get_pyarrow2pandas_type_mapper(dtype_backend=dtype_backend),
             safe=safe,
             timestamp_as_object=timestamp_as_object,
         )
     if index is not None:
         df.set_index(index, inplace=True)
     return df
 
@@ -203,14 +205,15 @@
     con: Any,
     cursor_args: List[Any],
     chunksize: int,
     index_col: Optional[Union[str, List[str]]],
     safe: bool,
     dtype: Optional[Dict[str, pa.DataType]],
     timestamp_as_object: bool,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"],
 ) -> Iterator[pd.DataFrame]:
     with con.cursor() as cursor:
         cursor.execute(*cursor_args)
         if _oracledb_found:
             decimal_dtypes = oracle.detect_oracle_decimal_datatype(cursor)
             _logger.debug("steporig: %s", dtype)
             if decimal_dtypes and dtype is not None:
@@ -226,24 +229,26 @@
             yield _records2df(
                 records=records,
                 cols_names=cols_names,
                 index=index_col,
                 safe=safe,
                 dtype=dtype,
                 timestamp_as_object=timestamp_as_object,
+                dtype_backend=dtype_backend,
             )
 
 
 def _fetch_all_results(
     con: Any,
     cursor_args: List[Any],
     index_col: Optional[Union[str, List[str]]] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "pyarrow",
 ) -> pd.DataFrame:
     with con.cursor() as cursor:
         cursor.execute(*cursor_args)
         cols_names = _get_cols_names(cursor.description)
         if _oracledb_found:
             decimal_dtypes = oracle.detect_oracle_decimal_datatype(cursor)
             _logger.debug("steporig: %s", dtype)
@@ -255,27 +260,29 @@
         return _records2df(
             records=cast(List[Tuple[Any]], cursor.fetchall()),
             cols_names=cols_names,
             index=index_col,
             dtype=dtype,
             safe=safe,
             timestamp_as_object=timestamp_as_object,
+            dtype_backend=dtype_backend,
         )
 
 
 @overload
 def read_sql_query(
     sql: str,
     con: Any,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -283,14 +290,15 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -298,49 +306,53 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 def read_sql_query(
     sql: str,
     con: Any,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Read SQL Query (generic)."""
     args = _convert_params(sql, params)
     try:
         if chunksize is None:
             return _fetch_all_results(
                 con=con,
                 cursor_args=args,
                 index_col=index_col,
                 dtype=dtype,
                 safe=safe,
                 timestamp_as_object=timestamp_as_object,
+                dtype_backend=dtype_backend,
             )
 
         return _iterate_results(
             con=con,
             cursor_args=args,
             chunksize=chunksize,
             index_col=index_col,
             dtype=dtype,
             safe=safe,
             timestamp_as_object=timestamp_as_object,
+            dtype_backend=dtype_backend,
         )
     except Exception as ex:
         con.rollback()
         _logger.error(ex)
         raise
```

### Comparing `awswrangler-3.1.1/awswrangler/_distributed.py` & `awswrangler-3.2.0/awswrangler/_distributed.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 """Distributed engine and memory format configuration."""
 
 # pylint: disable=import-outside-toplevel
 
 import importlib.util
+import os
 import threading
 from collections import defaultdict
 from enum import Enum, unique
 from functools import wraps
 from importlib import reload
 from typing import Any, Callable, Dict, Literal, Optional, TypeVar, cast
 
+EngineLiteral = Literal["python", "ray"]
+MemoryFormatLiteral = Literal["pandas", "modin"]
+
+FunctionType = TypeVar("FunctionType", bound=Callable[..., Any])
+
+
+WR_ENGINE: Optional[EngineLiteral] = os.getenv("WR_ENGINE")  # type: ignore[assignment]
+WR_MEMORY_FORMAT: Optional[MemoryFormatLiteral] = os.getenv("WR_MEMORY_FORMAT")  # type: ignore[assignment]
+
 
 @unique
 class EngineEnum(Enum):
     """Execution engine enum."""
 
     RAY = "ray"
     PYTHON = "python"
@@ -23,23 +33,18 @@
 class MemoryFormatEnum(Enum):
     """Memory format enum."""
 
     MODIN = "modin"
     PANDAS = "pandas"
 
 
-EngineLiteral = Literal["python", "ray"]
-MemoryFormatLiteral = Literal["pandas", "modin"]
-FunctionType = TypeVar("FunctionType", bound=Callable[..., Any])
-
-
 class Engine:
     """Execution engine configuration class."""
 
-    _engine: Optional[EngineEnum] = None
+    _engine: Optional[EngineEnum] = EngineEnum[WR_ENGINE.upper()] if WR_ENGINE else None
     _initialized_engine: Optional[EngineEnum] = None
     _registry: Dict[EngineLiteral, Dict[str, Callable[..., Any]]] = defaultdict(dict)
     _lock: threading.RLock = threading.RLock()
 
     @classmethod
     def get_installed(cls) -> EngineEnum:
         """Get the installed distribution engine.
@@ -69,51 +74,49 @@
         with cls._lock:
             return cls._engine if cls._engine else cls.get_installed()
 
     @classmethod
     def set(cls, name: EngineLiteral) -> None:
         """Set the distribution engine."""
         with cls._lock:
-            cls._engine = EngineEnum._member_map_[  # type: ignore[assignment]  # pylint: disable=protected-access,no-member
-                name.upper()
-            ]
+            cls._engine = EngineEnum[name.upper()]
 
     @classmethod
     def dispatch_func(cls, source_func: FunctionType, value: Optional[EngineLiteral] = None) -> FunctionType:
         """Dispatch a func based on value or the distribution engine and the source function."""
         try:
             with cls._lock:
                 return cls._registry[value or cls.get().value][source_func.__name__]  # type: ignore[return-value]
         except KeyError:
             return getattr(source_func, "_source_func", source_func)
 
     @classmethod
-    def register_func(cls, source_func: Callable[..., Any], destination_func: Callable[..., Any]) -> Callable[..., Any]:
+    def register_func(cls, source_func: FunctionType, destination_func: FunctionType) -> None:
         """Register a func based on the distribution engine and source function."""
         with cls._lock:
             cls._registry[cls.get().value][source_func.__name__] = destination_func
-        return destination_func
 
     @classmethod
     def dispatch_on_engine(cls, func: FunctionType) -> FunctionType:
         """Dispatch on engine function decorator."""
 
         @wraps(func)
         def wrapper(*args: Any, **kw: Dict[str, Any]) -> Any:
+            cls.initialize(name=cls.get().value)
             return cls.dispatch_func(func)(*args, **kw)
 
         # Save the original function
         wrapper._source_func = func  # type: ignore[attr-defined]  # pylint: disable=protected-access
         return wrapper  # type: ignore[return-value]
 
     @classmethod
     def register(cls, name: Optional[EngineLiteral] = None) -> None:
         """Register the distribution engine dispatch methods."""
         with cls._lock:
-            engine_name = cast(EngineLiteral, name or cls.get_installed().value)
+            engine_name = cast(EngineLiteral, name or cls.get().value)
             cls.set(engine_name)
             cls._registry.clear()
 
             if engine_name == EngineEnum.RAY.value:
                 from awswrangler.distributed.ray._register import register_ray
 
                 register_ray()
@@ -123,30 +126,29 @@
         """Initialize the distribution engine."""
         with cls._lock:
             engine_name = cast(EngineLiteral, name or cls.get_installed().value)
             if engine_name == EngineEnum.RAY.value:
                 from awswrangler.distributed.ray import initialize_ray
 
                 initialize_ray()
-            cls.register(engine_name)
-            cls._initialized_engine = cls.get()
+            cls._initialized_engine = EngineEnum[engine_name.upper()]
 
     @classmethod
     def is_initialized(cls, name: Optional[EngineLiteral] = None) -> bool:
         """Check if the distribution engine is initialized."""
         with cls._lock:
             engine_name = cast(EngineLiteral, name or cls.get_installed().value)
 
             return False if not cls._initialized_engine else cls._initialized_engine.value == engine_name
 
 
 class MemoryFormat:
     """Memory format configuration class."""
 
-    _enum: Optional[MemoryFormatEnum] = None
+    _enum: Optional[MemoryFormatEnum] = MemoryFormatEnum[WR_MEMORY_FORMAT.upper()] if WR_MEMORY_FORMAT else None
     _lock: threading.RLock = threading.RLock()
 
     @classmethod
     def get_installed(cls) -> MemoryFormatEnum:
         """Get the installed memory format.
 
         This is the format that can be imported.
@@ -174,15 +176,15 @@
         with cls._lock:
             return cls._enum if cls._enum else cls.get_installed()
 
     @classmethod
     def set(cls, name: EngineLiteral) -> None:
         """Set the memory format."""
         with cls._lock:
-            cls._enum = MemoryFormatEnum._member_map_[name.upper()]  # type: ignore[assignment]  # pylint: disable=protected-access,no-member
+            cls._enum = MemoryFormatEnum[name.upper()]
 
             _reload()
 
 
 def _reload() -> None:
     """Reload Pandas proxy module."""
     import awswrangler.pandas
```

### Comparing `awswrangler-3.1.1/awswrangler/_executor.py` & `awswrangler-3.2.0/awswrangler/_executor.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/_sql_formatter.py` & `awswrangler-3.2.0/awswrangler/_sql_formatter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,207 +1,182 @@
 """Formatting logic for SQL parameters."""
 import datetime
 import decimal
 import re
-from enum import Enum
-from typing import Any, Dict, Generic, Optional, Sequence, Type, TypeVar
+from abc import ABC, abstractmethod
+from typing import Any, Callable, Dict, Optional, Sequence, Type
 
+from typing_extensions import Literal
 
-class _EngineType(Enum):
-    PRESTO = "presto"
-    HIVE = "hive"
-    PARTIQL = "partiql"
+from awswrangler import exceptions
 
-    def __str__(self) -> str:
-        return self.value
+_EngineTypeLiteral = Literal["presto", "hive", "partiql"]
 
 
-_NoneType = type(None)
-_PythonType = TypeVar("_PythonType")
-_PythonTypeMapValue = TypeVar("_PythonTypeMapValue")
-
-
-class _AbstractType(Generic[_PythonType]):
-    def __init__(self, data: _PythonType, engine: _EngineType):
-        self.data: _PythonType = data
-        self.engine: _EngineType = engine
-
-    def __str__(self) -> str:
-        raise NotImplementedError(f"{type(self)} not implemented for engine={self.engine}.")
-
-
-class _NullType(_AbstractType[_NoneType]):
-    def __str__(self) -> str:
-        if self.engine == _EngineType.PARTIQL:
-            return "null"
+class _Engine(ABC):
+    def __init__(self, engine_name: _EngineTypeLiteral) -> None:
+        self.engine_name = engine_name
 
+    def format_null(self, value: None = None) -> str:
         return "NULL"
 
+    @abstractmethod
+    def format_string(self, value: str) -> str:
+        pass
 
-class _StringType(_AbstractType[str]):
-    supported_formats = {"s", "i"}
+    def format_bool(self, value: bool) -> str:
+        return str(value).upper()
 
-    def __str__(self) -> str:
-        if self.engine in [_EngineType.PRESTO, _EngineType.PARTIQL]:
-            return f"""'{self.data.replace("'", "''")}'"""
+    def format_integer(self, value: int) -> str:
+        return str(value)
 
-        if self.engine == _EngineType.HIVE:
-            return "'{}'".format(
-                self.data.replace("\\", "\\\\")
-                .replace("'", "\\'")
-                .replace("\r", "\\r")
-                .replace("\n", "\\n")
-                .replace("\t", "\\t")
-            )
+    def format_float(self, value: float) -> str:
+        return f"{value:f}"
 
-        return super().__str__()
+    def format_decimal(self, value: decimal.Decimal) -> str:
+        return f"DECIMAL '{value:f}'"
 
+    def format_timestamp(self, value: datetime.datetime) -> str:
+        if value.tzinfo is not None:
+            raise TypeError(f"Supports only timezone aware datatype, got {value}.")
 
-class _BooleanType(_AbstractType[bool]):
-    def __str__(self) -> str:
-        if self.engine == _EngineType.PARTIQL:
-            return "1" if self.data else "0"
+        return f"TIMESTAMP '{value.isoformat(sep=' ', timespec='milliseconds')}'"
 
-        return str(self.data).upper()
+    def format_date(self, value: datetime.date) -> str:
+        return f"DATE '{value.isoformat()}'"
 
+    def format_array(self, value: Sequence[Any]) -> str:
+        return f"ARRAY [{', '.join(map(self.format, value))}]"
 
-class _IntegerType(_AbstractType[int]):
-    def __str__(self) -> str:
-        return str(self.data)
+    def format_dict(self, value: Dict[Any, Any]) -> str:
+        if not value:
+            return "MAP()"
 
+        map_keys = list(value.keys())
+        key_type = type(map_keys[0])
+        for key in map_keys:
+            if key is None:
+                raise TypeError("Map key cannot be null.")
+            if not isinstance(key, key_type):
+                raise TypeError("All Map key elements must be the same type.")
 
-class _FloatType(_AbstractType[float]):
-    def __str__(self) -> str:
-        return f"{self.data:f}"
+        map_values = list(value.values())
+        return (
+            f"MAP(ARRAY [{', '.join(map(self.format, map_keys))}], ARRAY [{', '.join(map(self.format, map_values))}])"
+        )
 
+    def format(self, data: Any) -> str:
+        formats_dict: Dict[Type[Any], Callable[[Any], str]] = {
+            bool: self.format_bool,
+            str: self.format_string,
+            int: self.format_integer,
+            datetime.datetime: self.format_timestamp,
+            datetime.date: self.format_date,
+            decimal.Decimal: self.format_decimal,
+            float: self.format_float,
+            list: self.format_array,
+            tuple: self.format_array,
+            set: self.format_array,
+            dict: self.format_dict,
+        }
 
-class _DecimalType(_AbstractType[decimal.Decimal]):
-    def __str__(self) -> str:
-        if self.engine == _EngineType.PARTIQL:
-            return f"'{self.data}'"
+        if data is None:
+            return self.format_null()
 
-        return f"DECIMAL '{self.data:f}'"
+        for python_type, format_func in formats_dict.items():
+            if isinstance(data, python_type):
+                return format_func(data)
 
+        raise TypeError(f"Unsupported type {type(data)} in parameter.")
 
-class _TimestampType(_AbstractType[datetime.datetime]):
-    def __str__(self) -> str:
-        if self.data.tzinfo is not None:
-            raise TypeError(f"Supports only timezone aware datatype, got {self.data}.")
 
-        if self.engine == _EngineType.PARTIQL:
-            return f"'{self.data.isoformat()}'"
+class _PrestoEngine(_Engine):
+    def __init__(self) -> None:
+        super().__init__("presto")
 
-        return f"TIMESTAMP '{self.data.isoformat(sep=' ', timespec='milliseconds')}'"
+    def format_string(self, value: str) -> str:
+        return f"""'{value.replace("'", "''")}'"""
 
 
-class _DateType(_AbstractType[datetime.date]):
-    def __str__(self) -> str:
-        if self.engine == _EngineType.PARTIQL:
-            return f"'{self.data.isoformat()}'"
+class _HiveEngine(_Engine):
+    def __init__(self) -> None:
+        super().__init__("hive")
 
-        return f"DATE '{self.data.isoformat()}'"
+    def format_string(self, value: str) -> str:
+        return "'{}'".format(
+            value.replace("\\", "\\\\")
+            .replace("'", "\\'")
+            .replace("\r", "\\r")
+            .replace("\n", "\\n")
+            .replace("\t", "\\t")
+        )
 
 
-class _ArrayType(_AbstractType[Sequence[_PythonType]]):
-    def __str__(self) -> str:
-        if self.engine == _EngineType.PARTIQL:
-            super().__str__()
+class _PartiQLEngine(_Engine):
+    def __init__(self) -> None:
+        super().__init__("partiql")
 
-        return f"ARRAY [{', '.join(map(str, self.data))}]"
+    def format_null(self, value: None = None) -> str:
+        return "null"
 
+    def format_string(self, value: str) -> str:
+        return f"""'{value.replace("'", "''")}'"""
 
-class _MapType(_AbstractType[Dict[_PythonType, _PythonTypeMapValue]]):
-    def __str__(self) -> str:
-        if self.engine == _EngineType.PARTIQL:
-            super().__str__()
+    def format_bool(self, value: bool) -> str:
+        return "1" if value else "0"
 
-        if not self.data:
-            return "MAP()"
+    def format_decimal(self, value: decimal.Decimal) -> str:
+        return f"'{value}'"
 
-        map_keys = list(self.data.keys())
-        key_type = type(map_keys[0])
-        for key in map_keys:
-            if isinstance(key, _NullType):
-                raise TypeError("Map key cannot be null.")
-            if not isinstance(key, key_type):
-                raise TypeError("All Map key elements must be the same type.")
+    def format_timestamp(self, value: datetime.datetime) -> str:
+        if value.tzinfo is not None:
+            raise TypeError(f"Supports only timezone aware datatype, got {value}.")
 
-        map_values = list(self.data.values())
-        return f"MAP(ARRAY [{', '.join(map(str, map_keys))}], ARRAY [{', '.join(map(str, map_values))}])"
+        return f"'{value.isoformat()}'"
 
+    def format_date(self, value: datetime.date) -> str:
+        return f"'{value.isoformat()}'"
 
-_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore[valid-type]
-    bool: _BooleanType,
-    str: _StringType,
-    int: _IntegerType,
-    datetime.datetime: _TimestampType,
-    datetime.date: _DateType,
-    decimal.Decimal: _DecimalType,
-    float: _FloatType,
-}
-
-_ARRAY_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore[valid-type]
-    list: _ArrayType,
-    tuple: _ArrayType,
-    set: _ArrayType,
-}
-
-_MAP_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore[valid-type]
-    dict: _MapType,
-}
-
-
-def _create_abstract_type(
-    data: _PythonType,
-    engine: _EngineType,
-) -> _AbstractType[_PythonType]:
-    if data is None:
-        return _NullType(data=data, engine=engine)
-
-    for python_type, format_type in _FORMATS.items():
-        if isinstance(data, python_type):
-            return format_type(data=data, engine=engine)
-
-    for python_type, format_type in _ARRAY_FORMATS.items():
-        if isinstance(data, python_type):
-            return format_type(
-                [_create_abstract_type(item, engine=engine) for item in data],
-                engine=engine,
-            )
-
-    for python_type, format_type in _MAP_FORMATS.items():
-        if isinstance(data, python_type):
-            return format_type(
-                data={
-                    _create_abstract_type(mk, engine=engine): _create_abstract_type(mv, engine=engine)
-                    for mk, mv in data.items()
-                },
-                engine=engine,
-            )
+    def format_array(self, value: Sequence[Any]) -> str:
+        raise NotImplementedError(f"format_array not implemented for engine={self.engine_name}.")
 
-    raise TypeError(f"Unsupported type {type(data)} in parameter.")
+    def format_dict(self, value: Dict[Any, Any]) -> str:
+        raise NotImplementedError(f"format_dict not implemented for engine={self.engine_name}.")
 
 
-def _format_parameters(params: Dict[str, Any], engine: _EngineType) -> Dict[str, Any]:
+def _format_parameters(params: Dict[str, Any], engine: _Engine) -> Dict[str, Any]:
     processed_params = {}
 
     for k, v in params.items():
-        abs_type = _create_abstract_type(data=v, engine=engine)
-        processed_params[k] = str(abs_type)
+        processed_params[k] = engine.format(data=v)
 
     return processed_params
 
 
 _PATTERN = re.compile(r":([A-Za-z0-9_]+)(?![A-Za-z0-9_])")
 
 
-def _process_sql_params(sql: str, params: Optional[Dict[str, Any]], engine: _EngineType = _EngineType.PRESTO) -> str:
+def _create_engine(engine_type: _EngineTypeLiteral) -> _Engine:
+    if engine_type == "hive":
+        return _HiveEngine()
+
+    if engine_type == "presto":
+        return _PrestoEngine()
+
+    if engine_type == "partiql":
+        return _PartiQLEngine()
+
+    raise exceptions.InvalidArgumentValue(f"Unknown engine type: {engine_type}")
+
+
+def _process_sql_params(sql: str, params: Optional[Dict[str, Any]], engine_type: _EngineTypeLiteral = "presto") -> str:
     if params is None:
         params = {}
 
+    engine = _create_engine(engine_type)
     processed_params = _format_parameters(params, engine=engine)
 
     def replace(match: re.Match) -> str:  # type: ignore[type-arg]
         key = match.group(1)
 
         if key not in processed_params:
             # do not replace anything if the parameter is not provided
```

### Comparing `awswrangler-3.1.1/awswrangler/_utils.py` & `awswrangler-3.2.0/awswrangler/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 if TYPE_CHECKING:
     from boto3.resources.base import ServiceResource
     from botocore.client import BaseClient
     from mypy_boto3_athena import AthenaClient
     from mypy_boto3_dynamodb import DynamoDBClient, DynamoDBServiceResource
     from mypy_boto3_ec2 import EC2Client
     from mypy_boto3_emr.client import EMRClient
+    from mypy_boto3_emr_serverless import EMRServerlessClient
     from mypy_boto3_glue import GlueClient
     from mypy_boto3_kms.client import KMSClient
     from mypy_boto3_lakeformation.client import LakeFormationClient
     from mypy_boto3_logs.client import CloudWatchLogsClient
     from mypy_boto3_opensearch.client import OpenSearchServiceClient
     from mypy_boto3_opensearchserverless.client import OpenSearchServiceServerlessClient
     from mypy_boto3_quicksight.client import QuickSightClient
@@ -66,14 +67,15 @@
     from typing_extensions import Literal
 
     ServiceName = Literal[
         "athena",
         "dynamodb",
         "ec2",
         "emr",
+        "emr-serverless",
         "glue",
         "kms",
         "lakeformation",
         "logs",
         "opensearch",
         "opensearchserverless",
         "quicksight",
@@ -157,14 +159,19 @@
 
         @wraps(func)
         def inner(*args: Any, **kwargs: Any) -> Any:
             passed_unsupported_kwargs = set(unsupported_kwargs).intersection(  # type: ignore
                 set([key for key, value in kwargs.items() if value is not None])
             )
 
+            # Allow kwargs that didn't modify the default value
+            passed_unsupported_kwargs = {
+                key for key in passed_unsupported_kwargs if kwargs[key] != signature.parameters[key].default
+            }
+
             if condition_fn() and len(passed_unsupported_kwargs) > 0:
                 raise exceptions.InvalidArgument(f"{message} `{', '.join(passed_unsupported_kwargs)}`.")
 
             return func(*args, **kwargs)
 
         inner.__doc__ = _inject_kwargs_validation_doc(
             doc=func.__doc__,
@@ -327,14 +334,24 @@
     verify: Optional[Union[str, bool]] = None,
 ) -> "EMRClient":
     ...
 
 
 @overload
 def client(
+    service_name: 'Literal["emr-serverless"]',
+    session: Optional[boto3.Session] = None,
+    botocore_config: Optional[Config] = None,
+    verify: Optional[Union[str, bool]] = None,
+) -> "EMRServerlessClient":
+    ...
+
+
+@overload
+def client(
     service_name: 'Literal["glue"]',
     session: Optional[boto3.Session] = None,
     botocore_config: Optional[Config] = None,
     verify: Optional[Union[str, bool]] = None,
 ) -> "GlueClient":
     ...
```

### Comparing `awswrangler-3.1.1/awswrangler/annotations.py` & `awswrangler-3.2.0/awswrangler/annotations.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/athena/__init__.py` & `awswrangler-3.2.0/awswrangler/athena/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from awswrangler.athena._executions import (  # noqa
     get_query_execution,
     stop_query_execution,
     start_query_execution,
     wait_query,
 )
+from awswrangler.athena._spark import create_spark_session, run_spark_calculation
 from awswrangler.athena._read import (  # noqa
     get_query_results,
     read_sql_query,
     read_sql_table,
     unload,
 )
 from awswrangler.athena._utils import (  # noqa
@@ -38,14 +39,16 @@
     "get_query_executions",
     "get_query_results",
     "get_named_query_statement",
     "get_work_group",
     "generate_create_query",
     "list_query_executions",
     "repair_table",
+    "create_spark_session",
+    "run_spark_calculation",
     "create_ctas_table",
     "show_create_table",
     "start_query_execution",
     "stop_query_execution",
     "unload",
     "wait_query",
     "to_iceberg",
```

### Comparing `awswrangler-3.1.1/awswrangler/athena/_cache.py` & `awswrangler-3.2.0/awswrangler/athena/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Cache Module for Amazon Athena."""
 import datetime
 import logging
 import re
+import threading
 from heapq import heappop, heappush
 from typing import TYPE_CHECKING, Any, Dict, List, Match, NamedTuple, Optional, Tuple, Union
 
 import boto3
 
 from awswrangler import _utils
 
@@ -20,14 +21,15 @@
     file_format: Optional[str] = None
     query_execution_id: Optional[str] = None
     query_execution_payload: Optional[Dict[str, Any]] = None
 
 
 class _LocalMetadataCacheManager:
     def __init__(self) -> None:
+        self._lock: threading.Lock = threading.Lock()
         self._cache: Dict[str, Any] = {}
         self._pqueue: List[Tuple[datetime.datetime, str]] = []
         self._max_cache_size = 100
 
     def update_cache(self, items: List[Dict[str, Any]]) -> None:
         """
         Update the local metadata cache with new query metadata.
@@ -38,28 +40,33 @@
             List of query execution metadata which is returned by boto3 `batch_get_query_execution()`.
 
         Returns
         -------
         None
             None.
         """
-        if self._pqueue:
-            oldest_item = self._cache[self._pqueue[0][1]]
-            items = list(
-                filter(lambda x: x["Status"]["SubmissionDateTime"] > oldest_item["Status"]["SubmissionDateTime"], items)
-            )
-
-        cache_oversize = len(self._cache) + len(items) - self._max_cache_size
-        for _ in range(cache_oversize):
-            _, query_execution_id = heappop(self._pqueue)
-            del self._cache[query_execution_id]
-
-        for item in items[: self._max_cache_size]:
-            heappush(self._pqueue, (item["Status"]["SubmissionDateTime"], item["QueryExecutionId"]))
-            self._cache[item["QueryExecutionId"]] = item
+        with self._lock:
+            if self._pqueue:
+                oldest_item = self._cache.get(self._pqueue[0][1])
+                if oldest_item:
+                    items = list(
+                        filter(
+                            lambda x: x["Status"]["SubmissionDateTime"] > oldest_item["Status"]["SubmissionDateTime"],  # type: ignore[arg-type]
+                            items,
+                        )
+                    )
+
+            cache_oversize = len(self._cache) + len(items) - self._max_cache_size
+            for _ in range(cache_oversize):
+                _, query_execution_id = heappop(self._pqueue)
+                del self._cache[query_execution_id]
+
+            for item in items[: self._max_cache_size]:
+                heappush(self._pqueue, (item["Status"]["SubmissionDateTime"], item["QueryExecutionId"]))
+                self._cache[item["QueryExecutionId"]] = item
 
     def sorted_successful_generator(self) -> List[Dict[str, Any]]:
         """
         Sorts the entries in the local cache based on query Completion DateTime.
 
         This is useful to guarantee LRU caching rules.
```

### Comparing `awswrangler-3.1.1/awswrangler/athena/_executions.py` & `awswrangler-3.2.0/awswrangler/athena/_executions.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/athena/_executions.pyi` & `awswrangler-3.2.0/awswrangler/athena/_executions.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/athena/_read.py` & `awswrangler-3.2.0/awswrangler/athena/_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import uuid
 from datetime import date
 from typing import Any, Dict, Iterator, List, Optional, Union, cast
 
 import boto3
 import botocore.exceptions
 import pandas as pd
+from typing_extensions import Literal
 
 from awswrangler import _utils, catalog, exceptions, s3, typing
 from awswrangler._config import apply_configs
 from awswrangler._data_types import cast_pandas_with_athena_types
 from awswrangler._sql_formatter import _process_sql_params
 from awswrangler.athena._utils import (
     _QUERY_WAIT_POLLING_DELAY,
@@ -35,15 +36,15 @@
 
 
 def _extract_ctas_manifest_paths(path: str, boto3_session: Optional[boto3.Session] = None) -> List[str]:
     """Get the list of paths of the generated files."""
     bucket_name, key_path = _utils.parse_path(path)
     client_s3 = _utils.client(service_name="s3", session=boto3_session)
     body: bytes = client_s3.get_object(Bucket=bucket_name, Key=key_path)["Body"].read()
-    paths = [x for x in body.decode("utf-8").split("\n") if x != ""]
+    paths = [x for x in body.decode("utf-8").split("\n") if x]
     _logger.debug("Read %d paths from manifest file in: %s", len(paths), path)
     return paths
 
 
 def _fix_csv_types_generator(
     dfs: Iterator[pd.DataFrame], parse_dates: List[str], binaries: List[str]
 ) -> Iterator[pd.DataFrame]:
@@ -53,15 +54,15 @@
 
 
 def _add_query_metadata_generator(
     dfs: Iterator[pd.DataFrame], query_metadata: _QueryMetadata
 ) -> Iterator[pd.DataFrame]:
     """Add Query Execution metadata to every DF in iterator."""
     for df in dfs:
-        df = _apply_query_metadata(df=df, query_metadata=query_metadata)
+        df = _apply_query_metadata(df=df, query_metadata=query_metadata)  # ruff: noqa: PLW2901
         yield df
 
 
 def _fix_csv_types(df: pd.DataFrame, parse_dates: List[str], binaries: List[str]) -> pd.DataFrame:
     """Apply data types cast to a Pandas DataFrames."""
     if len(df.index) > 0:
         for col in parse_dates:
@@ -96,14 +97,15 @@
     categories: Optional[List[str]],
     chunksize: Optional[int],
     use_threads: Union[bool, int],
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     temp_table_fqn: Optional[str] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ret: Union[pd.DataFrame, Iterator[pd.DataFrame]]
     chunked: Union[bool, int] = False if chunksize is None else chunksize
     _logger.debug("Chunked: %s", chunked)
     if query_metadata.manifest_location is None:
         return _empty_dataframe_response(bool(chunked), query_metadata)
     manifest_path: str = query_metadata.manifest_location
@@ -115,15 +117,15 @@
         if not temp_table_fqn:
             raise exceptions.EmptyDataFrame("Query would return untyped, empty dataframe.")
         database, temp_table_name = map(lambda x: x.replace('"', ""), temp_table_fqn.split("."))
         dtype_dict = catalog.get_table_types(database=database, table=temp_table_name, boto3_session=boto3_session)
         if dtype_dict is None:
             raise exceptions.ResourceDoesNotExist(f"Temp table {temp_table_fqn} not found.")
         df = pd.DataFrame(columns=list(dtype_dict.keys()))
-        df = cast_pandas_with_athena_types(df=df, dtype=dtype_dict)
+        df = cast_pandas_with_athena_types(df=df, dtype=dtype_dict, dtype_backend=dtype_backend)
         df = _apply_query_metadata(df=df, query_metadata=query_metadata)
         if chunked:
             return (df,)
         return df
     if not pyarrow_additional_kwargs:
         pyarrow_additional_kwargs = {}
         if categories:
@@ -131,14 +133,15 @@
     _logger.debug("Reading Parquet result from %d paths", len(paths))
     ret = s3.read_parquet(
         path=paths,
         use_threads=use_threads,
         boto3_session=boto3_session,
         chunked=chunked,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+        dtype_backend=dtype_backend,
     )
 
     if chunked is False:
         ret = _apply_query_metadata(df=ret, query_metadata=query_metadata)
     else:
         ret = _add_query_metadata_generator(dfs=ret, query_metadata=query_metadata)
     paths_delete: List[str] = paths + [manifest_path, metadata_path]
@@ -165,14 +168,15 @@
 def _fetch_csv_result(
     query_metadata: _QueryMetadata,
     keep_files: bool,
     chunksize: Optional[int],
     use_threads: Union[bool, int],
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     _chunksize: Optional[int] = chunksize if isinstance(chunksize, int) else None
     _logger.debug("Chunksize: %s", _chunksize)
     if query_metadata.output_location is None or query_metadata.output_location.endswith(".csv") is False:
         chunked = _chunksize is not None
         return _empty_dataframe_response(chunked, query_metadata)
     path: str = query_metadata.output_location
@@ -185,14 +189,15 @@
         quoting=csv.QUOTE_ALL,
         keep_default_na=False,
         na_values=["", "NaN"],
         chunksize=_chunksize,
         skip_blank_lines=False,
         use_threads=False,
         boto3_session=boto3_session,
+        dtype_backend=dtype_backend,
     )
     _logger.debug("Start type casting...")
     if _chunksize is None:
         df = _fix_csv_types(df=ret, parse_dates=query_metadata.parse_dates, binaries=query_metadata.binaries)
         df = _apply_query_metadata(df=df, query_metadata=query_metadata)
         if keep_files is False:
             s3.delete_objects(
@@ -220,14 +225,15 @@
     categories: Optional[List[str]],
     chunksize: Optional[Union[int, bool]],
     use_threads: Union[bool, int],
     athena_query_wait_polling_delay: float,
     session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Fetch cached data and return it as a pandas DataFrame (or list of DataFrames)."""
     _logger.debug("cache_info:\n%s", cache_info)
     if cache_info.query_execution_id is None:
         raise RuntimeError("Trying to resolve with cache but w/o any query execution ID.")
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=cache_info.query_execution_id,
@@ -243,14 +249,15 @@
             keep_files=True,
             categories=categories,
             chunksize=chunksize,
             use_threads=use_threads,
             boto3_session=session,
             s3_additional_kwargs=s3_additional_kwargs,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            dtype_backend=dtype_backend,
         )
     if cache_info.file_format == "csv":
         return _fetch_csv_result(
             query_metadata=query_metadata,
             keep_files=True,
             chunksize=chunksize,
             use_threads=use_threads,
@@ -276,14 +283,15 @@
     ctas_bucketing_info: Optional[typing.BucketingInfoTuple],
     ctas_write_compression: Optional[str],
     athena_query_wait_polling_delay: float,
     use_threads: Union[bool, int],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ctas_query_info: Dict[str, Union[str, _QueryMetadata]] = create_ctas_table(
         sql=sql,
         database=database,
         ctas_table=name,
         ctas_database=alt_database,
         bucketing_info=ctas_bucketing_info,
@@ -306,14 +314,15 @@
         categories=categories,
         chunksize=chunksize,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
         temp_table_fqn=fully_qualified_name,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+        dtype_backend=dtype_backend,
     )
 
 
 def _resolve_query_without_cache_unload(
     sql: str,
     file_format: str,
     compression: Optional[str],
@@ -329,14 +338,15 @@
     kms_key: Optional[str],
     workgroup: Optional[str],
     use_threads: Union[bool, int],
     athena_query_wait_polling_delay: float,
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     query_metadata = _unload(
         sql=sql,
         path=s3_output,
         file_format=file_format,
         compression=compression,
         field_delimiter=field_delimiter,
@@ -355,14 +365,15 @@
             keep_files=keep_files,
             categories=categories,
             chunksize=chunksize,
             use_threads=use_threads,
             s3_additional_kwargs=s3_additional_kwargs,
             boto3_session=boto3_session,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            dtype_backend=dtype_backend,
         )
     raise exceptions.InvalidArgumentValue("Only PARQUET file format is supported when unload_approach=True.")
 
 
 def _resolve_query_without_cache_regular(
     sql: str,
     database: Optional[str],
@@ -374,14 +385,15 @@
     encryption: Optional[str],
     workgroup: Optional[str],
     kms_key: Optional[str],
     use_threads: Union[bool, int],
     athena_query_wait_polling_delay: float,
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
     s3_output = _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=boto3_session)
     s3_output = s3_output[:-1] if s3_output[-1] == "/" else s3_output
     _logger.debug("Executing sql: %s", sql)
     query_id: str = _start_query_execution(
         sql=sql,
@@ -397,22 +409,24 @@
     _logger.debug("Query id: %s", query_id)
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=query_id,
         boto3_session=boto3_session,
         categories=categories,
         metadata_cache_manager=_cache_manager,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
+        dtype_backend=dtype_backend,
     )
     return _fetch_csv_result(
         query_metadata=query_metadata,
         keep_files=keep_files,
         chunksize=chunksize,
         use_threads=use_threads,
         boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
+        dtype_backend=dtype_backend,
     )
 
 
 def _resolve_query_without_cache(
     # pylint: disable=too-many-branches,too-many-locals,too-many-return-statements,too-many-statements
     sql: str,
     database: str,
@@ -432,14 +446,15 @@
     ctas_bucketing_info: Optional[typing.BucketingInfoTuple],
     ctas_write_compression: Optional[str],
     athena_query_wait_polling_delay: float,
     use_threads: Union[bool, int],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """
     Execute a query in Athena and returns results as DataFrame, back to `read_sql_query`.
 
     Usually called by `read_sql_query` when using cache is not possible.
     """
     if ctas_approach is True:
@@ -464,14 +479,15 @@
                 ctas_bucketing_info=ctas_bucketing_info,
                 ctas_write_compression=ctas_write_compression,
                 athena_query_wait_polling_delay=athena_query_wait_polling_delay,
                 use_threads=use_threads,
                 s3_additional_kwargs=s3_additional_kwargs,
                 boto3_session=boto3_session,
                 pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+                dtype_backend=dtype_backend,
             )
         finally:
             catalog.delete_table_if_exists(database=ctas_database or database, table=name, boto3_session=boto3_session)
     elif unload_approach is True:
         if unload_parameters is None:
             unload_parameters = {}
         return _resolve_query_without_cache_unload(
@@ -490,14 +506,15 @@
             kms_key=kms_key,
             workgroup=workgroup,
             use_threads=use_threads,
             athena_query_wait_polling_delay=athena_query_wait_polling_delay,
             s3_additional_kwargs=s3_additional_kwargs,
             boto3_session=boto3_session,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            dtype_backend=dtype_backend,
         )
     return _resolve_query_without_cache_regular(
         sql=sql,
         database=database,
         data_source=data_source,
         s3_output=s3_output,
         keep_files=keep_files,
@@ -506,14 +523,15 @@
         encryption=encryption,
         workgroup=workgroup,
         kms_key=kms_key,
         use_threads=use_threads,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
+        dtype_backend=dtype_backend,
     )
 
 
 def _unload(
     sql: str,
     path: Optional[str],
     file_format: str,
@@ -597,14 +615,15 @@
     unsupported_kwargs=["boto3_session"],
 )
 def get_query_results(
     query_execution_id: str,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     categories: Optional[List[str]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunksize: Optional[Union[int, bool]] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Get AWS Athena SQL query results as a Pandas DataFrame.
 
@@ -617,14 +636,20 @@
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     categories: List[str], optional
         List of columns names that should be returned as pandas.Categorical.
         Recommended for memory restricted environments.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunksize : Union[int, bool], optional
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
         If an `INTEGER` is passed awswrangler will iterate on the data by number of rows equal the received INTEGER.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
@@ -668,23 +693,25 @@
             keep_files=True,
             categories=categories,
             chunksize=chunksize,
             use_threads=use_threads,
             boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            dtype_backend=dtype_backend,
         )
     if statement_type == "DML" and not query_info["Query"].startswith("INSERT"):
         return _fetch_csv_result(
             query_metadata=query_metadata,
             keep_files=True,
             chunksize=chunksize,
             use_threads=use_threads,
             boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
+            dtype_backend=dtype_backend,
         )
     raise exceptions.UndetectedType(f"""Unable to get results for: {query_info["Query"]}.""")
 
 
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
@@ -705,26 +732,27 @@
     keep_files: bool = True,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
     data_source: Optional[str] = None,
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     params: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Execute any SQL query on AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -780,15 +808,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -877,14 +905,20 @@
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
     athena_query_wait_polling_delay: float, default: 0.25 seconds
         Interval in seconds for how often the function will check if the Athena query has completed.
     params: Dict[str, any], optional
         Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
         The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
         `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     pyarrow_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
         e.g. pyarrow_additional_kwargs={'split_blocks': True}.
@@ -959,14 +993,15 @@
                 categories=categories,
                 chunksize=chunksize,
                 use_threads=use_threads,
                 session=boto3_session,
                 athena_query_wait_polling_delay=athena_query_wait_polling_delay,
                 s3_additional_kwargs=s3_additional_kwargs,
                 pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+                dtype_backend=dtype_backend,
             )
         except Exception as e:  # pylint: disable=broad-except
             _logger.error(e)  # if there is anything wrong with the cache, just fallback to the usual path
             _logger.debug("Corrupted cache. Continuing to execute query...")
 
     ctas_parameters = ctas_parameters if ctas_parameters else {}
     ctas_database = ctas_parameters.get("database")
@@ -993,14 +1028,15 @@
         ctas_bucketing_info=ctas_bucketing_info,
         ctas_write_compression=ctas_write_compression,
         athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+        dtype_backend=dtype_backend,
     )
 
 
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
 )
@@ -1018,26 +1054,27 @@
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     keep_files: bool = True,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
     data_source: Optional[str] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Extract the full table AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -1093,15 +1130,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.1.1/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.2.0/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -1182,14 +1219,20 @@
         AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
         instance of AthenaCacheSettings or as a regular Python dict.
         If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
         `keep_files` and `ctas_temp_table_name` params.
         If reading cached data fails for any reason, execution falls back to the usual query run path.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     pyarrow_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
         Valid values include "split_blocks", "self_destruct", "ignore_metadata".
         e.g. pyarrow_additional_kwargs={'split_blocks': True}.
@@ -1223,14 +1266,15 @@
         keep_files=keep_files,
         use_threads=use_threads,
         boto3_session=boto3_session,
         athena_cache_settings=athena_cache_settings,
         data_source=data_source,
         s3_additional_kwargs=s3_additional_kwargs,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+        dtype_backend=dtype_backend,
     )
 
 
 @apply_configs
 def unload(
     sql: str,
     path: str,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awswrangler-3.1.1/awswrangler/athena/_read.pyi` & `awswrangler-3.2.0/awswrangler/athena/_read.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -8,48 +8,52 @@
 
 @overload
 def get_query_results(
     query_execution_id: str,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     categories: Optional[List[str]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: Union[None, Literal[False]] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> pd.DataFrame: ...
 @overload
 def get_query_results(
     query_execution_id: str,
     *,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     categories: Optional[List[str]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: Literal[True],
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def get_query_results(
     query_execution_id: str,
     *,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     categories: Optional[List[str]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: bool,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
 def get_query_results(
     query_execution_id: str,
     *,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     categories: Optional[List[str]] = ...,
     chunksize: int,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def read_sql_query(  # pylint: disable=too-many-arguments
     sql: str,
     database: str,
@@ -66,14 +70,15 @@
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
     params: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> pd.DataFrame: ...
 @overload
 def read_sql_query(
     sql: str,
     database: str,
@@ -91,14 +96,15 @@
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
     params: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def read_sql_query(
     sql: str,
     database: str,
@@ -116,14 +122,15 @@
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
     params: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
 def read_sql_query(
     sql: str,
     database: str,
@@ -141,14 +148,15 @@
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
     params: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def read_sql_query(
     sql: str,
     database: str,
@@ -166,14 +174,15 @@
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
     athena_query_wait_polling_delay: float = ...,
     params: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
 def read_sql_table(
     table: str,
     database: str,
@@ -189,14 +198,15 @@
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> pd.DataFrame: ...
 @overload
 def read_sql_table(
     table: str,
     database: str,
@@ -212,14 +222,15 @@
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def read_sql_table(
     table: str,
     database: str,
@@ -235,14 +246,15 @@
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
 def read_sql_table(
     table: str,
     database: str,
@@ -258,14 +270,15 @@
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
 def read_sql_table(
     table: str,
     database: str,
@@ -281,14 +294,15 @@
     encryption: Optional[str] = ...,
     kms_key: Optional[str] = ...,
     keep_files: bool = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
     data_source: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 def unload(
     sql: str,
     path: str,
     database: str,
```

### Comparing `awswrangler-3.1.1/awswrangler/athena/_utils.py` & `awswrangler-3.2.0/awswrangler/athena/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Union,
     cast,
 )
 
 import boto3
 import botocore.exceptions
 import pandas as pd
+from typing_extensions import Literal
 
 from awswrangler import _data_types, _utils, catalog, exceptions, s3, sts, typing
 from awswrangler._config import apply_configs
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 
 from . import _executions
 from ._cache import _cache_manager, _LocalMetadataCacheManager
@@ -92,19 +93,18 @@
 
     # encryption
     if wg_config.enforced is True:
         if wg_config.encryption is not None:
             args["ResultConfiguration"]["EncryptionConfiguration"] = {"EncryptionOption": wg_config.encryption}
             if wg_config.kms_key is not None:
                 args["ResultConfiguration"]["EncryptionConfiguration"]["KmsKey"] = wg_config.kms_key
-    else:
-        if encryption is not None:
-            args["ResultConfiguration"]["EncryptionConfiguration"] = {"EncryptionOption": encryption}
-            if kms_key is not None:
-                args["ResultConfiguration"]["EncryptionConfiguration"]["KmsKey"] = kms_key
+    elif encryption is not None:
+        args["ResultConfiguration"]["EncryptionConfiguration"] = {"EncryptionOption": encryption}
+        if kms_key is not None:
+            args["ResultConfiguration"]["EncryptionConfiguration"]["KmsKey"] = kms_key
 
     # database
     if database is not None:
         args["QueryExecutionContext"] = {"Database": database}
         if data_source is not None:
             args["QueryExecutionContext"]["Catalog"] = data_source
 
@@ -182,16 +182,16 @@
     return df
 
 
 def _parse_describe_table(df: pd.DataFrame) -> pd.DataFrame:
     origin_df_dict = df.to_dict()
     target_df_dict: Dict[str, List[Union[str, bool]]] = {"Column Name": [], "Type": [], "Partition": [], "Comment": []}
     for index, col_name in origin_df_dict["col_name"].items():
-        col_name = col_name.strip()
-        if col_name.startswith("#") or col_name == "":
+        col_name = col_name.strip()  # ruff: noqa: PLW2901
+        if col_name.startswith("#") or not col_name:
             pass
         elif col_name in target_df_dict["Column Name"]:
             index_col_name = target_df_dict["Column Name"].index(col_name)
             target_df_dict["Partition"][index_col_name] = True
         else:
             target_df_dict["Column Name"].append(col_name)
             target_df_dict["Type"].append(origin_df_dict["data_type"][index].strip())
@@ -203,14 +203,15 @@
 def _get_query_metadata(  # pylint: disable=too-many-statements
     query_execution_id: str,
     boto3_session: Optional[boto3.Session] = None,
     categories: Optional[List[str]] = None,
     query_execution_payload: Optional[Dict[str, Any]] = None,
     metadata_cache_manager: Optional[_LocalMetadataCacheManager] = None,
     athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> _QueryMetadata:
     """Get query metadata."""
     if (query_execution_payload is not None) and (query_execution_payload["Status"]["State"] in _QUERY_FINAL_STATES):
         if query_execution_payload["Status"]["State"] != "SUCCEEDED":
             reason: str = query_execution_payload["Status"]["StateChangeReason"]
             raise exceptions.QueryFailed(f"Query error: {reason}")
         _query_execution_payload: Dict[str, Any] = query_execution_payload
@@ -228,15 +229,15 @@
     parse_timestamps: List[str] = []
     parse_dates: List[str] = []
     converters: Dict[str, Any] = {}
     binaries: List[str] = []
     col_name: str
     col_type: str
     for col_name, col_type in cols_types.items():
-        pandas_type: str = _data_types.athena2pandas(dtype=col_type)
+        pandas_type: str = _data_types.athena2pandas(dtype=col_type, dtype_backend=dtype_backend)
         if (categories is not None) and (col_name in categories):
             dtype[col_name] = "category"
         elif pandas_type in ["datetime64", "date"]:
             parse_timestamps.append(col_name)
             if pandas_type == "date":
                 parse_dates.append(col_name)
         elif pandas_type == "bytes":
```

### Comparing `awswrangler-3.1.1/awswrangler/athena/_write_iceberg.py` & `awswrangler-3.2.0/awswrangler/athena/_write_iceberg.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Amazon Athena Module containing all to_* write functions."""
 
 import logging
 import uuid
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import boto3
 import pandas as pd
 
 from awswrangler import _utils, catalog, exceptions, s3
 from awswrangler._config import apply_configs
 from awswrangler.athena._executions import wait_query
@@ -21,31 +21,40 @@
 
 def _create_iceberg_table(
     df: pd.DataFrame,
     database: str,
     table: str,
     path: str,
     wg_config: _WorkGroupConfig,
+    partition_cols: Optional[List[str]],
+    additional_table_properties: Optional[Dict[str, Any]],
     index: bool = False,
     data_source: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> None:
     if not path:
         raise exceptions.InvalidArgumentValue("Must specify table location to create the table.")
 
     columns_types, _ = catalog.extract_athena_types(df=df, index=index)
     cols_str: str = ", ".join([f"{k} {v}" for k, v in columns_types.items()])
+    partition_cols_str: str = f"PARTITIONED BY ({', '.join([col for col in partition_cols])})" if partition_cols else ""
+    table_properties_str: str = (
+        ", " + ", ".join([f"'{key}'='{value}'" for key, value in additional_table_properties.items()])
+        if additional_table_properties
+        else ""
+    )
 
     create_sql: str = (
         f"CREATE TABLE IF NOT EXISTS {table} ({cols_str}) "
+        f"{partition_cols_str} "
         f"LOCATION '{path}' "
-        f"TBLPROPERTIES ( 'table_type' ='ICEBERG', 'format'='parquet' )"
+        f"TBLPROPERTIES ('table_type' ='ICEBERG', 'format'='parquet'{table_properties_str})"
     )
 
     query_id: str = _start_query_execution(
         sql=create_sql,
         workgroup=workgroup,
         wg_config=wg_config,
         database=database,
@@ -64,21 +73,23 @@
 def to_iceberg(
     df: pd.DataFrame,
     database: str,
     table: str,
     temp_path: Optional[str] = None,
     index: bool = False,
     table_location: Optional[str] = None,
+    partition_cols: Optional[List[str]] = None,
     keep_files: bool = True,
     data_source: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    additional_table_properties: Optional[Dict[str, Any]] = None,
 ) -> None:
     """
     Insert into Athena Iceberg table using INSERT INTO ... SELECT. Will create Iceberg table if it does not exist.
 
     Creates temporary external table, writes staged files and inserts via INSERT INTO ... SELECT.
 
     Parameters
@@ -93,14 +104,19 @@
         AWS Glue/Athena table name.
     temp_path : str
         Amazon S3 location to store temporary results. Workgroup config will be used if not provided.
     index: bool
         Should consider the DataFrame index as a column?.
     table_location : str, optional
         Amazon S3 location for the table. Will only be used to create a new table if it does not exist.
+    partition_cols: List[str], optional
+        List of column names that will be used to create partitions, including support for transform
+        functions (e.g. "day(ts)").
+
+        https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-creating-tables.html#querying-iceberg-partitioning
     keep_files : bool
         Whether staging files produced by Athena are retained. 'True' by default.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
     workgroup : str, optional
         Athena workgroup.
     encryption : str, optional
@@ -108,14 +124,19 @@
     kms_key : str, optional
         For SSE-KMS, this is the KMS key ARN or ID.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
+    additional_table_properties : Optional[Dict[str, Any]]
+        Additional table properties.
+        e.g. additional_table_properties={'write_target_data_file_size_bytes': '536870912'}
+
+        https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-creating-tables.html#querying-iceberg-table-properties
 
     Returns
     -------
     None
 
     Examples
     --------
@@ -159,14 +180,16 @@
         if not catalog.does_table_exist(database=database, table=table, boto3_session=boto3_session):
             _create_iceberg_table(
                 df=df,
                 database=database,
                 table=table,
                 path=table_location,  # type: ignore[arg-type]
                 wg_config=wg_config,
+                partition_cols=partition_cols,
+                additional_table_properties=additional_table_properties,
                 index=index,
                 data_source=data_source,
                 workgroup=workgroup,
                 encryption=encryption,
                 kms_key=kms_key,
                 boto3_session=boto3_session,
             )
```

### Comparing `awswrangler-3.1.1/awswrangler/catalog/__init__.py` & `awswrangler-3.2.0/awswrangler/catalog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 """Amazon Glue Catalog Module."""
 
-from awswrangler.catalog._add import add_column, add_csv_partitions, add_json_partitions, add_parquet_partitions  # noqa
+from awswrangler.catalog._add import (
+    add_column,
+    add_csv_partitions,
+    add_json_partitions,
+    add_orc_partitions,
+    add_parquet_partitions,
+)
+
+# noqa
 from awswrangler.catalog._create import (  # noqa
     _create_csv_table,
     _create_json_table,
     _create_parquet_table,
     create_csv_table,
     create_database,
     create_json_table,
+    create_orc_table,
     create_parquet_table,
     overwrite_table_parameters,
     upsert_table_parameters,
 )
 from awswrangler.catalog._delete import (  # noqa
     delete_all_partitions,
     delete_column,
@@ -50,28 +59,30 @@
 )
 
 __all__ = [
     "add_column",
     "add_csv_partitions",
     "add_json_partitions",
     "add_parquet_partitions",
+    "add_orc_partitions",
     "does_table_exist",
     "delete_column",
     "drop_duplicated_columns",
     "extract_athena_types",
     "rename_duplicated_columns",
     "sanitize_column_name",
     "sanitize_dataframe_columns_names",
     "sanitize_table_name",
     "_create_csv_table",
     "_create_parquet_table",
     "_create_json_table",
     "create_csv_table",
     "create_database",
     "create_parquet_table",
+    "create_orc_table",
     "create_json_table",
     "overwrite_table_parameters",
     "upsert_table_parameters",
     "_get_table_input",
     "databases",
     "get_columns_comments",
     "get_connection",
```

### Comparing `awswrangler-3.1.1/awswrangler/catalog/_add.py` & `awswrangler-3.2.0/awswrangler/catalog/_add.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from awswrangler import _utils, exceptions, typing
 from awswrangler._config import apply_configs
 from awswrangler.catalog._definitions import (
     _check_column_type,
     _csv_partition_definition,
     _json_partition_definition,
+    _orc_partition_definition,
     _parquet_partition_definition,
     _update_table_definition,
 )
 from awswrangler.catalog._utils import _catalog_id, _transaction_id, sanitize_table_name
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
@@ -283,14 +284,92 @@
                 location=k,
                 values=v,
                 bucketing_info=bucketing_info,
                 compression=compression,
                 columns_types=columns_types,
                 partitions_parameters=partitions_parameters,
             )
+            for k, v in partitions_values.items()
+        ]
+        _add_partitions(
+            database=database, table=table, boto3_session=boto3_session, inputs=inputs, catalog_id=catalog_id
+        )
+
+
+@apply_configs
+def add_orc_partitions(
+    database: str,
+    table: str,
+    partitions_values: Dict[str, List[str]],
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
+    catalog_id: Optional[str] = None,
+    compression: Optional[str] = None,
+    boto3_session: Optional[boto3.Session] = None,
+    columns_types: Optional[Dict[str, str]] = None,
+    partitions_parameters: Optional[Dict[str, str]] = None,
+) -> None:
+    """Add partitions (metadata) to a ORC Table in the AWS Glue Catalog.
+
+    Parameters
+    ----------
+    database : str
+        Database name.
+    table : str
+        Table name.
+    partitions_values: Dict[str, List[str]]
+        Dictionary with keys as S3 path locations and values as a list of partitions values as str
+        (e.g. {'s3://bucket/prefix/y=2020/m=10/': ['2020', '10']}).
+    bucketing_info: Tuple[List[str], int], optional
+        Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
+        second element.
+        Only `str`, `int` and `bool` are supported as column data types for bucketing.
+    catalog_id : str, optional
+        The ID of the Data Catalog from which to retrieve Databases.
+        If none is provided, the AWS account ID is used by default.
+    compression: str, optional
+        Compression style (``None``, ``snappy``, ``zlib``, etc).
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
+    columns_types: Optional[Dict[str, str]]
+        Only required for Hive compability.
+        Dictionary with keys as column names and values as data types (e.g. {'col0': 'bigint', 'col1': 'double'}).
+        P.S. Only materialized columns please, not partition columns.
+    partitions_parameters: Optional[Dict[str, str]]
+        Dictionary with key-value pairs defining partition parameters.
+
+    Returns
+    -------
+    None
+        None.
+
+    Examples
+    --------
+    >>> import awswrangler as wr
+    >>> wr.catalog.add_orc_partitions(
+    ...     database='default',
+    ...     table='my_table',
+    ...     partitions_values={
+    ...         's3://bucket/prefix/y=2020/m=10/': ['2020', '10'],
+    ...         's3://bucket/prefix/y=2020/m=11/': ['2020', '11'],
+    ...         's3://bucket/prefix/y=2020/m=12/': ['2020', '12']
+    ...     }
+    ... )
+
+    """
+    table = sanitize_table_name(table=table)
+    if partitions_values:
+        inputs: List[Dict[str, Any]] = [
+            _orc_partition_definition(
+                location=k,
+                values=v,
+                bucketing_info=bucketing_info,
+                compression=compression,
+                columns_types=columns_types,
+                partitions_parameters=partitions_parameters,
+            )
             for k, v in partitions_values.items()
         ]
         _add_partitions(
             database=database, table=table, boto3_session=boto3_session, inputs=inputs, catalog_id=catalog_id
         )
```

### Comparing `awswrangler-3.1.1/awswrangler/catalog/_create.py` & `awswrangler-3.2.0/awswrangler/catalog/_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 import logging
 from typing import TYPE_CHECKING, Any, Dict, Literal, Optional
 
 import boto3
 
 from awswrangler import _utils, exceptions, typing
 from awswrangler._config import apply_configs
-from awswrangler.catalog._definitions import _csv_table_definition, _json_table_definition, _parquet_table_definition
+from awswrangler.catalog._definitions import (
+    _csv_table_definition,
+    _json_table_definition,
+    _orc_table_definition,
+    _parquet_table_definition,
+)
 from awswrangler.catalog._delete import delete_all_partitions, delete_table_if_exists
 from awswrangler.catalog._get import _get_table_input
 from awswrangler.catalog._utils import _catalog_id, _transaction_id, sanitize_column_name, sanitize_table_name
 
 if TYPE_CHECKING:
     from mypy_boto3_glue import GlueClient
 
@@ -331,14 +336,76 @@
         partitions_types=partitions_types,
         transaction_id=transaction_id,
         athena_partition_projection_settings=athena_partition_projection_settings,
         catalog_id=catalog_id,
     )
 
 
+def _create_orc_table(
+    database: str,
+    table: str,
+    path: str,
+    columns_types: Dict[str, str],
+    table_type: Optional[str],
+    partitions_types: Optional[Dict[str, str]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
+    catalog_id: Optional[str],
+    compression: Optional[str],
+    description: Optional[str],
+    parameters: Optional[Dict[str, str]],
+    columns_comments: Optional[Dict[str, str]],
+    mode: str,
+    catalog_versioning: bool,
+    transaction_id: Optional[str],
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings],
+    boto3_session: Optional[boto3.Session],
+    catalog_table_input: Optional[Dict[str, Any]],
+) -> None:
+    table = sanitize_table_name(table=table)
+    partitions_types = {} if partitions_types is None else partitions_types
+    _logger.debug("catalog_table_input: %s", catalog_table_input)
+
+    table_input: Dict[str, Any]
+    if (catalog_table_input is not None) and (mode in ("append", "overwrite_partitions")):
+        table_input = catalog_table_input
+
+        is_table_updated = _update_table_input(table_input, columns_types)
+        if is_table_updated:
+            mode = "update"
+    else:
+        table_input = _orc_table_definition(
+            table=table,
+            path=path,
+            columns_types=columns_types,
+            table_type=table_type,
+            partitions_types=partitions_types,
+            bucketing_info=bucketing_info,
+            compression=compression,
+        )
+    table_exist: bool = catalog_table_input is not None
+    _logger.debug("table_exist: %s", table_exist)
+    _create_table(
+        database=database,
+        table=table,
+        description=description,
+        parameters=parameters,
+        columns_comments=columns_comments,
+        mode=mode,
+        catalog_versioning=catalog_versioning,
+        boto3_session=boto3_session,
+        table_input=table_input,
+        table_type=table_type,
+        table_exist=table_exist,
+        partitions_types=partitions_types,
+        transaction_id=transaction_id,
+        athena_partition_projection_settings=athena_partition_projection_settings,
+        catalog_id=catalog_id,
+    )
+
+
 def _create_csv_table(  # pylint: disable=too-many-arguments,too-many-locals
     database: str,
     table: str,
     path: Optional[str],
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Optional[Dict[str, str]],
@@ -809,14 +876,176 @@
         database=database,
         table=table,
         path=path,
         columns_types=columns_types,
         table_type=table_type,
         partitions_types=partitions_types,
         bucketing_info=bucketing_info,
+        catalog_id=catalog_id,
+        compression=compression,
+        description=description,
+        parameters=parameters,
+        columns_comments=columns_comments,
+        mode=mode,
+        catalog_versioning=catalog_versioning,
+        transaction_id=transaction_id,
+        athena_partition_projection_settings=athena_partition_projection_settings,
+        boto3_session=boto3_session,
+        catalog_table_input=catalog_table_input,
+    )
+
+
+@apply_configs
+def create_orc_table(
+    database: str,
+    table: str,
+    path: str,
+    columns_types: Dict[str, str],
+    table_type: Optional[str] = None,
+    partitions_types: Optional[Dict[str, str]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
+    catalog_id: Optional[str] = None,
+    compression: Optional[str] = None,
+    description: Optional[str] = None,
+    parameters: Optional[Dict[str, str]] = None,
+    columns_comments: Optional[Dict[str, str]] = None,
+    mode: Literal["overwrite", "append"] = "overwrite",
+    catalog_versioning: bool = False,
+    transaction_id: Optional[str] = None,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
+    boto3_session: Optional[boto3.Session] = None,
+) -> None:
+    """Create a ORC Table (Metadata Only) in the AWS Glue Catalog.
+
+    'https://docs.aws.amazon.com/athena/latest/ug/data-types.html'
+
+    Parameters
+    ----------
+    database : str
+        Database name.
+    table : str
+        Table name.
+    path : str
+        Amazon S3 path (e.g. s3://bucket/prefix/).
+    columns_types: Dict[str, str]
+        Dictionary with keys as column names and values as data types (e.g. {'col0': 'bigint', 'col1': 'double'}).
+    table_type: str, optional
+        The type of the Glue Table (EXTERNAL_TABLE, GOVERNED...). Set to EXTERNAL_TABLE if None
+    partitions_types: Dict[str, str], optional
+        Dictionary with keys as partition names and values as data types (e.g. {'col2': 'date'}).
+    bucketing_info: Tuple[List[str], int], optional
+        Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
+        second element.
+        Only `str`, `int` and `bool` are supported as column data types for bucketing.
+    catalog_id : str, optional
+        The ID of the Data Catalog from which to retrieve Databases.
+        If none is provided, the AWS account ID is used by default.
+    compression: str, optional
+        Compression style (``None``, ``snappy``, ``gzip``, etc).
+    description: str, optional
+        Table description
+    parameters: Dict[str, str], optional
+        Key/value pairs to tag the table.
+    columns_comments: Dict[str, str], optional
+        Columns names and the related comments (e.g. {'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}).
+    mode: str
+        'overwrite' to recreate any possible existing table or 'append' to keep any possible existing table.
+    catalog_versioning : bool
+        If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
+    transaction_id: str, optional
+        The ID of the transaction (i.e. used with GOVERNED tables).
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Parameters of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
+
+    Returns
+    -------
+    None
+        None.
+
+    Examples
+    --------
+    >>> import awswrangler as wr
+    >>> wr.catalog.create_parquet_table(
+    ...     database='default',
+    ...     table='my_table',
+    ...     path='s3://bucket/prefix/',
+    ...     columns_types={'col0': 'bigint', 'col1': 'double'},
+    ...     partitions_types={'col2': 'date'},
+    ...     compression='snappy',
+    ...     description='My own table!',
+    ...     parameters={'source': 'postgresql'},
+    ...     columns_comments={'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}
+    ... )
+
+    """
+    catalog_table_input: Optional[Dict[str, Any]] = _get_table_input(
+        database=database,
+        table=table,
+        boto3_session=boto3_session,
+        transaction_id=transaction_id,
+        catalog_id=catalog_id,
+    )
+    _create_orc_table(
+        database=database,
+        table=table,
+        path=path,
+        columns_types=columns_types,
+        table_type=table_type,
+        partitions_types=partitions_types,
+        bucketing_info=bucketing_info,
         catalog_id=catalog_id,
         compression=compression,
         description=description,
         parameters=parameters,
         columns_comments=columns_comments,
         mode=mode,
         catalog_versioning=catalog_versioning,
```

### Comparing `awswrangler-3.1.1/awswrangler/catalog/_definitions.py` & `awswrangler-3.2.0/awswrangler/catalog/_definitions.py`

 * *Files 15% similar despite different names*

```diff
@@ -100,14 +100,86 @@
     if columns_types is not None:
         definition["StorageDescriptor"]["Columns"] = [
             {"Name": cname, "Type": dtype} for cname, dtype in columns_types.items()
         ]
     return definition
 
 
+def _orc_table_definition(
+    table: str,
+    path: str,
+    columns_types: Dict[str, str],
+    table_type: Optional[str],
+    partitions_types: Dict[str, str],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
+    compression: Optional[str],
+) -> Dict[str, Any]:
+    compressed: bool = compression is not None
+    return {
+        "Name": table,
+        "PartitionKeys": [{"Name": cname, "Type": dtype} for cname, dtype in partitions_types.items()],
+        "TableType": "EXTERNAL_TABLE" if table_type is None else table_type,
+        "Parameters": {"classification": "orc", "compressionType": str(compression).lower(), "typeOfData": "file"},
+        "StorageDescriptor": {
+            "Columns": [{"Name": cname, "Type": dtype} for cname, dtype in columns_types.items()],
+            "Location": path,
+            "InputFormat": "org.apache.hadoop.hive.ql.io.orc.OrcInputFormat",
+            "OutputFormat": "org.apache.hadoop.hive.ql.io.orc.OrcOutputFormat",
+            "Compressed": compressed,
+            "NumberOfBuckets": -1 if bucketing_info is None else bucketing_info[1],
+            "SerdeInfo": {
+                "SerializationLibrary": "org.apache.hadoop.hive.ql.io.orc.OrcSerde",
+                "Parameters": {"serialization.format": "1"},
+            },
+            "BucketColumns": [] if bucketing_info is None else bucketing_info[0],
+            "StoredAsSubDirectories": False,
+            "SortColumns": [],
+            "Parameters": {
+                "CrawlerSchemaDeserializerVersion": "1.0",
+                "classification": "orc",
+                "compressionType": str(compression).lower(),
+                "typeOfData": "file",
+            },
+        },
+    }
+
+
+def _orc_partition_definition(
+    location: str,
+    values: List[str],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
+    compression: Optional[str],
+    columns_types: Optional[Dict[str, str]],
+    partitions_parameters: Optional[Dict[str, str]],
+) -> Dict[str, Any]:
+    compressed: bool = compression is not None
+    definition: Dict[str, Any] = {
+        "StorageDescriptor": {
+            "InputFormat": "org.apache.hadoop.hive.ql.io.orc.OrcInputFormat",
+            "OutputFormat": "org.apache.hadoop.hive.ql.io.orc.OrcOutputFormat",
+            "Location": location,
+            "Compressed": compressed,
+            "SerdeInfo": {
+                "Parameters": {"serialization.format": "1"},
+                "SerializationLibrary": "org.apache.hadoop.hive.ql.io.orc.OrcSerde",
+            },
+            "StoredAsSubDirectories": False,
+            "NumberOfBuckets": -1 if bucketing_info is None else bucketing_info[1],
+            "BucketColumns": [] if bucketing_info is None else bucketing_info[0],
+        },
+        "Values": values,
+        "Parameters": {} if partitions_parameters is None else partitions_parameters,
+    }
+    if columns_types is not None:
+        definition["StorageDescriptor"]["Columns"] = [
+            {"Name": cname, "Type": dtype} for cname, dtype in columns_types.items()
+        ]
+    return definition
+
+
 def _csv_table_definition(
     table: str,
     path: Optional[str],
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Dict[str, str],
     bucketing_info: Optional[typing.BucketingInfoTuple],
```

### Comparing `awswrangler-3.1.1/awswrangler/catalog/_delete.py` & `awswrangler-3.2.0/awswrangler/catalog/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/catalog/_get.py` & `awswrangler-3.2.0/awswrangler/catalog/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/catalog/_utils.py` & `awswrangler-3.2.0/awswrangler/catalog/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/chime.py` & `awswrangler-3.2.0/awswrangler/chime.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/cloudwatch.py` & `awswrangler-3.2.0/awswrangler/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/data_api/rds.py` & `awswrangler-3.2.0/awswrangler/data_api/_connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,160 +1,162 @@
-"""RDS Data API Connector."""
-import logging
-import time
-import uuid
-from typing import Any, Dict, List, Optional
-
-import boto3
+"""Data API Connector base class."""
+import datetime as dt
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
+from decimal import Decimal
+from types import TracebackType
+from typing import Any, Dict, List, Optional, Type, Union
 
 import awswrangler.pandas as pd
-from awswrangler import _utils
-from awswrangler.data_api import _connector
 
 
-class RdsDataApi(_connector.DataApiConnector):
-    """Provides access to the RDS Data API.
+class DataApiConnector(ABC):
+    """Base class for Data API (RDS, Redshift, etc.) connectors."""
 
-    Parameters
-    ----------
-    resource_arn: str
-        ARN for the RDS resource.
-    database: str
-        Target database name.
-    secret_arn: str
-        The ARN for the secret to be used for authentication.
-    sleep: float
-        Number of seconds to sleep between connection attempts to paused clusters - defaults to 0.5.
-    backoff: float
-        Factor by which to increase the sleep between connection attempts to paused clusters - defaults to 1.0.
-    retries: int
-        Maximum number of connection attempts to paused clusters - defaults to 10.
-    boto3_session : boto3.Session(), optional
-        The boto3 session. If `None`, the default boto3 session is used.
-    """
+    def execute(
+        self,
+        sql: str,
+        database: Optional[str] = None,
+        transaction_id: Optional[str] = None,
+        parameters: Optional[List[Dict[str, Any]]] = None,
+    ) -> pd.DataFrame:
+        """Execute SQL statement against a Data API Service.
+
+        Parameters
+        ----------
+        sql: str
+            SQL statement to execute.
+
+        Returns
+        -------
+        A Pandas DataFrame containing the execution results.
+        """
+        request_id: str = self._execute_statement(
+            sql, database=database, transaction_id=transaction_id, parameters=parameters
+        )
+        return self._get_statement_result(request_id)
 
-    def __init__(
+    def batch_execute(
         self,
-        resource_arn: str,
-        database: str,
-        secret_arn: str = "",
-        sleep: float = 0.5,
-        backoff: float = 1.0,
-        retries: int = 30,
-        boto3_session: Optional[boto3.Session] = None,
+        sql: Union[str, List[str]],
+        database: Optional[str] = None,
+        transaction_id: Optional[str] = None,
+        parameter_sets: Optional[List[List[Dict[str, Any]]]] = None,
     ) -> None:
-        self.resource_arn = resource_arn
-        self.database = database
-        self.secret_arn = secret_arn
-        self.wait_config = _connector.WaitConfig(sleep, backoff, retries)
-        self.client = _utils.client(service_name="rds-data", session=boto3_session)
-        self.results: Dict[str, Dict[str, Any]] = {}
-        logger: logging.Logger = logging.getLogger(__name__)
-        super().__init__(self.client, logger)
-
-    def _execute_statement(self, sql: str, database: Optional[str] = None) -> str:
-        if database is None:
-            database = self.database
-
-        sleep: float = self.wait_config.sleep
-        total_tries: int = 0
-        total_sleep: float = 0
-        response: Optional[Dict[str, Any]] = None
-        last_exception: Optional[Exception] = None
-        while total_tries < self.wait_config.retries:
-            try:
-                response = self.client.execute_statement(
-                    resourceArn=self.resource_arn,
-                    database=database,
-                    sql=sql,
-                    secretArn=self.secret_arn,
-                    includeResultMetadata=True,
-                )
-                self.logger.debug(
-                    "Response received after %s tries and sleeping for a total of %s seconds", total_tries, total_sleep
-                )
-                break
-            except self.client.exceptions.BadRequestException as exception:
-                last_exception = exception
-                total_sleep += sleep
-                self.logger.debug("BadRequestException occurred: %s", exception)
-                self.logger.debug(
-                    "Cluster may be paused - sleeping for %s seconds for a total of %s before retrying",
-                    sleep,
-                    total_sleep,
-                )
-                time.sleep(sleep)
-                total_tries += 1
-                sleep *= self.wait_config.backoff
-
-        if response is None:
-            self.logger.exception("Maximum BadRequestException retries reached for query %s", sql)
-            raise last_exception  # type: ignore[misc]
-
-        request_id: str = uuid.uuid4().hex
-        self.results[request_id] = response
-        return request_id
+        """Batch execute SQL statements against a Data API Service.
 
+        Parameters
+        ----------
+        sql: str
+            SQL statement to execute.
+        """
+        self._batch_execute_statement(
+            sql, database=database, transaction_id=transaction_id, parameter_sets=parameter_sets
+        )
+
+    def __enter__(self) -> "DataApiConnector":
+        return self
+
+    @abstractmethod
+    def close(self) -> None:
+        """Close underlying endpoint connections."""
+        pass
+
+    def __exit__(
+        self,
+        exception_type: Optional[Type[BaseException]],
+        exception_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> Optional[bool]:
+        self.close()
+        return None
+
+    @abstractmethod
+    def begin_transaction(self, database: Optional[str] = None, schema: Optional[str] = None) -> str:
+        pass
+
+    @abstractmethod
+    def commit_transaction(self, transaction_id: str) -> str:
+        pass
+
+    @abstractmethod
+    def rollback_transaction(self, transaction_id: str) -> str:
+        pass
+
+    @abstractmethod
+    def _execute_statement(
+        self,
+        sql: str,
+        database: Optional[str] = None,
+        transaction_id: Optional[str] = None,
+        parameters: Optional[List[Dict[str, Any]]] = None,
+    ) -> str:
+        pass
+
+    @abstractmethod
+    def _batch_execute_statement(
+        self,
+        sql: Union[str, List[str]],
+        database: Optional[str] = None,
+        transaction_id: Optional[str] = None,
+        parameter_sets: Optional[List[List[Dict[str, Any]]]] = None,
+    ) -> str:
+        pass
+
+    @abstractmethod
     def _get_statement_result(self, request_id: str) -> pd.DataFrame:
-        try:
-            result = self.results.pop(request_id)
-        except KeyError as exception:
-            raise KeyError(f"Request {request_id} not found in results {self.results}") from exception
-
-        if "records" not in result:
-            return pd.DataFrame()
-
-        rows: List[List[Any]] = []
-        for record in result["records"]:
-            row: List[Any] = [
-                _connector.DataApiConnector._get_column_value(column)  # pylint: disable=protected-access
-                for column in record
-            ]
-            rows.append(row)
-
-        column_names: List[str] = [column["name"] for column in result["columnMetadata"]]
-        dataframe = pd.DataFrame(rows, columns=column_names)
-        return dataframe
-
-
-def connect(
-    resource_arn: str, database: str, secret_arn: str = "", boto3_session: Optional[boto3.Session] = None, **kwargs: Any
-) -> RdsDataApi:
-    """Create a RDS Data API connection.
-
-    Parameters
-    ----------
-    resource_arn: str
-        ARN for the RDS resource.
-    database: str
-        Target database name.
-    secret_arn: str
-        The ARN for the secret to be used for authentication.
-    boto3_session : boto3.Session(), optional
-        The boto3 session. If `None`, the default boto3 session is used.
-    **kwargs
-        Any additional kwargs are passed to the underlying RdsDataApi class.
-
-    Returns
-    -------
-    A RdsDataApi connection instance that can be used with `wr.rds.data_api.read_sql_query`.
-    """
-    return RdsDataApi(resource_arn, database, secret_arn=secret_arn, boto3_session=boto3_session, **kwargs)
-
-
-def read_sql_query(sql: str, con: RdsDataApi, database: Optional[str] = None) -> pd.DataFrame:
-    """Run an SQL query on an RdsDataApi connection and return the result as a DataFrame.
-
-    Parameters
-    ----------
-    sql: str
-        SQL query to run.
-    con: RdsDataApi
-        A RdsDataApi connection instance
-    database: str
-        Database to run query on - defaults to the database specified by `con`.
-
-    Returns
-    -------
-    A Pandas DataFrame containing the query results.
-    """
-    return con.execute(sql, database=database)
+        pass
+
+    @staticmethod
+    def _get_column_value(  # pylint: disable=too-many-return-statements
+        column_value: Dict[str, Any], col_type: Optional[str] = None
+    ) -> Any:
+        """Return the first non-null key value for a given dictionary.
+
+        The key names for a given record depend on the column type: stringValue, longValue, etc.
+
+        Therefore, a record in the response does not have consistent key names. The ColumnMetadata
+        typeName information could be used to infer the key, but there is no direct mapping here
+        that could be easily parsed with creating a static dictionary:
+            varchar -> stringValue
+            int2 -> longValue
+            timestamp -> stringValue
+
+        What has been observed is that each record appears to have a single key, so this function
+        iterates over the keys and returns the first non-null value. If none are found, None is
+        returned.
+
+        Documentation:
+            https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Client.get_statement_result
+            https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService.Client.execute_statement
+        """
+        for key in column_value:
+            if column_value[key] is not None:
+                if (key == "isNull") and column_value[key]:
+                    return None
+                if key == "arrayValue":
+                    raise ValueError(f"arrayValue not supported yet - could not extract {column_value[key]}")
+
+                if key == "stringValue":
+                    if col_type == "DATETIME":
+                        return dt.datetime.strptime(column_value[key], "%Y-%m-%d %H:%M:%S")
+
+                    if col_type == "DATE":
+                        return dt.datetime.strptime(column_value[key], "%Y-%m-%d").date()
+
+                    if col_type == "TIME":
+                        return dt.datetime.strptime(column_value[key], "%H:%M:%S").time()
+
+                    if col_type == "DECIMAL":
+                        return Decimal(column_value[key])
+
+                return column_value[key]
+        return None
+
+
+@dataclass
+class WaitConfig:
+    """Holds standard wait configuration values."""
+
+    sleep: float
+    backoff: float
+    retries: int
```

### Comparing `awswrangler-3.1.1/awswrangler/data_api/redshift.py` & `awswrangler-3.2.0/awswrangler/data_api/redshift.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """Redshift Data API Connector."""
 import logging
 import time
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import boto3
 
 import awswrangler.pandas as pd
-from awswrangler import _utils
+from awswrangler import _utils, exceptions
 from awswrangler.data_api import _connector
 
+if TYPE_CHECKING:
+    from mypy_boto3_redshift_data.client import RedshiftDataAPIServiceClient
+    from mypy_boto3_redshift_data.type_defs import ColumnMetadataTypeDef
+
+
+_logger = logging.getLogger(__name__)
+
 
 class RedshiftDataApi(_connector.DataApiConnector):
     """Provides access to a Redshift cluster via the Data API.
 
     Note
     ----
     When connecting to a standard Redshift cluster, `cluster_id` is used.
@@ -48,35 +55,63 @@
         secret_arn: str = "",
         db_user: str = "",
         sleep: float = 0.25,
         backoff: float = 1.5,
         retries: int = 15,
         boto3_session: Optional[boto3.Session] = None,
     ) -> None:
+        super().__init__()
+
+        self.client = _utils.client(service_name="redshift-data", session=boto3_session)
+
         self.cluster_id = cluster_id
         self.database = database
         self.workgroup_name = workgroup_name
         self.secret_arn = secret_arn
         self.db_user = db_user
-        self.client = _utils.client(service_name="redshift-data", session=boto3_session)
         self.waiter = RedshiftDataApiWaiter(self.client, sleep, backoff, retries)
-        logger: logging.Logger = logging.getLogger(__name__)
-        super().__init__(self.client, logger)
+
+    def close(self) -> None:
+        """Close underlying endpoint connections."""
+        self.client.close()
+
+    def begin_transaction(self, database: Optional[str] = None, schema: Optional[str] = None) -> str:
+        """Start an SQL transaction."""
+        raise NotImplementedError("Redshift Data API does not support transactions.")
+
+    def commit_transaction(self, transaction_id: str) -> str:
+        """Commit an SQL transaction."""
+        raise NotImplementedError("Redshift Data API does not support transactions.")
+
+    def rollback_transaction(self, transaction_id: str) -> str:
+        """Roll back an SQL transaction."""
+        raise NotImplementedError("Redshift Data API does not support transactions.")
 
     def _validate_redshift_target(self) -> None:
-        if self.database == "":
+        if not self.database:
             raise ValueError("`database` must be set for connection")
-        if self.cluster_id == "" and self.workgroup_name == "":
+        if not self.cluster_id and not self.workgroup_name:
             raise ValueError("Either `cluster_id` or `workgroup_name`(Redshift Serverless) must be set for connection")
 
     def _validate_auth_method(self) -> None:
-        if self.workgroup_name == "" and self.secret_arn == "" and self.db_user == "":
+        if not self.workgroup_name and not self.secret_arn and not self.db_user:
             raise ValueError("Either `secret_arn` or `db_user` must be set for authentication")
 
-    def _execute_statement(self, sql: str, database: Optional[str] = None) -> str:
+    def _execute_statement(
+        self,
+        sql: str,
+        database: Optional[str] = None,
+        transaction_id: Optional[str] = None,
+        parameters: Optional[List[Dict[str, Any]]] = None,
+    ) -> str:
+        if transaction_id:
+            exceptions.InvalidArgument("`transaction_id` not supported for Redshift Data API")
+        if parameters:
+            exceptions.InvalidArgument("`parameters` not supported for Redshift Data API")
+
         self._validate_redshift_target()
         self._validate_auth_method()
         credentials = {}
         if self.secret_arn:
             credentials = {"SecretArn": self.secret_arn}
         elif self.db_user:
             credentials = {"DbUser": self.db_user}
@@ -85,40 +120,48 @@
             database = self.database
 
         if self.cluster_id:
             redshift_target = {"ClusterIdentifier": self.cluster_id}
         elif self.workgroup_name:
             redshift_target = {"WorkgroupName": self.workgroup_name}
 
-        self.logger.debug("Executing %s", sql)
+        _logger.debug("Executing %s", sql)
         response = self.client.execute_statement(
-            **redshift_target,
+            **redshift_target,  # type: ignore[arg-type]
             Database=database,
             Sql=sql,
-            **credentials,
+            **credentials,  # type: ignore[arg-type]
         )
-        return str(response["Id"])
+        return response["Id"]
+
+    def _batch_execute_statement(
+        self,
+        sql: Union[str, List[str]],
+        database: Optional[str] = None,
+        transaction_id: Optional[str] = None,
+        parameter_sets: Optional[List[List[Dict[str, Any]]]] = None,
+    ) -> str:
+        raise NotImplementedError("Batch execute statement not support for Redshift Data API.")
 
     def _get_statement_result(self, request_id: str) -> pd.DataFrame:
         self.waiter.wait(request_id)
-        response: Dict[str, Any]
-        response = self.client.describe_statement(Id=request_id)
-        if not response["HasResultSet"]:
+        describe_response = self.client.describe_statement(Id=request_id)
+        if not describe_response["HasResultSet"]:
             return pd.DataFrame()
 
         paginator = self.client.get_paginator("get_statement_result")
         response_iterator = paginator.paginate(Id=request_id)
 
         rows: List[List[Any]] = []
-        column_metadata: List[Dict[str, str]]
+        column_metadata: List["ColumnMetadataTypeDef"]
         for response in response_iterator:
             column_metadata = response["ColumnMetadata"]
             for record in response["Records"]:
                 row: List[Any] = [
-                    _connector.DataApiConnector._get_column_value(column)  # pylint: disable=protected-access
+                    _connector.DataApiConnector._get_column_value(column)  # type: ignore[arg-type]  # pylint: disable=protected-access
                     for column in record
                 ]
                 rows.append(row)
 
         column_names: List[str] = [column["name"] for column in column_metadata]
         dataframe = pd.DataFrame(rows, columns=column_names)
         return dataframe
@@ -135,18 +178,17 @@
         Number of seconds to sleep between tries.
     backoff: float
         Factor by which to increase the sleep between tries.
     retries: int
         Maximum number of tries.
     """
 
-    def __init__(self, client: Any, sleep: float, backoff: float, retries: int) -> None:
+    def __init__(self, client: "RedshiftDataAPIServiceClient", sleep: float, backoff: float, retries: int) -> None:
         self.client = client
         self.wait_config = _connector.WaitConfig(sleep, backoff, retries)
-        self.logger: logging.Logger = logging.getLogger(__name__)
 
     def wait(self, request_id: str) -> bool:
         """Wait for the `describe_statement` function of self.client to return a completed status.
 
         Parameters
         ----------
         request_id:
@@ -158,24 +200,24 @@
         Raises RedshiftDataApiExecutionFailedException if FAILED or ABORTED.
         Raises RedshiftDataApiExecutionTimeoutException if retries exceeded before completion.
         """
         sleep: float = self.wait_config.sleep
         total_sleep: float = 0
         total_tries: int = 0
         while total_tries <= self.wait_config.retries:
-            response: Dict[str, Any] = self.client.describe_statement(Id=request_id)
+            response = self.client.describe_statement(Id=request_id)
             status: str = response["Status"]
             if status == "FINISHED":
                 return True
             if status in ["ABORTED", "FAILED"]:
                 error = response["Error"]
                 raise RedshiftDataApiFailedException(
                     f"Request {request_id} failed with status {status} and error {error}"
                 )
-            self.logger.debug("Statement execution status %s - sleeping for %s seconds", status, sleep)
+            _logger.debug("Statement execution status %s - sleeping for %s seconds", status, sleep)
             time.sleep(sleep)
             sleep = sleep * self.wait_config.backoff
             total_tries += 1
             total_sleep += sleep
         raise RedshiftDataApiTimeoutException(
             f"Request {request_id} timed out after {total_tries} tries and {total_sleep}s total sleep"
         )
```

### Comparing `awswrangler-3.1.1/awswrangler/data_quality/_create.py` & `awswrangler-3.2.0/awswrangler/data_quality/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/data_quality/_get.py` & `awswrangler-3.2.0/awswrangler/data_quality/_get.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/data_quality/_utils.py` & `awswrangler-3.2.0/awswrangler/data_quality/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,12 +171,20 @@
     client_glue = _utils.client(service_name="glue", session=boto3_session)
 
     results = client_glue.batch_get_data_quality_result(
         ResultIds=result_ids,
     )["Results"]
     rule_results: List[Dict[str, Any]] = []
     for result in results:
-        rules = result["RuleResults"]
-        for rule in rules:
-            rule["ResultId"] = result["ResultId"]  # type: ignore[typeddict-unknown-key]
-        rule_results.extend(cast(List[Dict[str, Any]], rules))
+        rule_results.extend(
+            cast(
+                List[Dict[str, Any]],
+                [
+                    dict(
+                        ((k, d[k]) for k in ("Name", "Description", "Result") if k in d),  # type: ignore[literal-required]
+                        **{"ResultId": result["ResultId"]},
+                    )
+                    for d in result["RuleResults"]
+                ],
+            )
+        )
     return pd.json_normalize(rule_results)
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/_core.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Ray Module."""
 import logging
 import os
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, TypeVar, Union
 
 from awswrangler._config import apply_configs
 from awswrangler._distributed import EngineEnum, engine
 
 if engine.get() == EngineEnum.RAY or TYPE_CHECKING:
     import ray
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+FunctionType = TypeVar("FunctionType", bound=Callable[..., Any])
+
+
 class RayLogger:
     """Create discrete Logger instance for Ray Tasks."""
 
     def __init__(
         self,
         logging_level: int = logging.INFO,
         format: str = "%(asctime)s::%(levelname)-2s::%(name)s::%(message)s",  # pylint: disable=redefined-builtin
@@ -27,18 +30,18 @@
     def get_logger(self, name: Union[str, Any] = None) -> Optional[logging.Logger]:
         """Return logger object."""
         return logging.getLogger(name)
 
 
 @apply_configs
 def ray_logger(
-    function: Callable[..., Any],
+    function: FunctionType,
     configure_logging: bool = True,
     logging_level: int = logging.INFO,
-) -> Callable[..., Any]:
+) -> FunctionType:
     """
     Decorate callable to add RayLogger.
 
     Parameters
     ----------
     function : Callable[..., Any]
         Callable as input to decorator.
@@ -53,29 +56,29 @@
         if configure_logging:
             RayLogger(logging_level=logging_level).get_logger(name=function.__name__)
         return function(*args, **kwargs)
 
     return wrapper
 
 
-def ray_remote(**options: Any) -> Callable[..., Any]:
+def ray_remote(**options: Any) -> Callable[[FunctionType], FunctionType]:
     """
     Decorate with @ray.remote providing .options().
 
     Parameters
     ----------
     options : Any
         Ray remote options
 
     Returns
     -------
     Callable[..., Any]
     """
 
-    def remote_decorator(function: Callable[..., Any]) -> Callable[..., Any]:
+    def remote_decorator(function: FunctionType) -> FunctionType:
         """
         Decorate callable to wrap within ray.remote.
 
         Parameters
         ----------
         function : Callable[..., Any]
             Callable as input to ray.remote.
@@ -160,15 +163,15 @@
         # Detect an existing cluster
         ray_address = os.environ.get("RAY_ADDRESS")
         if not address and ray_address:
             _logger.info("Using address %s set in the environment variable RAY_ADDRESS", ray_address)
             address = ray_address
 
         if address:
-            _logger.info("Connecting to a Ray cluster at: %s", address)
+            _logger.info("Connecting to a Ray instance at: %s", address)
             ray.init(
                 address=address,
                 include_dashboard=include_dashboard,
                 ignore_reinit_error=ignore_reinit_error,
                 configure_logging=configure_logging,
                 log_to_driver=log_to_driver,
                 logging_level=logging_level,
@@ -189,9 +192,9 @@
                 "object_store_memory": object_store_memory,
                 "_redis_password": redis_password,
                 "_memory": object_store_memory,
                 "runtime_env": {
                     "env_vars": {var: os.environ.get(var) for var in ray_runtime_env_vars if os.environ.get(var)}
                 },
             }
-            _logger.info("Starting a Ray cluster")
+            _logger.info("Initializing a Ray instance")
             ray.init(**ray_init_kwargs)
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/_core.pyi` & `awswrangler-3.2.0/awswrangler/distributed/ray/_core.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/_executor.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/_executor.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/_register.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/_register.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,27 +10,30 @@
     split_pandas_frame,
     table_refs_to_df,
 )
 from awswrangler.distributed.ray import ray_remote
 from awswrangler.distributed.ray._executor import _get_ray_executor
 from awswrangler.distributed.ray._utils import ensure_worker_count
 from awswrangler.distributed.ray.s3._list import _list_objects_s3fs
+from awswrangler.distributed.ray.s3._read_orc import _read_orc_metadata_file_distributed
 from awswrangler.distributed.ray.s3._read_parquet import _read_parquet_metadata_file_distributed
 from awswrangler.dynamodb._read import _read_scan
 from awswrangler.dynamodb._write import _put_df, _put_items
 from awswrangler.lakeformation._read import _get_work_unit_results
 from awswrangler.s3._copy import _copy_objects
 from awswrangler.s3._delete import _delete_objects
 from awswrangler.s3._describe import _describe_object
 from awswrangler.s3._list import _list_objects_paginate
+from awswrangler.s3._read_orc import _read_orc, _read_orc_metadata_file
 from awswrangler.s3._read_parquet import _read_parquet, _read_parquet_metadata_file
 from awswrangler.s3._read_text import _read_text
 from awswrangler.s3._select import _select_object_content, _select_query
 from awswrangler.s3._wait import _wait_object_batch
 from awswrangler.s3._write_dataset import _to_buckets, _to_partitions
+from awswrangler.s3._write_orc import _to_orc
 from awswrangler.s3._write_parquet import _to_parquet
 from awswrangler.s3._write_text import _to_text
 from awswrangler.timestream._write import _write_batch, _write_df
 
 
 def register_ray() -> None:
     """Register dispatched Ray and Modin (on Ray) methods."""
@@ -51,46 +54,47 @@
         _put_df,
         _put_items,
         _write_batch,
         _write_df,
     ]:
         engine.register_func(func, ray_remote()(func))
 
-    for o_f, d_f in {
-        _get_executor: _get_ray_executor,
-        _list_objects_paginate: _list_objects_s3fs,
-        _read_parquet_metadata_file: ray_remote()(_read_parquet_metadata_file_distributed),
-        ensure_worker_or_thread_count: ensure_worker_count,
-    }.items():
-        engine.register_func(o_f, d_f)  # type: ignore[arg-type]
+    # Register dispatch methods for Ray
+    engine.register_func(_get_executor, _get_ray_executor)
+    engine.register_func(_list_objects_paginate, _list_objects_s3fs)
+    engine.register_func(_read_parquet_metadata_file, ray_remote()(_read_parquet_metadata_file_distributed))
+    engine.register_func(_read_orc_metadata_file, ray_remote()(_read_orc_metadata_file_distributed))
+    engine.register_func(ensure_worker_or_thread_count, ensure_worker_count)
 
     if memory_format.get() == MemoryFormatEnum.MODIN:
         from awswrangler.distributed.ray.modin._data_types import pyarrow_types_from_pandas_distributed
         from awswrangler.distributed.ray.modin._utils import (
             _arrow_refs_to_df,
             _copy_modin_df_shallow,
             _is_pandas_or_modin_frame,
             _split_modin_frame,
         )
+        from awswrangler.distributed.ray.modin.s3._read_orc import _read_orc_distributed
         from awswrangler.distributed.ray.modin.s3._read_parquet import _read_parquet_distributed
         from awswrangler.distributed.ray.modin.s3._read_text import _read_text_distributed
         from awswrangler.distributed.ray.modin.s3._write_dataset import (
             _to_buckets_distributed,
             _to_partitions_distributed,
         )
+        from awswrangler.distributed.ray.modin.s3._write_orc import _to_orc_distributed
         from awswrangler.distributed.ray.modin.s3._write_parquet import _to_parquet_distributed
         from awswrangler.distributed.ray.modin.s3._write_text import _to_text_distributed
 
-        for o_f, d_f in {
-            pyarrow_types_from_pandas: pyarrow_types_from_pandas_distributed,
-            _read_parquet: _read_parquet_distributed,
-            _read_text: _read_text_distributed,
-            _to_buckets: _to_buckets_distributed,
-            _to_parquet: _to_parquet_distributed,
-            _to_partitions: _to_partitions_distributed,
-            _to_text: _to_text_distributed,
-            copy_df_shallow: _copy_modin_df_shallow,
-            is_pandas_frame: _is_pandas_or_modin_frame,
-            split_pandas_frame: _split_modin_frame,
-            table_refs_to_df: _arrow_refs_to_df,
-        }.items():
-            engine.register_func(o_f, d_f)  # type: ignore[arg-type]
+        # Register dispatch methods for Modin
+        engine.register_func(pyarrow_types_from_pandas, pyarrow_types_from_pandas_distributed)
+        engine.register_func(_read_parquet, _read_parquet_distributed)
+        engine.register_func(_read_text, _read_text_distributed)
+        engine.register_func(_to_buckets, _to_buckets_distributed)
+        engine.register_func(_to_parquet, _to_parquet_distributed)
+        engine.register_func(_to_partitions, _to_partitions_distributed)
+        engine.register_func(_to_text, _to_text_distributed)
+        engine.register_func(_read_orc, _read_orc_distributed)
+        engine.register_func(_to_orc, _to_orc_distributed)
+        engine.register_func(copy_df_shallow, _copy_modin_df_shallow)
+        engine.register_func(is_pandas_frame, _is_pandas_or_modin_frame)
+        engine.register_func(split_pandas_frame, _split_modin_frame)
+        engine.register_func(table_refs_to_df, _arrow_refs_to_df)
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/_utils.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/__init__.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Ray Datasources Module."""
 
 from awswrangler.distributed.ray.datasources.arrow_csv_datasource import ArrowCSVDatasource
 from awswrangler.distributed.ray.datasources.arrow_json_datasource import ArrowJSONDatasource
+from awswrangler.distributed.ray.datasources.arrow_orc_datasource import ArrowORCDatasource
 from awswrangler.distributed.ray.datasources.arrow_parquet_base_datasource import ArrowParquetBaseDatasource
 from awswrangler.distributed.ray.datasources.arrow_parquet_datasource import ArrowParquetDatasource
 from awswrangler.distributed.ray.datasources.pandas_file_based_datasource import UserProvidedKeyBlockWritePathProvider
 from awswrangler.distributed.ray.datasources.pandas_text_datasource import (
     PandasCSVDataSource,
     PandasFWFDataSource,
     PandasJSONDatasource,
     PandasTextDatasource,
 )
 
 __all__ = [
     "ArrowCSVDatasource",
     "ArrowJSONDatasource",
+    "ArrowORCDatasource",
     "ArrowParquetBaseDatasource",
     "ArrowParquetDatasource",
     "PandasCSVDataSource",
     "PandasFWFDataSource",
     "PandasJSONDatasource",
     "PandasTextDatasource",
     "UserProvidedKeyBlockWritePathProvider",
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_json_datasource.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_json_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 (https://github.com/ray-project/ray/blob/ray-2.0.0/python/ray/data/datasource/parquet_datasource.py) with a few changes
 and customized to ensure compatibility with AWS SDK for pandas behavior. Changes from the original implementation,
 are documented in the comments and marked with (AWS SDK for pandas) prefix.
 """
 # pylint: disable=redefined-outer-name,import-outside-toplevel,reimported
 
 import logging
-import time
 from typing import Any, Callable, Dict, Iterator, List, Optional, Union
 
 import numpy as np
 
 # fs required to implicitly trigger S3 subsystem initialization
 import pyarrow.fs  # noqa: F401 pylint: disable=unused-import
-import ray
 from pyarrow.dataset import ParquetFileFragment
 from pyarrow.lib import Schema
 from ray import cloudpickle
 from ray.data._internal.output_buffer import BlockOutputBuffer
+from ray.data._internal.progress_bar import ProgressBar
 from ray.data.block import Block, BlockAccessor
 from ray.data.context import DatasetContext
 from ray.data.datasource import Reader, ReadTask
 from ray.data.datasource.file_based_datasource import _resolve_paths_and_filesystem
 from ray.data.datasource.file_meta_provider import (
     DefaultParquetMetadataProvider,
     ParquetMetadataProvider,
     _handle_read_os_error,
 )
 
+from awswrangler import exceptions
 from awswrangler._arrow import _add_table_partitions, _df_to_table
 from awswrangler.distributed.ray import ray_remote
 from awswrangler.distributed.ray.datasources.arrow_parquet_base_datasource import ArrowParquetBaseDatasource
 from awswrangler.s3._write import _COMPRESSION_2_EXT
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
@@ -185,28 +185,36 @@
     raise final_exception  # type: ignore[misc]
 
 
 class _ArrowParquetDatasourceReader(Reader[Any]):  # pylint: disable=too-many-instance-attributes
     def __init__(
         self,
         paths: Union[str, List[str]],
+        local_uri: bool = False,
         filesystem: Optional["pyarrow.fs.FileSystem"] = None,
         columns: Optional[List[str]] = None,
         schema: Optional[Schema] = None,
         meta_provider: ParquetMetadataProvider = DefaultParquetMetadataProvider(),
         _block_udf: Optional[Callable[[Block[Any]], Block[Any]]] = None,
         **reader_args: Any,
     ):
         import pyarrow as pa
         import pyarrow.parquet as pq
 
         paths, filesystem = _resolve_paths_and_filesystem(paths, filesystem)
         if len(paths) == 1:
             paths = paths[0]
 
+        self._local_scheduling = None
+        if local_uri:
+            import ray
+            from ray.util.scheduling_strategies import NodeAffinitySchedulingStrategy
+
+            self._local_scheduling = NodeAffinitySchedulingStrategy(ray.get_runtime_context().get_node_id(), soft=False)
+
         dataset_kwargs = reader_args.pop("dataset_kwargs", {})
         try:
             pq_ds = pq.ParquetDataset(paths, **dataset_kwargs, filesystem=filesystem, use_legacy_dataset=False)
         except OSError as e:
             _handle_read_os_error(e, paths)
         if schema is None:
             schema = pq_ds.schema
@@ -226,17 +234,24 @@
                     exc_info=True,
                 )
                 inferred_schema = schema
         else:
             inferred_schema = schema
 
         try:
-            self._metadata = meta_provider.prefetch_file_metadata(pq_ds.pieces) or []
+            prefetch_remote_args = {}
+            if self._local_scheduling:
+                prefetch_remote_args["scheduling_strategy"] = self._local_scheduling
+            self._metadata = meta_provider.prefetch_file_metadata(pq_ds.pieces, **prefetch_remote_args) or []
         except OSError as e:
             _handle_read_os_error(e, paths)
+        except pyarrow.ArrowInvalid as ex:
+            if "Parquet file size is 0 bytes" in str(ex):
+                raise exceptions.InvalidFile(f"Invalid Parquet file. {str(ex)}")
+            raise
         self._pq_ds = pq_ds
         self._meta_provider = meta_provider
         self._inferred_schema = inferred_schema
         self._block_udf = _block_udf
         self._reader_args = reader_args
         self._columns = columns
         self._schema = schema
@@ -303,40 +318,46 @@
         if not DatasetContext.get_current().decoding_size_estimation:
             return PARQUET_ENCODING_RATIO_ESTIMATE_DEFAULT
 
         # Sample a few rows from Parquet files to estimate the encoding ratio.
         # Launch tasks to sample multiple files remotely in parallel.
         # Evenly distributed to sample N rows in i-th row group in i-th file.
         # TODO(ekl/cheng) take into account column pruning.
-        start_time = time.perf_counter()
         num_files = len(self._pq_ds.pieces)
         num_samples = int(num_files * PARQUET_ENCODING_RATIO_ESTIMATE_SAMPLING_RATIO)
         min_num_samples = min(PARQUET_ENCODING_RATIO_ESTIMATE_MIN_NUM_SAMPLES, num_files)
         max_num_samples = min(PARQUET_ENCODING_RATIO_ESTIMATE_MAX_NUM_SAMPLES, num_files)
         num_samples = max(min(num_samples, max_num_samples), min_num_samples)
 
         # Evenly distributed to choose which file to sample, to avoid biased prediction
         # if data is skewed.
         file_samples = [
             self._pq_ds.pieces[idx] for idx in np.linspace(0, num_files - 1, num_samples).astype(int).tolist()
         ]
 
         futures = []
-        for idx, sample in enumerate(file_samples):
-            # Sample i-th row group in i-th file.
+        sample_piece = ray_remote(scheduling_strategy=self._local_scheduling or "SPREAD")(_sample_piece)
+        for sample in file_samples:
+            # Sample the first rows batch in i-th file.
             # Use SPREAD scheduling strategy to avoid packing many sampling tasks on
             # same machine to cause OOM issue, as sampling can be memory-intensive.
-            futures.append(_sample_piece(_SerializedPiece(sample), idx))
-        sample_ratios = ray.get(futures)
+            serialized_sample = _SerializedPiece(sample)
+            futures.append(
+                sample_piece(
+                    self._reader_args,
+                    self._columns,
+                    self._schema,
+                    serialized_sample,
+                )
+            )
+        sample_bar = ProgressBar("Parquet Files Sample", len(futures))
+        sample_ratios = sample_bar.fetch_until_complete(futures)
+        sample_bar.close()  # type: ignore[no-untyped-call]
         ratio = np.mean(sample_ratios)
-
-        sampling_duration = time.perf_counter() - start_time
-        if sampling_duration > 5:
-            _logger.info("Parquet input size estimation took %s seconds.", round(sampling_duration, 2))
-        _logger.debug("Estimated Parquet encoding ratio from sampling is %s.", ratio)
+        _logger.debug(f"Estimated Parquet encoding ratio from sampling is {ratio}.")
         return max(ratio, PARQUET_ENCODING_RATIO_ESTIMATE_LOWER_BOUND)  # type: ignore[no-any-return]
 
 
 # (AWS SDK for pandas) The following are the changes to the original ray implementation:
 # 1. Use _add_table_partitions to add partition columns. The behavior is controlled by Pandas SDK
 #    native `dataset` parameter. The partitions are loaded relative to the `path_root` prefix.
 def _read_pieces(
@@ -385,36 +406,48 @@
                 if output_buffer.has_next():
                     yield output_buffer.next()
     output_buffer.finalize()
     if output_buffer.has_next():
         yield output_buffer.next()
 
 
-@ray_remote(scheduling_strategy="SPREAD")
 def _sample_piece(
+    reader_args: Any,
+    columns: Optional[List[str]],
+    schema: Optional[Union[type, "pyarrow.lib.Schema"]],
     file_piece: _SerializedPiece,
-    row_group_id: int,
 ) -> float:
-    # Sample the `row_group_id`-th row group from file piece `serialized_piece`.
+    # Sample the first rows batch from file piece `serialized_piece`.
     # Return the encoding ratio calculated from the sampled rows.
     piece = _deserialize_pieces_with_retry([file_piece])[0]
 
-    # If required row group index is out of boundary, sample the last row group.
-    row_group_id = min(piece.num_row_groups - 1, row_group_id)
-    assert (
-        0 <= row_group_id <= piece.num_row_groups - 1
-    ), f"Required row group id {row_group_id} is not in expected bound"
-
-    row_group = piece.subset(row_group_ids=[row_group_id])
-    metadata = row_group.metadata.row_group(0)
-    num_rows = min(PARQUET_ENCODING_RATIO_ESTIMATE_NUM_ROWS, metadata.num_rows)
-    assert num_rows > 0 and metadata.num_rows > 0, (
-        f"Sampled number of rows: {num_rows} and total number of rows: " f"{metadata.num_rows} should be positive"
+    # Only sample the first row group.
+    piece = piece.subset(row_group_ids=[0])
+    batch_size = max(min(piece.metadata.num_rows, PARQUET_ENCODING_RATIO_ESTIMATE_NUM_ROWS), 1)
+    # Use the batch_size calculated above, and ignore the one specified by user if set.
+    # This is to avoid sampling too few or too many rows.
+    reader_args.pop("batch_size", None)
+    reader_args.pop("path_root", None)
+    batches = piece.to_batches(
+        columns=columns,
+        schema=schema,
+        batch_size=batch_size,
+        **reader_args,
     )
-
-    parquet_size: float = metadata.total_byte_size / metadata.num_rows
-    # Set batch_size to num_rows will instruct Arrow Parquet reader to read exactly
-    # num_rows into memory, o.w. it will read more rows by default in batch manner.
-    in_memory_size: float = row_group.head(num_rows, batch_size=num_rows).nbytes / num_rows
-    ratio: float = in_memory_size / parquet_size
-    _logger.debug("Estimated Parquet encoding ratio is %s for piece %s.", ratio, piece)
-    return in_memory_size / parquet_size
+    # Use first batch in-memory size as ratio estimation.
+    try:
+        batch = next(batches)
+    except StopIteration:
+        ratio = PARQUET_ENCODING_RATIO_ESTIMATE_LOWER_BOUND
+    else:
+        if batch.num_rows > 0:
+            in_memory_size = batch.nbytes / batch.num_rows
+            metadata = piece.metadata
+            total_size = 0
+            for idx in range(metadata.num_row_groups):
+                total_size += metadata.row_group(idx).total_byte_size
+            file_size = total_size / metadata.num_rows
+            ratio = in_memory_size / file_size
+        else:
+            ratio = PARQUET_ENCODING_RATIO_ESTIMATE_LOWER_BOUND
+    _logger.debug(f"Estimated Parquet encoding ratio is {ratio} for piece {piece} " f"with batch size {batch_size}.")
+    return ratio
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         super().__init__()
 
         self._write_paths: List[str] = []
 
     def _read_file(self, f: pyarrow.NativeFile, path: str, **reader_args: Any) -> pd.DataFrame:
         raise NotImplementedError()
 
-    def do_write(  # pylint: disable=arguments-differ
+    def do_write(  # type: ignore[override] # pylint: disable=arguments-differ
         self,
         blocks: List[ObjectRef[pd.DataFrame]],
         metadata: List[BlockMetadata],
         path: str,
         dataset_uuid: str,
         filesystem: Optional[pyarrow.fs.FileSystem] = None,
         try_create_dir: bool = True,
@@ -137,15 +137,15 @@
                 file_format=file_suffix,
             )
             write_task = write_block_fn(write_path, block)
             write_tasks.append(write_task)
 
         return write_tasks
 
-    def write(  # type: ignore[override]
+    def write(
         self,
         blocks: Iterable[Union[Block[pd.DataFrame], ObjectRef[pd.DataFrame]]],
         ctx: TaskContext,
         path: str,
         dataset_uuid: str,
         filesystem: Optional[pyarrow.fs.FileSystem] = None,
         block_path_provider: BlockWritePathProvider = DefaultBlockWritePathProvider(),
@@ -194,15 +194,15 @@
             builder.add_block(ray_get(block) if isinstance(block, ray.ObjectRef) else block)  # type: ignore[arg-type]
         block = builder.build()
 
         write_path = block_path_provider(
             path,
             filesystem=filesystem,
             dataset_uuid=dataset_uuid,
-            block=block,
+            block=block,  # type: ignore[arg-type]
             block_index=ctx.task_idx,
             file_format=file_suffix,
         )
 
         return write_block(write_path, block)
 
     def _get_file_suffix(self, file_format: str, compression: Optional[str]) -> str:
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/datasources/pandas_text_datasource.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/datasources/pandas_text_datasource.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/_core.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/_data_types.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/_data_types.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/_utils.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_parquet.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_parquet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Modin on Ray S3 read parquet module (PRIVATE)."""
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import modin.pandas as pd
 import pyarrow as pa
 from ray.data import read_datasource
 from ray.data.datasource import FastFileMetadataProvider
 
 from awswrangler.distributed.ray.datasources import ArrowParquetBaseDatasource, ArrowParquetDatasource
@@ -33,15 +33,15 @@
     use_threads: Union[bool, int],
     parallelism: int,
     version_ids: Optional[Dict[str, str]],
     s3_client: Optional["S3Client"],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     arrow_kwargs: Dict[str, Any],
     bulk_read: bool,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+) -> pd.DataFrame:
     dataset_kwargs = {}
     if coerce_int96_timestamp_unit:
         dataset_kwargs["coerce_int96_timestamp_unit"] = coerce_int96_timestamp_unit
 
     dataset = read_datasource(
         **_resolve_datasource_parameters(bulk_read),
         parallelism=parallelism,
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_read_text.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_read_text.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,22 +117,22 @@
     raise exceptions.UnsupportedType("Unsupported read format")
 
 
 def _read_text_distributed(  # pylint: disable=unused-argument
     read_format: str,
     paths: List[str],
     path_root: Optional[str],
+    use_threads: Union[bool, int],
+    s3_client: Optional["S3Client"],
     s3_additional_kwargs: Optional[Dict[str, str]],
     dataset: bool,
     ignore_index: bool,
     parallelism: int,
     version_ids: Optional[Dict[str, str]],
     pandas_kwargs: Dict[str, Any],
-    use_threads: Union[bool, int],
-    s3_client: Optional["S3Client"],
 ) -> pd.DataFrame:
     try:
         configuration: Dict[str, Any] = _parse_configuration(  # type: ignore[assignment]
             read_format,
             version_ids,
             s3_additional_kwargs,
             pandas_kwargs,
```

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_dataset.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_dataset.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_parquet.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/modin/s3/_write_text.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/modin/s3/_write_text.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/s3/_list.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/distributed/ray/s3/_read_parquet.py` & `awswrangler-3.2.0/awswrangler/distributed/ray/s3/_read_parquet.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/dynamodb/_delete.py` & `awswrangler-3.2.0/awswrangler/dynamodb/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/dynamodb/_read.py` & `awswrangler-3.2.0/awswrangler/dynamodb/_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 
 import boto3
 import pyarrow as pa
 from boto3.dynamodb.conditions import ConditionBase
 from boto3.dynamodb.types import Binary
 from botocore.exceptions import ClientError
+from typing_extensions import Literal
 
 import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._distributed import engine
 from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.dynamodb._utils import _serialize_kwargs, execute_statement, get_table
@@ -395,29 +396,30 @@
             items_iterator=cast(Iterator[_ItemsListType], items), as_dataframe=as_dataframe, arrow_kwargs=arrow_kwargs
         )
     else:
         return _convert_items(items=cast(_ItemsListType, items), as_dataframe=as_dataframe, arrow_kwargs=arrow_kwargs)
 
 
 @_utils.validate_distributed_kwargs(
-    unsupported_kwargs=["boto3_session"],
+    unsupported_kwargs=["boto3_session", "dtype_backend"],
 )
 def read_items(  # pylint: disable=too-many-branches
     table_name: str,
     index_name: Optional[str] = None,
     partition_values: Optional[Sequence[Any]] = None,
     sort_values: Optional[Sequence[Any]] = None,
     filter_expression: Optional[Union[ConditionBase, str]] = None,
     key_condition_expression: Optional[Union[ConditionBase, str]] = None,
     expression_attribute_names: Optional[Dict[str, str]] = None,
     expression_attribute_values: Optional[Dict[str, Any]] = None,
     consistent: bool = False,
     columns: Optional[Sequence[str]] = None,
     allow_full_scan: bool = False,
     max_items_evaluated: Optional[int] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     as_dataframe: bool = True,
     chunked: bool = False,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame], _ItemsListType, Iterator[_ItemsListType]]:
     """Read items from given DynamoDB table.
@@ -460,14 +462,20 @@
         Defaults to False.
     columns : Sequence[str], optional
         Attributes to retain in the returned items. Defaults to None (all attributes).
     allow_full_scan : bool
         If True, allow full table scan without any filtering. Defaults to False.
     max_items_evaluated : int, optional
         Limit the number of items evaluated in case of query or scan operations. Defaults to None (all matching items).
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     as_dataframe : bool
         If True, return items as pd.DataFrame, otherwise as list/dict. Defaults to True.
     chunked : bool
         If `True` an iterable of DataFrames/lists is returned. False by default.
     use_threads : Union[bool, int]
         Used for Parallel Scan requests. True (default) to enable concurrency, False to disable multiple threads.
         If enabled os.cpu_count() is used as the max number of threads.
@@ -572,15 +580,17 @@
     ...     table_name='my-table',
     ...     filter_expression='#operator = :v',
     ...     expression_attribute_names={'#operator': 'operator'},
     ...     expression_attribute_values={':v': 'this-value'}
     ... )
 
     """
-    arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
+    arrow_kwargs = _data_types.pyarrow2pandas_defaults(
+        use_threads=use_threads, kwargs=pyarrow_additional_kwargs, dtype_backend=dtype_backend
+    )
 
     # Extract key schema
     table_key_schema = get_table(table_name=table_name, boto3_session=boto3_session).key_schema
 
     # Detect sort key, if any
     if len(table_key_schema) == 1:
         partition_key, sort_key = table_key_schema[0]["AttributeName"], None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awswrangler-3.1.1/awswrangler/dynamodb/_read.pyi` & `awswrangler-3.2.0/awswrangler/dynamodb/_read.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: Literal[True] = ...,
     chunked: Literal[False] = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> pd.DataFrame: ...
 @overload
@@ -82,14 +83,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: Literal[True] = ...,
     chunked: Literal[True],
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
@@ -103,14 +105,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: Literal[False],
     chunked: Literal[False] = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> _ItemsListType: ...
 @overload
@@ -124,14 +127,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: Literal[False],
     chunked: Literal[True],
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[_ItemsListType]: ...
 @overload
@@ -145,14 +149,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: bool,
     chunked: Literal[False] = ...,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, _ItemsListType]: ...
 @overload
@@ -166,14 +171,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: bool,
     chunked: Literal[True],
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[Iterator[pd.DataFrame], Iterator[_ItemsListType]]: ...
 @overload
@@ -187,14 +193,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: Literal[True],
     chunked: bool,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
@@ -208,14 +215,15 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: Literal[False],
     chunked: bool,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[_ItemsListType, Iterator[_ItemsListType]]: ...
 @overload
@@ -229,13 +237,14 @@
     key_condition_expression: Optional[Union[ConditionBase, str]] = ...,
     expression_attribute_names: Optional[Dict[str, str]] = ...,
     expression_attribute_values: Optional[Dict[str, Any]] = ...,
     consistent: bool = ...,
     columns: Optional[Sequence[str]] = ...,
     allow_full_scan: bool = ...,
     max_items_evaluated: Optional[int] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     as_dataframe: bool,
     chunked: bool,
     use_threads: Union[bool, int] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame], _ItemsListType, Iterator[_ItemsListType]]: ...
```

### Comparing `awswrangler-3.1.1/awswrangler/dynamodb/_utils.py` & `awswrangler-3.2.0/awswrangler/dynamodb/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,32 +156,30 @@
     """
     names: Dict[str, Any] = {}
     values: Dict[str, Any] = {}
     serializer = TypeSerializer()
 
     if "FilterExpression" in kwargs and not isinstance(kwargs["FilterExpression"], str):
         builder = ConditionExpressionBuilder()
-        exp_string, names, values = builder.build_expression(kwargs["FilterExpression"], False)  # type: ignore[assignment]
+        exp_string, names, values = builder.build_expression(kwargs["FilterExpression"], False)
         kwargs["FilterExpression"] = exp_string
 
     if "ExpressionAttributeNames" in kwargs:
         kwargs["ExpressionAttributeNames"].update(names)
-    else:
-        if names:
-            kwargs["ExpressionAttributeNames"] = names
+    elif names:
+        kwargs["ExpressionAttributeNames"] = names
 
     values = {k: serializer.serialize(v) for k, v in values.items()}
     if "ExpressionAttributeValues" in kwargs:
         kwargs["ExpressionAttributeValues"] = {
             k: serializer.serialize(v) for k, v in kwargs["ExpressionAttributeValues"].items()
         }
         kwargs["ExpressionAttributeValues"].update(values)
-    else:
-        if values:
-            kwargs["ExpressionAttributeValues"] = values
+    elif values:
+        kwargs["ExpressionAttributeValues"] = values
 
     return kwargs
 
 
 def _validate_items(items: Union[List[Dict[str, Any]], List[Mapping[str, Any]]], dynamodb_table: "Table") -> None:
     """Validate if all items have the required keys for the Amazon DynamoDB table.
```

### Comparing `awswrangler-3.1.1/awswrangler/dynamodb/_write.py` & `awswrangler-3.2.0/awswrangler/dynamodb/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/emr.py` & `awswrangler-3.2.0/awswrangler/emr.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/exceptions.py` & `awswrangler-3.2.0/awswrangler/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,22 @@
     """QueryFailed exception."""
 
 
 class QueryCancelled(Exception):
     """QueryCancelled exception."""
 
 
+class SessionFailed(Exception):
+    """SessionFailed exception."""
+
+
+class CalculationFailed(Exception):
+    """CalculationFailed exception."""
+
+
 class EmptyDataFrame(Exception):
     """EmptyDataFrame exception."""
 
 
 class InvalidConnection(Exception):
     """InvalidConnection exception."""
 
@@ -139,7 +147,11 @@
 
 class TimestreamLoadError(Exception):
     """TimestreamLoadError exception."""
 
 
 class NeptuneLoadError(Exception):
     """NeptuneLoadError."""
+
+
+class EMRServerlessJobError(Exception):
+    """EMRServerlessJobError."""
```

### Comparing `awswrangler-3.1.1/awswrangler/lakeformation/__init__.py` & `awswrangler-3.2.0/awswrangler/lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/lakeformation/_read.py` & `awswrangler-3.2.0/awswrangler/lakeformation/_read.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import itertools
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import boto3
 import pandas as pd
 from pyarrow import NativeFile, RecordBatchStreamReader, Table
+from typing_extensions import Literal
 
 from awswrangler import _data_types, _utils, catalog
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
 from awswrangler._executor import _BaseExecutor, _get_executor
-from awswrangler._sql_formatter import _EngineType, _process_sql_params
+from awswrangler._sql_formatter import _process_sql_params
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 from awswrangler.lakeformation._utils import commit_transaction, start_transaction, wait_query
 
 if TYPE_CHECKING:
     from mypy_boto3_lakeformation.client import LakeFormationClient
 
 _logger: logging.Logger = logging.getLogger(__name__)
@@ -73,22 +74,23 @@
         token_work_units,
     )
     return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
 
 
 @apply_configs
 @_utils.validate_distributed_kwargs(
-    unsupported_kwargs=["boto3_session"],
+    unsupported_kwargs=["boto3_session", "dtype_backend"],
 )
 def read_sql_query(
     sql: str,
     database: str,
     transaction_id: Optional[str] = None,
     query_as_of_time: Optional[str] = None,
     catalog_id: Optional[str] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     use_threads: bool = True,
     boto3_session: Optional[boto3.Session] = None,
     params: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> pd.DataFrame:
     """Execute PartiQL query on AWS Glue Table (Transaction ID or time travel timestamp). Return Pandas DataFrame.
 
@@ -118,14 +120,20 @@
         Cannot be specified alongside query_as_of_time.
     query_as_of_time : str, optional
         The time as of when to read the table contents. Must be a valid Unix epoch timestamp.
         Cannot be specified alongside transaction_id.
     catalog_id : str, optional
         The ID of the Data Catalog from which to retrieve Databases.
         If none is provided, the AWS account ID is used by default.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     use_threads : bool
         True to enable concurrent requests, False to disable multiple threads.
         When enabled, os.cpu_count() is used as the max number of threads.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if boto3_session receives None.
     params : Dict[str, any], optional
         Dict of parameters used to format the partiQL query. Only named parameters are supported.
@@ -165,51 +173,54 @@
     ...     params={"name": "filtered_name", "city": "filtered_city"}
     ... )
 
     """
     client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
     commit_trans: bool = False
 
-    sql = _process_sql_params(sql, params, engine=_EngineType.PARTIQL)
+    sql = _process_sql_params(sql, params, engine_type="partiql")
 
     if not any([transaction_id, query_as_of_time]):
         _logger.debug("Neither `transaction_id` nor `query_as_of_time` were specified, starting transaction")
         transaction_id = start_transaction(read_only=True, boto3_session=boto3_session)
         commit_trans = True
     args: Dict[str, Optional[str]] = _catalog_id(
         catalog_id=catalog_id,
         **_transaction_id(transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database),
     )
     result = client_lakeformation.start_query_planning(
         QueryString=sql,
         QueryPlanningContext=args,  # type: ignore[arg-type]
     )
     query_id: str = result["QueryId"]
-    arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
+    arrow_kwargs = _data_types.pyarrow2pandas_defaults(
+        use_threads=use_threads, kwargs=pyarrow_additional_kwargs, dtype_backend=dtype_backend
+    )
     df = _resolve_sql_query(
         query_id=query_id,
         use_threads=use_threads,
         boto3_session=boto3_session,
         arrow_kwargs=arrow_kwargs,
     )
     if commit_trans:
         commit_transaction(transaction_id=transaction_id, boto3_session=boto3_session)  # type: ignore[arg-type]
     return df
 
 
 @apply_configs
 @_utils.validate_distributed_kwargs(
-    unsupported_kwargs=["boto3_session"],
+    unsupported_kwargs=["boto3_session", "dtype_backend"],
 )
 def read_sql_table(
     table: str,
     database: str,
     transaction_id: Optional[str] = None,
     query_as_of_time: Optional[str] = None,
     catalog_id: Optional[str] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     use_threads: bool = True,
     boto3_session: Optional[boto3.Session] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> pd.DataFrame:
     """Extract all rows from AWS Glue Table (Transaction ID or time travel timestamp). Return Pandas DataFrame.
 
     Note
@@ -232,14 +243,20 @@
         Cannot be specified alongside query_as_of_time.
     query_as_of_time : str, optional
         The time as of when to read the table contents. Must be a valid Unix epoch timestamp.
         Cannot be specified alongside transaction_id.
     catalog_id : str, optional
         The ID of the Data Catalog from which to retrieve Databases.
         If none is provided, the AWS account ID is used by default.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     use_threads : bool
         True to enable concurrent requests, False to disable multiple threads.
         When enabled, os.cpu_count() is used as the max number of threads.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if boto3_session receives None.
     pyarrow_additional_kwargs : Dict[str, Any], optional
         Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
@@ -279,11 +296,12 @@
     table = catalog.sanitize_table_name(table=table)
     return read_sql_query(
         sql=f"SELECT * FROM {table}",
         database=database,
         transaction_id=transaction_id,
         query_as_of_time=query_as_of_time,
         catalog_id=catalog_id,
+        dtype_backend=dtype_backend,
         use_threads=use_threads,
         boto3_session=boto3_session,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awswrangler-3.1.1/awswrangler/lakeformation/_utils.py` & `awswrangler-3.2.0/awswrangler/lakeformation/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/mysql.py` & `awswrangler-3.2.0/awswrangler/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,14 +178,15 @@
     con: "pymysql.connections.Connection[Any]",
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -193,14 +194,15 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -208,28 +210,30 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(pymysql, "pymysql")
 def read_sql_query(
     sql: str,
     con: "pymysql.connections.Connection[Any]",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding to the result set of the query string.
 
     Parameters
     ----------
     sql : str
         SQL query.
@@ -247,14 +251,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -276,28 +286,30 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 @overload
 def read_sql_table(
     table: str,
     con: "pymysql.connections.Connection[Any]",
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -306,14 +318,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -322,14 +335,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(pymysql, "pymysql")
 def read_sql_table(
     table: str,
@@ -337,14 +351,15 @@
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding the table.
 
     Parameters
     ----------
     table : str
         Table name.
@@ -365,14 +380,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -395,14 +416,15 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 _ToSqlModeLiteral = Literal[
     "append", "overwrite", "upsert_replace_into", "upsert_duplicate_key", "upsert_distinct", "ignore"
 ]
```

### Comparing `awswrangler-3.1.1/awswrangler/neptune/__init__.py` & `awswrangler-3.2.0/awswrangler/neptune/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities Module for Amazon Neptune."""
+from awswrangler.neptune._client import BulkLoadParserConfiguration
 from awswrangler.neptune._gremlin_parser import GremlinParser
 from awswrangler.neptune._neptune import (
     bulk_load,
     bulk_load_from_files,
     connect,
     execute_gremlin,
     execute_opencypher,
@@ -19,8 +20,9 @@
     "to_property_graph",
     "to_rdf_graph",
     "connect",
     "bulk_load",
     "bulk_load_from_files",
     "GremlinParser",
     "flatten_nested_df",
+    "BulkLoadParserConfiguration",
 ]
```

### Comparing `awswrangler-3.1.1/awswrangler/neptune/_client.py` & `awswrangler-3.2.0/awswrangler/neptune/_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # mypy: disable-error-code=name-defined
 """Amazon NeptuneClient Module."""
 
+import json
 import logging
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, List, Optional, TypedDict, Union, cast
 
 import boto3
 from botocore.auth import SigV4Auth
 from botocore.awsrequest import AWSPreparedRequest, AWSRequest
+from typing_extensions import Literal, NotRequired
 
 import awswrangler.neptune._gremlin_init as gremlin
 from awswrangler import _utils, exceptions
 from awswrangler.neptune._gremlin_parser import GremlinParser
 
 gremlin_python = _utils.import_optional_dependency("gremlin_python")
 opencypher = _utils.import_optional_dependency("requests")
@@ -23,14 +25,36 @@
 
 DEFAULT_PORT = 8182
 NEPTUNE_SERVICE_NAME = "neptune-db"
 HTTP_PROTOCOL = "https"
 WS_PROTOCOL = "wss"
 
 
+class BulkLoadParserConfiguration(TypedDict):
+    """Typed dictionary representing the additional parser configuration for the Neptune Bulk Loader."""
+
+    namedGraphUri: NotRequired[str]
+    """
+    The default graph for all RDF formats when no graph is specified
+    (for non-quads formats and NQUAD entries with no graph).
+    """
+    baseUri: NotRequired[str]
+    """The base URI for RDF/XML and Turtle formats."""
+    allowEmptyStrings: NotRequired[bool]
+    """
+    Gremlin users need to be able to pass empty string values("") as node
+    and edge properties when loading CSV data.
+    If ``allowEmptyStrings`` is set to ``false`` (the default),
+    such empty strings are treated as nulls and are not loaded.
+
+    If allowEmptyStrings is set to true, the loader treats empty strings
+    as valid property values and loads them accordingly.
+    """
+
+
 class NeptuneClient:
     """Class representing a Neptune cluster connection."""
 
     def __init__(
         self,
         host: str,
         port: int = DEFAULT_PORT,
@@ -276,51 +300,95 @@
             The result of the call to the status API for the Neptune cluster
         """
         url = f"{HTTP_PROTOCOL}://{self.host}:{self.port}/status"
         req = self._prepare_request("GET", url, data="")
         res = self._http_session.send(req)
         return res.json()
 
-    def load(self, s3_path: str, role_arn: str, parallelism: str = "HIGH", format: str = "csv") -> str:
+    def load(
+        self,
+        s3_path: str,
+        role_arn: str,
+        parallelism: Literal["LOW", "MEDIUM", "HIGH", "OVERSUBSCRIBE"] = "HIGH",
+        mode: Literal["RESUME", "NEW", "AUTO"] = "AUTO",
+        format: str = "csv",
+        parser_configuration: Optional[BulkLoadParserConfiguration] = None,
+        update_single_cardinality_properties: Literal["TRUE", "FALSE"] = "FALSE",
+        queue_request: Literal["TRUE", "FALSE"] = "FALSE",
+        dependencies: Optional[List[str]] = None,
+    ) -> str:
         """
         Start the Neptune Loader command for loading CSV data from external files on S3 into a Neptune DB cluster.
 
         Parameters
         ----------
         s3_path: str
             Amazon S3 URI that identifies a single file, multiple files, a folder, or multiple folders.
             Neptune loads every data file in any folder that is specified.
         role_arn: str
             The Amazon Resource Name (ARN) for an IAM role to be assumed by the Neptune DB instance for access to the S3 bucket.
             For information about creating a role that has access to Amazon S3 and then associating it with a Neptune cluster,
             see `Prerequisites: IAM Role and Amazon S3 Access <https://docs.aws.amazon.com/neptune/latest/userguide/bulk-load-tutorial-IAM.html>`_.
         parallelism: str
             Specifies the number of threads used by the bulk load process.
+        mode: str
+            The load job mode.
+
+            In ```RESUME``` mode, the loader looks for a previous load from this source, and if it finds one, resumes that load job.
+            If no previous load job is found, the loader stops.
+
+            In ```NEW``` mode, the creates a new load request regardless of any previous loads.
+            You can use this mode to reload all the data from a source after dropping previously loaded data from your Neptune cluster, or to load new data available at the same source.
+
+            In ```AUTO``` mode, the loader looks for a previous load job from the same source, and if it finds one, resumes that job, just as in ```RESUME``` mode.
         format: str
             The format of the data. For more information about data formats for the Neptune Loader command,
             see `Using the Amazon Neptune Bulk Loader to Ingest Data <https://docs.aws.amazon.com/neptune/latest/userguide/load-api-reference-load.html#:~:text=The%20format%20of%20the%20data.%20For%20more%20information%20about%20data%20formats%20for%20the%20Neptune%20Loader%20command%2C%20see%20Using%20the%20Amazon%20Neptune%20Bulk%20Loader%20to%20Ingest%20Data.>`_.
+        parser_configuration: dict[str, Any], optional
+            An optional object with additional parser configuration values.
+            Each of the child parameters is also optional: ``namedGraphUri``, ``baseUri`` and ``allowEmptyStrings``.
+        update_single_cardinality_properties: str
+            An optional parameter that controls how the bulk loader
+            treats a new value for single-cardinality vertex or edge properties.
+        queue_request: str
+            An optional flag parameter that indicates whether the load request can be queued up or not.
+
+            If omitted or set to ``"FALSE"``, the load request will fail if another load job is already running.
+        dependencies: list[str], optional
+            An optional parameter that can make a queued load request contingent on the successful completion of one or more previous jobs in the queue.
 
         Returns
         -------
         str
             ID of the load job
         """
-        data = {
+        data: Dict[str, Any] = {
             "source": s3_path,
             "format": format,
             "iamRoleArn": role_arn,
-            "mode": "AUTO",
+            "mode": mode,
             "region": self.region,
             "failOnError": "TRUE",
             "parallelism": parallelism,
+            "updateSingleCardinalityProperties": update_single_cardinality_properties,
+            "queueRequest": queue_request,
         }
+        if parser_configuration:
+            data["parserConfiguration"] = parser_configuration
+        if dependencies:
+            data["dependencies"] = dependencies
 
         url = f"https://{self.host}:{self.port}/loader"
 
-        req = self._prepare_request("POST", url, data=data)
+        req = self._prepare_request(
+            method="POST",
+            url=url,
+            data=json.dumps(data),
+            headers={"Content-Type": "application/json; charset=utf-8"},
+        )
         res = self._http_session.send(req)
 
         _logger.debug(res)
         if res.ok:
             return cast(str, res.json()["payload"]["loadId"])
 
         raise exceptions.NeptuneLoadError(f"Status Code: {res.status_code} Reason: {res.reason} Message: {res.text}")
```

### Comparing `awswrangler-3.1.1/awswrangler/neptune/_gremlin_init.py` & `awswrangler-3.2.0/awswrangler/neptune/_gremlin_init.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/neptune/_gremlin_parser.py` & `awswrangler-3.2.0/awswrangler/neptune/_gremlin_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         # If this is a scalar then create a Map with it
         elif not hasattr(data, "__len__") or isinstance(data, str):
             data = {0: data}
 
         for k, v in data.items():
             # If the key is a Vertex or an Edge do special processing
             if isinstance(k, (gremlin.Vertex, gremlin.Edge)):
-                k = k.id
+                k = k.id  # ruff: noqa: PLW2901
 
             # If the value is a list do special processing to make it a scalar if the list is of length 1
             if isinstance(v, list) and len(v) == 1:
                 d[k] = v[0]
             else:
                 d[k] = v
```

### Comparing `awswrangler-3.1.1/awswrangler/neptune/_neptune.py` & `awswrangler-3.2.0/awswrangler/neptune/_neptune.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # mypy: disable-error-code=name-defined
 """Amazon Neptune Module."""
 
 import logging
 import re
 import time
-from typing import Any, Callable, Dict, Literal, Optional, TypeVar, Union
+from typing import Any, Callable, Dict, List, Literal, Optional, TypeVar, Union
 
 import boto3
 
 import awswrangler.neptune._gremlin_init as gremlin
 import awswrangler.pandas as pd
 from awswrangler import _utils, exceptions, s3
 from awswrangler._config import apply_configs
-from awswrangler.neptune._client import NeptuneClient
+from awswrangler.neptune._client import BulkLoadParserConfiguration, NeptuneClient
 
 gremlin_python = _utils.import_optional_dependency("gremlin_python")
 opencypher = _utils.import_optional_dependency("requests")
 sparql = _utils.import_optional_dependency("SPARQLWrapper")
 
 _logger: logging.Logger = logging.getLogger(__name__)
 FuncT = TypeVar("FuncT", bound=Callable[..., Any])
@@ -281,14 +281,18 @@
 def bulk_load(
     client: NeptuneClient,
     df: pd.DataFrame,
     path: str,
     iam_role: str,
     neptune_load_wait_polling_delay: float = 0.25,
     load_parallelism: Literal["LOW", "MEDIUM", "HIGH", "OVERSUBSCRIBE"] = "HIGH",
+    parser_configuration: Optional[BulkLoadParserConfiguration] = None,
+    update_single_cardinality_properties: Literal["TRUE", "FALSE"] = "FALSE",
+    queue_request: Literal["TRUE", "FALSE"] = "FALSE",
+    dependencies: Optional[List[str]] = None,
     keep_files: bool = False,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, str]] = None,
 ) -> None:
     """
     Write records into Amazon Neptune using the Neptune Bulk Loader.
@@ -308,14 +312,26 @@
         The Amazon Resource Name (ARN) for an IAM role to be assumed by the Neptune DB instance for access to the S3 bucket.
         For information about creating a role that has access to Amazon S3 and then associating it with a Neptune cluster,
         see `Prerequisites: IAM Role and Amazon S3 Access <https://docs.aws.amazon.com/neptune/latest/userguide/bulk-load-tutorial-IAM.html>`_.
     neptune_load_wait_polling_delay: float
         Interval in seconds for how often the function will check if the Neptune bulk load has completed.
     load_parallelism: str
         Specifies the number of threads used by Neptune's bulk load process.
+    parser_configuration: dict[str, Any], optional
+        An optional object with additional parser configuration values.
+        Each of the child parameters is also optional: ``namedGraphUri``, ``baseUri`` and ``allowEmptyStrings``.
+    update_single_cardinality_properties: str
+        An optional parameter that controls how the bulk loader
+        treats a new value for single-cardinality vertex or edge properties.
+    queue_request: str
+        An optional flag parameter that indicates whether the load request can be queued up or not.
+
+        If omitted or set to ``"FALSE"``, the load request will fail if another load job is already running.
+    dependencies: list[str], optional
+        An optional parameter that can make a queued load request contingent on the successful completion of one or more previous jobs in the queue.
     keep_files: bool
         Whether to keep stage files or delete them. False by default.
     use_threads: bool | int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session: boto3.Session(), optional
@@ -348,16 +364,21 @@
     try:
         s3.to_csv(df, path, use_threads=use_threads, dataset=True, index=False)
 
         bulk_load_from_files(
             client=client,
             path=path,
             iam_role=iam_role,
+            format="csv",
             neptune_load_wait_polling_delay=neptune_load_wait_polling_delay,
             load_parallelism=load_parallelism,
+            parser_configuration=parser_configuration,
+            update_single_cardinality_properties=update_single_cardinality_properties,
+            queue_request=queue_request,
+            dependencies=dependencies,
         )
     finally:
         if keep_files is False:
             _logger.debug("Deleting objects in S3 path: %s", path)
             s3.delete_objects(
                 path=path,
                 use_threads=use_threads,
@@ -368,69 +389,94 @@
 
 @apply_configs
 @_utils.check_optional_dependency(sparql, "SPARQLWrapper")
 def bulk_load_from_files(
     client: NeptuneClient,
     path: str,
     iam_role: str,
+    format: Literal["csv", "opencypher", "ntriples", "nquads", "rdfxml", "turtle"] = "csv",
     neptune_load_wait_polling_delay: float = 0.25,
     load_parallelism: Literal["LOW", "MEDIUM", "HIGH", "OVERSUBSCRIBE"] = "HIGH",
+    parser_configuration: Optional[BulkLoadParserConfiguration] = None,
+    update_single_cardinality_properties: Literal["TRUE", "FALSE"] = "FALSE",
+    queue_request: Literal["TRUE", "FALSE"] = "FALSE",
+    dependencies: Optional[List[str]] = None,
 ) -> None:
     """
-    Load CSV files from S3 into Amazon Neptune using the Neptune Bulk Loader.
+    Load files from S3 into Amazon Neptune using the Neptune Bulk Loader.
 
     For more information about the Bulk Loader see
     `here <https://docs.aws.amazon.com/neptune/latest/userguide/bulk-load.html>`_.
 
     Parameters
     ----------
     client: NeptuneClient
         Instance of the neptune client to use
     path: str
         S3 Path that the Neptune Bulk Loader will load data from.
     iam_role: str
         The Amazon Resource Name (ARN) for an IAM role to be assumed by the Neptune DB instance for access to the S3 bucket.
         For information about creating a role that has access to Amazon S3 and then associating it with a Neptune cluster,
         see `Prerequisites: IAM Role and Amazon S3 Access <https://docs.aws.amazon.com/neptune/latest/userguide/bulk-load-tutorial-IAM.html>`_.
+    format: str
+        The format of the data.
     neptune_load_wait_polling_delay: float
         Interval in seconds for how often the function will check if the Neptune bulk load has completed.
     load_parallelism: str
         Specifies the number of threads used by Neptune's bulk load process.
+    parser_configuration: dict[str, Any], optional
+        An optional object with additional parser configuration values.
+        Each of the child parameters is also optional: ``namedGraphUri``, ``baseUri`` and ``allowEmptyStrings``.
+    update_single_cardinality_properties: str
+        An optional parameter that controls how the bulk loader
+        treats a new value for single-cardinality vertex or edge properties.
+    queue_request: str
+        An optional flag parameter that indicates whether the load request can be queued up or not.
+
+        If omitted or set to ``"FALSE"``, the load request will fail if another load job is already running.
+    dependencies: list[str], optional
+        An optional parameter that can make a queued load request contingent on the successful completion of one or more previous jobs in the queue.
+
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> client = wr.neptune.connect("MY_NEPTUNE_ENDPOINT", 8182)
     >>> wr.neptune.bulk_load_from_files(
     ...     client=client,
     ...     path="s3://my-bucket/stage-files/",
-    ...     iam_role="arn:aws:iam::XXX:role/XXX"
+    ...     iam_role="arn:aws:iam::XXX:role/XXX",
+    ...     format="csv",
     ... )
     """
     _logger.debug("Starting Neptune Bulk Load from %s", path)
     load_id = client.load(
         path,
         iam_role,
-        format="csv",
+        format=format,
         parallelism=load_parallelism,
+        parser_configuration=parser_configuration,
+        update_single_cardinality_properties=update_single_cardinality_properties,
+        queue_request=queue_request,
+        dependencies=dependencies,
     )
 
     while True:
         status_response = client.load_status(load_id)
 
         status: str = status_response["payload"]["overallStatus"]["status"]
         if status == "LOAD_COMPLETED":
             break
 
         if status not in BULK_LOAD_IN_PROGRESS_STATES:
             raise exceptions.NeptuneLoadError(f"Load {load_id} failed with {status}: {status_response}")
 
         time.sleep(neptune_load_wait_polling_delay)
 
-    _logger.debug("Neptune load %s has succeeded in loading data from %s", load_id, path)
+    _logger.debug("Neptune load %s has succeeded in loading %s data from %s", load_id, format, path)
 
 
 def connect(host: str, port: int, iam_enabled: bool = False, **kwargs: Any) -> NeptuneClient:
     """Create a connection to a Neptune cluster.
 
     Parameters
     ----------
@@ -461,24 +507,23 @@
     row: Any,
     ignore_cardinality: bool = False,
 ) -> "gremlin.GraphTraversalSource":
     for column, value in row.items():
         if column not in ["~id", "~label", "~to", "~from"]:
             if ignore_cardinality and pd.notna(value):
                 g = g.property(_get_column_name(column), value)
-            else:
+            elif use_header_cardinality:
                 # If the column header is specifying the cardinality then use it
-                if use_header_cardinality:
-                    if column.lower().find("(single)") > 0 and pd.notna(value):
-                        g = g.property(gremlin.Cardinality.single, _get_column_name(column), value)
-                    else:
-                        g = _expand_properties(g, _get_column_name(column), value)
+                if column.lower().find("(single)") > 0 and pd.notna(value):
+                    g = g.property(gremlin.Cardinality.single, _get_column_name(column), value)
                 else:
-                    # If not using header cardinality then use the default of set
-                    g = _expand_properties(g, column, value)
+                    g = _expand_properties(g, _get_column_name(column), value)
+            else:
+                # If not using header cardinality then use the default of set
+                g = _expand_properties(g, column, value)
     return g
 
 
 def _expand_properties(g: "gremlin.GraphTraversalSource", column: str, value: Any) -> "gremlin.GraphTraversalSource":
     # If this is a list then expand it out into multiple property calls
     if isinstance(value, list) and len(value) > 0:
         for item in value:
```

### Comparing `awswrangler-3.1.1/awswrangler/neptune/_utils.py` & `awswrangler-3.2.0/awswrangler/neptune/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """DataFrame type enum."""
 
     VERTEX = 1
     EDGE = 2
     UPDATE = 3
 
 
-def write_gremlin_df(client: NeptuneClient, df: pd.DataFrame, mode: WriteDFType, batch_size: int) -> bool:
+def write_gremlin_df(client: "NeptuneClient", df: pd.DataFrame, mode: WriteDFType, batch_size: int) -> bool:
     """Write the provided DataFrame using Gremlin.
 
     Parameters
     ----------
     client : NeptuneClient
         The Neptune client to write the DataFrame
     df : pd.DataFrame
@@ -63,15 +63,15 @@
                 raise exceptions.QueryFailed(
                     """Failed to insert part or all of the data in the DataFrame, please check the log output."""
                 )
 
     return _run_gremlin_insert(client, g)
 
 
-def _run_gremlin_insert(client: NeptuneClient, g: GraphTraversalSource) -> bool:
+def _run_gremlin_insert(client: "NeptuneClient", g: GraphTraversalSource) -> bool:
     translator = Translator("g")
     s = translator.translate(g.bytecode)
     s = s.replace("Cardinality.", "")  # hack to fix parser error for set cardinality
     _logger.debug(s)
     res = client.write_gremlin(s)
     return res
```

### Comparing `awswrangler-3.1.1/awswrangler/opensearch/_read.py` & `awswrangler-3.2.0/awswrangler/opensearch/_read.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/opensearch/_utils.py` & `awswrangler-3.2.0/awswrangler/opensearch/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/opensearch/_write.py` & `awswrangler-3.2.0/awswrangler/opensearch/_write.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,19 +195,18 @@
     ... )
 
     """
     body = {}
     if mappings:
         if _get_distribution(client) == "opensearch" or _get_version_major(client) >= 7:
             body["mappings"] = mappings  # doc type deprecated
+        elif doc_type:
+            body["mappings"] = {doc_type: mappings}
         else:
-            if doc_type:
-                body["mappings"] = {doc_type: mappings}
-            else:
-                body["mappings"] = {index: mappings}
+            body["mappings"] = {index: mappings}
     if settings:
         body["settings"] = settings
     if not body:
         body = None  # type: ignore[assignment]
 
     # ignore 400 cause by IndexAlreadyExistsException when creating an index
     response: Dict[str, Any] = client.indices.create(index, body=body, ignore=400)
@@ -257,14 +256,15 @@
 def index_json(
     client: "opensearchpy.OpenSearch",
     path: str,
     index: str,
     doc_type: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = boto3.Session(),
     json_path: Optional[str] = None,
+    use_threads: Union[bool, int] = False,
     **kwargs: Any,
 ) -> Any:
     """Index all documents from JSON file to OpenSearch index.
 
     The JSON file should be in a JSON-Lines text format (newline-delimited JSON) - https://jsonlines.org/
     OR if the is a single large JSON please provide `json_path`.
 
@@ -281,14 +281,18 @@
     json_path : str, optional
         JsonPath expression to specify explicit path to a single name element
         in a JSON hierarchical data structure.
         Read more about `JsonPath <https://jsonpath.com>`_
     boto3_session : boto3.Session(), optional
         Boto3 Session to be used to access s3 if s3 path is provided.
         The default boto3 Session will be used if boto3_session receive None.
+    use_threads : bool, int
+        True to enable concurrent requests, False to disable multiple threads.
+        If enabled os.cpu_count() will be used as the max number of threads.
+        If integer is provided, specified number is used.
     **kwargs :
         KEYWORD arguments forwarded to :func:`~awswrangler.opensearch.index_documents`
         which is used to execute the operation
 
     Returns
     -------
     Dict[str, Any]
@@ -321,24 +325,27 @@
         documents = [json.loads(line) for line in lines]
         if json_path:
             documents = _get_documents_w_json_path(documents, json_path)
     else:  # local path
         documents = list(_file_line_generator(path, is_json=True))
         if json_path:
             documents = _get_documents_w_json_path(documents, json_path)
-    return index_documents(client=client, documents=documents, index=index, doc_type=doc_type, **kwargs)
+    return index_documents(
+        client=client, documents=documents, index=index, doc_type=doc_type, use_threads=use_threads, **kwargs
+    )
 
 
 @_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def index_csv(
     client: "opensearchpy.OpenSearch",
     path: str,
     index: str,
     doc_type: Optional[str] = None,
     pandas_kwargs: Optional[Dict[str, Any]] = None,
+    use_threads: Union[bool, int] = False,
     **kwargs: Any,
 ) -> Any:
     """Index all documents from a CSV file to OpenSearch index.
 
     Parameters
     ----------
     client : OpenSearch
@@ -350,14 +357,18 @@
     doc_type : str, optional
         Name of the document type (for Elasticsearch versions 5.x and earlier).
     pandas_kwargs : Dict[str, Any], optional
         Dictionary of arguments forwarded to pandas.read_csv().
         e.g. pandas_kwargs={'sep': '|', 'na_values': ['null', 'none']}
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
         Note: these params values are enforced: `skip_blank_lines=True`
+    use_threads : bool, int
+        True to enable concurrent requests, False to disable multiple threads.
+        If enabled os.cpu_count() will be used as the max number of threads.
+        If integer is provided, specified number is used.
     **kwargs :
         KEYWORD arguments forwarded to :func:`~awswrangler.opensearch.index_documents`
         which is used to execute the operation
 
     Returns
     -------
     Dict[str, Any]
@@ -393,33 +404,42 @@
     enforced_pandas_params = {
         "skip_blank_lines": True,
         # 'na_filter': True  # will generate Nan value for empty cells. We remove Nan keys in _df_doc_generator
         # Note: if the user will pass na_filter=False null fields will be indexed as well ({"k1": null, "k2": null})
     }
     pandas_kwargs.update(enforced_pandas_params)
     df = pd.read_csv(path, **pandas_kwargs)
-    return index_df(client, df=df, index=index, doc_type=doc_type, **kwargs)
+    return index_df(client, df=df, index=index, doc_type=doc_type, use_threads=use_threads, **kwargs)
 
 
 @_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def index_df(
-    client: "opensearchpy.OpenSearch", df: pd.DataFrame, index: str, doc_type: Optional[str] = None, **kwargs: Any
+    client: "opensearchpy.OpenSearch",
+    df: pd.DataFrame,
+    index: str,
+    doc_type: Optional[str] = None,
+    use_threads: Union[bool, int] = False,
+    **kwargs: Any,
 ) -> Any:
     """Index all documents from a DataFrame to OpenSearch index.
 
     Parameters
     ----------
     client : OpenSearch
         instance of opensearchpy.OpenSearch to use.
     df : pd.DataFrame
         Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
     index : str
         Name of the index.
     doc_type : str, optional
         Name of the document type (for Elasticsearch versions 5.x and earlier).
+    use_threads : bool, int
+        True to enable concurrent requests, False to disable multiple threads.
+        If enabled os.cpu_count() will be used as the max number of threads.
+        If integer is provided, specified number is used.
     **kwargs :
         KEYWORD arguments forwarded to :func:`~awswrangler.opensearch.index_documents`
         which is used to execute the operation
 
     Returns
     -------
     Dict[str, Any]
@@ -435,38 +455,51 @@
     >>> client = wr.opensearch.connect(host='DOMAIN-ENDPOINT')
     >>> wr.opensearch.index_df(
     ...     client=client,
     ...     df=pd.DataFrame([{'_id': '1'}, {'_id': '2'}, {'_id': '3'}]),
     ...     index='sample-index1'
     ... )
     """
-    return index_documents(client=client, documents=_df_doc_generator(df), index=index, doc_type=doc_type, **kwargs)
+    return index_documents(
+        client=client,
+        documents=_df_doc_generator(df),
+        index=index,
+        doc_type=doc_type,
+        use_threads=use_threads,
+        **kwargs,
+    )
 
 
 @_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def index_documents(
     client: "opensearchpy.OpenSearch",
     documents: Iterable[Mapping[str, Any]],
     index: str,
     doc_type: Optional[str] = None,
     keys_to_write: Optional[List[str]] = None,
     id_keys: Optional[List[str]] = None,
     ignore_status: Optional[Union[List[Any], Tuple[Any]]] = None,
     bulk_size: int = 1000,
     chunk_size: Optional[int] = 500,
     max_chunk_bytes: Optional[int] = 100 * 1024 * 1024,
-    max_retries: Optional[int] = 5,
-    initial_backoff: Optional[int] = 2,
-    max_backoff: Optional[int] = 600,
+    max_retries: Optional[int] = None,
+    initial_backoff: Optional[int] = None,
+    max_backoff: Optional[int] = None,
+    use_threads: Union[bool, int] = False,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     """Index all documents to OpenSearch index.
 
     Note
     ----
+    `max_retries`, `initial_backoff`, and `max_backoff` are not supported with parallel bulk
+     (when `use_threads`is set to True).
+
+    Note
+    ----
     Some of the args are referenced from opensearch-py client library (bulk helpers)
     https://opensearch-py.readthedocs.io/en/latest/helpers.html#opensearchpy.helpers.bulk
     https://opensearch-py.readthedocs.io/en/latest/helpers.html#opensearchpy.helpers.streaming_bulk
 
     If you receive `Error 429 (Too Many Requests) /_bulk` please to to decrease `bulk_size` value.
     Please also consider modifying the cluster size and instance type -
     Read more here: https://aws.amazon.com/premiumsupport/knowledge-center/resolve-429-error-es/
@@ -498,14 +531,18 @@
         maximum number of times a document will be retried when
         ``429`` is received, set to 0 (default) for no retries on ``429`` (default: 2)
     initial_backoff : int, optional
         number of seconds we should wait before the first retry.
         Any subsequent retries will be powers of ``initial_backoff*2**retry_number`` (default: 2)
     max_backoff: int, optional
         maximum number of seconds a retry will wait (default: 600)
+    use_threads : bool, int
+        True to enable concurrent requests, False to disable multiple threads.
+        If enabled os.cpu_count() will be used as the max number of threads.
+        If integer is provided, specified number is used.
     **kwargs :
         KEYWORD arguments forwarded to bulk operation
         elasticsearch >= 7.10.2 / opensearch: \
 https://opensearch.org/docs/opensearch/rest-api/document-apis/bulk/#url-parameters
         elasticsearch < 7.10.2: \
 https://opendistro.github.io/for-elasticsearch-docs/docs/elasticsearch/rest-api-reference/#url-parameters
 
@@ -525,14 +562,19 @@
     ...     documents=[{'_id': '1', 'value': 'foo'}, {'_id': '2', 'value': 'bar'}],
     ...     index='sample-index1'
     ... )
     """
     if "refresh" in kwargs and _is_serverless(client):
         raise exceptions.NotSupported("Refresh policy not supported in OpenSearch Serverless.")
 
+    if use_threads and any([max_retries, initial_backoff, max_backoff]):
+        raise exceptions.InvalidArgumentCombination(
+            "`max_retries`, `initial_backoff`, and `max_backoff` are not supported when `use_threads` is set to True"
+        )
+
     if not isinstance(documents, list):
         documents = list(documents)
     total_documents = len(documents)
     _logger.debug("indexing %s documents into %s", total_documents, index)
 
     actions = _actions_generator(
         documents, index, doc_type, keys_to_write=keys_to_write, id_keys=id_keys, bulk_size=bulk_size
@@ -553,28 +595,38 @@
                 widgets=widgets, max_value=total_documents, prefix="Indexing: "
             ).start()
         for i, bulk_chunk_documents in enumerate(actions):
             if i == 1:  # second bulk iteration, in case the index didn't exist before
                 refresh_interval = _get_refresh_interval(client, index)
                 _disable_refresh_interval(client, index)
             _logger.debug("running bulk index of %s documents", len(bulk_chunk_documents))
-            _success, _errors = opensearchpy.helpers.bulk(
-                client=client,
-                actions=bulk_chunk_documents,
-                ignore_status=ignore_status,
-                chunk_size=chunk_size,
-                max_chunk_bytes=max_chunk_bytes,
-                max_retries=max_retries,
-                initial_backoff=initial_backoff,
-                max_backoff=max_backoff,
-                request_timeout=30,
+            bulk_kwargs = {
+                "ignore_status": ignore_status,
+                "chunk_size": chunk_size,
+                "max_chunk_bytes": max_chunk_bytes,
+                "request_timeout": 30,
                 **kwargs,
-            )
-            success += _success
-            errors += _errors
+            }
+            _logger.debug("running bulk with kwargs: %s", bulk_kwargs)
+            if use_threads:
+                # Parallel bulk does not support max_retries, initial_backoff & max_backoff
+                for _success, _errors in opensearchpy.helpers.parallel_bulk(
+                    client, bulk_chunk_documents, **bulk_kwargs
+                ):
+                    success += _success
+                    errors += _errors
+            else:
+                # Defaults
+                bulk_kwargs["max_retries"] = 5 if not max_retries else max_retries
+                bulk_kwargs["initial_backoff"] = 2 if not initial_backoff else initial_backoff
+                bulk_kwargs["max_backoff"] = 600 if not max_backoff else max_backoff
+
+                _success, _errors = opensearchpy.helpers.bulk(client, bulk_chunk_documents, **bulk_kwargs)
+                success += _success
+                errors += _errors
             _logger.debug("indexed %s documents (%s/%s)", _success, success, total_documents)
             if progressbar:
                 progress_bar.update(success, force=True)
     except opensearchpy.TransportError as e:
         if str(e.status_code) == "429":  # Too Many Requests
             _logger.error(
                 "Error 429 (Too Many Requests):"
```

### Comparing `awswrangler-3.1.1/awswrangler/oracle.py` & `awswrangler-3.2.0/awswrangler/oracle.py`

 * *Files 10% similar despite different names*

```diff
@@ -197,14 +197,15 @@
     con: "oracledb.Connection",
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -212,14 +213,15 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -227,28 +229,30 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(oracledb, "oracledb")
 def read_sql_query(
     sql: str,
     con: "oracledb.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding to the result set of the query string.
 
     Parameters
     ----------
     sql : str
         SQL query.
@@ -266,14 +270,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -294,28 +304,30 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 @overload
 def read_sql_table(
     table: str,
     con: "oracledb.Connection",
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -324,14 +336,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -340,14 +353,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(oracledb, "oracledb")
 def read_sql_table(
     table: str,
@@ -355,14 +369,15 @@
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding the table.
 
     Parameters
     ----------
     table : str
         Table name.
@@ -383,14 +398,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -413,14 +434,15 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 def _generate_insert_statement(
     table_identifier: str,
     df: pd.DataFrame,
     use_column_names: bool,
@@ -565,15 +587,15 @@
             else:
                 sql = _generate_insert_statement(table_identifier, df, use_column_names)
 
             placeholder_parameter_pair_generator = _db_utils.generate_placeholder_parameter_pairs(
                 df=df, column_placeholders=column_placeholders, chunksize=chunksize
             )
             for _, parameters in placeholder_parameter_pair_generator:
-                parameters = list(zip(*[iter(parameters)] * len(df.columns)))
+                parameters = list(zip(*[iter(parameters)] * len(df.columns)))  # ruff: noqa: PLW2901
                 _logger.debug("sql: %s", sql)
                 cursor.executemany(sql, parameters)
 
             con.commit()
     except Exception as ex:
         con.rollback()
         _logger.error(ex)
```

### Comparing `awswrangler-3.1.1/awswrangler/pandas/__init__.py` & `awswrangler-3.2.0/awswrangler/pandas/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """Pandas "proxy" package."""
 import logging
 from typing import TYPE_CHECKING
 
-from packaging import version
-from pandas import __version__ as _PANDAS_VERSION
-
 from awswrangler._distributed import MemoryFormatEnum, memory_format
 
 if TYPE_CHECKING or memory_format.get() == MemoryFormatEnum.PANDAS:
     from pandas import *  # noqa: F403
 
     # Explicit import because mypy doesn't support forward references to a star import
     from pandas import (  # noqa: F401
@@ -40,20 +37,14 @@
         to_datetime,
     )
 else:
     raise ImportError(f"Unknown memory format {memory_format}")
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
-if version.parse(_PANDAS_VERSION) >= version.parse("2.0.0"):
-    _logger.warning(
-        "Pandas version 2.x was detected. Please note awswrangler currently does not support pyarrow-backed ArrowDtype "
-        "DataFrames."
-    )
-
 __all__ = [
     "DataFrame",
     "Series",
     "concat",
     "isna",
     "isnull",
     "json_normalize",
```

### Comparing `awswrangler-3.1.1/awswrangler/postgresql.py` & `awswrangler-3.2.0/awswrangler/postgresql.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     con: Any,
     chunksize: int,
     index_col: Optional[Union[str, List[str]]],
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]],
     safe: bool,
     dtype: Optional[Dict[str, pa.DataType]],
     timestamp_as_object: bool,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"],
 ) -> Iterator[pd.DataFrame]:
     """
     Iterate through the results using server-side cursor.
 
     Note: Pg8000 is not fully DB API 2.0 - compliant with fetchmany() fetching all result set. Using server-side cursor
     allows fetching only specific amount of results reducing memory impact. Ultimately we'd like pg8000 to add full
     support for fetchmany() or add SSCursor implementation similar to MySQL and revise this implementation in the future.
@@ -107,14 +108,15 @@
                 yield _db_utils._records2df(
                     records=records,
                     cols_names=_db_utils._get_cols_names(cursor.description),
                     index=index_col,
                     safe=safe,
                     dtype=dtype,
                     timestamp_as_object=timestamp_as_object,
+                    dtype_backend=dtype_backend,
                 )
         finally:
             cursor.execute(f"CLOSE {sscursor_name}")
 
 
 @_utils.check_optional_dependency(pg8000, "pg8000")
 def connect(
@@ -212,14 +214,15 @@
     con: "pg8000.Connection",
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -227,14 +230,15 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -242,28 +246,30 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(pg8000, "pg8000")
 def read_sql_query(
     sql: str,
     con: "pg8000.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding to the result set of the query string.
 
     Parameters
     ----------
     sql : str
         SQL query.
@@ -281,14 +287,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -311,38 +323,41 @@
             con=con,
             chunksize=chunksize,
             index_col=index_col,
             params=params,
             safe=safe,
             dtype=dtype,
             timestamp_as_object=timestamp_as_object,
+            dtype_backend=dtype_backend,
         )
     return _db_utils.read_sql_query(
         sql=sql,
         con=con,
         index_col=index_col,
         params=params,
         chunksize=None,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 @overload
 def read_sql_table(
     table: str,
     con: "pg8000.Connection",
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -351,14 +366,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -367,14 +383,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(pg8000, "pg8000")
 def read_sql_table(
     table: str,
@@ -382,14 +399,15 @@
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding the table.
 
     Parameters
     ----------
     table : str
         Table name.
@@ -410,14 +428,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -440,14 +464,15 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 _ToSqlModeLiteral = Literal["append", "overwrite", "upsert"]
 
 
 @_utils.check_optional_dependency(pg8000, "pg8000")
```

### Comparing `awswrangler-3.1.1/awswrangler/quicksight/__init__.py` & `awswrangler-3.2.0/awswrangler/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/quicksight/_cancel.py` & `awswrangler-3.2.0/awswrangler/quicksight/_cancel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/quicksight/_create.py` & `awswrangler-3.2.0/awswrangler/quicksight/_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """Amazon QuickSight Create Module."""
 
 import logging
 import uuid
-from typing import Any, Dict, List, Literal, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Optional, Set, TypeVar, Union, cast
 
 import boto3
 
 from awswrangler import _utils, exceptions, sts
-from awswrangler.quicksight._get_list import get_data_source_arn, get_dataset_id, list_users
-from awswrangler.quicksight._utils import extract_athena_query_columns, extract_athena_table_columns
+from awswrangler.quicksight._get_list import get_data_source_arn, get_dataset_id, list_groups, list_users
+from awswrangler.quicksight._utils import (
+    _QuicksightPrincipalList,
+    extract_athena_query_columns,
+    extract_athena_table_columns,
+)
+
+if TYPE_CHECKING:
+    from mypy_boto3_quicksight.type_defs import GroupTypeDef, UserTypeDef
+
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
+
 _ALLOWED_ACTIONS: Dict[str, Dict[str, List[str]]] = {
     "data_source": {
         "allowed_to_use": [
             "quicksight:DescribeDataSource",
             "quicksight:DescribeDataSourcePermissions",
             "quicksight:PassDataSource",
         ],
@@ -48,59 +57,104 @@
             "quicksight:CancelIngestion",
             "quicksight:UpdateDataSetPermissions",
         ],
     },
 }
 
 
-def _usernames_to_arns(user_names: List[str], all_users: List[Dict[str, Any]]) -> List[str]:
-    return [cast(str, u["Arn"]) for u in all_users if u.get("UserName") in user_names]
+def _groupnames_to_arns(group_names: Set[str], all_groups: List["GroupTypeDef"]) -> List[str]:
+    return [u["Arn"] for u in all_groups if u.get("GroupName") in group_names]
 
 
-def _generate_permissions(
+def _usernames_to_arns(user_names: Set[str], all_users: List["UserTypeDef"]) -> List[str]:
+    return [u["Arn"] for u in all_users if u.get("UserName") in user_names]
+
+
+_PrincipalTypeDef = TypeVar("_PrincipalTypeDef", "UserTypeDef", "GroupTypeDef")
+
+
+def _generate_permissions_base(
     resource: str,
     namespace: str,
     account_id: str,
     boto3_session: Optional[boto3.Session],
-    allowed_to_use: Optional[List[str]] = None,
-    allowed_to_manage: Optional[List[str]] = None,
+    allowed_to_use: Optional[List[str]],
+    allowed_to_manage: Optional[List[str]],
+    principal_names_to_arns_func: Callable[[Set[str], List[_PrincipalTypeDef]], List[str]],
+    list_principals: Callable[[str, str, Optional[boto3.Session]], List[Dict[str, Any]]],
 ) -> List[Dict[str, Union[str, List[str]]]]:
     permissions: List[Dict[str, Union[str, List[str]]]] = []
     if (allowed_to_use is None) and (allowed_to_manage is None):
         return permissions
 
-    # Forcing same user not be in both lists at the same time.
-    if (allowed_to_use is not None) and (allowed_to_manage is not None):
-        allowed_to_use = list(set(allowed_to_use) - set(allowed_to_manage))
+    allowed_to_use_set = set(allowed_to_use) if allowed_to_use else None
+    allowed_to_manage_set = set(allowed_to_manage) if allowed_to_manage else None
 
-    all_users: List[Dict[str, Any]] = list_users(
-        namespace=namespace, account_id=account_id, boto3_session=boto3_session
-    )
+    # Forcing same principal not be in both lists at the same time.
+    if (allowed_to_use_set is not None) and (allowed_to_manage_set is not None):
+        allowed_to_use_set = allowed_to_use_set - allowed_to_manage_set
+
+    all_principals = cast(List[_PrincipalTypeDef], list_principals(namespace, account_id, boto3_session))
 
-    if allowed_to_use is not None:
-        allowed_arns: List[str] = _usernames_to_arns(user_names=allowed_to_use, all_users=all_users)
+    if allowed_to_use_set is not None:
+        allowed_arns: List[str] = principal_names_to_arns_func(allowed_to_use_set, all_principals)
         permissions += [
             {
                 "Principal": arn,
                 "Actions": _ALLOWED_ACTIONS[resource]["allowed_to_use"],
             }
             for arn in allowed_arns
         ]
-    if allowed_to_manage is not None:
-        allowed_arns = _usernames_to_arns(user_names=allowed_to_manage, all_users=all_users)
+    if allowed_to_manage_set is not None:
+        allowed_arns = principal_names_to_arns_func(allowed_to_manage_set, all_principals)
         permissions += [
             {
                 "Principal": arn,
                 "Actions": _ALLOWED_ACTIONS[resource]["allowed_to_manage"],
             }
             for arn in allowed_arns
         ]
     return permissions
 
 
+def _generate_permissions(
+    resource: str,
+    namespace: str,
+    account_id: str,
+    boto3_session: Optional[boto3.Session],
+    allowed_users_to_use: Optional[List[str]] = None,
+    allowed_groups_to_use: Optional[List[str]] = None,
+    allowed_users_to_manage: Optional[List[str]] = None,
+    allowed_groups_to_manage: Optional[List[str]] = None,
+) -> List[Dict[str, Union[str, List[str]]]]:
+    permissions_users = _generate_permissions_base(
+        resource=resource,
+        namespace=namespace,
+        account_id=account_id,
+        boto3_session=boto3_session,
+        allowed_to_use=allowed_users_to_use,
+        allowed_to_manage=allowed_users_to_manage,
+        principal_names_to_arns_func=_usernames_to_arns,
+        list_principals=list_users,
+    )
+
+    permissions_groups = _generate_permissions_base(
+        resource=resource,
+        namespace=namespace,
+        account_id=account_id,
+        boto3_session=boto3_session,
+        allowed_to_use=allowed_groups_to_use,
+        allowed_to_manage=allowed_groups_to_manage,
+        principal_names_to_arns_func=_groupnames_to_arns,
+        list_principals=list_groups,
+    )
+
+    return permissions_users + permissions_groups
+
+
 def _generate_transformations(
     rename_columns: Optional[Dict[str, str]],
     cast_columns_types: Optional[Dict[str, str]],
     tag_columns: Optional[Dict[str, List[Dict[str, Any]]]],
 ) -> List[Dict[str, Dict[str, Any]]]:
     trans: List[Dict[str, Dict[str, Any]]] = []
     if rename_columns is not None:
@@ -111,19 +165,35 @@
             trans.append({"CastColumnTypeOperation": {"ColumnName": k, "NewColumnType": v.upper()}})
     if tag_columns is not None:
         for k, tags in tag_columns.items():
             trans.append({"TagColumnOperation": {"ColumnName": k, "Tags": tags}})
     return trans
 
 
+_AllowedType = Optional[Union[List[str], _QuicksightPrincipalList]]
+
+
+def _get_principal_names(principals: _AllowedType, type: Literal["users", "groups"]) -> Optional[List[str]]:
+    if principals is None:
+        return None
+
+    if isinstance(principals, list):
+        if type == "users":
+            return principals
+        else:
+            return None
+
+    return principals.get(type)
+
+
 def create_athena_data_source(
     name: str,
     workgroup: str = "primary",
-    allowed_to_use: Optional[List[str]] = None,
-    allowed_to_manage: Optional[List[str]] = None,
+    allowed_to_use: _AllowedType = None,
+    allowed_to_manage: _AllowedType = None,
     tags: Optional[Dict[str, str]] = None,
     account_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     namespace: str = "default",
 ) -> None:
     """Create a QuickSight data source pointing to an Athena/Workgroup.
 
@@ -136,21 +206,27 @@
     ----------
     name : str
         Data source name.
     workgroup : str
         Athena workgroup.
     tags : Dict[str, str], optional
         Key/Value collection to put on the Cluster.
-        e.g. {"foo": "boo", "bar": "xoo"})
-    allowed_to_use : optional
-        List of principals that will be allowed to see and use the data source.
-        e.g. ["John"]
-    allowed_to_manage : optional
-        List of principals that will be allowed to see, use, update and delete the data source.
-        e.g. ["Mary"]
+        e.g. ```{"foo": "boo", "bar": "xoo"})```
+    allowed_to_use: dict["users" | "groups", list[str]], optional
+        Dictionary containing usernames and groups that will be allowed to see and
+        use the data.
+        e.g. ```{"users": ["john", "Mary"], "groups": ["engineering", "customers"]}```
+        Alternatively, if a list of string is passed,
+        it will be interpreted as a list of usernames only.
+    allowed_to_manage: dict["users" | "groups", list[str]], optional
+        Dictionary containing usernames and groups that will be allowed to see, use,
+        update and delete the data source.
+        e.g. ```{"users": ["Mary"], "groups": ["engineering"]}```
+        Alternatively, if a list of string is passed,
+        it will be interpreted as a list of usernames only.
     account_id : str, optional
         If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     namespace : str
         The namespace. Currently, you should set this to default.
 
@@ -176,19 +252,21 @@
         "Name": name,
         "Type": "ATHENA",
         "DataSourceParameters": {"AthenaParameters": {"WorkGroup": workgroup}},
         "SslProperties": {"DisableSsl": True},
     }
     permissions: List[Dict[str, Union[str, List[str]]]] = _generate_permissions(
         resource="data_source",
+        namespace=namespace,
         account_id=account_id,
         boto3_session=boto3_session,
-        allowed_to_use=allowed_to_use,
-        allowed_to_manage=allowed_to_manage,
-        namespace=namespace,
+        allowed_users_to_use=_get_principal_names(allowed_to_use, "users"),
+        allowed_users_to_manage=_get_principal_names(allowed_to_manage, "users"),
+        allowed_groups_to_use=_get_principal_names(allowed_to_use, "groups"),
+        allowed_groups_to_manage=_get_principal_names(allowed_to_manage, "groups"),
     )
     if permissions:
         args["Permissions"] = permissions
     if tags is not None:
         _tags: List[Dict[str, str]] = [{"Key": k, "Value": v} for k, v in tags.items()]
         args["Tags"] = _tags
     client.create_data_source(**args)
@@ -199,16 +277,16 @@
     database: Optional[str] = None,
     table: Optional[str] = None,
     sql: Optional[str] = None,
     sql_name: Optional[str] = None,
     data_source_name: Optional[str] = None,
     data_source_arn: Optional[str] = None,
     import_mode: Literal["SPICE", "DIRECT_QUERY"] = "DIRECT_QUERY",
-    allowed_to_use: Optional[List[str]] = None,
-    allowed_to_manage: Optional[List[str]] = None,
+    allowed_to_use: _AllowedType = None,
+    allowed_to_manage: _AllowedType = None,
     logical_table_alias: str = "LogicalTable",
     rename_columns: Optional[Dict[str, str]] = None,
     cast_columns_types: Optional[Dict[str, str]] = None,
     tag_columns: Optional[Dict[str, List[Dict[str, Any]]]] = None,
     tags: Optional[Dict[str, str]] = None,
     account_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
@@ -247,20 +325,26 @@
         QuickSight data source ARN.
     import_mode : str
         Indicates whether you want to import the data into SPICE.
         'SPICE'|'DIRECT_QUERY'
     tags : Dict[str, str], optional
         Key/Value collection to put on the Cluster.
         e.g. {"foo": "boo", "bar": "xoo"}
-    allowed_to_use : optional
-        List of usernames that will be allowed to see and use the data source.
-        e.g. ["john", "Mary"]
-    allowed_to_manage : optional
-        List of usernames that will be allowed to see, use, update and delete the data source.
-        e.g. ["Mary"]
+    allowed_to_use: dict["users" | "groups", list[str]], optional
+        Dictionary containing usernames and groups that will be allowed to see and
+        use the data.
+        e.g. ```{"users": ["john", "Mary"], "groups": ["engineering", "customers"]}```
+        Alternatively, if a list of string is passed,
+        it will be interpreted as a list of usernames only.
+    allowed_to_manage: dict["users" | "groups", list[str]], optional
+        Dictionary containing usernames and groups that will be allowed to see, use,
+        update and delete the data source.
+        e.g. ```{"users": ["Mary"], "groups": ["engineering"]}```
+        Alternatively, if a list of string is passed,
+        it will be interpreted as a list of usernames only.
     logical_table_alias : str
         A display name for the logical table.
     rename_columns : Dict[str, str], optional
         Dictionary to map column renames. e.g. {"old_name": "new_name", "old_name2": "new_name2"}
     cast_columns_types : Dict[str, str], optional
         Dictionary to map column casts. e.g. {"col_name": "STRING", "col_name2": "DECIMAL"}
         Valid types: 'STRING'|'INTEGER'|'DECIMAL'|'DATETIME'
@@ -343,21 +427,24 @@
         "LogicalTableMap": {table_uuid: {"Alias": logical_table_alias, "Source": {"PhysicalTableId": table_uuid}}},
     }
     trans: List[Dict[str, Dict[str, Any]]] = _generate_transformations(
         rename_columns=rename_columns, cast_columns_types=cast_columns_types, tag_columns=tag_columns
     )
     if trans:
         args["LogicalTableMap"][table_uuid]["DataTransforms"] = trans
+
     permissions: List[Dict[str, Union[str, List[str]]]] = _generate_permissions(
         resource="dataset",
+        namespace=namespace,
         account_id=account_id,
         boto3_session=boto3_session,
-        allowed_to_use=allowed_to_use,
-        allowed_to_manage=allowed_to_manage,
-        namespace=namespace,
+        allowed_users_to_use=_get_principal_names(allowed_to_use, "users"),
+        allowed_users_to_manage=_get_principal_names(allowed_to_manage, "users"),
+        allowed_groups_to_use=_get_principal_names(allowed_to_use, "groups"),
+        allowed_groups_to_manage=_get_principal_names(allowed_to_manage, "groups"),
     )
     if permissions:
         args["Permissions"] = permissions
     if tags is not None:
         _tags: List[Dict[str, str]] = [{"Key": k, "Value": v} for k, v in tags.items()]
         args["Tags"] = _tags
     client.create_data_set(**args)
```

### Comparing `awswrangler-3.1.1/awswrangler/quicksight/_delete.py` & `awswrangler-3.2.0/awswrangler/quicksight/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/quicksight/_describe.py` & `awswrangler-3.2.0/awswrangler/quicksight/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/quicksight/_get_list.py` & `awswrangler-3.2.0/awswrangler/quicksight/_get_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/quicksight/_utils.py` & `awswrangler-3.2.0/awswrangler/quicksight/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Internal (private) Amazon QuickSight Utilities Module."""
 
 import logging
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, TypedDict
 
 import boto3
+from typing_extensions import NotRequired
 
 from awswrangler import _data_types, athena, catalog, exceptions
 from awswrangler.quicksight._get_list import list_data_sources
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+class _QuicksightPrincipalList(TypedDict):
+    users: NotRequired[List[str]]
+    groups: NotRequired[List[str]]
+
+
 def extract_athena_table_columns(
     database: str, table: str, boto3_session: Optional[boto3.Session]
 ) -> List[Dict[str, str]]:
     """Extract athena columns data types from table and raising an exception if not exist."""
     dtypes: Optional[Dict[str, str]] = catalog.get_table_types(
         database=database, table=table, boto3_session=boto3_session
     )
```

### Comparing `awswrangler-3.1.1/awswrangler/redshift/_connect.py` & `awswrangler-3.2.0/awswrangler/redshift/_connect.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/redshift/_read.py` & `awswrangler-3.2.0/awswrangler/redshift/_read.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import boto3
 import pyarrow as pa
 
 import awswrangler.pandas as pd
 from awswrangler import _databases as _db_utils
 from awswrangler import _utils, exceptions, s3
+from awswrangler._config import apply_configs
 from awswrangler._distributed import EngineEnum, engine
 
 from ._connect import _validate_connection
 from ._utils import _make_s3_auth_string
 
 redshift_connector = _utils.import_optional_dependency("redshift_connector")
 
@@ -19,40 +20,44 @@
 
 
 def _read_parquet_iterator(
     path: str,
     keep_files: bool,
     use_threads: Union[bool, int],
     chunked: Union[bool, int],
+    dtype_backend: Literal["numpy_nullable", "pyarrow"],
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, str]],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]],
 ) -> Iterator[pd.DataFrame]:
     dfs: Iterator[pd.DataFrame] = s3.read_parquet(
         path=path,
         chunked=chunked,
         dataset=False,
         use_threads=use_threads,
+        dtype_backend=dtype_backend,
         boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
     yield from dfs
     if keep_files is False:
         s3.delete_objects(
             path=path, use_threads=use_threads, boto3_session=boto3_session, s3_additional_kwargs=s3_additional_kwargs
         )
 
 
+@apply_configs
 @_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def read_sql_query(
     sql: str,
     con: "redshift_connector.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding to the result set of the query string.
 
@@ -70,14 +75,20 @@
     index_col : Union[str, List[str]], optional
         Column(s) to set as index(MultiIndex).
     params :  Union[List, Tuple, Dict], optional
         List of parameters to pass to execute method.
         The syntax used to pass parameters is database driver dependent.
         Check your database driver documentation for which of the five syntax styles,
         described in PEP 249’s paramstyle, is supported.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunksize : int, optional
         If specified, return an iterator where chunksize is the number of rows to include in each chunk.
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
@@ -108,24 +119,27 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
+@apply_configs
 @_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def read_sql_table(
     table: str,
     con: "redshift_connector.Connection",
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding the table.
 
@@ -146,14 +160,20 @@
     index_col : Union[str, List[str]], optional
         Column(s) to set as index(MultiIndex).
     params :  Union[List, Tuple, Dict], optional
         List of parameters to pass to execute method.
         The syntax used to pass parameters is database driver dependent.
         Check your database driver documentation for which of the five syntax styles,
         described in PEP 249's paramstyle, is supported.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunksize : int, optional
         If specified, return an iterator where chunksize is the number of rows to include in each chunk.
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
@@ -185,14 +205,15 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 @_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def unload_to_files(
     sql: str,
     path: str,
@@ -297,47 +318,52 @@
             iam_role=iam_role,
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
             aws_session_token=aws_session_token,
             boto3_session=boto3_session,
         )
 
-        sql = (
+        # Escape quotation marks in SQL
+        sql = sql.replace("'", "''")
+
+        unload_sql = (
             f"UNLOAD ('{sql}')\n"
             f"TO '{path}'\n"
             f"{auth_str}"
             "ALLOWOVERWRITE\n"
             "PARALLEL ON\n"
             f"FORMAT {format_str}\n"
             "ENCRYPTED"
             f"{kms_key_id_str}"
             f"{partition_str}"
             f"{region_str}"
             f"{max_file_size_str}"
             f"{manifest_str};"
         )
-        _logger.debug("Executing unload query:\n%s", sql)
-        cursor.execute(sql)
+        _logger.debug("Executing unload query:\n%s", unload_sql)
+        cursor.execute(unload_sql)
 
 
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
 )
+@apply_configs
 @_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def unload(
     sql: str,
     path: str,
     con: "redshift_connector.Connection",
     iam_role: Optional[str] = None,
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     aws_session_token: Optional[str] = None,
     region: Optional[str] = None,
     max_file_size: Optional[float] = None,
     kms_key_id: Optional[str] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunked: Union[bool, int] = False,
     keep_files: bool = False,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, str]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
@@ -403,14 +429,20 @@
         Specify a decimal value between 5.0 MB and 6200.0 MB. If None, the default
         maximum file size is 6200.0 MB.
     kms_key_id : str, optional
         Specifies the key ID for an AWS Key Management Service (AWS KMS) key to be
         used to encrypt data files on Amazon S3.
     keep_files : bool
         Should keep stage files?
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunked : Union[int, bool]
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
         If an `INTEGER` is passed awswrangler will iterate on the data by number of rows equal the received INTEGER.
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
@@ -459,14 +491,15 @@
     )
     if chunked is False:
         df: pd.DataFrame = s3.read_parquet(
             path=path,
             chunked=chunked,
             dataset=False,
             use_threads=use_threads,
+            dtype_backend=dtype_backend,
             boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
         )
         if keep_files is False:
             _logger.debug("Deleting objects in S3 path: %s", path)
             s3.delete_objects(
@@ -476,12 +509,13 @@
                 s3_additional_kwargs=s3_additional_kwargs,
             )
         return df
     return _read_parquet_iterator(
         path=path,
         chunked=chunked,
         use_threads=use_threads,
+        dtype_backend=dtype_backend,
         boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
         keep_files=keep_files,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
```

### Comparing `awswrangler-3.1.1/awswrangler/redshift/_utils.py` & `awswrangler-3.2.0/awswrangler/redshift/_utils.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/redshift/_write.py` & `awswrangler-3.2.0/awswrangler/redshift/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/__init__.py` & `awswrangler-3.2.0/awswrangler/s3/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from awswrangler.s3._copy import copy_objects, merge_datasets  # noqa
 from awswrangler.s3._delete import delete_objects  # noqa
 from awswrangler.s3._describe import describe_objects, get_bucket_region, size_objects  # noqa
 from awswrangler.s3._download import download  # noqa
 from awswrangler.s3._list import does_object_exist, list_buckets, list_directories, list_objects  # noqa
 from awswrangler.s3._read_deltalake import read_deltalake  # noqa
 from awswrangler.s3._read_excel import read_excel  # noqa
+from awswrangler.s3._read_orc import read_orc, read_orc_metadata, read_orc_table  # noqa
 from awswrangler.s3._read_parquet import read_parquet, read_parquet_metadata, read_parquet_table  # noqa
 from awswrangler.s3._read_text import read_csv, read_fwf, read_json  # noqa
 from awswrangler.s3._select import select_query
 from awswrangler.s3._upload import upload  # noqa
 from awswrangler.s3._wait import wait_objects_exist, wait_objects_not_exist  # noqa
 from awswrangler.s3._write_deltalake import to_deltalake  # noqa
 from awswrangler.s3._write_excel import to_excel  # noqa
+from awswrangler.s3._write_orc import to_orc  # noqa
 from awswrangler.s3._write_parquet import store_parquet_metadata, to_parquet  # noqa
 from awswrangler.s3._write_text import to_csv, to_json  # noqa
 
 __all__ = [
     "copy_objects",
     "merge_datasets",
     "delete_objects",
@@ -28,22 +30,26 @@
     "list_buckets",
     "list_directories",
     "list_objects",
     "read_deltalake",
     "read_parquet",
     "read_parquet_metadata",
     "read_parquet_table",
+    "read_orc",
+    "read_orc_metadata",
+    "read_orc_table",
     "read_csv",
     "read_fwf",
     "read_json",
     "wait_objects_exist",
     "wait_objects_not_exist",
     "select_query",
     "store_parquet_metadata",
     "to_parquet",
+    "to_orc",
     "to_csv",
     "to_json",
     "to_deltalake",
     "to_excel",
     "read_excel",
     "download",
     "upload",
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_copy.py` & `awswrangler-3.2.0/awswrangler/s3/_copy.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_delete.py` & `awswrangler-3.2.0/awswrangler/s3/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_describe.py` & `awswrangler-3.2.0/awswrangler/s3/_describe.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_download.py` & `awswrangler-3.2.0/awswrangler/s3/_download.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_fs.py` & `awswrangler-3.2.0/awswrangler/s3/_fs.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_list.py` & `awswrangler-3.2.0/awswrangler/s3/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_list.pyi` & `awswrangler-3.2.0/awswrangler/s3/_list.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -65,46 +65,50 @@
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> Union[List[str], Iterator[List[str]]]: ...
 @overload
 def list_objects(
     path: str,
     chunked: Literal[False],
+    suffix: Union[str, List[str], None] = ...,
     ignore_suffix: Union[str, List[str], None] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> List[str]: ...
 @overload
 def list_objects(
     path: str,
+    suffix: Union[str, List[str], None] = ...,
     ignore_suffix: Union[str, List[str], None] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> List[str]: ...
 @overload
 def list_objects(
     path: str,
     chunked: Literal[True],
+    suffix: Union[str, List[str], None] = ...,
     ignore_suffix: Union[str, List[str], None] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> Iterator[List[str]]: ...
 @overload
 def list_objects(
     path: str,
     chunked: bool,
+    suffix: Union[str, List[str], None] = ...,
     ignore_suffix: Union[str, List[str], None] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> Union[List[str], Iterator[List[str]]]: ...
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_read_deltalake.py` & `awswrangler-3.2.0/awswrangler/s3/_read_deltalake.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 """Amazon S3 Read Delta Lake Module (PRIVATE)."""
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 import boto3
+from typing_extensions import Literal
 
 import awswrangler.pandas as pd
 from awswrangler import _data_types, _utils
+from awswrangler._config import apply_configs
 
 if TYPE_CHECKING:
     try:
         import deltalake
     except ImportError:
         pass
 else:
     deltalake = _utils.import_optional_dependency("deltalake")
 
 
 def _set_default_storage_options_kwargs(
     boto3_session: Optional[boto3.Session], s3_additional_kwargs: Optional[Dict[str, Any]]
 ) -> Dict[str, Any]:
     defaults = {key.upper(): value for key, value in _utils.boto3_to_primitives(boto3_session=boto3_session).items()}
+    defaults["AWS_REGION"] = defaults.pop("REGION_NAME")
     s3_additional_kwargs = s3_additional_kwargs or {}
     return {
         **defaults,
         **s3_additional_kwargs,
     }
 
 
 @_utils.check_optional_dependency(deltalake, "deltalake")
+@apply_configs
 def read_deltalake(
     path: Optional[str] = None,
     version: Optional[int] = None,
     partitions: Optional[List[Tuple[str, str, Any]]] = None,
     columns: Optional[List[str]] = None,
     without_files: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     use_threads: bool = True,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, str]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> pd.DataFrame:
     """Load a Deltalake table data from an S3 path.
 
@@ -58,14 +63,20 @@
         for filter syntax.
     columns: Optional[List[str]]
         The columns to project. This can be a list of column names to include
         (order and duplicates are preserved).
     without_files: bool
         If True, load the table without tracking files (memory-friendly).
         Some append-only applications might not need to track files.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     use_threads : bool
         True to enable concurrent requests, False to disable multiple threads.
         When enabled, os.cpu_count() is used as the max number of threads.
     boto3_session: Optional[boto3.Session()]
         Boto3 Session. If None, the default boto3 session is used.
     s3_additional_kwargs: Optional[Dict[str, str]]
         Forwarded to the Delta Table class for the storage options of the S3 backend.
@@ -77,15 +88,17 @@
     df: pd.DataFrame
         DataFrame with the results.
 
     See Also
     --------
     deltalake.DeltaTable : Create a DeltaTable instance with the deltalake library.
     """
-    arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
+    arrow_kwargs = _data_types.pyarrow2pandas_defaults(
+        use_threads=use_threads, kwargs=pyarrow_additional_kwargs, dtype_backend=dtype_backend
+    )
     storage_options = _set_default_storage_options_kwargs(boto3_session, s3_additional_kwargs)
     return (
         deltalake.DeltaTable(
             table_uri=path,
             version=version,
             storage_options=storage_options,
             without_files=without_files,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_read_excel.py` & `awswrangler-3.2.0/awswrangler/s3/_read_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_read_parquet.py` & `awswrangler-3.2.0/awswrangler/s3/_read_parquet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,67 @@
 """Amazon S3 Read PARQUET Module (PRIVATE)."""
 
 import datetime
 import functools
 import itertools
 import logging
+import warnings
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
-    Iterable,
     Iterator,
     List,
     Optional,
-    Tuple,
     Union,
 )
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 import pyarrow.dataset
 import pyarrow.parquet
+from packaging import version
+from typing_extensions import Literal
 
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._arrow import _add_table_partitions, _table_to_df
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
 from awswrangler._executor import _BaseExecutor, _get_executor
-from awswrangler.catalog._get import _get_partitions
-from awswrangler.catalog._utils import _catalog_id
-from awswrangler.distributed.ray import ray_get
+from awswrangler.distributed.ray import ray_get  # noqa: F401
 from awswrangler.s3._fs import open_s3_object
 from awswrangler.s3._list import _path2list
 from awswrangler.s3._read import (
     _apply_partition_filter,
     _check_version_id,
     _extract_partitions_dtypes_from_table_details,
-    _extract_partitions_metadata_from_paths,
     _get_path_ignore_suffix,
     _get_path_root,
+    _get_paths_for_glue_table,
+    _InternalReadTableMetadataReturnValue,
+    _TableMetadataReader,
 )
-from awswrangler.typing import RayReadParquetSettings
+from awswrangler.typing import RayReadParquetSettings, _ReadTableMetadataReturnValue
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
 
 BATCH_READ_BLOCK_SIZE = 65_536
 CHUNKED_READ_S3_BLOCK_SIZE = 10_485_760  # 10 MB (20 * 2**20)
 FULL_READ_S3_BLOCK_SIZE = 20_971_520  # 20 MB (20 * 2**20)
 METADATA_READ_S3_BLOCK_SIZE = 131_072  # 128 KB (128 * 2**10)
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _ensure_locations_are_valid(paths: Iterable[str]) -> Iterator[str]:
-    for path in paths:
-        suffix: str = path.rpartition("/")[2]
-        # If the suffix looks like a partition,
-        if (suffix != "") and (suffix.count("=") == 1):
-            # the path should end in a '/' character.
-            path = f"{path}/"
-        yield path
-
-
 def _pyarrow_parquet_file_wrapper(
-    source: Any, coerce_int96_timestamp_unit: Optional[str] = None
+    source: Any,
+    coerce_int96_timestamp_unit: Optional[str] = None,
 ) -> pyarrow.parquet.ParquetFile:
     try:
         return pyarrow.parquet.ParquetFile(source=source, coerce_int96_timestamp_unit=coerce_int96_timestamp_unit)
     except pyarrow.ArrowInvalid as ex:
         if str(ex) == "Parquet file size is 0 bytes":
             _logger.warning("Ignoring empty file...")
             return None
@@ -98,74 +90,32 @@
             source=f, coerce_int96_timestamp_unit=coerce_int96_timestamp_unit
         )
         if pq_file:
             return pq_file.schema.to_arrow_schema()
         return None
 
 
-def _read_schemas_from_files(
-    paths: List[str],
-    sampling: float,
-    use_threads: Union[bool, int],
-    s3_client: "S3Client",
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    version_ids: Optional[Dict[str, str]] = None,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-) -> List[pa.schema]:
-    paths = _utils.list_sampling(lst=paths, sampling=sampling)
-
-    executor: _BaseExecutor = _get_executor(use_threads=use_threads)
-    schemas = ray_get(
-        executor.map(
-            _read_parquet_metadata_file,
-            s3_client,
-            paths,
-            itertools.repeat(s3_additional_kwargs),
-            itertools.repeat(use_threads),
-            [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
-            itertools.repeat(coerce_int96_timestamp_unit),
+class _ParquetTableMetadataReader(_TableMetadataReader):
+    def _read_metadata_file(
+        self,
+        s3_client: Optional["S3Client"],
+        path: str,
+        s3_additional_kwargs: Optional[Dict[str, str]],
+        use_threads: Union[bool, int],
+        version_id: Optional[str] = None,
+        coerce_int96_timestamp_unit: Optional[str] = None,
+    ) -> pa.schema:
+        return _read_parquet_metadata_file(
+            s3_client=s3_client,
+            path=path,
+            s3_additional_kwargs=s3_additional_kwargs,
+            use_threads=use_threads,
+            version_id=version_id,
+            coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
         )
-    )
-    return [schema for schema in schemas if schema is not None]
-
-
-def _validate_schemas(schemas: List[pa.schema], validate_schema: bool) -> pa.schema:
-    first: pa.schema = schemas[0]
-    if len(schemas) == 1:
-        return first
-    first_dict = {s.name: s.type for s in first}
-    if validate_schema:
-        for schema in schemas[1:]:
-            if first_dict != {s.name: s.type for s in schema}:
-                raise exceptions.InvalidSchemaConvergence(
-                    f"At least 2 different schemas were detected:\n    1 - {first}\n    2 - {schema}."
-                )
-    return pa.unify_schemas(schemas)
-
-
-def _validate_schemas_from_files(
-    validate_schema: bool,
-    paths: List[str],
-    sampling: float,
-    use_threads: Union[bool, int],
-    s3_client: "S3Client",
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    version_ids: Optional[Dict[str, str]] = None,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-) -> pa.schema:
-    schemas: List[pa.schema] = _read_schemas_from_files(
-        paths=paths,
-        sampling=sampling,
-        use_threads=use_threads,
-        s3_client=s3_client,
-        s3_additional_kwargs=s3_additional_kwargs,
-        version_ids=version_ids,
-        coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-    )
-    return _validate_schemas(schemas, validate_schema)
 
 
 def _read_parquet_metadata(
     path: Union[str, List[str]],
     path_suffix: Optional[str],
     path_ignore_suffix: Union[str, List[str], None],
     ignore_empty: bool,
@@ -174,89 +124,84 @@
     sampling: float,
     dataset: bool,
     use_threads: Union[bool, int],
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, str]],
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     coerce_int96_timestamp_unit: Optional[str] = None,
-) -> Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]:
+) -> _InternalReadTableMetadataReturnValue:
     """Handle wr.s3.read_parquet_metadata internally."""
-    s3_client = _utils.client(service_name="s3", session=boto3_session)
-    path_root: Optional[str] = _get_path_root(path=path, dataset=dataset)
-    paths: List[str] = _path2list(
+    reader = _ParquetTableMetadataReader()
+    return reader.read_table_metadata(
         path=path,
-        s3_client=s3_client,
-        suffix=path_suffix,
-        ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=path_ignore_suffix),
+        version_id=version_id,
+        path_suffix=path_suffix,
+        path_ignore_suffix=path_ignore_suffix,
         ignore_empty=ignore_empty,
-        s3_additional_kwargs=s3_additional_kwargs,
-    )
-    version_ids = _check_version_id(paths=paths, version_id=version_id)
-
-    # Files
-    schemas: List[pa.schema] = _read_schemas_from_files(
-        paths=paths,
+        ignore_null=ignore_null,
+        dtype=dtype,
         sampling=sampling,
+        dataset=dataset,
         use_threads=use_threads,
-        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
-        version_ids=version_ids,
+        boto3_session=boto3_session,
         coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
     )
-    merged_schemas = _validate_schemas(schemas=schemas, validate_schema=False)
-
-    columns_types: Dict[str, str] = _data_types.athena_types_from_pyarrow_schema(
-        schema=merged_schemas, partitions=None, ignore_null=ignore_null
-    )[0]
-
-    # Partitions
-    partitions_types: Optional[Dict[str, str]] = None
-    partitions_values: Optional[Dict[str, List[str]]] = None
-    if (dataset is True) and (path_root is not None):
-        partitions_types, partitions_values = _extract_partitions_metadata_from_paths(path=path_root, paths=paths)
-
-    # Casting
-    if dtype:
-        for k, v in dtype.items():
-            if columns_types and k in columns_types:
-                columns_types[k] = v
-            if partitions_types and k in partitions_types:
-                partitions_types[k] = v
-
-    return columns_types, partitions_types, partitions_values
 
 
 def _read_parquet_file(
     s3_client: Optional["S3Client"],
     path: str,
     path_root: Optional[str],
     columns: Optional[List[str]],
     coerce_int96_timestamp_unit: Optional[str],
     s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
     version_id: Optional[str] = None,
+    schema: Optional[pa.schema] = None,
 ) -> pa.Table:
     s3_block_size: int = FULL_READ_S3_BLOCK_SIZE if columns else -1  # One shot for a full read or see constant
     with open_s3_object(
         path=path,
         mode="rb",
         version_id=version_id,
         use_threads=use_threads,
         s3_block_size=s3_block_size,
         s3_additional_kwargs=s3_additional_kwargs,
         s3_client=s3_client,
     ) as f:
-        pq_file: Optional[pyarrow.parquet.ParquetFile] = _pyarrow_parquet_file_wrapper(
-            source=f,
-            coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-        )
-        if pq_file is None:
-            raise exceptions.InvalidFile(f"Invalid Parquet file: {path}")
+        if schema and version.parse(pa.__version__) >= version.parse("8.0.0"):
+            try:
+                table = pyarrow.parquet.read_table(
+                    f,
+                    columns=columns,
+                    schema=schema,
+                    use_threads=False,
+                    use_pandas_metadata=False,
+                    coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
+                )
+            except pyarrow.ArrowInvalid as ex:
+                if "Parquet file size is 0 bytes" in str(ex):
+                    raise exceptions.InvalidFile(f"Invalid Parquet file: {path}")
+                raise
+        else:
+            if schema:
+                warnings.warn(
+                    "Your version of pyarrow does not support reading with schema. Consider an upgrade to pyarrow 8+.",
+                    UserWarning,
+                )
+            pq_file: Optional[pyarrow.parquet.ParquetFile] = _pyarrow_parquet_file_wrapper(
+                source=f,
+                coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
+            )
+            if pq_file is None:
+                raise exceptions.InvalidFile(f"Invalid Parquet file: {path}")
+            table = pq_file.read(columns=columns, use_threads=False, use_pandas_metadata=False)
         return _add_table_partitions(
-            table=pq_file.read(columns=columns, use_threads=False, use_pandas_metadata=False),
+            table=table,
             path=path,
             path_root=path_root,
         )
 
 
 def _read_parquet_chunked(
     s3_client: Optional["S3Client"],
@@ -326,47 +271,51 @@
     use_threads: Union[bool, int],
     parallelism: int,
     version_ids: Optional[Dict[str, str]],
     s3_client: Optional["S3Client"],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     arrow_kwargs: Dict[str, Any],
     bulk_read: bool,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+) -> pd.DataFrame:
     executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     tables = executor.map(
         _read_parquet_file,
         s3_client,
         paths,
         itertools.repeat(path_root),
         itertools.repeat(columns),
         itertools.repeat(coerce_int96_timestamp_unit),
         itertools.repeat(s3_additional_kwargs),
         itertools.repeat(use_threads),
         [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
+        itertools.repeat(schema),
     )
     return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
 
 
 @_utils.validate_distributed_kwargs(
-    unsupported_kwargs=["boto3_session", "version_id", "s3_additional_kwargs"],
+    unsupported_kwargs=["boto3_session", "version_id", "s3_additional_kwargs", "dtype_backend"],
 )
+@apply_configs
 def read_parquet(
     path: Union[str, List[str]],
     path_root: Optional[str] = None,
     dataset: bool = False,
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
     ignore_empty: bool = True,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
     columns: Optional[List[str]] = None,
     validate_schema: bool = False,
     coerce_int96_timestamp_unit: Optional[str] = None,
+    schema: Optional[pa.Schema] = None,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     version_id: Optional[Union[str, Dict[str, str]]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunked: Union[bool, int] = False,
     use_threads: Union[bool, int] = True,
     ray_args: Optional[RayReadParquetSettings] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
@@ -425,31 +374,39 @@
     partition_filter : Callable[[Dict[str, str]], bool], optional
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-data-wrangler.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-data-wrangler.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
+    schema : pyarrow.Schema, optional
+        Schema to use whem reading the file.
     last_modified_begin : datetime, optional
         Filter S3 objects by Last modified date.
         Filter is only applied after listing all objects.
     last_modified_end : datetime, optional
         Filter S3 objects by Last modified date.
         Filter is only applied after listing all objects.
     version_id: Optional[Union[str, Dict[str, str]]]
         Version id of the object or mapping of object path to version id.
         (e.g. {'s3://bucket/key0': '121212', 's3://bucket/key1': '343434'})
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunked : Union[int, bool]
         If passed, the data is split into an iterable of DataFrames (Memory friendly).
         If `True` an iterable of DataFrames is returned without guarantee of chunksize.
         If an `INTEGER` is passed, an iterable of DataFrames is returned with maximum rows
         equal to the received INTEGER.
     use_threads : Union[bool, int], default True
         True to enable concurrent requests, False to disable multiple threads.
@@ -530,38 +487,31 @@
         paths = _apply_partition_filter(path_root=path_root, paths=paths, filter_func=partition_filter)
     if len(paths) < 1:
         raise exceptions.NoFilesFound(f"No files Found on: {path}.")
 
     version_ids = _check_version_id(paths=paths, version_id=version_id)
 
     # Create PyArrow schema based on file metadata, columns filter, and partitions
-    schema: Optional[pa.schema] = None
     if validate_schema and not bulk_read:
-        schema = _validate_schemas_from_files(
-            validate_schema=validate_schema,
+        metadata_reader = _ParquetTableMetadataReader()
+        schema = metadata_reader.validate_schemas(
             paths=paths,
-            sampling=1.0,
-            use_threads=use_threads,
+            path_root=path_root,
+            columns=columns,
+            validate_schema=validate_schema,
             s3_client=s3_client,
+            version_ids=version_ids,
+            use_threads=use_threads,
             s3_additional_kwargs=s3_additional_kwargs,
             coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-            version_ids=version_ids,
         )
-        if path_root:
-            partition_types, _ = _extract_partitions_metadata_from_paths(path=path_root, paths=paths)
-            if partition_types:
-                partition_schema = pa.schema(
-                    fields={k: _data_types.athena2pyarrow(dtype=v) for k, v in partition_types.items()}
-                )
-                schema = pa.unify_schemas([schema, partition_schema])
-        if columns:
-            schema = pa.schema([schema.field(column) for column in columns], schema.metadata)
-        _logger.debug("Resolved pyarrow schema:\n%s", schema)
 
-    arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
+    arrow_kwargs = _data_types.pyarrow2pandas_defaults(
+        use_threads=use_threads, kwargs=pyarrow_additional_kwargs, dtype_backend=dtype_backend
+    )
 
     if chunked:
         return _read_parquet_chunked(
             s3_client=s3_client,
             paths=paths,
             path_root=path_root,
             columns=columns,
@@ -585,28 +535,29 @@
         s3_additional_kwargs=s3_additional_kwargs,
         arrow_kwargs=arrow_kwargs,
         version_ids=version_ids,
         bulk_read=bulk_read,
     )
 
 
-@apply_configs
 @_utils.validate_distributed_kwargs(
-    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs", "dtype_backend"],
 )
+@apply_configs
 def read_parquet_table(
     table: str,
     database: str,
     filename_suffix: Union[str, List[str], None] = None,
     filename_ignore_suffix: Union[str, List[str], None] = None,
     catalog_id: Optional[str] = None,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
     columns: Optional[List[str]] = None,
     validate_schema: bool = True,
     coerce_int96_timestamp_unit: Optional[str] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunked: Union[bool, int] = False,
     use_threads: Union[bool, int] = True,
     ray_args: Optional[RayReadParquetSettings] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
@@ -650,22 +601,28 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function must receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values must be strings and the function
         must return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     columns : List[str], optional
         List of columns to read from the file(s).
     validate_schema : bool, default False
         Check that the schema is consistent across individual files.
     coerce_int96_timestamp_unit : str, optional
         Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
         Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunked : Union[int, bool]
         If passed, the data is split into an iterable of DataFrames (Memory friendly).
         If `True` an iterable of DataFrames is returned without guarantee of chunksize.
         If an `INTEGER` is passed, an iterable of DataFrames is returned with maximum rows
         equal to the received INTEGER.
     use_threads : Union[bool, int], default True
         True to enable concurrent requests, False to disable multiple threads.
@@ -704,68 +661,50 @@
     Reading Parquet Dataset with PUSH-DOWN filter over partitions
 
     >>> import awswrangler as wr
     >>> my_filter = lambda x: True if x["city"].startswith("new") else False
     >>> df = wr.s3.read_parquet_table(path, dataset=True, partition_filter=my_filter)
 
     """
-    client_glue = _utils.client(service_name="glue", session=boto3_session)
-    s3_client = _utils.client(service_name="s3", session=boto3_session)
-    res = client_glue.get_table(**_catalog_id(catalog_id=catalog_id, DatabaseName=database, Name=table))
-    try:
-        location: str = res["Table"]["StorageDescriptor"]["Location"]
-        path: str = location if location.endswith("/") else f"{location}/"
-    except KeyError as ex:
-        raise exceptions.InvalidTable(f"Missing s3 location for {database}.{table}.") from ex
-    path_root: Optional[str] = None
-    paths: Union[str, List[str]] = path
-    # If filter is available, fetch & filter out partitions
-    # Then list objects & process individual object keys under path_root
-    if partition_filter:
-        available_partitions_dict = _get_partitions(
-            database=database,
-            table=table,
-            catalog_id=catalog_id,
-            boto3_session=boto3_session,
-        )
-        available_partitions = list(_ensure_locations_are_valid(available_partitions_dict.keys()))
-        if available_partitions:
-            paths = []
-            path_root = path
-            partitions: Union[str, List[str]] = _apply_partition_filter(
-                path_root=path_root, paths=available_partitions, filter_func=partition_filter
-            )
-            for partition in partitions:
-                paths += _path2list(
-                    path=partition,
-                    s3_client=s3_client,
-                    suffix=filename_suffix,
-                    ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=filename_ignore_suffix),
-                    s3_additional_kwargs=s3_additional_kwargs,
-                )
+    paths: Union[str, List[str]]
+    path_root: Optional[str]
+
+    paths, path_root, res = _get_paths_for_glue_table(
+        table=table,
+        database=database,
+        filename_suffix=filename_suffix,
+        filename_ignore_suffix=filename_ignore_suffix,
+        catalog_id=catalog_id,
+        partition_filter=partition_filter,
+        boto3_session=boto3_session,
+        s3_additional_kwargs=s3_additional_kwargs,
+    )
 
     df = read_parquet(
         path=paths,
         path_root=path_root,
         dataset=True,
         path_suffix=filename_suffix if path_root is None else None,
         path_ignore_suffix=filename_ignore_suffix if path_root is None else None,
         columns=columns,
         validate_schema=validate_schema,
         coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
+        dtype_backend=dtype_backend,
         chunked=chunked,
         use_threads=use_threads,
         ray_args=ray_args,
         boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
 
     partial_cast_function = functools.partial(
-        _data_types.cast_pandas_with_athena_types, dtype=_extract_partitions_dtypes_from_table_details(response=res)
+        _data_types.cast_pandas_with_athena_types,
+        dtype=_extract_partitions_dtypes_from_table_details(response=res),
+        dtype_backend=dtype_backend,
     )
     if _utils.is_pandas_frame(df):
         return partial_cast_function(df)
     # df is a generator, so map is needed for casting dtypes
     return map(partial_cast_function, df)
 
 
@@ -783,15 +722,15 @@
     ignore_null: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     sampling: float = 1.0,
     coerce_int96_timestamp_unit: Optional[str] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Tuple[Dict[str, str], Optional[Dict[str, str]]]:
+) -> _ReadTableMetadataReturnValue:
     """Read Apache Parquet file(s) metadata from an S3 prefix or list of S3 objects paths.
 
     The concept of `dataset` enables more complex features like partitioning
     and catalog integration (AWS Glue Catalog).
 
     This function accepts Unix shell-style wildcards in the path argument.
     * (matches everything), ? (matches any single character),
@@ -861,22 +800,23 @@
     >>> import awswrangler as wr
     >>> columns_types, partitions_types = wr.s3.read_parquet_metadata(path=[
     ...     's3://bucket/filename0.parquet',
     ...     's3://bucket/filename1.parquet'
     ... ])
 
     """
-    return _read_parquet_metadata(
+    columns_types, partitions_types, _ = _read_parquet_metadata(
         path=path,
         version_id=version_id,
         path_suffix=path_suffix,
         path_ignore_suffix=path_ignore_suffix,
         ignore_empty=ignore_empty,
         ignore_null=ignore_null,
         dtype=dtype,
         sampling=sampling,
         dataset=dataset,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
         coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-    )[:2]
+    )
+    return _ReadTableMetadataReturnValue(columns_types, partitions_types)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_read_parquet.pyi` & `awswrangler-3.2.0/awswrangler/s3/_read_parquet.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -73,17 +73,19 @@
     path_suffix: Union[str, List[str], None] = ...,
     path_ignore_suffix: Union[str, List[str], None] = ...,
     ignore_empty: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    schema: Optional[pa.Schema] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: Literal[False] = ...,
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> pd.DataFrame: ...
@@ -96,17 +98,19 @@
     path_suffix: Union[str, List[str], None] = ...,
     path_ignore_suffix: Union[str, List[str], None] = ...,
     ignore_empty: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    schema: Optional[pa.Schema] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: Literal[True],
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
@@ -119,17 +123,19 @@
     path_suffix: Union[str, List[str], None] = ...,
     path_ignore_suffix: Union[str, List[str], None] = ...,
     ignore_empty: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    schema: Optional[pa.Schema] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: bool,
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
@@ -142,17 +148,19 @@
     path_suffix: Union[str, List[str], None] = ...,
     path_ignore_suffix: Union[str, List[str], None] = ...,
     ignore_empty: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    schema: Optional[pa.Schema] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: int,
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
@@ -164,14 +172,15 @@
     filename_suffix: Union[str, List[str], None] = ...,
     filename_ignore_suffix: Union[str, List[str], None] = ...,
     catalog_id: Optional[str] = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: Literal[False] = ...,
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> pd.DataFrame: ...
@@ -183,14 +192,15 @@
     filename_suffix: Union[str, List[str], None] = ...,
     filename_ignore_suffix: Union[str, List[str], None] = ...,
     catalog_id: Optional[str] = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: Literal[True],
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
@@ -202,14 +212,15 @@
     filename_suffix: Union[str, List[str], None] = ...,
     filename_ignore_suffix: Union[str, List[str], None] = ...,
     catalog_id: Optional[str] = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: bool,
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
@@ -221,14 +232,15 @@
     filename_suffix: Union[str, List[str], None] = ...,
     filename_ignore_suffix: Union[str, List[str], None] = ...,
     catalog_id: Optional[str] = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     columns: Optional[List[str]] = ...,
     validate_schema: bool = ...,
     coerce_int96_timestamp_unit: Optional[str] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunked: int,
     use_threads: Union[bool, int] = ...,
     ray_args: Optional[RayReadParquetSettings] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
 ) -> Iterator[pd.DataFrame]: ...
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_read_text.py` & `awswrangler-3.2.0/awswrangler/s3/_read_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import itertools
 import logging
 import pprint
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Union
 
 import boto3
 import pandas as pd
+from typing_extensions import Literal
 
 from awswrangler import _utils, exceptions
 from awswrangler._distributed import engine
 from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.s3._list import _path2list
 from awswrangler.s3._read import (
     _apply_partition_filter,
@@ -47,15 +48,15 @@
     s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
     dataset: bool,
     ignore_index: bool,
     parallelism: int,
     version_ids: Optional[Dict[str, str]],
     pandas_kwargs: Dict[str, Any],
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+) -> pd.DataFrame:
     parser_func = _resolve_format(read_format)
     executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     tables = executor.map(
         _read_text_file,
         s3_client,
         paths,
         [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
@@ -153,14 +154,15 @@
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     ignore_empty: bool = True,
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunksize: Optional[int] = None,
     dataset: bool = False,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
     ray_args: Optional[RaySettings] = None,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Read CSV file(s) from a received S3 prefix or list of S3 objects paths.
@@ -210,26 +212,32 @@
     last_modified_end: datetime, optional
         Filter the s3 files by the Last modified date of the object.
         The filter is applied only after list all s3 files.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forward to botocore requests, only "SSECustomerAlgorithm" and "SSECustomerKey" arguments will be considered.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunksize: int, optional
         If specified, return an generator where chunksize is the number of rows to include in each chunk.
     dataset : bool
         If `True` read a CSV dataset instead of simple file(s) loading all the related partitions as columns.
     partition_filter : Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs :
         KEYWORD arguments forwarded to pandas.read_csv(). You can NOT pass `pandas_kwargs` explicitly, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', na_values=['null', 'none'], skip_blank_lines=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
@@ -272,14 +280,18 @@
     """
     if "pandas_kwargs" in pandas_kwargs:
         raise exceptions.InvalidArgument(
             "You can NOT pass `pandas_kwargs` explicitly, just add valid "
             "Pandas arguments in the function call and awswrangler will accept it."
             "e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', skip_blank_lines=True)"
         )
+
+    if dtype_backend != "numpy_nullable":
+        pandas_kwargs["dtype_backend"] = dtype_backend
+
     s3_client = _utils.client(service_name="s3", session=boto3_session)
     ignore_index: bool = "index_col" not in pandas_kwargs
     return _read_text_format(
         read_format="csv",
         path=path,
         path_suffix=path_suffix,
         path_ignore_suffix=path_ignore_suffix,
@@ -377,15 +389,15 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_fwf(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_fwf(path='s3://bucket/prefix/', widths=[1, 3], names=["c0", "c1"])
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_fwf.html
@@ -466,14 +478,15 @@
     ignore_empty: bool = True,
     orient: str = "columns",
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     chunksize: Optional[int] = None,
     dataset: bool = False,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
     ray_args: Optional[RaySettings] = None,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Read JSON file(s) from a received S3 prefix or list of S3 objects paths.
@@ -525,27 +538,33 @@
     last_modified_end: datetime, optional
         Filter the s3 files by the Last modified date of the object.
         The filter is applied only after list all s3 files.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forward to botocore requests, only "SSECustomerAlgorithm" and "SSECustomerKey" arguments will be considered.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     chunksize: int, optional
         If specified, return an generator where chunksize is the number of rows to include in each chunk.
     dataset: bool
         If `True` read a JSON dataset instead of simple file(s) loading all the related partitions as columns.
         If `True`, the `lines=True` will be assumed by default.
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
     ray_args: typing.RaySettings, optional
         Parameters of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_json(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_json('s3://bucket/prefix/', lines=True, keep_default_dates=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_json.html
@@ -588,19 +607,24 @@
     """
     if "pandas_kwargs" in pandas_kwargs:
         raise exceptions.InvalidArgument(
             "You can NOT pass `pandas_kwargs` explicit, just add valid "
             "Pandas arguments in the function call and awswrangler will accept it."
             "e.g. wr.s3.read_json(path, lines=True, keep_default_dates=True)"
         )
+    if dtype_backend != "numpy_nullable":
+        pandas_kwargs["dtype_backend"] = dtype_backend
+
     s3_client = _utils.client(service_name="s3", session=boto3_session)
+
     if (dataset is True) and ("lines" not in pandas_kwargs):
         pandas_kwargs["lines"] = True
     pandas_kwargs["orient"] = orient
     ignore_index: bool = orient not in ("split", "index", "columns")
+
     return _read_text_format(
         read_format="json",
         path=path,
         path_suffix=path_suffix,
         path_ignore_suffix=path_ignore_suffix,
         version_id=version_id,
         ignore_empty=ignore_empty,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_read_text.pyi` & `awswrangler-3.2.0/awswrangler/s3/_read_text.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Union, overload
 
 import boto3
 import pandas as pd
+from typing_extensions import Literal
 
 from awswrangler.typing import RaySettings
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
 
 def _read_text(  # pylint: disable=W0613
@@ -31,14 +32,15 @@
     version_id: Optional[Union[str, Dict[str, str]]] = ...,
     ignore_empty: bool = ...,
     use_threads: Union[bool, int] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: None = ...,
     dataset: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     ray_args: Optional[RaySettings] = ...,
     **pandas_kwargs: Any,
 ) -> pd.DataFrame: ...
 @overload
@@ -50,14 +52,15 @@
     version_id: Optional[Union[str, Dict[str, str]]] = ...,
     ignore_empty: bool = ...,
     use_threads: Union[bool, int] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: int,
     dataset: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     ray_args: Optional[RaySettings] = ...,
     **pandas_kwargs: Any,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
@@ -69,14 +72,15 @@
     version_id: Optional[Union[str, Dict[str, str]]] = ...,
     ignore_empty: bool = ...,
     use_threads: Union[bool, int] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: Optional[int],
     dataset: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     ray_args: Optional[RaySettings] = ...,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
@@ -88,14 +92,15 @@
     ignore_empty: bool = ...,
     orient: str = ...,
     use_threads: Union[bool, int] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: None = ...,
     dataset: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     ray_args: Optional[RaySettings] = ...,
     **pandas_kwargs: Any,
 ) -> pd.DataFrame: ...
 @overload
@@ -108,14 +113,15 @@
     ignore_empty: bool = ...,
     orient: str = ...,
     use_threads: Union[bool, int] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: int,
     dataset: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     ray_args: Optional[RaySettings] = ...,
     **pandas_kwargs: Any,
 ) -> Iterator[pd.DataFrame]: ...
 @overload
@@ -128,14 +134,15 @@
     ignore_empty: bool = ...,
     orient: str = ...,
     use_threads: Union[bool, int] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
     chunksize: Optional[int],
     dataset: bool = ...,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
     ray_args: Optional[RaySettings] = ...,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]: ...
 @overload
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_read_text_core.py` & `awswrangler-3.2.0/awswrangler/s3/_read_text_core.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_select.py` & `awswrangler-3.2.0/awswrangler/s3/_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 import pprint
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Union
 
 import boto3
 import pandas as pd
 import pyarrow as pa
+from typing_extensions import Literal
 
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._distributed import engine
 from awswrangler._executor import _BaseExecutor, _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._describe import size_objects
 from awswrangler.s3._list import _path2list
@@ -157,14 +158,15 @@
     scan_range_chunk_size: Optional[int] = None,
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
     ignore_empty: bool = True,
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> pd.DataFrame:
     r"""Filter contents of Amazon S3 objects based on SQL statement.
 
     Note: Scan ranges are only supported for uncompressed CSV/JSON, CSV (without quoted delimiters)
@@ -202,14 +204,20 @@
         If integer is provided, specified number is used.
     last_modified_begin : datetime, optional
         Filter S3 objects by Last modified date.
         Filter is only applied after listing all objects.
     last_modified_end : datetime, optional
         Filter S3 objects by Last modified date.
         Filter is only applied after listing all objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session is used if none is provided.
     s3_additional_kwargs : Dict[str, Any], optional
         Forwarded to botocore requests.
         Valid values: "SSECustomerAlgorithm", "SSECustomerKey", "ExpectedBucketOwner".
         e.g. s3_additional_kwargs={'SSECustomerAlgorithm': 'md5'}.
     pyarrow_additional_kwargs : Dict[str, Any], optional
@@ -290,13 +298,15 @@
         "boto3_session": boto3_session,
         "s3_additional_kwargs": s3_additional_kwargs,
     }
 
     if pyarrow_additional_kwargs and "schema" in pyarrow_additional_kwargs:
         select_kwargs["schema"] = pyarrow_additional_kwargs.pop("schema")
 
-    arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
+    arrow_kwargs = _data_types.pyarrow2pandas_defaults(
+        use_threads=use_threads, kwargs=pyarrow_additional_kwargs, dtype_backend=dtype_backend
+    )
     executor: _BaseExecutor = _get_executor(use_threads=use_threads)
     tables = list(
         itertools.chain(*ray_get([_select_query(path=path, executor=executor, **select_kwargs) for path in paths]))
     )
     return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_upload.py` & `awswrangler-3.2.0/awswrangler/s3/_upload.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_wait.py` & `awswrangler-3.2.0/awswrangler/s3/_wait.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_write_concurrent.py` & `awswrangler-3.2.0/awswrangler/s3/_write_concurrent.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_write_dataset.py` & `awswrangler-3.2.0/awswrangler/s3/_write_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,16 @@
     **func_kwargs: Any,
 ) -> Tuple[List[str], Dict[str, List[str]]]:
     partitions_values: Dict[str, List[str]] = {}
     proxy: _WriteProxy = _WriteProxy(use_threads=concurrent_partitioning)
     s3_client = client(service_name="s3", session=boto3_session)
     for keys, subgroup in df.groupby(by=partition_cols, observed=True):
         # Keys are either a primitive type or a tuple if partitioning by multiple cols
-        keys = (keys,) if not isinstance(keys, tuple) else keys
-        subgroup = subgroup.drop(partition_cols, axis="columns")
+        keys = (keys,) if not isinstance(keys, tuple) else keys  # ruff: noqa: PLW2901
+        subgroup = subgroup.drop(partition_cols, axis="columns")  # ruff: noqa: PLW2901
         prefix = _delete_objects(
             keys=keys,
             path_root=path_root,
             use_threads=use_threads,
             mode=mode,
             partition_cols=partition_cols,
             partitions_types=partitions_types,
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_write_deltalake.py` & `awswrangler-3.2.0/awswrangler/s3/_write_deltalake.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     deltalake = _utils.import_optional_dependency("deltalake")
 
 
 def _set_default_storage_options_kwargs(
     boto3_session: Optional[boto3.Session], s3_additional_kwargs: Optional[Dict[str, Any]], s3_allow_unsafe_rename: bool
 ) -> Dict[str, Any]:
     defaults = {key.upper(): value for key, value in _utils.boto3_to_primitives(boto3_session=boto3_session).items()}
+    defaults["AWS_REGION"] = defaults.pop("REGION_NAME")
     s3_additional_kwargs = s3_additional_kwargs or {}
     return {
         **defaults,
         **s3_additional_kwargs,
         "AWS_S3_ALLOW_UNSAFE_RENAME": "TRUE" if s3_allow_unsafe_rename else "FALSE",
     }
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_write_excel.py` & `awswrangler-3.2.0/awswrangler/s3/_write_excel.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/s3/_write_parquet.py` & `awswrangler-3.2.0/awswrangler/s3/_write_parquet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,49 @@
 """Amazon PARQUET S3 Parquet Write Module (PRIVATE)."""
 
 import logging
 import math
-import uuid
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Literal, Optional, Tuple, Union, cast
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 import pyarrow.lib
 import pyarrow.parquet
 
-from awswrangler import _data_types, _utils, catalog, exceptions, lakeformation, typing
+from awswrangler import _utils, catalog, exceptions, typing
 from awswrangler._arrow import _df_to_table
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
-from awswrangler._utils import copy_df_shallow
-from awswrangler.s3._delete import delete_objects
+from awswrangler.catalog._create import _create_parquet_table
 from awswrangler.s3._fs import open_s3_object
 from awswrangler.s3._read_parquet import _read_parquet_metadata
-from awswrangler.s3._write import _COMPRESSION_2_EXT, _apply_dtype, _sanitize, _validate_args
+from awswrangler.s3._write import (
+    _COMPRESSION_2_EXT,
+    _get_chunk_file_path,
+    _get_file_path,
+    _get_write_table_args,
+    _S3WriteStrategy,
+    _validate_args,
+)
 from awswrangler.s3._write_concurrent import _WriteProxy
-from awswrangler.s3._write_dataset import _to_dataset
-from awswrangler.typing import BucketingInfoTuple, GlueTableSettings, _S3WriteDataReturnValue
+from awswrangler.typing import (
+    AthenaPartitionProjectionSettings,
+    BucketingInfoTuple,
+    GlueTableSettings,
+    _S3WriteDataReturnValue,
+)
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3Client
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _get_file_path(
-    path_root: Optional[str] = None,
-    path: Optional[str] = None,
-    filename_prefix: Optional[str] = None,
-    compression_ext: str = "",
-    bucket_id: Optional[int] = None,
-    extension: str = ".parquet",
-) -> str:
-    if bucket_id is not None:
-        filename_prefix = f"{filename_prefix}_bucket-{bucket_id:05d}"
-    if path is None and path_root is not None:
-        file_path: str = f"{path_root}{filename_prefix}{compression_ext}{extension}"
-    elif path is not None and path_root is None:
-        file_path = path
-    else:
-        raise RuntimeError("path and path_root received at the same time.")
-    return file_path
-
-
-def _get_chunk_file_path(file_counter: int, file_path: str) -> str:
-    slash_index: int = file_path.rfind("/")
-    dot_index: int = file_path.find(".", slash_index)
-    file_index: str = "_" + str(file_counter)
-    if dot_index == -1:
-        file_path = file_path + file_index
-    else:
-        file_path = file_path[:dot_index] + file_index + file_path[dot_index:]
-    return file_path
-
-
-def _get_write_table_args(pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
-    write_table_args: Dict[str, Any] = {}
-    if pyarrow_additional_kwargs and "write_table_args" in pyarrow_additional_kwargs:
-        write_table_args = pyarrow_additional_kwargs.pop("write_table_args")
-    return write_table_args
-
-
 @contextmanager
 def _new_writer(
     file_path: str,
     compression: Optional[str],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]],
     schema: pa.Schema,
     s3_client: "S3Client",
@@ -167,15 +139,15 @@
             chunk_size=max_rows_by_file,
             use_threads=use_threads,
         )
     return proxy.close()  # blocking
 
 
 @engine.dispatch_on_engine
-def _to_parquet(
+def _to_parquet(  # pylint: disable=unused-argument
     df: pd.DataFrame,
     schema: pa.Schema,
     index: bool,
     compression: Optional[str],
     compression_ext: str,
     pyarrow_additional_kwargs: Dict[str, Any],
     cpus: int,
@@ -183,18 +155,23 @@
     s3_client: Optional["S3Client"],
     s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
     path: Optional[str] = None,
     path_root: Optional[str] = None,
     filename_prefix: Optional[str] = None,
     max_rows_by_file: Optional[int] = 0,
+    bucketing: bool = False,
 ) -> List[str]:
     s3_client = s3_client if s3_client else _utils.client(service_name="s3")
     file_path = _get_file_path(
-        path_root=path_root, path=path, filename_prefix=filename_prefix, compression_ext=compression_ext
+        path_root=path_root,
+        path=path,
+        filename_prefix=filename_prefix,
+        compression_ext=compression_ext,
+        extension=".parquet",
     )
     table: pa.Table = _df_to_table(df, schema, index, dtype)
     if max_rows_by_file is not None and max_rows_by_file > 0:
         paths: List[str] = _to_parquet_chunked(
             file_path=file_path,
             s3_client=s3_client,
             s3_additional_kwargs=s3_additional_kwargs,
@@ -217,14 +194,124 @@
             use_threads=use_threads,
         ) as writer:
             writer.write_table(table, **write_table_args)
         paths = [file_path]
     return paths
 
 
+class _S3ParquetWriteStrategy(_S3WriteStrategy):
+    @property
+    def _write_to_s3_func(self) -> Callable[..., List[str]]:
+        return _to_parquet
+
+    def _write_to_s3(
+        self,
+        df: pd.DataFrame,
+        schema: pa.Schema,
+        index: bool,
+        compression: Optional[str],
+        compression_ext: str,
+        pyarrow_additional_kwargs: Dict[str, Any],
+        cpus: int,
+        dtype: Dict[str, str],
+        s3_client: Optional["S3Client"],
+        s3_additional_kwargs: Optional[Dict[str, str]],
+        use_threads: Union[bool, int],
+        path: Optional[str] = None,
+        path_root: Optional[str] = None,
+        filename_prefix: Optional[str] = None,
+        max_rows_by_file: Optional[int] = 0,
+        bucketing: bool = False,
+    ) -> List[str]:
+        return _to_parquet(
+            df=df,
+            schema=schema,
+            index=index,
+            compression=compression,
+            compression_ext=compression_ext,
+            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            cpus=cpus,
+            dtype=dtype,
+            s3_client=s3_client,
+            s3_additional_kwargs=s3_additional_kwargs,
+            use_threads=use_threads,
+            path=path,
+            path_root=path_root,
+            filename_prefix=filename_prefix,
+            max_rows_by_file=max_rows_by_file,
+            bucketing=bucketing,
+        )
+
+    def _create_glue_table(
+        self,
+        database: str,
+        table: str,
+        path: str,
+        columns_types: Dict[str, str],
+        table_type: Optional[str] = None,
+        partitions_types: Optional[Dict[str, str]] = None,
+        bucketing_info: Optional[BucketingInfoTuple] = None,
+        catalog_id: Optional[str] = None,
+        compression: Optional[str] = None,
+        description: Optional[str] = None,
+        parameters: Optional[Dict[str, str]] = None,
+        columns_comments: Optional[Dict[str, str]] = None,
+        mode: str = "overwrite",
+        catalog_versioning: bool = False,
+        transaction_id: Optional[str] = None,
+        athena_partition_projection_settings: Optional[AthenaPartitionProjectionSettings] = None,
+        boto3_session: Optional[boto3.Session] = None,
+        catalog_table_input: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        return _create_parquet_table(
+            database=database,
+            table=table,
+            path=path,
+            columns_types=columns_types,
+            table_type=table_type,
+            partitions_types=partitions_types,
+            bucketing_info=bucketing_info,
+            catalog_id=catalog_id,
+            compression=compression,
+            description=description,
+            parameters=parameters,
+            columns_comments=columns_comments,
+            mode=mode,
+            catalog_versioning=catalog_versioning,
+            transaction_id=transaction_id,
+            athena_partition_projection_settings=athena_partition_projection_settings,
+            boto3_session=boto3_session,
+            catalog_table_input=catalog_table_input,
+        )
+
+    def _add_glue_partitions(
+        self,
+        database: str,
+        table: str,
+        partitions_values: Dict[str, List[str]],
+        bucketing_info: Optional[BucketingInfoTuple] = None,
+        catalog_id: Optional[str] = None,
+        compression: Optional[str] = None,
+        boto3_session: Optional[boto3.Session] = None,
+        columns_types: Optional[Dict[str, str]] = None,
+        partitions_parameters: Optional[Dict[str, str]] = None,
+    ) -> None:
+        return catalog.add_parquet_partitions(
+            database=database,
+            table=table,
+            partitions_values=partitions_values,
+            bucketing_info=bucketing_info,
+            compression=compression,
+            boto3_session=boto3_session,
+            catalog_id=catalog_id,
+            columns_types=columns_types,
+            partitions_parameters=partitions_parameters,
+        )
+
+
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
 )
 def to_parquet(  # pylint: disable=too-many-arguments,too-many-locals,too-many-branches,too-many-statements
     df: pd.DataFrame,
     path: Optional[str] = None,
@@ -318,26 +405,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode: str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/004%20-%20Parquet%20Datasets.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/004%20-%20Parquet%20Datasets.html
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised. True by default.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
@@ -612,197 +699,55 @@
     )
 
     # Evaluating compression
     if _COMPRESSION_2_EXT.get(compression, None) is None:
         raise exceptions.InvalidCompression(f"{compression} is invalid, please use None, 'snappy', 'gzip' or 'zstd'.")
     compression_ext: str = _COMPRESSION_2_EXT[compression]
 
-    # Initializing defaults
-    partition_cols = partition_cols if partition_cols else []
-    dtype = dtype if dtype else {}
-    partitions_values: Dict[str, List[str]] = {}
-    mode = "append" if mode is None else mode
-    commit_trans: bool = False
-    if transaction_id:
-        table_type = "GOVERNED"
-
-    filename_prefix = filename_prefix + uuid.uuid4().hex if filename_prefix else uuid.uuid4().hex
-    cpus: int = _utils.ensure_cpu_count(use_threads=use_threads)
-    s3_client = _utils.client(service_name="s3", session=boto3_session)
     # Pyarrow defaults
     if not pyarrow_additional_kwargs:
         pyarrow_additional_kwargs = {}
     if not pyarrow_additional_kwargs.get("coerce_timestamps"):
         pyarrow_additional_kwargs["coerce_timestamps"] = "ms"
     if "flavor" not in pyarrow_additional_kwargs:
         pyarrow_additional_kwargs["flavor"] = "spark"
 
-    # Sanitize table to respect Athena's standards
-    if (sanitize_columns is True) or (database is not None and table is not None):
-        df, dtype, partition_cols, bucketing_info = _sanitize(
-            df=copy_df_shallow(df),
-            dtype=dtype,
-            partition_cols=partition_cols,
-            bucketing_info=bucketing_info,
-        )
-
-    # Evaluating dtype
-    catalog_table_input: Optional[Dict[str, Any]] = None
-    if database is not None and table is not None:
-        catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
-            database=database,
-            table=table,
-            boto3_session=boto3_session,
-            transaction_id=transaction_id,
-            catalog_id=catalog_id,
-        )
-        catalog_path: Optional[str] = None
-        if catalog_table_input:
-            table_type = catalog_table_input["TableType"]
-            catalog_path = catalog_table_input["StorageDescriptor"]["Location"]
-        if path is None:
-            if catalog_path:
-                path = catalog_path
-            else:
-                raise exceptions.InvalidArgumentValue(
-                    "Glue table does not exist in the catalog. Please pass the `path` argument to create it."
-                )
-        elif path and catalog_path:
-            if path.rstrip("/") != catalog_path.rstrip("/"):
-                raise exceptions.InvalidArgumentValue(
-                    f"The specified path: {path}, does not match the existing Glue catalog table path: {catalog_path}"
-                )
-        if (table_type == "GOVERNED") and (not transaction_id):
-            _logger.debug("`transaction_id` not specified for GOVERNED table, starting transaction")
-            transaction_id = lakeformation.start_transaction(
-                read_only=False,
-                boto3_session=boto3_session,
-            )
-            commit_trans = True
-
-    df = _apply_dtype(df=df, dtype=dtype, catalog_table_input=catalog_table_input, mode=mode)
-    schema: pa.Schema = _data_types.pyarrow_schema_from_pandas(
-        df=df, index=index, ignore_cols=partition_cols, dtype=dtype
+    strategy = _S3ParquetWriteStrategy()
+    return strategy.write(
+        df=df,
+        path=path,
+        index=index,
+        compression=compression,
+        pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+        max_rows_by_file=max_rows_by_file,
+        use_threads=use_threads,
+        boto3_session=boto3_session,
+        s3_additional_kwargs=s3_additional_kwargs,
+        sanitize_columns=sanitize_columns,
+        dataset=dataset,
+        filename_prefix=filename_prefix,
+        partition_cols=partition_cols,
+        bucketing_info=bucketing_info,
+        concurrent_partitioning=concurrent_partitioning,
+        mode=mode,
+        catalog_versioning=catalog_versioning,
+        schema_evolution=schema_evolution,
+        database=database,
+        table=table,
+        description=description,
+        parameters=parameters,
+        columns_comments=columns_comments,
+        table_type=table_type,
+        transaction_id=transaction_id,
+        regular_partitions=regular_partitions,
+        dtype=dtype,
+        athena_partition_projection_settings=athena_partition_projection_settings,
+        catalog_id=catalog_id,
+        compression_ext=compression_ext,
     )
-    _logger.debug("Resolved pyarrow schema: \n%s", schema)
-
-    if dataset is False:
-        paths = _to_parquet(
-            df,
-            path=path,
-            filename_prefix=filename_prefix,
-            schema=schema,
-            index=index,
-            cpus=cpus,
-            compression=compression,
-            compression_ext=compression_ext,
-            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            s3_client=s3_client,
-            s3_additional_kwargs=s3_additional_kwargs,
-            dtype=dtype,
-            max_rows_by_file=max_rows_by_file,
-            use_threads=use_threads,
-        )
-    else:
-        columns_types: Dict[str, str] = {}
-        partitions_types: Dict[str, str] = {}
-        if (database is not None) and (table is not None):
-            columns_types, partitions_types = _data_types.athena_types_from_pandas_partitioned(
-                df=df, index=index, partition_cols=partition_cols, dtype=dtype
-            )
-            if schema_evolution is False:
-                _utils.check_schema_changes(columns_types=columns_types, table_input=catalog_table_input, mode=mode)
-
-            create_table_args: Dict[str, Any] = {
-                "database": database,
-                "table": table,
-                "path": path,
-                "columns_types": columns_types,
-                "table_type": table_type,
-                "partitions_types": partitions_types,
-                "bucketing_info": bucketing_info,
-                "compression": compression,
-                "description": description,
-                "parameters": parameters,
-                "columns_comments": columns_comments,
-                "boto3_session": boto3_session,
-                "mode": mode,
-                "transaction_id": transaction_id,
-                "catalog_versioning": catalog_versioning,
-                "athena_partition_projection_settings": athena_partition_projection_settings,
-                "catalog_id": catalog_id,
-                "catalog_table_input": catalog_table_input,
-            }
-
-            if (catalog_table_input is None) and (table_type == "GOVERNED"):
-                catalog._create_parquet_table(**create_table_args)  # pylint: disable=protected-access
-                create_table_args["catalog_table_input"] = catalog._get_table_input(  # pylint: disable=protected-access
-                    database=database,
-                    table=table,
-                    boto3_session=boto3_session,
-                    transaction_id=transaction_id,
-                    catalog_id=catalog_id,
-                )
-
-        paths, partitions_values = _to_dataset(
-            func=_to_parquet,
-            concurrent_partitioning=concurrent_partitioning,
-            df=df,
-            path_root=path,  # type: ignore[arg-type]
-            filename_prefix=filename_prefix,
-            index=index,
-            compression=compression,
-            compression_ext=compression_ext,
-            catalog_id=catalog_id,
-            database=database,
-            table=table,
-            table_type=table_type,
-            transaction_id=transaction_id,
-            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            cpus=cpus,
-            use_threads=use_threads,
-            partition_cols=partition_cols,
-            partitions_types=partitions_types,
-            bucketing_info=bucketing_info,
-            dtype=dtype,
-            mode=mode,
-            boto3_session=boto3_session,
-            s3_additional_kwargs=s3_additional_kwargs,
-            schema=schema,
-            max_rows_by_file=max_rows_by_file,
-        )
-        if database and table:
-            try:
-                catalog._create_parquet_table(**create_table_args)  # pylint: disable=protected-access
-                if partitions_values and (regular_partitions is True) and (table_type != "GOVERNED"):
-                    catalog.add_parquet_partitions(
-                        database=database,
-                        table=table,
-                        partitions_values=partitions_values,
-                        bucketing_info=bucketing_info,
-                        compression=compression,
-                        boto3_session=boto3_session,
-                        catalog_id=catalog_id,
-                        columns_types=columns_types,
-                    )
-                if commit_trans:
-                    lakeformation.commit_transaction(
-                        transaction_id=transaction_id,  # type: ignore[arg-type]
-                        boto3_session=boto3_session,
-                    )
-            except Exception:
-                _logger.debug("Catalog write failed, cleaning up S3 objects (len(paths): %s).", len(paths))
-                delete_objects(
-                    path=paths,
-                    use_threads=use_threads,
-                    boto3_session=boto3_session,
-                    s3_additional_kwargs=s3_additional_kwargs,
-                )
-                raise
-    return {"paths": paths, "partitions_values": partitions_values}
 
 
 @apply_configs
 @_utils.validate_distributed_kwargs(
     unsupported_kwargs=["boto3_session"],
 )
 def store_parquet_metadata(  # pylint: disable=too-many-arguments,too-many-locals
```

### Comparing `awswrangler-3.1.1/awswrangler/s3/_write_text.py` & `awswrangler-3.2.0/awswrangler/s3/_write_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,26 +165,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions")). False by default.
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
@@ -769,26 +769,26 @@
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
     mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
         If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
         (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.1.1/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.2.0/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
     glue_table_settings: dict (GlueTableSettings), optional
         Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
```

### Comparing `awswrangler-3.1.1/awswrangler/secretsmanager.py` & `awswrangler-3.2.0/awswrangler/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/sqlserver.py` & `awswrangler-3.2.0/awswrangler/sqlserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,14 +179,15 @@
     con: "pyodbc.Connection",
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -194,14 +195,15 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_query(
     sql: str,
@@ -209,28 +211,30 @@
     *,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(pyodbc, "pyodbc")
 def read_sql_query(
     sql: str,
     con: "pyodbc.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding to the result set of the query string.
 
     Parameters
     ----------
     sql : str
         SQL query.
@@ -248,14 +252,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -276,28 +286,30 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 @overload
 def read_sql_table(
     table: str,
     con: "pyodbc.Connection",
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: None = ...,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> pd.DataFrame:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -306,14 +318,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: int,
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Iterator[pd.DataFrame]:
     ...
 
 
 @overload
 def read_sql_table(
     table: str,
@@ -322,14 +335,15 @@
     schema: Optional[str] = ...,
     index_col: Optional[Union[str, List[str]]] = ...,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
     chunksize: Optional[int],
     dtype: Optional[Dict[str, pa.DataType]] = ...,
     safe: bool = ...,
     timestamp_as_object: bool = ...,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = ...,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ...
 
 
 @_utils.check_optional_dependency(pyodbc, "pyodbc")
 def read_sql_table(
     table: str,
@@ -337,14 +351,15 @@
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
+    dtype_backend: Literal["numpy_nullable", "pyarrow"] = "numpy_nullable",
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding the table.
 
     Parameters
     ----------
     table : str
         Table name.
@@ -365,14 +380,20 @@
     dtype : Dict[str, pyarrow.DataType], optional
         Specifying the datatype for columns.
         The keys should be the column names and the values should be the PyArrow types.
     safe : bool
         Check for overflows or other unsafe data type conversions.
     timestamp_as_object : bool
         Cast non-nanosecond timestamps (np.datetime64) to objects.
+    dtype_backend: str, optional
+        Which dtype_backend to use, e.g. whether a DataFrame should have NumPy arrays,
+        nullable dtypes are used for all dtypes that have a nullable implementation when
+        “numpy_nullable” is set, pyarrow is used for all dtypes if “pyarrow” is set.
+
+        The dtype_backends are still experimential. The "pyarrow" backend is only supported with Pandas 2.0 or above.
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
@@ -395,14 +416,15 @@
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
+        dtype_backend=dtype_backend,
     )
 
 
 @_utils.check_optional_dependency(pyodbc, "pyodbc")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
```

### Comparing `awswrangler-3.1.1/awswrangler/sts.py` & `awswrangler-3.2.0/awswrangler/sts.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/timestream/__init__.py` & `awswrangler-3.2.0/awswrangler/timestream/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """Amazon Timestream Module."""
 
 
 from awswrangler.timestream._create import create_database, create_table
 from awswrangler.timestream._delete import delete_database, delete_table
 from awswrangler.timestream._list import list_databases, list_tables
-from awswrangler.timestream._read import query
-from awswrangler.timestream._write import batch_load, batch_load_from_files, wait_batch_load_task, write
+from awswrangler.timestream._read import query, unload, unload_to_files
+from awswrangler.timestream._write import (
+    batch_load,
+    batch_load_from_files,
+    wait_batch_load_task,
+    write,
+)
 
 __all__ = [
     "create_database",
     "create_table",
     "delete_database",
     "delete_table",
     "list_databases",
     "list_tables",
     "query",
     "write",
     "batch_load",
     "batch_load_from_files",
     "wait_batch_load_task",
+    "unload_to_files",
+    "unload",
 ]
```

### Comparing `awswrangler-3.1.1/awswrangler/timestream/_create.py` & `awswrangler-3.2.0/awswrangler/timestream/_create.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/timestream/_delete.py` & `awswrangler-3.2.0/awswrangler/timestream/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/timestream/_list.py` & `awswrangler-3.2.0/awswrangler/timestream/_list.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/timestream/_write.py` & `awswrangler-3.2.0/awswrangler/timestream/_write.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.1.1/awswrangler/typing.py` & `awswrangler-3.2.0/awswrangler/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Module with parameter types."""
 
-from typing import Dict, List, Literal, Tuple, TypedDict
+from typing import Dict, List, Literal, NamedTuple, Optional, Tuple, TypedDict
 
 from typing_extensions import NotRequired, Required
 
 BucketingInfoTuple = Tuple[List[str], int]
 
 
 class GlueTableSettings(TypedDict):
@@ -219,7 +219,16 @@
     paths: Required[List[str]]
     """List of all stored files paths on S3."""
     partitions_values: Required[Dict[str, List[str]]]
     """
     Dictionary of partitions added with keys as S3 path locations
     and values as a list of partitions values as str.
     """
+
+
+class _ReadTableMetadataReturnValue(NamedTuple):
+    """Named tuple defining the return value of the ``read_*_metadata`` functions."""
+
+    columns_types: Dict[str, str]
+    """Dictionary containing column names and types."""
+    partitions_types: Optional[Dict[str, str]]
+    """Dictionary containing partition names and types, if partitioned."""
```

### Comparing `awswrangler-3.1.1/pyproject.toml` & `awswrangler-3.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awswrangler"
-version = "3.1.1"
+version = "3.2.0"
 description = "Pandas on AWS."
 authors = ["Amazon Web Services"]
 license = "Apache License 2.0"
 
 readme = "README.md"
 
 include = ["README.md", "LICENSE.txt", "NOTICE.txt", "THIRD_PARTY.txt", "awswrangler/py.typed"]
@@ -81,34 +81,34 @@
 [tool.poetry.dev-dependencies]
 # Build
 setuptools = "*"
 wheel = "^0.38.1"
 
 # Lint
 black = "^23.1.0"
-boto3-stubs = {version = "1.26.47", extras = ["athena", "chime", "cloudwatch", "dynamodb", "ec2", "emr", "glue", "kms", "lakeformation", "logs", "neptune", "opensearch", "opensearchserverless", "quicksight", "rds", "rds-data", "redshift", "redshift-data", "s3", "secretsmanager", "ssm", "sts", "timestream-query", "timestream-write"]}
+boto3-stubs = {version = "1.26.151", extras = ["athena", "chime", "cloudwatch", "dynamodb", "ec2", "emr", "emr-serverless", "glue", "kms", "lakeformation", "logs", "neptune", "opensearch", "opensearchserverless", "quicksight", "rds", "rds-data", "redshift", "redshift-data", "s3", "secretsmanager", "ssm", "sts", "timestream-query", "timestream-write"]}
 doc8 = "^1.0"
 mypy = "^1.0"
 pylint = "^2.17"
-ruff = "^0.0.240"
+ruff = "^0.0.270"
 isort = "^5.9.2"
 flake8 = "^5.0.1"
 pydocstyle = "^6.1.1"
 
 # Test
 moto = "^4.1"
 openpyxl = "^3.0"
 pyparsing = "^3.0.7"
 pytest = "^7.1.2"
 pytest-cov = "^4.0"
 pytest-rerunfailures = "^11.1"
 pytest-timeout = "^2.1.0"
 pytest-xdist = "^3.0.2"
 s3fs = "0.4.2"  # Must be pinned to 0.4.2
-tox = "^4.5.0"
+tox = "^4.6.0"
 
 # Docs
 bump2version = "^1.0.1"
 IPython = "^8.10.0"
 jupyterlab = "^3.0"
 nbsphinx = "^0.8.8"
 nbsphinx-link = "^1.3.0"
@@ -142,15 +142,15 @@
   | dev
   | .coverage
 )/
 '''
 
 [tool.ruff]
 select = ["D", "E", "F", "I001", "I002", "PL", "W"]
-ignore = ["E501", "PLR2004", "PLR0913", "PLR0915"]
+ignore = ["E501", "PLR2004", "PLR0911", "PLR0912", "PLR0913", "PLR0915"]
 fixable = ["I001"]
 exclude = [
     ".eggs",
     ".git",
     ".mypy_cache",
     ".ruff_cache",
     ".tox",
```

### Comparing `awswrangler-3.1.1/PKG-INFO` & `awswrangler-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awswrangler
-Version: 3.1.1
+Version: 3.2.0
 Summary: Pandas on AWS.
 Home-page: https://aws-sdk-pandas.readthedocs.io/
 License: Apache-2.0
 Keywords: pandas,aws
 Author: Amazon Web Services
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -67,15 +67,15 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/3.1.1-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/3.2.0-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
@@ -155,33 +155,33 @@
 """)
 
 ```
 
 ## At scale
 AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
 
-The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
+The quickest way to get started is to use AWS Glue with Ray. Read our [docs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html), our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/), or head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials) to discover even more features.
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/about.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/install.html#from-source)
-- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html)
-  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#getting-started)
-  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#supported-apis)
-  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/scale.html#resources)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/about.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/install.html#from-source)
+- [**At scale**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html)
+  - [Getting Started](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#getting-started)
+  - [Supported APIs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#supported-apis)
+  - [Resources](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/scale.html#resources)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -214,39 +214,39 @@
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
   - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
   - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
   - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
   - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
   - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
   - [039 - Athena Iceberg](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/039%20-%20Athena%20Iceberg.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#opensearch)
-  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-glue-data-quality)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#global-configurations)
-  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.1.1/api.html#distributed-ray)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#opensearch)
+  - [AWS Glue Data Quality](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-glue-data-quality)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#global-configurations)
+  - [Distributed - Ray](https://aws-sdk-pandas.readthedocs.io/en/3.2.0/api.html#distributed-ray)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

