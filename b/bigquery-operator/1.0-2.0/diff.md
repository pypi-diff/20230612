# Comparing `tmp/bigquery_operator-1.0-py3-none-any.whl.zip` & `tmp/bigquery_operator-2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6989 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      118 b- defN 22-Sep-15 14:12 bigquery_operator/__init__.py
--rw-rw-r--  2.0 unx    19061 b- defN 22-Sep-15 14:50 bigquery_operator/operator.py
--rw-rw-r--  2.0 unx     1365 b- defN 22-Sep-15 14:12 bigquery_operator/operator_quick_setup.py
--rw-rw-r--  2.0 unx     1074 b- defN 22-Sep-15 14:57 bigquery_operator-1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1647 b- defN 22-Sep-15 14:57 bigquery_operator-1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-15 14:57 bigquery_operator-1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 22-Sep-15 14:57 bigquery_operator-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      696 b- defN 22-Sep-15 14:57 bigquery_operator-1.0.dist-info/RECORD
-8 files, 24071 bytes uncompressed, 5763 bytes compressed:  76.1%
+Zip file size: 7891 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      118 b- defN 23-May-10 08:51 bigquery_operator/__init__.py
+-rw-rw-r--  2.0 unx    23488 b- defN 23-Jun-12 20:18 bigquery_operator/operator.py
+-rw-rw-r--  2.0 unx     1702 b- defN 23-Jun-12 20:18 bigquery_operator/operator_quick_setup.py
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-12 20:48 bigquery_operator-2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1698 b- defN 23-Jun-12 20:48 bigquery_operator-2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-12 20:48 bigquery_operator-2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-12 20:48 bigquery_operator-2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      696 b- defN 23-Jun-12 20:48 bigquery_operator-2.0.dist-info/RECORD
+8 files, 28886 bytes uncompressed, 6665 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: bigquery_operator/operator.py
 Comment: 
 
 Filename: bigquery_operator/operator_quick_setup.py
 Comment: 
 
-Filename: bigquery_operator-1.0.dist-info/LICENSE
+Filename: bigquery_operator-2.0.dist-info/LICENSE
 Comment: 
 
-Filename: bigquery_operator-1.0.dist-info/METADATA
+Filename: bigquery_operator-2.0.dist-info/METADATA
 Comment: 
 
-Filename: bigquery_operator-1.0.dist-info/WHEEL
+Filename: bigquery_operator-2.0.dist-info/WHEEL
 Comment: 
 
-Filename: bigquery_operator-1.0.dist-info/top_level.txt
+Filename: bigquery_operator-2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bigquery_operator-1.0.dist-info/RECORD
+Filename: bigquery_operator-2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bigquery_operator/operator.py

