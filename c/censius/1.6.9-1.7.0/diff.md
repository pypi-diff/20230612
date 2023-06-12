# Comparing `tmp/censius-1.6.9.tar.gz` & `tmp/censius-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censius-1.6.9.tar", last modified: Wed Apr  5 05:53:54 2023, max compression
+gzip compressed data, was "censius-1.7.0.tar", last modified: Mon Jun 12 16:51:54 2023, max compression
```

## Comparing `censius-1.6.9.tar` & `censius-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-05 05:53:54.372840 censius-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-05 05:53:50.000000 censius-1.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-05 05:53:50.000000 censius-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 05:53:54.372840 censius-1.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-05 05:53:50.000000 censius-1.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/src/censius/
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/Explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/ExplanationType.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/Prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-04-05 05:53:50.000000 censius-1.6.9/src/censius/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:53:54.372840 censius-1.6.9/src/censius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 05:53:54.000000 censius-1.6.9/src/censius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.729897 censius-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-12 16:51:54.729897 censius-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-12 16:51:52.000000 censius-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 16:51:52.000000 censius-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:51:54.729897 censius-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-12 16:51:52.000000 censius-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.725897 censius-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.725897 censius-1.7.0/src/censius/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/CensiusParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.729897 censius-1.7.0/src/censius/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/Explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/ExplanationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.729897 censius-1.7.0/src/censius/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/UseCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.725897 censius-1.7.0/src/censius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/top_level.txt
```

### Comparing `censius-1.6.9/PKG-INFO` & `censius-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.6.9
+Version: 1.7.0
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.6.9/setup.py` & `censius-1.7.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="censius",
-    version="1.6.9",
+    version="1.7.0",
     description="API for Censius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["censius/client"],
     package_dir={"": "src"},
-    packages=["censius"],
+    packages=["censius", "censius.nlp", "censius.ml"],
     install_requires=["requests", "jsonschema", "pandas", "numpy"],
     extras_require={"dev": ["pytest>=3.7", "pdoc3==0.9.2"]},
     url="https://github.com/Censius/censius-logs-python-sdk",
     author="Censius",
     author_email="dev@censius.ai",
     keywords=[],
 )
```

### Comparing `censius-1.6.9/src/censius/CensiusClient.py` & `censius-1.7.0/src/censius/ml/CensiusClient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,84 @@
 import json
-import logging
 import os
 
 import numpy as np
 import pandas as pd
 import requests
 from jsonschema import validate
 from jsonschema.exceptions import ValidationError
 
