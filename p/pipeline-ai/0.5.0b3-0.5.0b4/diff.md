# Comparing `tmp/pipeline_ai-0.5.0b3.tar.gz` & `tmp/pipeline_ai-0.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_ai-0.5.0b3.tar", max compression
+gzip compressed data, was "pipeline_ai-0.5.0b4.tar", max compression
```

## Comparing `pipeline_ai-0.5.0b3.tar` & `pipeline_ai-0.5.0b4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0    10176 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/LICENSE
--rw-r--r--   0        0        0     6130 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/README.md
--rw-r--r--   0        0        0      434 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/__init__.py
--rw-r--r--   0        0        0      135 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/__main__.py
--rw-r--r--   0        0        0       62 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/__init__.py
--rw-r--r--   0        0        0       62 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/asyncio/__init__.py
--rw-r--r--   0        0        0     8380 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/asyncio/cloud.py
--rw-r--r--   0        0        0    29923 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/cloud.py
--rw-r--r--   0        0        0      974 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/environments.py
--rw-r--r--   0        0        0     3247 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/configuration/__init__.py
--rw-r--r--   0        0        0    11693 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/__init__.py
--rw-r--r--   0        0        0     8254 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/environments.py
--rw-r--r--   0        0        0     2587 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/remote.py
--rw-r--r--   0        0        0     2011 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/runs.py
--rw-r--r--   0        0        0     4838 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/tags.py
--rw-r--r--   0        0        0     4868 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/docker/__init__.py
--rw-r--r--   0        0        0      276 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/InvalidSchema.py
--rw-r--r--   0        0        0      283 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/MissingActiveToken.py
--rw-r--r--   0        0        0      312 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/NonChargeableProfile.py
--rw-r--r--   0        0        0      309 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/PipelineNotDeployed.py
--rw-r--r--   0        0        0      546 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/__init__.py
--rw-r--r--   0        0        0     4752 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/decorators.py
--rw-r--r--   0        0        0     1528 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/environment/__init__.py
--rw-r--r--   0        0        0     2015 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/function.py
--rw-r--r--   0        0        0    10909 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/graph.py
--rw-r--r--   0        0        0      877 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/graph_node.py
--rw-r--r--   0        0        0     1091 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/huggingface/TransformersModelForCausalLM.py
--rw-r--r--   0        0        0        0 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/huggingface/__init__.py
--rw-r--r--   0        0        0     1161 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/model.py
--rw-r--r--   0        0        0     3488 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/pipeline.py
--rw-r--r--   0        0        0     1861 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/variable.py
--rw-r--r--   0        0        0     1712 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/wrappers.py
--rw-r--r--   0        0        0        0 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/schemas/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/base.py
--rw-r--r--   0        0        0      369 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/compute_requirements.py
--rw-r--r--   0        0        0      558 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/data.py
--rw-r--r--   0        0        0      573 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/deployment.py
--rw-r--r--   0        0        0      516 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/environment.py
--rw-r--r--   0        0        0      714 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/file.py
--rw-r--r--   0        0        0     2426 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/function.py
--rw-r--r--   0        0        0     5236 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/metrics.py
--rw-r--r--   0        0        0      569 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/milestones_register.py
--rw-r--r--   0        0        0     1599 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/model.py
--rw-r--r--   0        0        0      739 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/onboarding.py
--rw-r--r--   0        0        0      944 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/pagination.py
--rw-r--r--   0        0        0     5817 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/pipeline.py
--rw-r--r--   0        0        0     1261 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/pipeline_file.py
--rw-r--r--   0        0        0      537 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/project.py
--rw-r--r--   0        0        0        0 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/redis/__init__.py
--rw-r--r--   0        0        0      234 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/redis/command.py
--rw-r--r--   0        0        0      337 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/request.py
--rw-r--r--   0        0        0      261 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/resource.py
--rw-r--r--   0        0        0     3839 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/run.py
--rw-r--r--   0        0        0     1031 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/runnable.py
--rw-r--r--   0        0        0      167 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/tag.py
--rw-r--r--   0        0        0     1668 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/token.py
--rw-r--r--   0        0        0     3827 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/user.py
--rw-r--r--   0        0        0     2493 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/validators.py
--rw-r--r--   0        0        0      320 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/worker.py
--rw-r--r--   0        0        0     1924 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/util/__init__.py
--rw-r--r--   0        0        0     1129 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/util/logging.py
--rw-r--r--   0        0        0      241 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/util/torch_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/__init__.py
--rw-r--r--   0        0        0      287 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/environments.py
--rw-r--r--   0        0        0     3131 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/http.py
--rw-r--r--   0        0        0     4354 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/pipelines.py
--rw-r--r--   0        0        0        0 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/schemas/__init__.py
--rw-r--r--   0        0        0     3769 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/schemas/runs.py
--rw-r--r--   0        0        0     4571 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/uploading.py
--rw-r--r--   0        0        0     1249 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pyproject.toml
--rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b3/PKG-INFO
+-rw-r--r--   0        0        0    10176 2023-06-12 18:32:31.036103 pipeline_ai-0.5.0b4/LICENSE
+-rw-r--r--   0        0        0     6130 2023-06-12 18:32:31.036103 pipeline_ai-0.5.0b4/README.md
+-rw-r--r--   0        0        0      434 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/__init__.py
+-rw-r--r--   0        0        0      135 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/__main__.py
+-rw-r--r--   0        0        0       62 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/api/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/api/asyncio/__init__.py
+-rw-r--r--   0        0        0     8379 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/api/asyncio/cloud.py
+-rw-r--r--   0        0        0    29923 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/api/cloud.py
+-rw-r--r--   0        0        0      974 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/api/environments.py
+-rw-r--r--   0        0        0     3231 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/configuration/__init__.py
+-rw-r--r--   0        0        0    11667 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/console/__init__.py
+-rw-r--r--   0        0        0     8254 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/console/environments.py
+-rw-r--r--   0        0        0     2587 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/console/remote.py
+-rw-r--r--   0        0        0     2011 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/console/runs.py
+-rw-r--r--   0        0        0     4838 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/console/tags.py
+-rw-r--r--   0        0        0     4868 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/docker/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/exceptions/InvalidSchema.py
+-rw-r--r--   0        0        0      283 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/exceptions/MissingActiveToken.py
+-rw-r--r--   0        0        0      312 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/exceptions/NonChargeableProfile.py
+-rw-r--r--   0        0        0      309 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/exceptions/PipelineNotDeployed.py
+-rw-r--r--   0        0        0      546 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/__init__.py
+-rw-r--r--   0        0        0     4751 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/decorators.py
+-rw-r--r--   0        0        0     1528 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/environment/__init__.py
+-rw-r--r--   0        0        0     2015 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/function.py
+-rw-r--r--   0        0        0    10909 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/graph.py
+-rw-r--r--   0        0        0      877 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/graph_node.py
+-rw-r--r--   0        0        0     1090 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/huggingface/TransformersModelForCausalLM.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/huggingface/__init__.py
+-rw-r--r--   0        0        0     1160 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/model.py
+-rw-r--r--   0        0        0     3473 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/pipeline.py
+-rw-r--r--   0        0        0     1859 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/variable.py
+-rw-r--r--   0        0        0     1712 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/objects/wrappers.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/base.py
+-rw-r--r--   0        0        0      369 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/compute_requirements.py
+-rw-r--r--   0        0        0      558 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/data.py
+-rw-r--r--   0        0        0      573 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/deployment.py
+-rw-r--r--   0        0        0      516 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/environment.py
+-rw-r--r--   0        0        0      714 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/file.py
+-rw-r--r--   0        0        0     2426 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/function.py
+-rw-r--r--   0        0        0     5236 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/metrics.py
+-rw-r--r--   0        0        0      569 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/milestones_register.py
+-rw-r--r--   0        0        0     1599 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/model.py
+-rw-r--r--   0        0        0      739 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/onboarding.py
+-rw-r--r--   0        0        0      943 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/pagination.py
+-rw-r--r--   0        0        0     5817 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/pipeline.py
+-rw-r--r--   0        0        0     1261 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/pipeline_file.py
+-rw-r--r--   0        0        0      537 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/project.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/redis/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/redis/command.py
+-rw-r--r--   0        0        0      337 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/request.py
+-rw-r--r--   0        0        0      261 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/resource.py
+-rw-r--r--   0        0        0     3839 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/run.py
+-rw-r--r--   0        0        0     1031 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/runnable.py
+-rw-r--r--   0        0        0      167 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/tag.py
+-rw-r--r--   0        0        0     1668 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/token.py
+-rw-r--r--   0        0        0     3827 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/user.py
+-rw-r--r--   0        0        0     2493 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/validators.py
+-rw-r--r--   0        0        0      320 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/schemas/worker.py
+-rw-r--r--   0        0        0     1924 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/util/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/util/logging.py
+-rw-r--r--   0        0        0      241 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/util/torch_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/v3/__init__.py
+-rw-r--r--   0        0        0      286 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/v3/environments.py
+-rw-r--r--   0        0        0     2883 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/v3/http.py
+-rw-r--r--   0        0        0     4931 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/v3/pipelines.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/v3/schemas/__init__.py
+-rw-r--r--   0        0        0     3779 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/v3/schemas/runs.py
+-rw-r--r--   0        0        0     4571 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pipeline/v3/uploading.py
+-rw-r--r--   0        0        0     1250 2023-06-12 18:32:31.040104 pipeline_ai-0.5.0b4/pyproject.toml
+-rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b4/PKG-INFO
```

### Comparing `pipeline_ai-0.5.0b3/LICENSE` & `pipeline_ai-0.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/README.md` & `pipeline_ai-0.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/api/asyncio/cloud.py` & `pipeline_ai-0.5.0b4/pipeline/api/asyncio/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
             schema = FileCreate.__name__
             raise InvalidSchema(schema=schema)
         else:
             response.raise_for_status()
         return FileGet.parse_obj(response.json())
 
     async def upload_file(self, file_or_path) -> FileGet:
-
         if isinstance(file_or_path, str):
             # TODO: Change this to wrap the file object reader to convert to hex
             # everytime anything is read instead of reading it all at once.
 
             with open(file_or_path, "rb") as file:
                 buffer = file.read()
             hex_buffer = buffer.hex()
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/api/cloud.py` & `pipeline_ai-0.5.0b4/pipeline/api/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 import dill
 import httpx
 from pydantic import ValidationError
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
-from pipeline.configuration import current_configuration, PIPELINE_DIR
 from pipeline.api.environments import PipelineCloudEnvironment, resolve_environment_id
+from pipeline.configuration import PIPELINE_DIR, current_configuration
 from pipeline.exceptions.InvalidSchema import InvalidSchema
 from pipeline.exceptions.MissingActiveToken import MissingActiveToken
 from pipeline.objects.variable import PipelineFile
 from pipeline.schemas.base import BaseModel
 from pipeline.schemas.compute_requirements import ComputeRequirements
 from pipeline.schemas.data import DataGet
 from pipeline.schemas.file import FileFormat, FileGet
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/api/environments.py` & `pipeline_ai-0.5.0b4/pipeline/api/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/configuration/__init__.py` & `pipeline_ai-0.5.0b4/pipeline/configuration/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import os
-import yaml
 import json
