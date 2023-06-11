# Comparing `tmp/aws_hexagonal_adapters-1.0.1.tar.gz` & `tmp/aws_hexagonal_adapters-1.1.0.tar.gz`

## Comparing `aws_hexagonal_adapters-1.0.1.tar` & `aws_hexagonal_adapters-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,53 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.DS_Store
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/ruff.toml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/168cc38b04774c1d
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/618c6b6cc269398a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/75d3689fa3a76235
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/7c78c5206be80766
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/81d6bea09b3bfddc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/8f6d8158c77dd870
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/a41f533a26961e6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/a5ccc3b3108d4277
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c285b1f3993c3cc4
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c5082269dd966539
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c521446dd63755a4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/c82b673ec67750f8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/df318c36e6722395
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/fc051c84047f8578
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.ruff_cache/content/fff176ebb881786c
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/dynamo_db_service.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/event_bridge_service.py
--rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/s3_service.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ses_service.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/sqs_service.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ssm_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/nonexistent.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/test.txt
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/test_s3_service.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/LICENSE
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/README.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.DS_Store
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/ruff.toml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/168cc38b04774c1d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/1de8c6b619a63759
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/2c02fc70f6042b65
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/4648c93e9f05b58c
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/618c6b6cc269398a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/70b9b88ff97b0a54
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/75d3689fa3a76235
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/7c78c5206be80766
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/81d6bea09b3bfddc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/8f6d8158c77dd870
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/a41f533a26961e6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/a5ccc3b3108d4277
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/bf61e89bcc6acc26
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/c285b1f3993c3cc4
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/c5082269dd966539
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/c521446dd63755a4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/c82b673ec67750f8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/cfea03011d982be
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/df318c36e6722395
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/e98797e752907b49
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/fc051c84047f8578
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.ruff_cache/content/fff176ebb881786c
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/dynamo_db_service.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/event_bridge_service.py
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/s3_service.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/ses_service.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/sqs_service.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/ssm_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/nonexistent.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/test.txt
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/test_s3_service.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/README.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.1.0/PKG-INFO
```

### Comparing `aws_hexagonal_adapters-1.0.1/.DS_Store` & `aws_hexagonal_adapters-1.1.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/.ruff_cache/content/618c6b6cc269398a` & `aws_hexagonal_adapters-1.1.0/.ruff_cache/content/618c6b6cc269398a`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/dynamo_db_service.py` & `aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/dynamo_db_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,123 +1,163 @@
 # -*- coding: utf-8 -*-
 """Abstraction layer on top of AWS Event Bridge."""
 import os
 import boto3
-
-# noinspection PyPackageRequirements
+from botocore.config import Config
+from boto3.dynamodb.transform import TransformationInjector
+from boto3.dynamodb.types import TypeDeserializer
 from aws_lambda_powertools import Logger
 from botocore.exceptions import ClientError
 
 LOGGER = Logger(sampling_rate=float(os.environ["LOG_SAMPLING_RATE"]), level=os.environ["LOG_LEVEL"])
 
 
 class DynamoDBService:
     """Interact with DynamoDB using the AWS boto3 library."""
 
     def __init__(self, region_name="eu-west-1"):
-        """Initialize region in which operations will be performed.
+        """Initialize a region in which operations will be performed.
 
-        :param region_name: default eu-west-1
+        :param region_name: Default eu-west-1
         """
-        self.__client = boto3.resource(
+        config = Config(retries=dict(max_attempts=10))
+        self.__resource = boto3.resource(
             "dynamodb",
             region_name=region_name,
+            config=config,
             endpoint_url=f"https://dynamodb.{region_name}.amazonaws.com/",
         )
+        self.__client = boto3.client("dynamodb", region_name=region_name, config=config)
+
+        self.__transformation = TransformationInjector(deserializer=TypeDeserializer())
+
+    def scan_items(self, table_name: str, index_name: str = None):
+        """Get all items form table using client boto3 module.
+
+        :param table_name: The name of a DynamoDB table
+        :param index_name: The name of a DynamoDB index
+        :return:
+        """
+        paginator = self.__client.get_paginator("scan")
+        operation_parameters = {"TableName": table_name}
+
+        if index_name:
+            operation_parameters["IndexName"] = index_name
+
+        page_iterator = paginator.paginate(**operation_parameters)
+        service_model = self.__client._service_model.operation_model("Scan")
+        try:
+            for page in page_iterator:
+                self.__transformation.inject_attribute_value_output(page, service_model)
+                status_code = page.get("ResponseMetadata").get("HTTPStatusCode")
+                if status_code == 200:
+                    return page["Items"]
+        except ClientError as error:
+            LOGGER.error("Failed to put item into %s table due to %s", table_name, repr(error))
+            raise
 
     def put_item(self, table_name, item):
         """Save dict item to DynamoDB.
 
-        :param table_name: name of the table
-        :param item: dict with key/value pairs
+        :param table_name: Name of the table
+        :param item: Dictionary with key/value pairs
         :return: item saved to DynamoDB
         """
-        table = self.__client.Table(table_name)
+        table = self.__resource.Table(table_name)
+
         try:
             item = table.put_item(Item=item)
             LOGGER.info(f"Put item into {table_name} table")
             return item
         except ClientError as error:
             LOGGER.error(f"Failed to put item into {table_name} table due to {error}")
             raise
 
     def batch_put_items(self, table_name, items):
         """Save multiple items into DynamoDB table.
 
-        :param table_name: name of the table
-        :param items: list of dictionaries with key/value pairs
+        :param table_name: Name of the table
+        :param items: A list of dictionaries with key/value pairs
         :return:
         """
-        table = self.__client.Table(table_name)
+        table = self.__resource.Table(table_name)
+
         try:
             with table.batch_writer() as batch:
                 for item in items:
                     batch.put_item(Item=item)
             LOGGER.info(f"Put {len(items)} items into {table_name} table")
         except ClientError as error:
             LOGGER.error(f"Failed to batch put for {table_name} table due to {error}")
             raise
 
     def delete_item(self, table_name, item):
         """Delete an item from a table.
 
-        :param table_name: name of the table
-        :param item: dict with key/value pairs
+        :param table_name: Name of the table
+        :param item: Dictionary with key/value pairs
         :return: item deleted from the table
         """
-        table = self.__client.Table(table_name)
+        table = self.__resource.Table(table_name)
+
         try:
             item = table.delete_item(Key=item)
             LOGGER.info(f"Delete item in {table_name} table")
             return item
         except ClientError as error:
             LOGGER.error(f"Failed to delete item from {table_name} table due to {error}")
             raise
 
     def get_item(self, table_name, key):
         """Get item from the DynamoDB table.
 
-        :param table_name: name of the table
+        :param table_name: Name of the table
         :param key: hash key
         :return: item obtained from the table
         """
-        table = self.__client.Table(table_name)
+        table = self.__resource.Table(table_name)
+
         try:
             response = table.get_item(Key=key)
             LOGGER.info(f"Got item from {table_name} table")
             return response.get("Item")
         except ClientError as error:
             LOGGER.error(f"Failed to get item from {table_name} table due to {error}")
             raise
 
-    def update_item(self, table_name, key, expression, values):
-        """Update existing item or add new one if entry don't exist.
+    def update_item(self, table_name, key, expression=None, values="", condition=""):
+        """Update existing item or add new one if don't exist.
 
+        :param condition:
         :param table_name: name of the table
         :param key: hash key which will be updated or added if not exists
         :param expression: dynamodb expression used to update item in the table
         :param values: expression attribute values
         :return: NotImplemented
         """
-        table = self.__client.Table(table_name)
-        try:
-            table.update_item(Key=key, UpdateExpression=expression, ExpressionAttributeValues=values)
-            LOGGER.info(f"Updated item in {table_name} table")
+        if expression is None:
+            expression = {}
+        table = self.__resource.Table(table_name)
+        try:
+            table.update_item(
+                Key=key, UpdateExpression=expression, ExpressionAttributeValues=values, ConditionExpression=condition
+            )
+            LOGGER.info("Updated item in %s table", table_name)
         except ClientError as error:
-            LOGGER.error(f"Failed to update item in {table_name} table due to {error}")
+            LOGGER.error("Failed to update item in %s table due to %s", table_name, repr(error))
             raise
 
     def get_items(self, table_name, filter_expression=None):
         """Get multiple items from table.
 
-        :param table_name: name of the table
+        :param table_name: Name of the table
         :param filter_expression: dynamodb expression used to narrow returned results
         :return: dict with items
         """
-        table = self.__client.Table(table_name)
+        table = self.__resource.Table(table_name)
 
         try:
             if filter_expression:
                 response = table.scan(FilterExpression=filter_expression)
             else:
                 response = table.scan()
             data = response["Items"]
@@ -132,21 +172,21 @@
         except ClientError as error:
             LOGGER.error(f"Failed to scan items from {table_name} table due to {error}")
             raise
 
     def get_items_page(self, table_name, filter_expression, last_evaluated_key=None, limit=500):
         """Get all elements from table limited to default 500 items per page.
 
-        :param table_name: name of the table
+        :param table_name: The Name of the table
         :param filter_expression: dynamodb expression used to get items in the table
         :param last_evaluated_key: the last key to start pagination from
         :param limit: default 500 items will be returned in one pagination page
         :return: list of dictionaries
         """
-        table = self.__client.Table(table_name)
+        table = self.__resource.Table(table_name)
         try:
             if last_evaluated_key is None:
                 response = table.scan(FilterExpression=filter_expression, Limit=limit)
             else:
                 response = table.scan(
                     ExclusiveStartKey=last_evaluated_key,
                     FilterExpression=filter_expression,
@@ -157,25 +197,24 @@
         except ClientError as error:
             LOGGER.error(f"Failed to scan items from {table_name} table due to {error}")
             raise
 
     def query(self, table_name, **kwargs):
         """Query DynamoDB table using key/value pairs.
 
-        :param table_name: name of the table
-        :param kwargs: dict of key/value pairs
-        :return: list of dictionaries
+        :param table_name: Name of the table
+        :param kwargs: Dictionary of key/value pairs
+        :return: A list of dictionaries
         """
-        table = self.__client.Table(table_name)
-
+        table = self.__resource.Table(table_name)
         try:
             response = table.query(**kwargs)
             data = response["Items"]
             while "LastEvaluatedKey" in response:
                 kwargs["ExclusiveStartKey"] = response["LastEvaluatedKey"]
                 response = table.query(**kwargs)
                 data.extend(response["Items"])
-            LOGGER.info(f"Got {len(data)} items from {table_name} table")
+            LOGGER.info("Got %s items from %s table", len(data), table_name)
             return data
         except ClientError as error:
-            LOGGER.error(f"Failed to query items from {table_name} table due to {error}")
+            LOGGER.error("Failed to query items from %s table due to %s", table_name, repr(error))
             raise
```