-import censius.utils as utils
-from censius.constants import *
-from censius.schemas import (
+import censius.ml.utils as utils
+from censius.ml.constants import *
+from censius.ml.schemas import (
     batch_log_schema,
     bulk_log_schema,
     explanations_tabular_schema,
     individual_log_schema,
     log_explanations_schema,
     prediction_tabular_schema,
     process_model_schema,
     register_dataset_schema,
-    register_model_schema,
-    register_new_model_version_schema,
-    register_project_schema,
-    revise_model_schema,
+    register_new_model_version_schema_v2,
+    register_model_schema_v2,
     update_actual_schema,
     update_model_iteration_schema,
-    update_model_schema,
 )
-from censius.utils import check_time_format, make_post_request
+from censius.ml.utils import check_time_format, make_post_request
+from censius.CensiusParent import CensiusParent
 
 
-class CensiusClient(object):
-    def __init__(self, api_key, tenant_id):
-        if api_key == None or len(api_key) == 0:
-            raise ValueError("You need to pass an API key")
-        if tenant_id == None or len(tenant_id) == 0:
-            raise ValueError("You need to pass a tenant ID")
-        self.api_key = api_key
-        self.tenantKey = tenant_id
-
-    def register_project(self, *args, **kwargs):
-        try:
-            validate(instance=kwargs, schema=register_project_schema)
-        except ValidationError as e:
-            return e.message
-
-        Icon = None
-        if "icon" in kwargs:
-            Icon = str(kwargs["icon"])
-
-        Type = None
-        if "type" in kwargs:
-            Type = kwargs["type"]
-
-        Key = None
-        if "key" in kwargs:
-            Key = kwargs["key"]
-
-        payload = json.dumps(
-            {
-                k: v
-                for k, v in {
-                    "icon": Icon,
-                    "name": kwargs["name"],
-                    "key": Key,
-                    "type": Type,
-                    "apiKey": self.api_key,
-                    "tenantKey": self.tenantKey,
-                }.items()
-                if v
-            }
-        )
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
-
-        response = requests.request("POST", REGISTER_PROJECT_URL(), headers=headers, data=payload)
-        return self.__return_message(response)
-
+class CensiusClient(CensiusParent):
+    
+    # Will be deprecated soon
     def register_new_model_version(self, *args, **kwargs):
         try:
-            validate(instance=kwargs, schema=register_new_model_version_schema)
+            validate(instance=kwargs, schema=register_new_model_version_schema_v2)
         except ValidationError as e:
             return e.message
 
-        WindowSize = None
-        if "window_size" in kwargs:
-            WindowSize = kwargs["window_size"]
-
-        WindowStartTime = None
-        if "start_time" in kwargs:
-            WindowStartTime = kwargs["start_time"]
+        values = []
+        for i in kwargs["targets"]:
+            temp = {}
+            temp["target"] = i
+            values.append(temp)
 
         payload = json.dumps(
             {
                 k: v
                 for k, v in {
                     "userDefinedModelID": kwargs["model_id"],
                     "version": kwargs["model_version"],
                     "datasetId": kwargs["training_info"]["id"],
                     "targets": kwargs["targets"],
                     "features": kwargs["features"],
-                    "apiKey": self.api_key,
-                    "windowSize": WindowSize,
-                    "window_start_time": WindowStartTime,
-                    "tenantKey": self.tenantKey,
+                    "values": values,
                 }.items()
                 if v
             }
         )
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
 
         response = requests.request(
-            "POST", REGISTER_NEW_MODEL_VERSION(), headers=headers, data=payload
+            "POST",
+            REGISTER_NEW_MODEL_VERSION_V2_URL(self.project_id),
+            headers=headers,
+            data=payload,
         )
-        if "error" in response.json().keys():
-            return self.__return_message(response)
-        else:
-            values = []
-            for i in kwargs["targets"]:
-                temp = {}
-                temp["target"] = i
-                values.append(temp)
-            primary_response = response
-            self.process_model(
-                dataset_id=kwargs["training_info"]["id"],
-                model_id=response.json()["message"]["ID"],
-                project_id=kwargs["project_id"],
-                values=values,
-            )
-            return self.__return_message(primary_response)
+        return self.__return_message(response)
 
     def register_dataset(self, *args, **kwargs):
         try:
             validate(instance=kwargs, schema=register_dataset_schema)
         except ValidationError as e:
             return e.message
 
-        dataset_validation = utils.DataSetValidation()
-
         rawValues = None
         if "raw_values" in kwargs:
             rawValues = str(kwargs["raw_values"])
 
         timestampBase = None
         timestampCol = None
         unixInterval = None
@@ -177,86 +115,43 @@
                 return {"error": "unable to read the csv file"}
         elif file is not None:
             if (file.memory_usage().sum()) // 1000000 > 500:
                 return {"error": "Max allowed file size is 500 MB"}
 
         else:
             return {"error": "Please provide a df object or a file path"}
-        """
-            Standard validation for input dataframe
-            1. Check if input is dataframe
-            2. Check if input is empty
-            3. Check if input dataframe has any empty row in the middle
-        """
-        error_flag, error_message = dataset_validation.check_for_input_dataframe(file)
-        if error_flag:
-            return {"error": error_message}
-        else:
-            file.to_csv(file_name, index=False)
-
-        """
-            Validation for matching provided features and dataframe columns
-            1. Check if provided features are present in the dataframe
-            2. Check if provided features are of type string and alphanumeric
-            3. Check if provided features are of type string
-            4. Identify categorical features columns
-        """
-        provided_columns = [i["name"] for i in kwargs["features"]]
-        dataframe_columns = list(file.columns)
-        missing_columns = dataset_validation.check_provided_column_with_input_columns(
-            provided_columns, dataframe_columns, []
-        )
-        if missing_columns:
-            return {"error": f"Missing columns in the input dataframe: {missing_columns}"}
-
-        # 2. Check if provided features are of type string and alphanumeric
-        error_flag, error_list = dataset_validation.check_for_alphanumeric_features(
-            provided_columns
-        )
-        if error_flag:
-            return {"error": error_list}
 
-        # 3. Check if provided features are of type string
-        error_flag, error_list, cat_map = dataset_validation.fetch_categorical_features(
-            kwargs["features"]
-        )
-        if error_flag:
-            return {"error": error_list}
+        file.to_csv(file_name, index=False)
 
-        # 4. Identify categorical features columns
-        if cat_map:
-            error_flag, error_list = dataset_validation.validate_categorical_feature_from_input(
-                file, cat_map
-            )
-            if error_flag:
-                return {"error": error_list}
-
-        headers = {"Authorization": f"Bearer {self.api_key}"}
+        headers = {"Authorization": f"Token {self.api_key}"}
 
         payload = {
             "name": kwargs["name"],
-            "projectId": kwargs["project_id"],
+            "projectId": self.project_id,
             "version": Version,
             "features": json.dumps(kwargs["features"]),
-            "apiKey": self.api_key,
             "timestampCol": timestampCol,
             "unixInterval": unixInterval,
             "timestampType": timestampType,
             "rawValues": json.dumps(rawValues),
-            "tenantKey": self.tenantKey,
         }
         files = [("File", (file_name, open(os.getcwd() + "/" + file_name, "rb"), "text/csv"))]
 
         response = requests.request(
-            "POST", REGISTER_DATASET_URL(), headers=headers, data=payload, files=files
+            "POST",
+            REGISTER_DATASET_URL(self.project_id),
+            headers=headers,
+            data=payload,
+            files=files,
         )
         os.remove(os.getcwd() + "/" + file_name)
 
-        return self.__return_message(response)
+        return response.json()
 
+    ## Will be deprecated
     def process_model(self, *args, **kwargs):
         try:
             validate(instance=kwargs, schema=process_model_schema)
         except ValidationError as e:
             return e.message
 
         WindowSize = None
@@ -272,122 +167,92 @@
                 k: v
                 for k, v in {
                     "windowSize": WindowSize,
                     "window_start_time": WindowStartTime,
                     "dataset_id": kwargs["dataset_id"],
                     "model_id": kwargs["model_id"],
                     "values": kwargs["values"],
-                    "apiKey": self.api_key,
-                    "project_id": kwargs["project_id"],
+                    "project_id": self.project_id,
                 }.items()
                 if v
             }
         )
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
 
