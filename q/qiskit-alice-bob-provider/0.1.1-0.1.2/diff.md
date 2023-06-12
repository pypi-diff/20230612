# Comparing `tmp/qiskit_alice_bob_provider-0.1.1.tar.gz` & `tmp/qiskit_alice_bob_provider-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_alice_bob_provider-0.1.1.tar", last modified: Sun Jun  4 19:27:39 2023, max compression
+gzip compressed data, was "qiskit_alice_bob_provider-0.1.2.tar", last modified: Mon Jun 12 08:06:00 2023, max compression
```

## Comparing `qiskit_alice_bob_provider-0.1.1.tar` & `qiskit_alice_bob_provider-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)    11342 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/LICENSE
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/PKG-INFO
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1122 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/README.md
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2108 2023-06-04 19:26:25.000000 qiskit_alice_bob_provider-0.1.1/pyproject.toml
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      822 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/__init__.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      760 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/__init__.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3681 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/client.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     4469 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/jobs.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1286 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/targets.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5005 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/backend.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1857 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/custom_instructions.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1039 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/errors.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     7882 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/job.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2563 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/provider.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5871 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/qir_to_qiskit.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5112 2023-05-29 08:28:45.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/translation_plugin.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1086 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/utils.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/PKG-INFO
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1033 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/SOURCES.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)        1 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/dependency_links.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      120 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/entry_points.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      317 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/requires.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       26 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/top_level.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       38 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/setup.cfg
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       69 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/setup.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/tests/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1372 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/tests/test_against_real_server.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5145 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.1/tests/test_api.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5049 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_backend.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      295 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_provider.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1126 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_qir_to_qiskit.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5606 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/tests/test_translation_plugin.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      444 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)    11342 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/LICENSE
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/PKG-INFO
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1122 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/README.md
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2108 2023-06-12 08:04:04.000000 qiskit_alice_bob_provider-0.1.2/pyproject.toml
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      822 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/__init__.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      760 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/__init__.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3681 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/client.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     4469 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/jobs.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1286 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/targets.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5151 2023-06-09 14:28:03.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/backend.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1857 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/custom_instructions.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3186 2023-06-09 14:46:54.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/ensure_preparation_pass.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1039 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/errors.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     7882 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/job.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2563 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/provider.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5871 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/qir_to_qiskit.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5112 2023-06-09 14:25:47.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/translation_plugin.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1086 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/utils.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/PKG-INFO
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1124 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)        1 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      120 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/entry_points.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      317 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/requires.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       26 2023-06-12 08:06:00.000000 qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/top_level.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       38 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/setup.cfg
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       69 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/setup.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-12 08:06:00.962752 qiskit_alice_bob_provider-0.1.2/tests/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1372 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/tests/test_against_real_server.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5145 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.2/tests/test_api.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5049 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_backend.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1272 2023-06-09 14:26:04.000000 qiskit_alice_bob_provider-0.1.2/tests/test_ensure_preparation_pass.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      295 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_provider.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1126 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_qir_to_qiskit.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5606 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.2/tests/test_translation_plugin.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      444 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.2/tests/test_utils.py
```

### Comparing `qiskit_alice_bob_provider-0.1.1/LICENSE` & `qiskit_alice_bob_provider-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/PKG-INFO` & `qiskit_alice_bob_provider-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.1.1/README.md` & `qiskit_alice_bob_provider-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/pyproject.toml` & `qiskit_alice_bob_provider-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qiskit_alice_bob_provider"
 authors = [
     {name = "Alice & Bob Software Team"},
 ]
-version = "0.1.1"
+version = "0.1.2"
 description = "Provider for running Qiskit circuits on Alice & Bob QPUs and simulators"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 keywords = ["Qiskit", "Alice & Bob", "Quantum", "SDK"]
 classifiers=[
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/__init__.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/__init__.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/client.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/client.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/jobs.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/jobs.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/targets.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/api/targets.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/backend.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 #    limitations under the License.
 ##############################################################################
 
 from typing import Any, Dict
 
 from qiskit import QuantumCircuit
 from qiskit.providers import BackendV2, Options
-from qiskit.transpiler import Target
+from qiskit.transpiler import PassManager, Target
 from qiskit_qir import to_qir_module
 
 from .api import jobs
 from .api.client import ApiClient
+from .ensure_preparation_pass import EnsurePreparationPass
 from .job import AliceBobJob
 from .qir_to_qiskit import ab_target_to_qiskit_target
 from .utils import camel_to_snake_case, snake_to_camel_case
 
 
 class AliceBobBackend(BackendV2):
     """Class representing the single cat simulator target accessible via the
@@ -83,14 +84,15 @@
         options: Options = self.options
         for key, value in kwargs.items():
             if not hasattr(options, key):
                 raise ValueError(f'Backend does not support option "{key}"')
             options.update_options(**{key: value})
         input_params = _ab_input_params_from_options(options)
         job = jobs.create_job(self._api_client, self.name, input_params)
+        run_input = PassManager([EnsurePreparationPass()]).run(run_input)
         jobs.upload_input(
             self._api_client, job['id'], _qiskit_to_qir(run_input)
         )
         return AliceBobJob(
             backend=self,
             api_client=self._api_client,
             job_id=job['id'],
```

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/custom_instructions.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/custom_instructions.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/errors.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/job.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/provider.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/translation_plugin.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/translation_plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/utils.py` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/PKG-INFO` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-alice-bob-provider
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/SOURCES.txt` & `qiskit_alice_bob_provider-0.1.2/qiskit_alice_bob_provider.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 qiskit_alice_bob_provider/__init__.py
 qiskit_alice_bob_provider/backend.py
 qiskit_alice_bob_provider/custom_instructions.py
+qiskit_alice_bob_provider/ensure_preparation_pass.py
 qiskit_alice_bob_provider/errors.py
 qiskit_alice_bob_provider/job.py
 qiskit_alice_bob_provider/provider.py
 qiskit_alice_bob_provider/qir_to_qiskit.py
 qiskit_alice_bob_provider/translation_plugin.py
 qiskit_alice_bob_provider/utils.py
 qiskit_alice_bob_provider.egg-info/PKG-INFO
@@ -20,11 +21,12 @@
 qiskit_alice_bob_provider/api/__init__.py
 qiskit_alice_bob_provider/api/client.py
 qiskit_alice_bob_provider/api/jobs.py
 qiskit_alice_bob_provider/api/targets.py
 tests/test_against_real_server.py
 tests/test_api.py
 tests/test_backend.py
+tests/test_ensure_preparation_pass.py
 tests/test_provider.py
 tests/test_qir_to_qiskit.py
 tests/test_translation_plugin.py
 tests/test_utils.py
```

### Comparing `qiskit_alice_bob_provider-0.1.1/tests/test_against_real_server.py` & `qiskit_alice_bob_provider-0.1.2/tests/test_against_real_server.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/tests/test_api.py` & `qiskit_alice_bob_provider-0.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/tests/test_backend.py` & `qiskit_alice_bob_provider-0.1.2/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/tests/test_qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.1.2/tests/test_qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.1/tests/test_translation_plugin.py` & `qiskit_alice_bob_provider-0.1.2/tests/test_translation_plugin.py`

 * *Files identical despite different names*