```diff
@@ -1,62 +1,79 @@
-from typing import List, Optional
+import logging
+import time
+from typing import Optional, List, Tuple
 from datetime import datetime, timezone, timedelta
 from google.cloud import bigquery, exceptions
+from google.api_core.exceptions import PreconditionFailed
+logger = logging.getLogger(__name__)
 
 
 class Operator:
     """Wrapper for usual operations on a fixed BigQuery dataset.
 
     Args:
         client (google.cloud.bigquery.client.Client): Client to
             manage connections to the BigQuery API.
         dataset_id (str): The dataset id in the format
             'project_id.dataset_name'.
     """
-
     def __init__(
             self,
             client: bigquery.Client,
             dataset_id: str) -> None:
         self._client = client
         self._dataset_id = dataset_id
-        self._dataset_name = self._dataset_id.split('.')[-1]
+        self._check_dataset_id_format()
+        dataset_id_splitted = self._dataset_id.split('.')
+        self._dataset_project_id = dataset_id_splitted[0]
+        self._dataset_name = dataset_id_splitted[1]
+
+    def _check_dataset_id_format(self) -> None:
+        if self._dataset_id.count('.') != 1:
+            msg = 'dataset_id must contain exactly one dot'
+            raise ValueError(msg)
 
     @property
     def client(self) -> bigquery.Client:
         """google.cloud.bigquery.client.Client: The client."""
         return self._client
 
     @property
-    def project_id(self) -> str:
-        """str: the id of the project which the client acts on behalf of."""
+    def client_project_id(self) -> str:
+        """str: The id of the project which the client acts on behalf of."""
         return self._client.project
 
     @property
     def dataset_id(self) -> str:
         """str: The dataset id in the format 'project_id.dataset_name'."""
         return self._dataset_id
 
     @property
+    def dataset_project_id(self) -> str:
+        """str: The project id of the dataset."""
+        return self._dataset_project_id
+
+    @property
     def dataset_name(self) -> str:
         """str: The dataset name."""
         return self._dataset_name
 
     @staticmethod
     def _wait_for_jobs(jobs: List[bigquery.UnknownJob]) -> None:
         for job in jobs:
             job.result()
 
     @staticmethod
     def sample_query(query: str, size: int) -> str:
         """Sample randomly a query.
 
         The output query gives a subset of the lines given by the input query.
-        This subset has approximately ``size`` lines. Nonetheless, the cost of
-        the output query is the same as the cost of the input query.
+        This subset has approximately ``size`` lines. Nonetheless, the number
+        of gigabytes processed is the same for the output query and the
+        input query.
         """
         return (f'select * from ({query}) '
                 f'where rand() < {size}/(select count(*) from ({query}))')
 
     def instantiate_dataset(self) -> bigquery.Dataset:
         """Instantiate the dataset. No api call is made."""
         return bigquery.Dataset(self._dataset_id)
@@ -76,61 +93,54 @@
     def delete_dataset(self) -> None:
         """Delete the dataset."""
         self._client.delete_dataset(
             self._dataset_id,
             delete_contents=False,
             not_found_ok=False)
 
-    def create_dataset(
-            self,
-            location: Optional[str] = None,
-            default_time_to_live: Optional[int] = None) -> None:
-        """Create the dataset.
-
-        Args:
-            location (str, optional): Location in which the dataset is hosted.
-            default_time_to_live (int, optional): The default time to live
-                in days for the tables created in the dataset.
-        """
+    def create_dataset(self, location: str) -> None:
+        """Create the dataset."""
         dataset = self.instantiate_dataset()
         dataset.location = location
-        if default_time_to_live is not None:
-            default_table_expiration_ms = \
-                default_time_to_live * 24 * 60 * 60 * 1000
-        else:
-            default_table_expiration_ms = None
-        dataset.default_table_expiration_ms = default_table_expiration_ms
         self._client.create_dataset(dataset=dataset, exists_ok=False)
 
+    def create_dataset_if_not_exist(self, location: str) -> None:
+        """Create the dataset if it does not exist. Otherwise, check that
+        the actual location of the existing dataset equals the location
+        specified in the argument."""
+        if self.dataset_exists():
+            assert location == self.get_dataset().location
+        else:
+            self.create_dataset(location)
+
     def list_tables(self) -> List[str]:
         """List the names of the tables in the dataset."""
         tables = list(self._client.list_tables(self._dataset_id))
         table_names = sorted([t.table_id for t in tables])
         return table_names
 
     def clean_dataset(self) -> None:
         """Delete all the tables from the dataset."""
         for table_name in self.list_tables():
             self.delete_table(table_name)
 
-    def build_table_id(
-            self, table_name: str, dataset_id: Optional[str] = None):
+    @staticmethod
+    def _build_table_id(dataset_id: str, table_name: str) -> str:
+        return f'{dataset_id}.{table_name}'
+
+    def build_table_id(self, table_name: str) -> str:
         """Return a table id.
 
         Args:
             table_name (str): A table name.
-            dataset_id (str, optional): A dataset id in the format
-                'project_id.dataset_name'. If not passed, falls back to
-                self.dataset_id.
         Returns:
-            str: A table id in the format 'project_id.dataset_name.table_name'.
+            str: A table id in the format 'dataset_id.table_name' where
+                dataset_id is the argument passed to the __init__ method.
         """
-        if dataset_id is None:
-            dataset_id = self._dataset_id
-        return f'{dataset_id}.{table_name}'
+        return self._build_table_id(self._dataset_id, table_name)
 
     def instantiate_table(self, table_name: str) -> bigquery.Table:
         """Instantiate a table. No api call is made."""
         table_id = self.build_table_id(table_name)
         return bigquery.Table(table_id)
 
     def get_table(self, table_name: str) -> bigquery.Table:
@@ -147,70 +157,138 @@
             return False
 
     def delete_table(self, table_name: str) -> None:
         """Delete a table."""
         table_id = self.build_table_id(table_name)
         self._client.delete_table(table_id, not_found_ok=False)
 
+    def delete_table_if_exists(self, table_name: str) -> None:
+        """Delete a table if it exists."""
+        if self.table_exists(table_name):
+            self.delete_table(table_name)
+
+    def delete_table_if_mismatches(
+            self, reference: str, table_name: str) -> None:
+        """Delete a table if the format attributes of the table and the
+        reference table are not the same. The format attributes are given
+        by the method get_format_attributes."""
+        if self.table_exists(reference) and self.table_exists(table_name):
+            reference_format = self.get_format_attributes(reference)
+            table_format = self.get_format_attributes(table_name)
+            if reference_format != table_format:
+                self.delete_table(table_name)
+
     def create_empty_table(
             self,
             table_name: str,
+            pre_delete_if_exists: Optional[bool] = False,
+            time_to_live: Optional[int] = None,
             schema: Optional[List[bigquery.SchemaField]] = None,
             time_partitioning: Optional[bigquery.TimePartitioning] = None,
             range_partitioning: Optional[bigquery.RangePartitioning] = None,
             require_partition_filter: Optional[bool] = None,
             clustering_fields: Optional[List[str]] = None) -> None:
-        """Create a empty table. Only specify at
-        most one of time_partitioning or range_partitioning.
+        """Create a empty table. Only specify at most one of
+        time_partitioning or range_partitioning.
         """
+        if pre_delete_if_exists:
+            self.delete_table_if_exists(table_name)
         table = self.instantiate_table(table_name)
         table.schema = schema
         table.time_partitioning = time_partitioning
         table.range_partitioning = range_partitioning
         table.require_partition_filter = require_partition_filter
         table.clustering_fields = clustering_fields
         self._client.create_table(table, exists_ok=False)
+        if time_to_live is not None:
+            self.set_time_to_live(table_name, time_to_live)
 
     def table_is_empty(self, table_name: str) -> bool:
         """Return True if the table is empty."""
-        num_rows = self.get_table(table_name).num_rows
-        return num_rows == 0
+        return self.get_table(table_name).num_rows == 0
 
     def get_columns(self, table_name: str) -> List[str]:
         """Return the column names of a table."""
         schema = self.get_table(table_name).schema
         return [f.name for f in schema]
 
+    def get_table_rows(self, table_name: str) -> List[bigquery.Row]:
+        """Return the rows of a table."""
+        table_id = self.build_table_id(table_name)
+        res = list(self._client.list_rows(table_id))
+        return res
+
+    def get_query_rows(self, query: str) -> List[bigquery.Row]:
+        """Return the rows of a query."""
+        res = list(self._client.query(query).result())
+        return res
+
     def get_format_attributes(self, table_name):
         """Return the following table attributes:
         schema, time_partitioning, range_partitioning,
         require_partition_filter, clustering_fields.
         """
         res = dict()
         for a in ['schema', 'time_partitioning', 'range_partitioning',
                   'require_partition_filter', 'clustering_fields']:
             res[a] = getattr(self.get_table(table_name), a)
         return res
 
-    def set_time_to_live(self, table_name: str, nb_days: int) -> None:
-        """Set the time to live of a table in days."""
-        expiration_time = (datetime.now(timezone.utc) +
-                           timedelta(days=nb_days))
+    def set_time_to_live(
+            self,
+            table_name: str,
+            nb_days: int,
+            retry_delays: Tuple[int, ...] = (10, 30)) -> None:
+        """Set the time to live of a table in days. More precisely the
+        expires attribute of the table is set to UTC midnight between
+        (today + nb_days) and (today + nb_days + 1), if it has not already
+        this value.
+
+        We have noticed that some
+        unexpected google.api_core.exceptions.PreconditionFailed can
+        happen. That is why we try to update the table several times. If this
+        exception is raised, we try again after a delay. The retry delays
+        are specified in seconds in the argument retry_delays.
+        """
+        expiration_date = (
+                datetime.now(timezone.utc) +
+                timedelta(days=nb_days + 1)).date()
+        expiration_time = datetime.combine(
+            expiration_date, datetime.min.time(), tzinfo=timezone.utc)
+        for duration in retry_delays:
+            table = self.get_table(table_name)
+            if expiration_time == table.expires:
+                return
+            table.expires = expiration_time
+            try:
+                self._client.update_table(table, ['expires'])
+            except PreconditionFailed as e:
+                logger.warning(e)
+                logger.warning(f'sleeping {duration} seconds before next try')
+                time.sleep(duration)
         table = self.get_table(table_name)
+        if expiration_time == table.expires:
+            return
         table.expires = expiration_time
         self._client.update_table(table, ['expires'])
 
     def create_view(
             self,
             query: str,
-            destination_table_name: str) -> None:
+            destination_table_name: str,
+            pre_delete_if_exists: Optional[bool] = False,
+            time_to_live: Optional[int] = None) -> None:
         """Create a view."""
+        if pre_delete_if_exists:
+            self.delete_table_if_exists(destination_table_name)
         view = self.instantiate_table(destination_table_name)
         view.view_query = query
         self._client.create_table(view, exists_ok=False)
+        if time_to_live is not None:
+            self.set_time_to_live(destination_table_name, time_to_live)
 
     def _query_job(
             self,
             query: str,
             destination_table_name: str,
             write_disposition: bigquery.WriteDisposition
     ) -> bigquery.QueryJob:
@@ -220,25 +298,24 @@
         job = self._client.query(query=query, job_config=job_config)
         return job
 
     def _extract_job(
             self,
             source_table_name: str,
             destination_uri: str,
+            compression: bigquery.Compression,
             field_delimiter: str,
             print_header: bool
     ) -> bigquery.ExtractJob:
-        if not destination_uri.endswith('.csv.gz'):
-            raise ValueError("destination_uri must end with '.csv.gz'")
         source = self.build_table_id(source_table_name)
         job_config = bigquery.ExtractJobConfig()
+        job_config.destination_format = 'CSV'
+        job_config.compression = compression
         job_config.field_delimiter = field_delimiter
         job_config.print_header = print_header
-        job_config.destination_format = 'CSV'
-        job_config.compression = 'GZIP'
         job = self._client.extract_table(
             source=source,
             destination_uris=destination_uri,
             job_config=job_config)
         return job
 
     def _load_job(
@@ -268,16 +345,16 @@
     def _copy_job(
             self,
             source_table_name: str,
             destination_table_name: str,
             source_dataset_id: str,
             write_disposition: bigquery.WriteDisposition
     ) -> bigquery.CopyJob:
-        source_table_id = self.build_table_id(
-            source_table_name, dataset_id=source_dataset_id)
+        source_table_id = self._build_table_id(
+            source_dataset_id, source_table_name)
         destination_table_id = self.build_table_id(
             destination_table_name)
         job_config = bigquery.CopyJobConfig()
         job_config.write_disposition = write_disposition
         job = self._client.copy_table(
             sources=source_table_id,
             destination=destination_table_id,
@@ -300,25 +377,27 @@
         return [self._query_job(q, d, write_disposition)
                 for q, d in zip(queries, destination_table_names)]
 
     def _extract_jobs(
             self,
             source_table_names: List[str],
             destination_uris: List[str],
+            compression: bigquery.Compression,
             field_delimiter: str,
             print_header: bool
     ) -> List[bigquery.ExtractJob]:
         len_source_table_names = len(source_table_names)
         len_destination_uris = len(destination_uris)
         if len_source_table_names == 0:
             raise ValueError('source_table_names must not be empty')
         if len_source_table_names != len_destination_uris:
             raise ValueError('source_table_names and destination_uris '
                              'must have the same length')
-        return [self._extract_job(s, d, field_delimiter, print_header)
+        return [self._extract_job(
+            s, d, compression, field_delimiter, print_header)
                 for s, d in zip(source_table_names, destination_uris)]
 
     def _load_jobs(
             self,
             source_uris: List[str],
             destination_table_names: List[str],
             schemas: List[List[bigquery.SchemaField]],
@@ -355,127 +434,148 @@
             self._copy_job(s, d, source_dataset_id, write_disposition)
             for s, d in zip(source_table_names, destination_table_names)]
 
     def run_queries(
             self,
             queries: List[str],
             destination_table_names: List[str],
+            sample_size: Optional[int] = None,
+            time_to_live: Optional[int] = None,
             write_disposition: Optional[bigquery.WriteDisposition] =
             bigquery.WriteDisposition.WRITE_TRUNCATE) -> dict:
         """Run queries. Return monitoring as a dict in the format
-        {'duration': d, 'cost': c} where d is the execution duration in
-        seconds and c the execution cost in dollars.
+        {'duration': d, 'GB': gb} where d is the execution duration in
+        seconds and gb the number of gigabytes processed by the queries.
         """
+        if sample_size is not None:
+            queries = [self.sample_query(q, sample_size) for q in queries]
         start_timestamp = datetime.now(timezone.utc)
         jobs = self._query_jobs(
             queries, destination_table_names, write_disposition)
         self._wait_for_jobs(jobs)
         end_timestamp = datetime.now(timezone.utc)
         duration = round((end_timestamp - start_timestamp).total_seconds())
-        total_bytes_billed_list = [j.total_bytes_billed for j in jobs]
-        costs = [round(tbb / 10 ** 12 * 5, 5)
-                 for tbb in total_bytes_billed_list]
-        cost = sum(costs)
-        monitoring = {'duration': duration, 'cost': cost}
+        total_bytes_processed_list = [
+                j.total_bytes_processed for j in jobs]
+        gb_processed_list = [
+            round(tbb / 10 ** 9, 2) for tbb in total_bytes_processed_list]
+        gb_processed = sum(gb_processed_list)
+        monitoring = {'duration': duration, 'GB': gb_processed}
+        if time_to_live is not None:
+            for n in destination_table_names:
+                self.set_time_to_live(n, time_to_live)
         return monitoring
 
     def extract_tables(
             self,
             source_table_names: List[str],
             destination_uris: List[str],
+            compression: Optional[bigquery.Compression] = None,
             field_delimiter: Optional[str] = '|',
             print_header: Optional[bool] = True) -> None:
         """Extract tables from BigQuery to Storage. Each source table is
-        extracted as one or more compressed gzip csv files. Each destination
-        uri must end with '.csv.gz'.
+        extracted as one or more CSV files.
         """
         self._wait_for_jobs(self._extract_jobs(
             source_table_names,
             destination_uris,
+            compression,
             field_delimiter,
             print_header))
 
     def load_tables(
             self,
             source_uris: List[str],
             destination_table_names: List[str],
+            time_to_live: Optional[int] = None,
             schemas: Optional[List[List[bigquery.SchemaField]]] = None,
             field_delimiter: Optional[str] = '|',
             write_disposition: Optional[bigquery.WriteDisposition] =
             bigquery.WriteDisposition.WRITE_TRUNCATE) -> None:
         """Load Storage CSV files into BigQuery tables."""
         if schemas is None:
             schemas = [None]*len(source_uris)
         self._wait_for_jobs(self._load_jobs(
             source_uris, destination_table_names, schemas,
             field_delimiter, write_disposition))
+        if time_to_live is not None:
+            for n in destination_table_names:
+                self.set_time_to_live(n, time_to_live)
 
     def copy_tables(
             self,
             source_table_names: List[str],
             destination_table_names: List[str],
+            time_to_live: Optional[int] = None,
             source_dataset_id: Optional[str] = None,
             write_disposition: Optional[bigquery.WriteDisposition] =
             bigquery.WriteDisposition.WRITE_TRUNCATE) -> None:
         """Copy tables. ``source_dataset_id`` must be given in the format
         'project_id.dataset_name'. If not passed, falls back to
         self.dataset_id.
         """
         if source_dataset_id is None:
             source_dataset_id = self._dataset_id
         self._wait_for_jobs(self._copy_jobs(
             source_table_names, destination_table_names,
             source_dataset_id, write_disposition))
+        if time_to_live is not None:
+            for n in destination_table_names:
+                self.set_time_to_live(n, time_to_live)
 
     def run_query(
             self,
             query: str,
             destination_table_name: str,
+            sample_size: Optional[int] = None,
+            time_to_live: Optional[int] = None,
             write_disposition: Optional[bigquery.WriteDisposition] =
             bigquery.WriteDisposition.WRITE_TRUNCATE) -> dict:
         """Run a query. Return monitoring as a dict in the format
-        {'duration': d, 'cost': c} where d is the execution duration in
-        seconds and c the execution cost in dollars.
+        {'duration': d, 'GB': gb} where d is the execution duration in
+        seconds and gb the number of gigabytes processed by the query.
         """
         return self.run_queries(
-            [query], [destination_table_name], write_disposition)
+            [query], [destination_table_name],
+            sample_size, time_to_live, write_disposition)
 
     def extract_table(
             self,
             source_table_name: str,
             destination_uri: str,
+            compression: Optional[str] = None,
             field_delimiter: Optional[str] = '|',
             print_header: Optional[bool] = True) -> None:
-        """Extract a table. Data is extracted as a gzip compressed csv.
-        ``destination_uri`` must end with '.csv.gz'
-        """
+        """Extract a table."""
         self.extract_tables(
             [source_table_name], [destination_uri],
-            field_delimiter, print_header)
+            compression, field_delimiter, print_header)
 
     def load_table(
             self,
             source_uri: str,
             destination_table_name: str,
+            time_to_live: Optional[int] = None,
             schema: Optional[List[bigquery.SchemaField]] = None,
             field_delimiter: Optional[str] = '|',
             write_disposition: Optional[bigquery.WriteDisposition] =
             bigquery.WriteDisposition.WRITE_TRUNCATE) -> None:
         """Load one or more Storage CSV files into one BigQuery table."""
         self.load_tables(
-            [source_uri], [destination_table_name], [schema],
-            field_delimiter, write_disposition)
+            [source_uri], [destination_table_name], time_to_live,
+            [schema], field_delimiter, write_disposition)
 
     def copy_table(
             self,
             source_table_name: str,
             destination_table_name: str,
+            time_to_live: Optional[int] = None,
             source_dataset_id: Optional[str] = None,
             write_disposition: Optional[bigquery.WriteDisposition] =
             bigquery.WriteDisposition.WRITE_TRUNCATE) -> None:
         """Copy a table. ``source_dataset_id`` must be given in the format
         'project_id.dataset_name'. If not passed, falls back to
         self.dataset_id.
         """
         self.copy_tables(
-            [source_table_name], [destination_table_name],
+            [source_table_name], [destination_table_name], time_to_live,
             source_dataset_id, write_disposition)
```

