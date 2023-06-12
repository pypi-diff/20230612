# Comparing `tmp/astronomer_starship-1.0.1.tar.gz` & `tmp/astronomer_starship-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomer_starship-1.0.1.tar", max compression
+gzip compressed data, was "astronomer_starship-1.0.2.tar", max compression
```

## Comparing `astronomer_starship-1.0.1.tar` & `astronomer_starship-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      547 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/LICENSE
--rw-r--r--   0        0        0     9187 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/README.rst
--rw-r--r--   0        0        0        0 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/aeroscope/__init__.py
--rw-r--r--   0        0        0     2434 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/aeroscope/operators.py
--rw-r--r--   0        0        0     4126 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/aeroscope/plugins/__init__.py
--rw-r--r--   0        0        0      262 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/aeroscope/plugins/templates/aeroscope/formhelper.html
--rw-r--r--   0        0        0     2524 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/aeroscope/plugins/templates/aeroscope/main.html
--rw-r--r--   0        0        0     1561 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/aeroscope/util.py
--rw-r--r--   0        0        0        0 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/starship/__init__.py
--rw-r--r--   0        0        0    13578 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/starship/main.py
--rw-r--r--   0        0        0     7950 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/starship/operators.py
--rw-r--r--   0        0        0        0 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/starship/services/__init__.py
--rw-r--r--   0        0        0     7377 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/starship/services/astro_client.py
--rw-r--r--   0        0        0     4318 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/starship/services/local_airflow_client.py
--rw-r--r--   0        0        0     5230 2023-06-07 15:25:23.394750 astronomer_starship-1.0.1/astronomer/starship/services/remote_airflow_client.py
--rw-r--r--   0        0        0    39434 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/static/js/htmx.min.js
--rw-r--r--   0        0        0     7015 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/static/js/idiomorph.min.js
--rw-r--r--   0        0        0    20095 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/static/js/popper.js
--rw-r--r--   0        0        0    25717 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/static/js/tippy.js
--rw-r--r--   0        0        0     1309 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/static/tail-spin.svg
--rw-r--r--   0        0        0     2926 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/dag_row.html
--rw-r--r--   0        0        0      283 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/env_checkbox.html
--rw-r--r--   0        0        0      200 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/github_loop.html
--rw-r--r--   0        0        0      738 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/migrate_connection_button.html
--rw-r--r--   0        0        0      360 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/migrate_pool_button.html
--rw-r--r--   0        0        0      367 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/migrate_variable_button.html
--rw-r--r--   0        0        0     1194 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/tabs.html
--rw-r--r--   0        0        0     2088 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/tabs_loading.html
--rw-r--r--   0        0        0     1661 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/target_deployment_select.html
--rw-r--r--   0        0        0     1227 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/target_deployment_select_loading.html
--rw-r--r--   0        0        0      177 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/test_connection_label.html
--rw-r--r--   0        0        0     2644 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/token_modal.html
--rw-r--r--   0        0        0       15 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/user_label.html
--rw-r--r--   0        0        0     1759 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/connections.html
--rw-r--r--   0        0        0     1089 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/dags.html
--rw-r--r--   0        0        0     1847 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/env.html
--rw-r--r--   0        0        0      775 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/main.html
--rw-r--r--   0        0        0      980 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/migration.html
--rw-r--r--   0        0        0     1415 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/pools.html
--rw-r--r--   0        0        0     1376 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/templates/starship/variables.html
--rw-r--r--   0        0        0     1363 2023-06-07 15:25:23.398750 astronomer_starship-1.0.1/astronomer/starship/variables/operators.py
--rw-r--r--   0        0        0     2734 2023-06-07 15:25:23.406750 astronomer_starship-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 astronomer_starship-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      547 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/LICENSE
+-rw-r--r--   0        0        0     9187 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/README.rst
+-rw-r--r--   0        0        0        0 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/__init__.py
+-rw-r--r--   0        0        0     2434 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/operators.py
+-rw-r--r--   0        0        0     4126 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/plugins/__init__.py
+-rw-r--r--   0        0        0      262 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/plugins/templates/aeroscope/formhelper.html
+-rw-r--r--   0        0        0     2524 2023-06-12 21:22:15.214787 astronomer_starship-1.0.2/astronomer/aeroscope/plugins/templates/aeroscope/main.html
+-rw-r--r--   0        0        0     1561 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/aeroscope/util.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/__init__.py
+-rw-r--r--   0        0        0    13578 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/main.py
+-rw-r--r--   0        0        0     7950 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/operators.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/__init__.py
+-rw-r--r--   0        0        0     7382 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/astro_client.py
+-rw-r--r--   0        0        0     4318 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/local_airflow_client.py
+-rw-r--r--   0        0        0     5230 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/services/remote_airflow_client.py
+-rw-r--r--   0        0        0    39434 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/htmx.min.js
+-rw-r--r--   0        0        0     7015 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/idiomorph.min.js
+-rw-r--r--   0        0        0    20095 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/popper.js
+-rw-r--r--   0        0        0    25717 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/js/tippy.js
+-rw-r--r--   0        0        0     1309 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/static/tail-spin.svg
+-rw-r--r--   0        0        0     2926 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/dag_row.html
+-rw-r--r--   0        0        0      283 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/env_checkbox.html
+-rw-r--r--   0        0        0      200 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/github_loop.html
+-rw-r--r--   0        0        0      738 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_connection_button.html
+-rw-r--r--   0        0        0      360 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_pool_button.html
+-rw-r--r--   0        0        0      367 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_variable_button.html
+-rw-r--r--   0        0        0     1194 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs.html
+-rw-r--r--   0        0        0     2088 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs_loading.html
+-rw-r--r--   0        0        0     1661 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select.html
+-rw-r--r--   0        0        0     1227 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select_loading.html
+-rw-r--r--   0        0        0      177 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/test_connection_label.html
+-rw-r--r--   0        0        0     2644 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/token_modal.html
+-rw-r--r--   0        0        0       15 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/user_label.html
+-rw-r--r--   0        0        0     1759 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/connections.html
+-rw-r--r--   0        0        0     1089 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/dags.html
+-rw-r--r--   0        0        0     1847 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/env.html
+-rw-r--r--   0        0        0      775 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/main.html
+-rw-r--r--   0        0        0      980 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/migration.html
+-rw-r--r--   0        0        0     1415 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/pools.html
+-rw-r--r--   0        0        0     1376 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/templates/starship/variables.html
+-rw-r--r--   0        0        0     1363 2023-06-12 21:22:15.218787 astronomer_starship-1.0.2/astronomer/starship/variables/operators.py
+-rw-r--r--   0        0        0     2734 2023-06-12 21:22:15.226787 astronomer_starship-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 astronomer_starship-1.0.2/PKG-INFO
```

### Comparing `astronomer_starship-1.0.1/LICENSE` & `astronomer_starship-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/README.rst` & `astronomer_starship-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/aeroscope/operators.py` & `astronomer_starship-1.0.2/astronomer/aeroscope/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/aeroscope/plugins/__init__.py` & `astronomer_starship-1.0.2/astronomer/aeroscope/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/aeroscope/plugins/templates/aeroscope/main.html` & `astronomer_starship-1.0.2/astronomer/aeroscope/plugins/templates/aeroscope/main.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/aeroscope/util.py` & `astronomer_starship-1.0.2/astronomer/aeroscope/util.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/main.py` & `astronomer_starship-1.0.2/astronomer/starship/main.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/operators.py` & `astronomer_starship-1.0.2/astronomer/starship/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/services/astro_client.py` & `astronomer_starship-1.0.2/astronomer/starship/services/astro_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     if all_astro_deployments and all_astro_deployments.get(deployment):
         url = urlparse(all_astro_deployments[deployment]["webServerUrl"])
         return f"https:/{url.netloc}/{url.path}"
 
 
 def set_environment_variables(
-    deployment: str, token: str, remote_vars: Dict[Dict[str, Any]]
+    deployment: str, token: str, remote_vars: Dict[str, Dict[str, Any]]
 ):
     headers = {"Authorization": f"Bearer {token}"}
     client = GraphqlClient(endpoint=ASTROHUB_API, headers=headers)
     query = """
             fragment EnvironmentVariable on EnvironmentVariable {
                 key
                 value
```

### Comparing `astronomer_starship-1.0.1/astronomer/starship/services/local_airflow_client.py` & `astronomer_starship-1.0.2/astronomer/starship/services/local_airflow_client.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/services/remote_airflow_client.py` & `astronomer_starship-1.0.2/astronomer/starship/services/remote_airflow_client.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/static/js/htmx.min.js` & `astronomer_starship-1.0.2/astronomer/starship/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/static/js/idiomorph.min.js` & `astronomer_starship-1.0.2/astronomer/starship/static/js/idiomorph.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/static/js/popper.js` & `astronomer_starship-1.0.2/astronomer/starship/static/js/popper.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/static/js/tippy.js` & `astronomer_starship-1.0.2/astronomer/starship/static/js/tippy.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/static/tail-spin.svg` & `astronomer_starship-1.0.2/astronomer/starship/static/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/dag_row.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/dag_row.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/migrate_connection_button.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/migrate_connection_button.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/tabs.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/tabs_loading.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/tabs_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/target_deployment_select.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/target_deployment_select_loading.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/target_deployment_select_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/components/token_modal.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/components/token_modal.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/connections.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/connections.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/dags.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/dags.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/env.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/env.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/main.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/main.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/migration.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/migration.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/pools.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/pools.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/templates/starship/variables.html` & `astronomer_starship-1.0.2/astronomer/starship/templates/starship/variables.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/astronomer/starship/variables/operators.py` & `astronomer_starship-1.0.2/astronomer/starship/variables/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.1/pyproject.toml` & `astronomer_starship-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astronomer-starship"
-version = "1.0.1"
+version = "1.0.2"
 description = "Migrations to Astro"
 authors = ["ADE Team <ade@astronomer.io>"]
 readme = "README.rst"
 repository = "https://github.com/astronomer/starship"
 homepage = "https://astronomer.io"
 license = "Proprietary"
 packages = [{include = "astronomer"}]  #, from = "." }]
```

### Comparing `astronomer_starship-1.0.1/PKG-INFO` & `astronomer_starship-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-starship
-Version: 1.0.1
+Version: 1.0.2
 Summary: Migrations to Astro
 Home-page: https://astronomer.io
 License: Proprietary
 Author: ADE Team
 Author-email: ade@astronomer.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
```