+import os
 import sys
-import base64
-
 import typing as t
-
-
 from pathlib import Path
+
+import yaml
 from pydantic import BaseModel
 
 PIPELINE_DIR = Path(
     os.getenv(
         "PIPELINE_DIR",
         Path(os.getenv("LOCALAPPDATA")) / ".pipeline/"
         if (sys.platform == "win32" or sys.platform == "cygwin")
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/console/__init__.py` & `pipeline_ai-0.5.0b4/pipeline/console/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         help="List the authenticated remote compute services",
     )
 
     ##########
     # pipeline remote resources
     ##########
 
-    remote_resources_parser = remote_sub_parser.add_parser(
+    remote_sub_parser.add_parser(
         "resources",
         description="Manage resources on a remote compute service",
         help="Manage resources on a remote compute service",
     )
 
     ##########
     # pipeline runs
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/console/environments.py` & `pipeline_ai-0.5.0b4/pipeline/console/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/console/remote.py` & `pipeline_ai-0.5.0b4/pipeline/console/remote.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
 import argparse
+import json
 
 from tabulate import tabulate
 
 from pipeline import PipelineCloud, current_configuration
 from pipeline.exceptions.MissingActiveToken import MissingActiveToken
 from pipeline.util.logging import _print
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/console/runs.py` & `pipeline_ai-0.5.0b4/pipeline/console/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/console/tags.py` & `pipeline_ai-0.5.0b4/pipeline/console/tags.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/docker/__init__.py` & `pipeline_ai-0.5.0b4/pipeline/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/__init__.py` & `pipeline_ai-0.5.0b4/pipeline/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/decorators.py` & `pipeline_ai-0.5.0b4/pipeline/objects/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
     ):
         if model_class is not None:
             model_class.__pipeline_model__ = True
 
         self.model_class = model_class
 
     def __call__(self, *args, **kwargs):
-
         if len(args) + len(kwargs) == 1:
             self.model_class = args[0]
             self.model_class.__pipeline_model__ = True
             return self.__function_exe__
         else:
             return self.__function_exe__(*args, **kwargs)
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/environment/__init__.py` & `pipeline_ai-0.5.0b4/pipeline/objects/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/function.py` & `pipeline_ai-0.5.0b4/pipeline/objects/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/graph.py` & `pipeline_ai-0.5.0b4/pipeline/objects/graph.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/graph_node.py` & `pipeline_ai-0.5.0b4/pipeline/objects/graph_node.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/huggingface/TransformersModelForCausalLM.py` & `pipeline_ai-0.5.0b4/pipeline/objects/huggingface/TransformersModelForCausalLM.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         self.model_path = model_path
         self.tokenizer_path = tokenizer_path
         self.model = None
         self.tokenizer = None
 
     @pipeline_function
     def predict(self, input_data: str, model_kwargs: dict) -> str:
-
         input_ids = self.tokenizer(input_data, return_tensors="pt").input_ids
         gen_tokens = self.model.generate(input_ids, **model_kwargs)
         gen_text = self.tokenizer.batch_decode(gen_tokens)[0]
         return gen_text
 
     @pipeline_function(on_startup=True, run_once=True)
     def load(self) -> None:
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/model.py` & `pipeline_ai-0.5.0b4/pipeline/objects/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     name: str
     source: str
     hash: str
 
     model: Any
 
     def __init__(self, model: Any, *, name: str = "", local_id: str = None):
-
         self.name = name
         self.model = model
         try:
             self.source = inspect.getsource(model.__class__)
         except OSError:
             self.source = str(uuid.uuid4())
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/pipeline.py` & `pipeline_ai-0.5.0b4/pipeline/objects/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import inspect
 from pipeline.objects.function import Function
 from pipeline.objects.graph import Graph
 from pipeline.objects.graph_node import GraphNode
 from pipeline.objects.variable import Variable
 
 
 class Pipeline:
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/variable.py` & `pipeline_ai-0.5.0b4/pipeline/objects/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any
 
 from pipeline.schemas.pipeline import PipelineVariableGet
 from pipeline.util import generate_id, load_object
 
 
 class Variable:
-
     local_id: str
     remote_id: str
 
     name: str
 
     type_class: Any
 
@@ -45,15 +44,14 @@
                 is_output=schema.is_output,
                 name=schema.name,
                 local_id=schema.local_id,
             )
 
 
 class PipelineFile(Variable):