## bigquery_operator/operator_quick_setup.py

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 from google.auth import credentials as cred
 from google.cloud import bigquery
-from bigquery_operator.operator import Operator
+from bigquery_operator import operator
 
 
-class OperatorQuickSetup(Operator):
+class OperatorQuickSetup(operator.Operator):
     """The purpose of this class is to quickly set up an Operator.
 
     An instance of OperatorQuickSetup is simply an instance of the base class
     built with the following arguments:
 
     ::
 
@@ -21,16 +21,16 @@
 
         client = google.cloud.bigquery.Client(
             project=project_id,
             credentials=credentials)
         dataset_id = project_id + '.' + dataset_name
 
     Args:
-        project_id (str, optional): The project id.
-        dataset_name (str, optional): The dataset name.
+        project_id (str): The project id.
+        dataset_name (str): The dataset name.
         credentials (google.auth.credentials.Credentials): Credentials used to
             build the client. If not passed, falls back to the default inferred
             from the environment.
     """
     def __init__(
             self,
             project_id: str,
@@ -38,7 +38,17 @@
             credentials: Optional[cred.Credentials] = None) -> None:
         self._project_id = project_id
         client = bigquery.Client(
             project=self._project_id,
             credentials=credentials)
         dataset_id = f'{self._project_id}.{dataset_name}'
         super().__init__(client, dataset_id)
+
+    @property
+    def project_id(self) -> str:
+        """str: The project_id in the argument.
+
+        By construction, it is the common project_id of the client and
+        the dataset. For an instance of the base class, the project_id of the
+        client and the project_id of the dataset may be different.
+        """
+        return self._project_id
```

## Comparing `bigquery_operator-1.0.dist-info/LICENSE` & `bigquery_operator-2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bigquery_operator-1.0.dist-info/METADATA` & `bigquery_operator-2.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: bigquery-operator
-Version: 1.0
+Version: 2.0
 Summary: Wrapper for usual operations on a fixed BigQuery dataset.
 Home-page: UNKNOWN
 Author: Augustin Barillec
 Author-email: augustin.barillec@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://bigquery-operator.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/augustin-barillec/bigquery-operator
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 Requires-Dist: google-cloud-bigquery (==3.*)
 
 bigquery-operator
 =================
```