-        response = requests.request("POST", PROCESS_MODEL_URL(), headers=headers, data=payload)
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
+
+        response = requests.request(
+            "POST", PROCESS_MODEL_URL(self.project_id), headers=headers, data=payload
+        )
         return self.__return_message(response)
 
+    # Deprecated, Will be removed down the line
     def register_model(self, *args, **kwargs):
         try:
-            validate(instance=kwargs, schema=register_model_schema)
+            validate(instance=kwargs, schema=register_model_schema_v2)
         except ValidationError as e:
             return e.message
 
         targets = kwargs["targets"]
+        values = []
+        for i in targets:
+            temp = {}
+            temp["target"] = i
+            values.append(temp)
 
         features = kwargs["features"]
 
-        WindowSize = None
-        if "window_size" in kwargs:
-            WindowSize = kwargs["window_size"]
-
-        WindowStartTime = None
-        if "start_time" in kwargs:
-            WindowStartTime = kwargs["start_time"]
-
         payload = json.dumps(
             {
                 k: v
                 for k, v in {
                     "userDefinedModelID": kwargs["model_id"],
                     "version": kwargs["model_version"],
                     "datasetId": kwargs["training_info"]["id"],
                     "name": kwargs["model_name"],
-                    "projectId": kwargs["project_id"],
+                    "projectId": self.project_id,
                     "type": kwargs["model_type"],
                     "targets": targets,
                     "features": features,
-                    "apiKey": self.api_key,
-                    "windowSize": WindowSize,
-                    "window_start_time": WindowStartTime,
-                    "tenantKey": self.tenantKey,
+                    "values": values,
                 }.items()
                 if v
             }
         )
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
-
-        response = requests.request("POST", REGISTER_MODEL_URL(), headers=headers, data=payload)
-        if "error" in response.json().keys():
-            return self.__return_message(response)
-        else:
-            values = []
-            for i in targets:
-                temp = {}
-                temp["target"] = i
-                values.append(temp)
-            primary_response = response
-            self.process_model(
-                dataset_id=kwargs["training_info"]["id"],
-                project_id=kwargs["project_id"],
-                model_id=response.json()["message"]["ID"],
-                values=values,
-            )
-            return self.__return_message(primary_response)
-
-    def update_model(self, *args, **kwargs):
-        """
-        Update the model iteration
-        :param kwargs:
-        :return:
-        """
-        try:
-            validate(instance=kwargs, schema=update_model_schema)
-        except ValidationError as e:
-            validationError = e.schema["errorMessage"] if "errorMessage" in e.schema else e.message
-            return "ValidationError: " + validationError
-
-        # replace the model_id with user_defined_model_id
-        kwargs["user_defined_model_id"] = kwargs["model_id"]
-        del kwargs["model_id"]
-
-        header = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
-        payload = json.dumps(kwargs)
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
 
