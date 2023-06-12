# Comparing `tmp/shortloop_python-0.1.0.tar.gz` & `tmp/shortloop_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortloop_python-0.1.0.tar", max compression
+gzip compressed data, was "shortloop_python-0.1.1.tar", max compression
```

## Comparing `shortloop_python-0.1.0.tar` & `shortloop_python-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      439 2023-05-25 09:26:48.777248 shortloop_python-0.1.0/README.md
--rw-r--r--   0        0        0     1220 2023-05-25 09:27:30.437240 shortloop_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-05-25 09:20:28.777239 shortloop_python-0.1.0/shortloop_python/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/__init__.py
--rw-r--r--   0        0        0     1617 2023-05-24 06:00:11.057621 shortloop_python-0.1.0/shortloop_python/core/always_capture_sync.py
--rw-r--r--   0        0        0     6347 2023-05-25 09:20:28.857239 shortloop_python-0.1.0/shortloop_python/core/api_processor.py
--rw-r--r--   0        0        0     3118 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/auto_configuration.py
--rw-r--r--   0        0        0     1765 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/buffer/abstract_buffer_manager.py
--rw-r--r--   0        0        0      842 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/buffer/api_buffer_key.py
--rw-r--r--   0        0        0      404 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/buffer/buffer.py
--rw-r--r--   0        0        0     1908 2023-05-25 09:20:28.807239 shortloop_python-0.1.0/shortloop_python/core/buffer/buffer_manager_worker.py
--rw-r--r--   0        0        0     3111 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/buffer/discovered_buffer_manager.py
--rw-r--r--   0        0        0      548 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/buffer/no_op_buffer_manager.py
--rw-r--r--   0        0        0     4027 2023-05-18 17:45:18.316638 shortloop_python-0.1.0/shortloop_python/core/buffer/registered_buffer_manager.py
--rw-r--r--   0        0        0      832 2023-05-25 09:20:38.350575 shortloop_python-0.1.0/shortloop_python/core/buffer/simple_buffer.py
--rw-r--r--   0        0        0      373 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/config/config_manager.py
--rw-r--r--   0        0        0      316 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/config/config_update_listener.py
--rw-r--r--   0        0        0     1921 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/config/config_validators.py
--rw-r--r--   0        0        0     4233 2023-05-18 12:27:01.200735 shortloop_python-0.1.0/shortloop_python/core/config/simple_config_manager.py
--rw-r--r--   0        0        0      140 2023-05-25 09:20:28.797239 shortloop_python-0.1.0/shortloop_python/core/constant/__init__.py
--rw-r--r--   0        0        0      207 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/constant/http_method.py
--rw-r--r--   0        0        0      156 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/constant/segment_template_type.py
--rw-r--r--   0        0        0      163 2023-05-25 09:20:28.803906 shortloop_python-0.1.0/shortloop_python/core/filter/__init__.py
--rw-r--r--   0        0        0     1148 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/filter/always_capture_filter.py
--rw-r--r--   0        0        0     3041 2023-05-18 09:07:12.918937 shortloop_python-0.1.0/shortloop_python/core/filter/filter.py
--rw-r--r--   0        0        0      271 2023-05-25 09:20:28.807239 shortloop_python-0.1.0/shortloop_python/core/http/__init__.py
--rw-r--r--   0        0        0     2845 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/http/context.py
--rw-r--r--   0        0        0     5232 2023-05-23 13:36:11.628041 shortloop_python-0.1.0/shortloop_python/core/http/http_connection.py
--rw-r--r--   0        0        0     1260 2023-05-25 09:20:20.800570 shortloop_python-0.1.0/shortloop_python/core/http/http_request.py
--rw-r--r--   0        0        0      267 2023-05-18 14:40:16.839083 shortloop_python-0.1.0/shortloop_python/core/http/http_response.py
--rw-r--r--   0        0        0      350 2023-05-25 09:20:28.820572 shortloop_python-0.1.0/shortloop_python/core/model/__init__.py
--rw-r--r--   0        0        0     2044 2023-05-18 18:31:51.176937 shortloop_python-0.1.0/shortloop_python/core/model/agent_config.py
--rw-r--r--   0        0        0      692 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/model/api_config.py
--rw-r--r--   0        0        0     3277 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/model/api_sample.py
--rw-r--r--   0        0        0     1122 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/model/black_list_rule.py
--rw-r--r--   0        0        0      536 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/model/observed_api.py
--rw-r--r--   0        0        0     2068 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/model/sdk_options.py
--rw-r--r--   0        0        0     1955 2023-05-18 07:47:31.304319 shortloop_python-0.1.0/shortloop_python/core/model/uri.py
--rw-r--r--   0        0        0      199 2023-05-18 07:47:31.307653 shortloop_python-0.1.0/shortloop_python/core/scheduled_timer.py
--rw-r--r--   0        0        0     2085 2023-05-25 09:20:28.850572 shortloop_python-0.1.0/shortloop_python/core/shortlook_sdk.py
--rw-r--r--   0        0        0     1184 2023-05-18 07:47:31.307653 shortloop_python-0.1.0/shortloop_python/core/util/filter_utils.py
--rw-r--r--   0        0        0      420 2023-05-18 07:47:31.307653 shortloop_python-0.1.0/shortloop_python/core/util/masking_utils.py
--rw-r--r--   0        0        0      929 2023-05-18 07:47:31.307653 shortloop_python-0.1.0/shortloop_python/core/util/uri_utils.py
--rw-r--r--   0        0        0       87 2023-05-25 09:20:28.840572 shortloop_python-0.1.0/shortloop_python/integrations/__init__.py
--rw-r--r--   0        0        0     2255 2023-05-18 14:40:16.842416 shortloop_python-0.1.0/shortloop_python/integrations/django.py
--rw-r--r--   0        0        0      558 2023-05-19 07:57:55.836642 shortloop_python-0.1.0/shortloop_python/sdk_logger.py
--rw-r--r--   0        0        0      152 2023-05-18 07:47:31.307653 shortloop_python-0.1.0/shortloop_python/sdk_version.py
--rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 shortloop_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      439 2023-06-12 11:23:58.944592 shortloop_python-0.1.1/README.md
+-rw-r--r--   0        0        0     1220 2023-06-12 11:35:23.558860 shortloop_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-06-12 11:23:58.945584 shortloop_python-0.1.1/shortloop_python/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:23:58.945789 shortloop_python-0.1.1/shortloop_python/core/__init__.py
+-rw-r--r--   0        0        0     1617 2023-06-12 11:23:58.946003 shortloop_python-0.1.1/shortloop_python/core/always_capture_sync.py
+-rw-r--r--   0        0        0     6347 2023-06-12 11:23:58.946179 shortloop_python-0.1.1/shortloop_python/core/api_processor.py
+-rw-r--r--   0        0        0     3118 2023-06-12 11:23:58.946336 shortloop_python-0.1.1/shortloop_python/core/auto_configuration.py
+-rw-r--r--   0        0        0     1765 2023-06-12 11:23:58.946538 shortloop_python-0.1.1/shortloop_python/core/buffer/abstract_buffer_manager.py
+-rw-r--r--   0        0        0      842 2023-06-12 11:23:58.946678 shortloop_python-0.1.1/shortloop_python/core/buffer/api_buffer_key.py
+-rw-r--r--   0        0        0      404 2023-06-12 11:23:58.946866 shortloop_python-0.1.1/shortloop_python/core/buffer/buffer.py
+-rw-r--r--   0        0        0     1908 2023-06-12 11:23:58.947004 shortloop_python-0.1.1/shortloop_python/core/buffer/buffer_manager_worker.py
+-rw-r--r--   0        0        0     3111 2023-06-12 11:23:58.947157 shortloop_python-0.1.1/shortloop_python/core/buffer/discovered_buffer_manager.py
+-rw-r--r--   0        0        0      548 2023-06-12 11:23:58.947291 shortloop_python-0.1.1/shortloop_python/core/buffer/no_op_buffer_manager.py
+-rw-r--r--   0        0        0     4027 2023-06-12 11:23:58.947419 shortloop_python-0.1.1/shortloop_python/core/buffer/registered_buffer_manager.py
+-rw-r--r--   0        0        0      832 2023-06-12 11:23:58.947572 shortloop_python-0.1.1/shortloop_python/core/buffer/simple_buffer.py
+-rw-r--r--   0        0        0      373 2023-06-12 11:23:58.947779 shortloop_python-0.1.1/shortloop_python/core/config/config_manager.py
+-rw-r--r--   0        0        0      316 2023-06-12 11:23:58.947921 shortloop_python-0.1.1/shortloop_python/core/config/config_update_listener.py
+-rw-r--r--   0        0        0     1921 2023-06-12 11:23:58.948077 shortloop_python-0.1.1/shortloop_python/core/config/config_validators.py
+-rw-r--r--   0        0        0     4233 2023-06-12 11:23:58.948247 shortloop_python-0.1.1/shortloop_python/core/config/simple_config_manager.py
+-rw-r--r--   0        0        0      140 2023-06-12 11:23:58.948592 shortloop_python-0.1.1/shortloop_python/core/constant/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-12 11:23:58.948773 shortloop_python-0.1.1/shortloop_python/core/constant/http_method.py
+-rw-r--r--   0        0        0      156 2023-06-12 11:23:58.949037 shortloop_python-0.1.1/shortloop_python/core/constant/segment_template_type.py
+-rw-r--r--   0        0        0      163 2023-06-12 11:23:58.949294 shortloop_python-0.1.1/shortloop_python/core/filter/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-12 11:23:58.949442 shortloop_python-0.1.1/shortloop_python/core/filter/always_capture_filter.py
+-rw-r--r--   0        0        0     3041 2023-06-12 11:23:58.949593 shortloop_python-0.1.1/shortloop_python/core/filter/filter.py
+-rw-r--r--   0        0        0      271 2023-06-12 11:23:58.949807 shortloop_python-0.1.1/shortloop_python/core/http/__init__.py
+-rw-r--r--   0        0        0     2845 2023-06-12 11:23:58.949952 shortloop_python-0.1.1/shortloop_python/core/http/context.py
+-rw-r--r--   0        0        0     5232 2023-06-12 11:23:58.950111 shortloop_python-0.1.1/shortloop_python/core/http/http_connection.py
+-rw-r--r--   0        0        0     1260 2023-06-12 11:23:58.950257 shortloop_python-0.1.1/shortloop_python/core/http/http_request.py
+-rw-r--r--   0        0        0      267 2023-06-12 11:23:58.950434 shortloop_python-0.1.1/shortloop_python/core/http/http_response.py
+-rw-r--r--   0        0        0      350 2023-06-12 11:23:58.950634 shortloop_python-0.1.1/shortloop_python/core/model/__init__.py
+-rw-r--r--   0        0        0     2044 2023-06-12 11:23:58.950778 shortloop_python-0.1.1/shortloop_python/core/model/agent_config.py
+-rw-r--r--   0        0        0      692 2023-06-12 11:23:58.950913 shortloop_python-0.1.1/shortloop_python/core/model/api_config.py
+-rw-r--r--   0        0        0     3277 2023-06-12 11:23:58.951048 shortloop_python-0.1.1/shortloop_python/core/model/api_sample.py
+-rw-r--r--   0        0        0     1122 2023-06-12 11:23:58.951183 shortloop_python-0.1.1/shortloop_python/core/model/black_list_rule.py
+-rw-r--r--   0        0        0      536 2023-06-12 11:23:58.951348 shortloop_python-0.1.1/shortloop_python/core/model/observed_api.py
+-rw-r--r--   0        0        0     2068 2023-06-12 11:23:58.951520 shortloop_python-0.1.1/shortloop_python/core/model/sdk_options.py
+-rw-r--r--   0        0        0     1955 2023-06-12 11:23:58.951686 shortloop_python-0.1.1/shortloop_python/core/model/uri.py
+-rw-r--r--   0        0        0      199 2023-06-12 11:23:58.951820 shortloop_python-0.1.1/shortloop_python/core/scheduled_timer.py
+-rw-r--r--   0        0        0     2101 2023-06-12 11:23:58.951966 shortloop_python-0.1.1/shortloop_python/core/shortlook_sdk.py
+-rw-r--r--   0        0        0     1184 2023-06-12 11:23:58.952193 shortloop_python-0.1.1/shortloop_python/core/util/filter_utils.py
+-rw-r--r--   0        0        0      420 2023-06-12 11:23:58.952340 shortloop_python-0.1.1/shortloop_python/core/util/masking_utils.py
+-rw-r--r--   0        0        0      929 2023-06-12 11:23:58.952476 shortloop_python-0.1.1/shortloop_python/core/util/uri_utils.py
+-rw-r--r--   0        0        0       87 2023-06-12 11:23:58.952669 shortloop_python-0.1.1/shortloop_python/integrations/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-12 11:23:58.952960 shortloop_python-0.1.1/shortloop_python/integrations/django.py
+-rw-r--r--   0        0        0      558 2023-06-12 11:23:58.953206 shortloop_python-0.1.1/shortloop_python/sdk_logger.py
+-rw-r--r--   0        0        0      152 2023-06-12 11:23:58.953369 shortloop_python-0.1.1/shortloop_python/sdk_version.py
+-rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 shortloop_python-0.1.1/PKG-INFO
```

### Comparing `shortloop_python-0.1.0/pyproject.toml` & `shortloop_python-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shortloop-python"
-version = "0.1.0"
+version = "0.1.1"
 description = "Official Shortloop SDK for Python"
 authors = ["ShortLoop <hello@shortloop.dev>"]
 maintainers = ["ShortLoop <hello@shortloop.dev>"]
 homepage = "https://shortloop.dev"
 documentation = "https://docs.shortloop.dev"
 readme = "README.md"
 packages = [{include = "shortloop_python"}]
