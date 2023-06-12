# Comparing `tmp/kedro_neptune-0.1.6.tar.gz` & `tmp/kedro_neptune-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_neptune-0.1.6.tar", max compression
+gzip compressed data, was "kedro_neptune-0.2.0.tar", max compression
```

## Comparing `kedro_neptune-0.1.6.tar` & `kedro_neptune-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2583 2023-03-31 18:23:35.634082 kedro_neptune-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0    11354 2023-03-31 18:23:35.634082 kedro_neptune-0.1.6/LICENSE
--rw-r--r--   0        0        0     3100 2023-03-31 18:23:35.634082 kedro_neptune-0.1.6/README.md
--rw-r--r--   0        0        0     2592 2023-03-31 18:23:46.866085 kedro_neptune-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    17066 2023-03-31 18:23:35.634082 kedro_neptune-0.1.6/src/kedro_neptune/__init__.py
--rw-r--r--   0        0        0     1664 2023-03-31 18:23:35.634082 kedro_neptune-0.1.6/src/kedro_neptune/config.py
--rw-r--r--   0        0        0     1155 2023-03-31 18:23:35.634082 kedro_neptune-0.1.6/src/kedro_neptune/utils.py
--rw-r--r--   0        0        0      736 2023-03-31 18:23:35.634082 kedro_neptune-0.1.6/src/kedro_neptune/version.py
--rw-r--r--   0        0        0     4985 1970-01-01 00:00:00.000000 kedro_neptune-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2766 2023-06-12 12:09:09.666035 kedro_neptune-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11354 2023-06-12 12:09:09.666035 kedro_neptune-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3100 2023-06-12 12:09:09.666035 kedro_neptune-0.2.0/README.md
+-rw-r--r--   0        0        0     2592 2023-06-12 12:09:20.938132 kedro_neptune-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17572 2023-06-12 12:09:09.670035 kedro_neptune-0.2.0/src/kedro_neptune/__init__.py
+-rw-r--r--   0        0        0     1664 2023-06-12 12:09:09.670035 kedro_neptune-0.2.0/src/kedro_neptune/config.py
+-rw-r--r--   0        0        0     1155 2023-06-12 12:09:09.670035 kedro_neptune-0.2.0/src/kedro_neptune/utils.py
+-rw-r--r--   0        0        0      736 2023-06-12 12:09:09.670035 kedro_neptune-0.2.0/src/kedro_neptune/version.py
+-rw-r--r--   0        0        0     4985 1970-01-01 00:00:00.000000 kedro_neptune-0.2.0/PKG-INFO
```

### Comparing `kedro_neptune-0.1.6/CHANGELOG.md` & `kedro_neptune-0.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.2.0
+
+### Fixes
+- If `neptune` 'enabled' flag in the config is set to `false`, no neptune-related actions are taken ([#68](https://github.com/neptune-ai/kedro-neptune/pull/68))
+
+
 ##  0.1.5
 
 ### Fixes
 - Fixed some of latest `neptune-client` warning messages ([#58](https://github.com/neptune-ai/kedro-neptune/pull/58))
 - Fixed failing run on latest MacOS 12 ([#58](https://github.com/neptune-ai/kedro-neptune/pull/58))
 
 ### Changes
```

### Comparing `kedro_neptune-0.1.6/LICENSE` & `kedro_neptune-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_neptune-0.1.6/README.md` & `kedro_neptune-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro_neptune-0.1.6/pyproject.toml` & `kedro_neptune-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 repository = "https://github.com/neptune-ai/kedro-neptune"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations/kedro/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "kedro-neptune"
 readme = "README.md"
-version = "0.1.6"
+version = "0.2.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `kedro_neptune-0.1.6/src/kedro_neptune/__init__.py` & `kedro_neptune-0.2.0/src/kedro_neptune/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -237,28 +237,32 @@
     def __getstate__(self) -> dict:
         properties = self.__dict__.copy()
         properties["_run"] = None
         return properties
 
     def _set_run(self):
         neptune_config = get_neptune_config(settings)
-        self._run = neptune.init_run(
-            api_token=neptune_config.api_token,
-            project=neptune_config.project,
-            mode=_connection_mode(neptune_config.enabled),
-            capture_stdout=False,
-            capture_stderr=False,
-            capture_hardware_metrics=False,
-            capture_traceback=False,
-            source_files=None,
-        )
 
-    def _load(self) -> Handler:
+        if neptune_config.enabled:
+            self._run = neptune.init_run(
+                api_token=neptune_config.api_token,
+                project=neptune_config.project,
+                capture_stdout=False,
+                capture_stderr=False,
+                capture_hardware_metrics=False,
+                capture_traceback=False,
+                source_files=None,
+            )
+
+    def _load(self) -> Optional[Handler]:
         neptune_config = get_neptune_config(settings)
 
+        if not neptune_config.enabled:
+            return
+
         if self._run is None:
             self._set_run()
         self._loaded = True
 
         return self._run[neptune_config.base_namespace]
 
     def _release(self) -> None:
@@ -413,22 +417,29 @@
     def __init__(self):
         self._run_id: Optional[str] = None
         self._node_execution_timers: Dict[str, float] = {}
 
     @hook_impl
     def after_catalog_created(self, catalog: DataCatalog) -> None:
         self._run_id = hashlib.md5(str(time.time()).encode()).hexdigest()
-        os.environ["NEPTUNE_CUSTOM_RUN_ID"] = self._run_id
+
+        config = get_neptune_config(settings)
+
+        if config.enabled:
+            os.environ["NEPTUNE_CUSTOM_RUN_ID"] = self._run_id
 
         catalog.add(data_set_name="neptune_run", data_set=NeptuneRunDataSet())
 
     @hook_impl
     def before_pipeline_run(self, run_params: Dict[str, Any], pipeline: Pipeline, catalog: DataCatalog) -> None:
         config = get_neptune_config(settings)
 
+        if not config.enabled:
+            return
+
         run = neptune.init_run(
             api_token=config.api_token,
             project=config.project,
             mode=_connection_mode(config.enabled),
             custom_run_id=self._run_id,
             source_files=config.source_files or None,
         )
@@ -443,28 +454,38 @@
         log_command(namespace=current_namespace)
         log_run_params(namespace=current_namespace, run_params=run_params)
         log_data_catalog_metadata(namespace=current_namespace, catalog=catalog)
         log_pipeline_metadata(namespace=current_namespace, pipeline=pipeline)
 
     @hook_impl
     def before_node_run(self, node: Node, inputs: Dict[str, Any], catalog: DataCatalog):
+        config = get_neptune_config(settings)
+
+        if not config.enabled:
+            return
+
         run = catalog.load("neptune_run")
         current_namespace = run[f"nodes/{node.short_name}"]
 
         if inputs:
             current_namespace["inputs"] = stringify_unsupported(list(sorted(inputs.keys())))
 
         for input_name, input_value in inputs.items():
             if input_name.startswith("params:"):
                 current_namespace[f'parameters/{input_name[len("params:"):]}'] = input_value
 
         self._node_execution_timers[node.short_name] = time.time()
 
     @hook_impl
     def after_node_run(self, node: Node, catalog: DataCatalog, outputs: Dict[str, Any]) -> None:
+        config = get_neptune_config(settings)
+
+        if not config.enabled:
+            return
+
         execution_time = float(time.time() - self._node_execution_timers[node.short_name])
 
         run = catalog.load("neptune_run")
         current_namespace = run[f"nodes/{node.short_name}"]
         current_namespace["execution_time"] = execution_time
 
         if outputs:
@@ -475,13 +496,18 @@
             run.get_root_object().sync()
         else:
             run.sync()
         catalog.release("neptune_run")
 
     @hook_impl
     def after_pipeline_run(self, catalog: DataCatalog) -> None:
+        config = get_neptune_config(settings)
+
+        if not config.enabled:
+            return
+
         run = catalog.load("neptune_run")
         log_data_catalog_metadata(namespace=run, catalog=catalog)
         run.container.sync()
 
 
 neptune_hooks = NeptuneHooks()
```

### Comparing `kedro_neptune-0.1.6/src/kedro_neptune/config.py` & `kedro_neptune-0.2.0/src/kedro_neptune/config.py`

 * *Files identical despite different names*

### Comparing `kedro_neptune-0.1.6/src/kedro_neptune/utils.py` & `kedro_neptune-0.2.0/src/kedro_neptune/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_neptune-0.1.6/src/kedro_neptune/version.py` & `kedro_neptune-0.2.0/src/kedro_neptune/version.py`

 * *Files identical despite different names*

### Comparing `kedro_neptune-0.1.6/PKG-INFO` & `kedro_neptune-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-neptune
-Version: 0.1.6
+Version: 0.2.0
 Summary: Neptune.ai integration with Kedro
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