-        response = make_post_request(
-            UPDATE_MODEL_META,
-            header,
-            payload,
+        response = requests.request(
+            "POST",
+            REGISTER_MODEL_V2_URL(self.project_id),
+            headers=headers,
+            data=payload,
         )
         return self.__return_message(response)
 
     def log(self, *args, **kwargs):
         if len(args) > 0 and str(type(args[0])) == "<class 'list'>":
             return self.__batch_log(args[0])
         else:
             return self.__individual_log(**kwargs)
 
     def bulk_log(self, input, **kwargs):
         # check in input is dataframe or not
-        from collections import defaultdict
 
-        predictions_received, actuals_received, explanations_received = False, False, False
+        predictions_received, actuals_received, explanations_received = (
+            False,
+            False,
+            False,
+        )
         bulk_input_validation = utils.BulkLogsValidation()
-        bulk_input_processing = utils.BulkLogProcessing()
+        bulk_input_processing = utils.BulkLogProcessing(self.project_id)
         # ..> Standard Validation of datatypes and JSON schema
         """
             Standard validation for input dataframe
             1. Check if input is dataframe
             2. Check if input is empty
             3. Check if input dataframe has any empty row in the middle
         """
@@ -406,15 +271,18 @@
         """
             Standard Validation for <prediction_id_column>
             1. Check if <prediction_id_column> is in <input>
             2. Check if <prediction_id_column> is not Null
             3. Check if <prediction_id_column> is unique
         """
 
-        error_flag, error_message = bulk_input_validation.checks_for_prediction_id_column(
+        (
+            error_flag,
+            error_message,
+        ) = bulk_input_validation.checks_for_prediction_id_column(
             kwargs["prediction_id_column"], input
         )
         if error_flag:
             return {"error": True, "message": error_message}
         # if validation sucessful, change prediction_id_column datatype to string
         input[kwargs["prediction_id_column"]] = input[kwargs["prediction_id_column"]].astype(str)
 
@@ -439,15 +307,18 @@
                 Standard Validation for <prediction_column> 
                 1. Check if <prediction_column> is in <input>
                 2. Check if <prediction_column> is not Null
 
                 Note: <prediction_column>  datatype validation happens in the later section 
                 ↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓
             """
-            error_flag, error_message = bulk_input_validation.checks_for_prediction_column(
+            (
+                error_flag,
+                error_message,
+            ) = bulk_input_validation.checks_for_prediction_column(
                 prediction_tabular["prediction_column"], input
             )
             if error_flag:
                 return {"error": True, "message": error_message}
             prediction_column = prediction_tabular["prediction_column"]
             prediction_column_dt = str(input[prediction_column].dtype)
 
@@ -573,22 +444,32 @@
 
         """
             fetching registered dataset datatype from the server
         """
         payload = json.dumps(
             {"modelID": kwargs["model_id"], "modelVersion": kwargs["model_version"]}
         )
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
         try:
             response = requests.request(
-                "POST", BULK_LOG_DATATYPE_VALIDATION_URL, headers=headers, data=payload
+                "POST",
+                BULK_LOG_DATATYPE_VALIDATION_URL(self.project_id),
+                headers=headers,
+                data=payload,
             )
         except:
             return self.__return_message(
-                {"error": True, "message": "ConnectionError: Unable to connect to server."}
+                {
+                    "error": True,
+                    "message": "ConnectionError: Unable to connect to server.",
+                }
             )
 
         if response.status_code == 200:
             registered_dataset_details = json.loads(response.content)
             registered_dataset_to_datatype, registered_model_target = dict(), list()
             registered_dataset_to_datatype = registered_dataset_details["dataset_datatype"]
             registered_model_target_to_datatype = registered_dataset_details[
@@ -724,15 +605,15 @@
                     2. input_map
                     3. headers
                 Headers:
                     1. Authorization (using API Key)
                     2. Content-Type   
             """
             headers = {
-                "Authorization": f"Bearer {self.api_key}",
+                "Authorization": f"Token {self.api_key}",
                 "Content-Type": "application/json",
             }
             model_details = {
                 "modelID": kwargs["model_id"],
                 "modelVersion": kwargs["model_version"],
                 "predicitionsRecvd": predictions_received,
                 "actualsRecvd": actuals_received,
@@ -756,15 +637,15 @@
                 exp_input_map,
                 exp_registered_to_provided,
                 registered_dataset_to_datatype,
                 registered_model_target,
             )
 
             headers = {
-                "Authorization": f"Bearer {self.api_key}",
+                "Authorization": f"Token {self.api_key}",
                 "Content-Type": "application/json",
             }
             model_details = {
                 "modelID": kwargs["model_id"],
                 "modelVersion": kwargs["model_version"],
             }
             processed_input = input.rename(columns=exp_input_map, inplace=False)
@@ -788,23 +669,26 @@
             validationError = e.schema["errorMessage"] if "errorMessage" in e.schema else e.message
             return "ValidationError: " + validationError
 
         # replace the model_id with user_defined_model_id
         kwargs["user_defined_model_id"] = kwargs["model_id"]
         del kwargs["model_id"]
 
-        header = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        header = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
         payload = json.dumps(kwargs)
 
         # check if dataset_start_time is smaller than dataset_end_time
         if kwargs["dataset_start_datetime"] >= kwargs["dataset_end_datetime"]:
             return "ValidationError:  dataset_end_datetime must be greater than dataset_start_datetime"
 
         response = make_post_request(
-            ADD_MODEL_ITERATION,
+            ADD_MODEL_ITERATION(self.project_id),
             header,
             payload,
         )
         return self.__return_message(response)
 
     def __individual_log(self, *args, **kwargs):
         try:
@@ -836,17 +720,25 @@
                     "timestamp": kwargs["timestamp"],
                     "rawValues": raw_values,
                     "actual": actual,
                 }.items()
                 if v
             }
         )
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
 