### Comparing `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/event_bridge_service.py` & `aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/event_bridge_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/s3_service.py` & `aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/s3_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ses_service.py` & `aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/ses_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/sqs_service.py` & `aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/sqs_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/aws_hexagonal_adapters/ssm_service.py` & `aws_hexagonal_adapters-1.1.0/aws_hexagonal_adapters/ssm_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/tests/test_s3_service.py` & `aws_hexagonal_adapters-1.1.0/tests/test_s3_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/tests/.pytest_cache/v/cache/nodeids` & `aws_hexagonal_adapters-1.1.0/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/LICENSE` & `aws_hexagonal_adapters-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/README.md` & `aws_hexagonal_adapters-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-1.0.1/pyproject.toml` & `aws_hexagonal_adapters-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aws_hexagonal_adapters"
 description = "Adapters following hexagonal architecture to connect various AWS services."
-version = "1.0.1"
+version = "1.1.0"
 authors = [{name = "Tomasz Szuster", email = "tomasz.szuster@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
         "boto3>=1.26.71,<2.0.0",
```

### Comparing `aws_hexagonal_adapters-1.0.1/PKG-INFO` & `aws_hexagonal_adapters-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_hexagonal_adapters
-Version: 1.0.1
+Version: 1.1.0
 Summary: Adapters following hexagonal architecture to connect various AWS services.
 Project-URL: Home, https://github.com/airmonitor/aws-hexagonal-adapters
 Project-URL: Bug_Tracker, https://github.com/airmonitor/aws-hexagonal-adapters/issues
 Author-email: Tomasz Szuster <tomasz.szuster@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Szuster
```