```

### Comparing `shortloop_python-0.1.0/shortloop_python/core/always_capture_sync.py` & `shortloop_python-0.1.1/shortloop_python/core/always_capture_sync.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/api_processor.py` & `shortloop_python-0.1.1/shortloop_python/core/api_processor.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/auto_configuration.py` & `shortloop_python-0.1.1/shortloop_python/core/auto_configuration.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/buffer/abstract_buffer_manager.py` & `shortloop_python-0.1.1/shortloop_python/core/buffer/abstract_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/buffer/api_buffer_key.py` & `shortloop_python-0.1.1/shortloop_python/core/buffer/api_buffer_key.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/buffer/buffer_manager_worker.py` & `shortloop_python-0.1.1/shortloop_python/core/buffer/buffer_manager_worker.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/buffer/discovered_buffer_manager.py` & `shortloop_python-0.1.1/shortloop_python/core/buffer/discovered_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/buffer/no_op_buffer_manager.py` & `shortloop_python-0.1.1/shortloop_python/core/buffer/no_op_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/buffer/registered_buffer_manager.py` & `shortloop_python-0.1.1/shortloop_python/core/buffer/registered_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/buffer/simple_buffer.py` & `shortloop_python-0.1.1/shortloop_python/core/buffer/simple_buffer.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/config/config_validators.py` & `shortloop_python-0.1.1/shortloop_python/core/config/config_validators.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/config/simple_config_manager.py` & `shortloop_python-0.1.1/shortloop_python/core/config/simple_config_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/filter/always_capture_filter.py` & `shortloop_python-0.1.1/shortloop_python/core/filter/always_capture_filter.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/filter/filter.py` & `shortloop_python-0.1.1/shortloop_python/core/filter/filter.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/http/context.py` & `shortloop_python-0.1.1/shortloop_python/core/http/context.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/http/http_connection.py` & `shortloop_python-0.1.1/shortloop_python/core/http/http_connection.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/http/http_request.py` & `shortloop_python-0.1.1/shortloop_python/core/http/http_request.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/model/agent_config.py` & `shortloop_python-0.1.1/shortloop_python/core/model/agent_config.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/model/api_config.py` & `shortloop_python-0.1.1/shortloop_python/core/model/api_config.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/model/api_sample.py` & `shortloop_python-0.1.1/shortloop_python/core/model/api_sample.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/model/black_list_rule.py` & `shortloop_python-0.1.1/shortloop_python/core/model/black_list_rule.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/model/observed_api.py` & `shortloop_python-0.1.1/shortloop_python/core/model/observed_api.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/model/sdk_options.py` & `shortloop_python-0.1.1/shortloop_python/core/model/sdk_options.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/model/uri.py` & `shortloop_python-0.1.1/shortloop_python/core/model/uri.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/shortlook_sdk.py` & `shortloop_python-0.1.1/shortloop_python/core/shortlook_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     :param list(int) mask_headers: Headers names (case in-sensitive) that will be masked at the SDK level itself.
         Masking will happen locally before data is sent to ShortLoop servers. Ex: ["cookie", "x-auth"]
 
     :param str capture: TEST MODE
     """
     global options, initialized, auto_configuration
 
+    if 'check' in sys.argv:
+        return
+
     if not initialized:
         initialized = True
 
         opts: SdkOptions = SdkOptions(
             url, application_name, auth_key, environment, logging_enabled, log_level, mask_headers, capture
         )
         opts.sanitize()
@@ -57,8 +60,8 @@
             return
 
         options = opts
 
         auto_configuration = ShortLoopAutoConfiguration(opts=opts)
         auto_configuration.init()
 
-        print("ShortLoop Initialized with options: " + str(options))
+        print("ShortLoop Initialized !")
```

### Comparing `shortloop_python-0.1.0/shortloop_python/core/util/filter_utils.py` & `shortloop_python-0.1.1/shortloop_python/core/util/filter_utils.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/core/util/uri_utils.py` & `shortloop_python-0.1.1/shortloop_python/core/util/uri_utils.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/integrations/django.py` & `shortloop_python-0.1.1/shortloop_python/integrations/django.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/shortloop_python/sdk_logger.py` & `shortloop_python-0.1.1/shortloop_python/sdk_logger.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.0/PKG-INFO` & `shortloop_python-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortloop-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Official Shortloop SDK for Python
 Home-page: https://shortloop.dev
 Keywords: shortloop,middleware
 Author: ShortLoop
 Author-email: hello@shortloop.dev
 Maintainer: ShortLoop
 Maintainer-email: hello@shortloop.dev
```