-        response = requests.request("POST", LOG_URL(), headers=headers, data=payload)
+        response = requests.request(
+            "POST",
+            LOG_URL(self.project_id),
+            headers=headers,
+            data=payload,
+        )
 
         return self.__return_message(response)
 
     def __batch_log(self, *args, **kwargs):
         try:
             validate(instance=args[0], schema=batch_log_schema)
         except ValidationError as e:
@@ -875,36 +767,48 @@
                         "rawValues": raw_values,
                         "actual": actual,
                     }.items()
                     if v
                 }
             )
 
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
 
-        response = requests.request("POST", LOG_URL(), headers=headers, data=json.dumps(payload))
+        response = requests.request(
+            "POST", LOG_URL(self.project_id), headers=headers, data=json.dumps(payload)
+        )
         return self.__return_message(response)
 
     def update_actual(self, *args, **kwargs):
         try:
             validate(instance=kwargs, schema=update_actual_schema)
         except ValidationError as e:
             return e.message
 
         payload = json.dumps(
             {
                 "modelID": kwargs["model_id"],
+                "predictionID": kwargs["prediction_id"],
                 "modelVersion": kwargs["model_version"],
                 "actual": kwargs["actual"],
             }
         )
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
 
         response = requests.request(
-            "POST", UPDATE_ACTUAL_URL(kwargs["prediction_id"]), headers=headers, data=payload
+            "POST",
+            UPDATE_ACTUAL_URL(self.project_id),
+            headers=headers,
+            data=payload,
         )
         return self.__return_message(response)
 
     def log_explanation(self, *args, **kwargs):
         try:
             validate(instance=kwargs, schema=log_explanations_schema)
         except ValidationError as e:
@@ -913,24 +817,30 @@
         payload = json.dumps(
             {
                 k: v
                 for k, v in {
                     "modelID": kwargs["model_id"],
                     "modelVersion": kwargs["model_version"],
                     "log_id": kwargs["prediction_id"],
-                    "apiKey": self.api_key,
                     "explanation_type": kwargs["explanation_type"],
                     "explanation_values": kwargs["explanation_values"],
-                    "tenantKey": self.tenantKey,
                 }.items()
                 if v
             }
         )
-        headers = {"Authorization": "Bearer " + self.api_key, "Content-Type": "application/json"}
-        response = requests.request("POST", LOG_EXPLAINATIONS_URL(), headers=headers, data=payload)
+        headers = {
+            "Authorization": f"Token {self.api_key}",
+            "Content-Type": "application/json",
+        }
+        response = requests.request(
+            "POST",
+            LOG_EXPLAINATIONS_URL(self.project_id),
+            headers=headers,
+            data=payload,
+        )
         return self.__return_message(response)
 
     def __return_message(self, response):
         # if response is dict
         if isinstance(response, dict):
             return response
         try:
```

### Comparing `censius-1.6.9/src/censius/schemas.py` & `censius-1.7.0/src/censius/ml/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from censius import ExplanationType, ModelType, DatasetType, Dataset
-from censius.constants import BASE_MILLISECONDS_2000, CEIL_MILLISECONDS_2100
+from censius.ml import ExplanationType, ModelType, DatasetType, Dataset
+from censius.ml.constants import BASE_MILLISECONDS_2000, CEIL_MILLISECONDS_2100
 
 register_new_model_version_schema = {
     "type": "object",
     "properties": {
         "model_id": {"type": "string"},
         "training_info": {
             "type": "object",
@@ -26,14 +26,33 @@
         },
         "start_time": {"type": "integer"},
     },
     "required": ["training_info", "model_id", "model_version", "targets", "features"],
 }
 
 