-
     path: str
 
     def __init__(
         self,
         *,
         path: str = None,
         name: str = None,
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/objects/wrappers.py` & `pipeline_ai-0.5.0b4/pipeline/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/base.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/base.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/data.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/data.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/deployment.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/environment.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/environment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/file.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/function.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/metrics.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/milestones_register.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/milestones_register.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/model.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/onboarding.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/onboarding.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/pagination.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,10 @@
     #: Total number of resources available for pagination
     total: int
     #: Resource data
     data: List[DataType]
 
     @classmethod
     def of(cls, item_list: List[DataType], details: PaginationDetails, total: int):
-
         return Paginated(
             skip=details.skip, limit=details.limit, total=total, data=item_list
         )
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/pipeline.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/pipeline_file.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/pipeline_file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/project.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/project.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/run.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/run.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/runnable.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/runnable.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/token.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/token.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/user.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/user.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/schemas/validators.py` & `pipeline_ai-0.5.0b4/pipeline/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/util/__init__.py` & `pipeline_ai-0.5.0b4/pipeline/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pipeline/util/logging.py` & `pipeline_ai-0.5.0b4/pipeline/util/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,23 +28,21 @@
     log_str = (
         f"{PIPELINE_STR} {time_stamp} - [{levels[level]}{level}{bcolors.ENDC}]: {val}"
     )
     print(f"{log_str}")
 
 
 def set_print_to_file(path: str):
-
     global LOG_FILE
     if LOG_FILE is None:
         LOG_FILE = open(path, "w")
         sys.stdout = LOG_FILE
     else:
         raise Exception("Already printing to a log file.")
 
 
 def stop_print_to_file():
-
     global LOG_FILE
     if LOG_FILE is not None:
         LOG_FILE.close()
     else:
         raise Exception("Not printing to log file")
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/v3/http.py` & `pipeline_ai-0.5.0b4/pipeline/v3/http.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,37 +23,33 @@
     timeout=300,
 )
 
 
 def post(
     endpoint: str,
     json_data: dict = None,
+    raise_for_status: bool = True,
 ) -> httpx.Response:
-    try:
-        response = _client.post(
-            endpoint,
-            json=json_data,
-        )
+    response = _client.post(
+        endpoint,
+        json=json_data,
+    )
+    if raise_for_status:
         response.raise_for_status()
-    except httpx.HTTPStatusError as exc:
-        raise Exception(f"HTTP error: {exc.response.status_code}, {exc.response.text}")
 
     return response
 
 
 def get(
     endpoint: str,
 ) -> httpx.Response:
-    try:
-        response = _client.get(
-            endpoint,
-        )
-        response.raise_for_status()
-    except httpx.HTTPStatusError as exc:
-        raise Exception(f"HTTP error: {exc.response.status_code}, {exc.response.text}")
+    response = _client.get(
+        endpoint,
+    )
+    response.raise_for_status()
 
     return response
 
 
 def create_callback(encoder: MultipartEncoder) -> t.Callable:
     encoder_len = encoder.len
     bar = tqdm(
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/v3/pipelines.py` & `pipeline_ai-0.5.0b4/pipeline/v3/pipelines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import io
 import math
 import typing as t
 from multiprocessing import Pool
 from pathlib import Path
 
 import cloudpickle as cp
 import httpx
 
 from pipeline.objects import Graph, PipelineFile
 from pipeline.util.logging import _print
 from pipeline.v3 import http
-from pipeline.v3.schemas.runs import Run, RunInput, RunIOType, RunCreate
+from pipeline.v3.schemas.runs import Run, RunCreate, RunInput, RunIOType
 
 
 def upload_pipeline(
     graph: Graph,
     environment_id_or_name: t.Union[str, int],
 ):
     if graph._has_run_startup:
@@ -89,47 +88,63 @@
 
 def run_pipeline(
     pipeline_id_or_tag: t.Union[str, int],
     *data,
     async_run: bool = False,
     return_response: bool = False,
 ) -> t.Union[Run, httpx.Response]:
-    data_obj = io.BytesIO(cp.dumps(data))
-
     run_create_schema = RunCreate(
         pipeline_id_or_tag=pipeline_id_or_tag,
         input_data=_data_to_run_input(data),
         async_run=async_run,
     )
 
     res = http.post(
         "/v3/runs",
         json_data=run_create_schema.dict(),
+        raise_for_status=False,
     )
 
     if return_response:
         return res
 
     if res.status_code == 500:
         _print(
             f"Failed run (status={res.status_code}, text={res.text}, "
             f"headers={res.headers})",
             level="ERROR",
         )
         raise Exception(f"Error: {res.status_code}, {res.text}", res.status_code)
     elif res.status_code == 429:
+        _print(
+            f"Too many requests (status={res.status_code}, text={res.text})",
+            level="ERROR",
+        )
         raise Exception(
             "Too many requests, please try again later",
             res.status_code,
         )
-
-    try:
-        res.raise_for_status()
-    except httpx.HTTPStatusError as exc:
-        raise Exception(f"HTTP error: {exc.response.status_code}, {exc.response.text}")
+    elif res.status_code == 404:
+        _print(
+            f"Pipeline not found (status={res.status_code}, text={res.text})",
+            level="ERROR",
+        )
+        raise Exception("Pipeline not found", res.status_code)
+    elif res.status_code == 503:
+        _print(
+            f"Environment not cached (status={res.status_code}, text={res.text})",
+            level="ERROR",
+        )
+        raise Exception("Environment not cached", res.status_code)
+    elif res.status_code == 502:
+        _print(
+            "Gateway error",
+            level="ERROR",
+        )
+        raise Exception("Gateway error", res.status_code)
 
     # Everything is okay!
     run_get = Run.parse_obj(res.json())
 
     return run_get
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/v3/schemas/runs.py` & `pipeline_ai-0.5.0b4/pipeline/v3/schemas/runs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
+import json
 import typing as t
 from datetime import datetime
 from enum import Enum
-import json
 
 from pydantic import BaseModel
 
 
 class RunState(int, Enum):
     created: int = 0
     routing: int = 1
@@ -23,14 +23,15 @@
     api_received: int = 9
 
     in_queue: int = 16
     denied: int = 11
     resource_rejected: int = 14
     resource_died: int = 15
     retrying: int = 13
+    rerouting: int = 21
 
     completed: int = 10
     failed: int = 12
     rate_limited: int = 17
     lost: int = 18
     no_environment_installed: int = 19
 
@@ -66,16 +67,16 @@
 
 class RunFileType(Enum):
     input = "input"
     output = "output"
 
 
 class RunFile(BaseModel):
-    id: int
-    run_id: int
+    id: str
+    run_id: str
     io_type: RunFileType
     path: str
 
     class Config:
         # use_enum_values = True
         orm_mode = True
 
@@ -126,51 +127,51 @@
 class RunOutput(BaseModel):
     type: RunIOType
     value: t.Optional[t.Any]
     file: t.Optional[RunOutputFile]
 
 
 class RunResult(BaseModel):
-    run_id: int
+    run_id: str
     outputs: t.List[RunOutput]
 
     def result_array(self) -> t.List[t.Any]:
         return [output.value for output in self.outputs]
 
 
 class Run(BaseModel):
-    id: int
+    id: str
 
     created_at: datetime
 
-    pipeline_id: int
-    environment_id: int
+    pipeline_id: str
+    environment_id: str
     environment_hash: str
 
     state: RunState
     error: t.Optional[RunError]
 
     result: t.Optional[RunResult]
 
     class Config:
         # use_enum_values = True
         orm_mode = True
 
 
 class RunStateTransition(BaseModel):
-    run_id: int
+    run_id: str
     new_state: RunState
     time: datetime
 
 
 class RunInput(BaseModel):
     type: RunIOType
     value: t.Any
 
     file_name: t.Optional[str]
     file_path: t.Optional[str]
 
 
 class RunCreate(BaseModel):
-    pipeline_id_or_tag: t.Union[int, str]
+    pipeline_id_or_tag: str
     input_data: t.List[RunInput]
     async_run: bool = False
```

### Comparing `pipeline_ai-0.5.0b3/pipeline/v3/uploading.py` & `pipeline_ai-0.5.0b4/pipeline/v3/uploading.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b3/pyproject.toml` & `pipeline_ai-0.5.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "pipeline-ai"
-version = "0.5.0b3"
+version = "0.5.0b4"
+
 
 description = "Pipelines for machine learning workloads."
 authors = [
   "Paul Hetherington <ph@mystic.ai>",
   "Alex Pearwin <alex@mystic.ai>",
   "Neil Wang <neil@mystic.ai>",
   "Ross Gray <ross@mystic.ai>",
```

### Comparing `pipeline_ai-0.5.0b3/PKG-INFO` & `pipeline_ai-0.5.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-ai
-Version: 0.5.0b3
+Version: 0.5.0b4
 Summary: Pipelines for machine learning workloads.
 License: Apache-2.0
 Author: Paul Hetherington
 Author-email: ph@mystic.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