+register_new_model_version_schema_v2 = {
+    "type": "object",
+    "properties": {
+        "model_id": {"type": "string"},
+        "training_info": {
+            "type": "object",
+            "properties": {
+                "id": {"type": "integer"},
+                "method": {"type": "string", "enum": [Dataset.ID]},
+            },
+            "required": ["id", "method"],
+        },
+        "model_version": {"type": "string"},
+        "targets": {"type": "array", "items": {"type": "string"}},
+        "features": {"type": "array", "items": {"type": "string"}},
+    },
+    "required": ["training_info", "model_id", "model_version", "targets", "features"],
+}
+
 register_model_schema = {
     "type": "object",
     "properties": {
         "model_id": {"type": "string"},
         "training_info": {
             "type": "object",
             "properties": {
@@ -62,49 +81,83 @@
         "start_time": {"type": "integer"},
     },
     "required": [
         "training_info",
         "model_id",
         "model_version",
         "model_name",
-        "project_id",
         "model_type",
         "targets",
         "features",
     ],
 }
+
+
+register_model_schema_v2 = {
+    "type": "object",
+    "properties": {
+        "model_id": {"type": "string"},
+        "training_info": {
+            "type": "object",
+            "properties": {
+                "id": {"type": "integer"},
+                "method": {"type": "string", "enum": [Dataset.ID]},
+            },
+            "required": ["id", "method"],
+        },
+        "model_name": {"type": "string"},
+        "model_version": {"type": "string"},
+
+        "model_type": {
+            "type": "string",
+            "enum": [ModelType.BINARY_CLASSIFICATION, ModelType.REGRESSION],
+        },
+        "targets": {"type": "array", "items": {"type": "string"}},
+        "features": {"type": "array", "items": {"type": "string"}},
+
+
+    },
+    "required": [
+        "training_info",
+        "model_id",
+        "model_version",
+        "model_name",
+        "model_type",
+        "targets",
+        "features",
+    ],
+}
+
 register_dataset_schema = {
     "type": "object",
     "properties": {
         "name": {"type": "string"},
-        "project_id": {"type": "integer"},
         "features": {
             "type": "array",
             "items": {
                 "type": "object",
                 "properties": {
                     "name": {"type": "string"},
                     "type": {
                         "type": "string",
-                        "enum": [DatasetType.DECIMAL, DatasetType.INT, DatasetType.STRING],
+                        "enum": [DatasetType.DECIMAL, DatasetType.INT],
                     },
                 },
                 "required": ["name", "type"],
             },
         },
         "raw_values": {
             "type": "object",
             "properties": {
                 "name": {"type": "string"},
                 "type": {
                     "type": "string",
                     "enum": [
                         DatasetType.DECIMAL,
                         DatasetType.INT,
-                        DatasetType.STRING,
                         DatasetType.BOOLEAN,
                     ],
                 },
             },
             "required": ["name", "type"],
         },
         "version": {"type": "string"},
@@ -122,30 +175,33 @@
                         DatasetType.ISO,
                     ],
                 },
             },
             "required": ["name", "type"],
         },
     },
-    "required": ["name", "project_id", "features"],
+    "required": ["name", "features"],
 }
 
-
+## Will be deprecated
 process_model_schema = {
     "type": "object",
     "properties": {
         "dataset_id": {"type": "integer"},
         "model_id": {"type": "integer"},
         "values": {
             "type": "array",
             "items": {
                 "type": "object",
-                "properties": {"target": {"type": "string"}, "perdiction": {"type": "string"}},
+                "properties": {
+                    "target": {"type": "string"},
+                    "perdiction": {"type": "string"},
+                },
                 "required": ["target"],
-            }
+            },
         },
         "window_start_time": {"type": "integer"},
         "window_size": {
             "type": "object",
             "properties": {
                 "number": {"type": "integer"},
                 "unit": {"type": "string", "enum": ["day", "week", "hour"]},
@@ -202,15 +258,19 @@
                     "feature": {"type": "string"},
                     "input_column": {"type": "string"},
                 },
                 "required": ["feature", "input_column"],
             },
         },
     },
-    "required": ["prediction_column", "timestamp_column", "prediction_confidence_column"],
+    "required": [
+        "prediction_column",
+        "timestamp_column",
+        "prediction_confidence_column",
+    ],
 }
 
 explanations_tabular_schema = {
     "type": "object",
     "properties": {
         "type": {"type": "string"},
         "explanation_mapper": {
@@ -335,57 +395,14 @@
         "model_version",
         "explanation_type",
         "prediction_id",
         "explanation_values",
     ],
 }
 
-update_model_schema = {
-    "type": "object",
-    "properties": {
-        "model_id": {
-            "type": "string",
-            "errorMessage": "model_id is required, and must be string.",
-        },
-        "model_version": {
-            "type": "string",
-            "errorMessage": "model_version is required, and must be string.",
-        },
-        "update_meta": {
-            "type": "object",
-            # either one of the two is required
-            "anyOf": [
-                {
-                    "required": ["model_name"],
-                    "errorMessage": "Any of model_name, model_id, and model_version is required in `update_meta`",
-                },
-                {
-                    "required": ["model_id"],
-                    "errorMessage": "Any of model_name, model_id, and model_version is required in `update_meta`",
-                },
-                {
-                    "required": ["model_version"],
-                    "errorMessage": "Any of model_name, model_id, and model_version is required in `update_meta`",
-                },
-            ],
-            "properties": {
-                "model_name": {"type": "string"},
-                "model_id": {"type": "string"},
-                "model_version": {"type": "string"},
-            },
-        },
-    },
-    "required": [
-        "model_id",
-        "model_version",
-        "update_meta",
-    ],
-}
-
-
 update_model_iteration_schema = {
     "type": "object",
     "properties": {
         "model_id": {
             "type": "string",
             "errorMessage": "model_id is required, and must be string.",
         },
```

### Comparing `censius-1.6.9/src/censius/utils.py` & `censius-1.7.0/src/censius/ml/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,137 +1,54 @@
 import json
 import random
-import re
 import string
-import threading
 import time
 from multiprocessing.pool import ThreadPool
 from typing import Any, Tuple
-from urllib import request
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 import requests
 
-from censius.constants import *
+from censius.ml.constants import *
 
 
 class DataSetValidation:
     def __init__(self):
         self.datatype_mapper = {
             "int64": "integer",
             "float64": "decimal",
             "object": "text",
         }
+        self.inference_mapper = {"floating": "decimal", "integer": "integer"}
 
     def check_for_input_dataframe(self, input: Any) -> Tuple[bool, str]:
         # if input is not pandas dataframe return error
         if not isinstance(input, pd.DataFrame):
             return True, f" ValidationError: <input> is not a pandas dataframe"
         if input.empty:
             return True, "  ValidationError: <input> dataframe is empty"
         # ..> if dataframe has empty row in middle return error
         # if input.isnull().any().any():
         #     return True, "  ValidationError: <input> dataframe has empty row in middle"
         return False, ""
 
-    def check_for_alphanumeric_features(self, provided_columns: list) -> Tuple[bool, str]:
-        # ..> if dataframe column name should only have alphanumeric characters, or underscore is allowed
-        error_columns = []
-        for column in provided_columns:
-            if re.match(r"^[a-z0-9_]+$", column) is None:
-                error_columns.append(column)
-
-        if len(error_columns) > 0:
-            message = (
-                f"""
-                    ValidationError: Dataset feature, and target variable name are 
-                    only accepted if they satisfy following constraints: 
-                    Lowercase Alphanumeric, and underscore. 
-                    <input> dataframe has columns violating rule : {error_columns}
-                """,
-            )
-            # strip new line and spaces from the message
-            message = " ".join(message[0].split())
-            return (True, message)
-        return False, ""
-
     def check_provided_column_with_input_columns(
         self,
         provided_columns: list,
         input_columns: list,
         missing_columns=[],
     ) -> list:
         for column in provided_columns:
             # check if all the provided column name present in the dataframe or not.
             if column not in input_columns:
                 missing_columns.append(column)
         return missing_columns
 
-    def generate_random_string(self):
-        return "".join(random.choices(string.ascii_uppercase + string.digits, k=10))
-
-    def fetch_categorical_features(self, input: dict) -> Tuple[bool, list, dict]:
-        categorical_features_map = {}
-        error_list = []
-        for column in input:
-            if "categorical" in column and column["categorical"]:
-                if "category_map" not in column:
-                    error_list.append(
-                        f"  ValidationError: <category_map> key not found for <column>='{column['name']}'"
-                    )
-                    break
-                if not isinstance(column["category_map"], dict):
-                    error_list.append(
-                        f"  ValidationError: <category_map> for <column>='{column['name']}' is not a dictionary"
-                    )
-                    break
-                if len(column["category_map"]) == 0:
-                    error_list.append(
-                        f"  ValidationError: <category_map> for <column>='{column['name']}' is empty"
-                    )
-                    break
-                categorical_features_map[column["name"]] = column["category_map"]
-        return len(error_list) > 0, error_list, categorical_features_map
-
-    def validate_categorical_feature_from_input(
-        self, input: pd.DataFrame, categorical_features_map: dict
-    ) -> Tuple[bool, list]:
-        error_list = []
-        for column in categorical_features_map:
-            if column not in input.columns:
-                error_list.append(
-                    f"  ValidationError: <column>='{column}' not found in <input> dataframe"
-                )
-                break
-            if input[column].isnull().any():
-                error_list.append(
-                    f"  ValidationError: <column>='{column}' has null values, <column> must be NOT NULL"
-                )
-                break
-            if len(input[column].unique()) != len(categorical_features_map[column]):
-                len_input_unique_values = len(input[column].unique())
-                len_category_map_unique_values = len(categorical_features_map[column])
-
-                error_list.append(
-                    f"ValidationError: <column>='{column}' has unique values not equal to <category_map> ie: {len_input_unique_values} != {len_category_map_unique_values}"
-                )
-                break
-            if not set(input[column].unique()).issubset(
-                set(categorical_features_map[column].keys())
-            ):
-                input_unique_values = set(input[column].unique())
-                category_map_unique_values = set(categorical_features_map[column].keys())
-                error_list.append(
-                    f"ValidationError: <column>='{column}' has unique values not equal to <category_map> ie: {input_unique_values} != {category_map_unique_values}"
-                )
-                break
-        return len(error_list) > 0, error_list
-
 
 class BulkLogsValidation(DataSetValidation):
     def __init__(self):
         self.datatype_mapper = {
             "int64": "integer",
             "float64": "decimal",
             "object": "text",
@@ -227,15 +144,18 @@
             input - input dataframe
         output:
             error_flag: True - if any validation failed else False
             error_message: error message
         This function will check if the registered datatype with the input dataframe is same or not.
         """
         if prediction_id_column not in input.columns:
-            return True, "  ValidationError: <prediction_id_column> not found in <input> dataframe"
+            return (
+                True,
+                "  ValidationError: <prediction_id_column> not found in <input> dataframe",
+            )
 
         # if prediction_id_column has null return error
         if input[prediction_id_column].isnull().any():
             return (
                 True,
                 "  ValidationError: <prediction_id_column> has null values, <prediction_id_column> must be unique and NOT NULL",
             )
@@ -402,22 +322,21 @@
             if feature_name not in exp_tab_specified_feat:
                 error_columns.append(feature_name)
 
         return error_columns
 
 
 class BulkLogProcessing:
-    def __init__(self):
-        self.bulk_log_post_url = BULK_LOG_URL
-        self.bulk_explain_post_url = BULK_EXPLAINATIONS_URL
+    def __init__(self, project_id):
+        self.bulk_log_post_url = BULK_LOG_URL(project_id)
+        self.bulk_explain_post_url = BULK_EXPLAINATIONS_URL(project_id)
         self.bulk_chunk_size = BULK_CHUNK_SIZE
         self.bulk_log_data_key = "bulk_logs"
         self.bulk_explain_data_key = "bulk_explainations"
         self.insertion_wait_time = 15
-        pass
 
     # generate random 6 digit string for bulk log id
     def _generate_bulk_log_id_(self):
         return "".join(random.choices(string.ascii_uppercase + string.digits, k=10))
 
     def _dataframe_chunks(
         self,
@@ -641,7 +560,11 @@
     except requests.exceptions.RequestException as e:
         return {"message": "RequestError: {}".format(e)}
 
     if response.status_code == 200:
         return response
     else:
         return response
+
+
+# def build_url(project_id, gateway_key, route):
+#     return f"{CENSIUS_ENDPOINT}/api/sdkapi/{project_id}/{gateway_key}/frd/{route}"
```

### Comparing `censius-1.6.9/src/censius.egg-info/PKG-INFO` & `censius-1.7.0/src/censius.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.6.9
+Version: 1.7.0
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.6.9/src/censius.egg-info/SOURCES.txt` & `censius-1.7.0/src/censius.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 README.md
 pyproject.toml
 setup.py
-src/censius/CensiusClient.py
-src/censius/Dataset.py
-src/censius/DatasetType.py
-src/censius/Explanation.py
-src/censius/ExplanationType.py
-src/censius/ModelType.py
-src/censius/Prediction.py
+src/censius/CensiusParent.py
 src/censius/__init__.py
-src/censius/constants.py
 src/censius/endpoint.py
-src/censius/schemas.py
-src/censius/utils.py
+src/censius/helper.py
 src/censius.egg-info/PKG-INFO
 src/censius.egg-info/SOURCES.txt
 src/censius.egg-info/dependency_links.txt
 src/censius.egg-info/requires.txt
-src/censius.egg-info/top_level.txt
+src/censius.egg-info/top_level.txt
+src/censius/ml/CensiusClient.py
+src/censius/ml/Dataset.py
+src/censius/ml/DatasetType.py
+src/censius/ml/Explanation.py
+src/censius/ml/ExplanationType.py
+src/censius/ml/ModelType.py
+src/censius/ml/Prediction.py
+src/censius/ml/__init__.py
+src/censius/ml/constants.py
+src/censius/ml/schemas.py
+src/censius/ml/utils.py
+src/censius/nlp/CensiusClient.py
+src/censius/nlp/DatasetType.py
+src/censius/nlp/ModelType.py
+src/censius/nlp/UseCase.py
+src/censius/nlp/__init__.py
+src/censius/nlp/constants.py
+src/censius/nlp/schema.py
```

