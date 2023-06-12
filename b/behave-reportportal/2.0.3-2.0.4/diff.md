# Comparing `tmp/behave-reportportal-2.0.3.tar.gz` & `tmp/behave-reportportal-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behave-reportportal-2.0.3.tar", last modified: Thu Mar 30 14:39:07 2023, max compression
+gzip compressed data, was "behave-reportportal-2.0.4.tar", last modified: Mon Jun 12 12:11:33 2023, max compression
```

## Comparing `behave-reportportal-2.0.3.tar` & `behave-reportportal-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:39:07.522197 behave-reportportal-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-03-30 14:39:07.526197 behave-reportportal-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:39:07.522197 behave-reportportal-2.0.3/behave_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/behave_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/behave_reportportal/behave_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/behave_reportportal/behave_agent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/behave_reportportal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/behave_reportportal/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/behave_reportportal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 14:39:07.522197 behave-reportportal-2.0.3/behave_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-03-30 14:39:07.000000 behave-reportportal-2.0.3/behave_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-30 14:39:07.000000 behave-reportportal-2.0.3/behave_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 14:39:07.000000 behave-reportportal-2.0.3/behave_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 14:39:07.000000 behave-reportportal-2.0.3/behave_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 14:39:07.000000 behave-reportportal-2.0.3/behave_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-30 14:39:07.526197 behave-reportportal-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-30 14:39:02.000000 behave-reportportal-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/behave_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/behave_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/behave_agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/behave_reportportal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/behave_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 12:11:33.000000 behave-reportportal-2.0.4/behave_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 12:11:33.963541 behave-reportportal-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-12 12:11:28.000000 behave-reportportal-2.0.4/setup.py
```

### Comparing `behave-reportportal-2.0.3/LICENSE` & `behave-reportportal-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.3/PKG-INFO` & `behave-reportportal-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-reportportal
-Version: 2.0.3
+Version: 2.0.4
 Summary: Agent for reporting Behave results to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-behave
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,behave
 Classifier: Programming Language :: Python :: 3.6
@@ -68,24 +68,24 @@
 .. code-block:: bash
 
     behave -D config_file=<path_to_config_file>
 
 
 The :code:`behave.ini` file should have next mandatory fields under [report_portal] section:
 
-- :code:`token` - value could be found in the User Profile section
+- :code:`api_key` - value could be found in the User Profile section
 - :code:`project` - name of project in Report Portal
 - :code:`endpoint` - address of Report Portal Server
 
 Example of :code:`behave.ini`:
 
 .. code-block:: text
 
     [report_portal]
-    token = fb586627-32be-47dd-93c1-678873458a5f
+    api_key = fb586627-32be-47dd-93c1-678873458a5f
     endpoint = http://192.168.1.10:8080
     project = user_personal
     launch_name = AnyLaunchName
     launch_attributes = Slow Smoke
     launch_description = Smoke test
 
 The following parameters are optional:
```

### Comparing `behave-reportportal-2.0.3/README.rst` & `behave-reportportal-2.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -50,24 +50,24 @@
 .. code-block:: bash
 
     behave -D config_file=<path_to_config_file>
 
 
 The :code:`behave.ini` file should have next mandatory fields under [report_portal] section:
 
-- :code:`token` - value could be found in the User Profile section
+- :code:`api_key` - value could be found in the User Profile section
 - :code:`project` - name of project in Report Portal
 - :code:`endpoint` - address of Report Portal Server
 
 Example of :code:`behave.ini`:
 
 .. code-block:: text
 
     [report_portal]
-    token = fb586627-32be-47dd-93c1-678873458a5f
+    api_key = fb586627-32be-47dd-93c1-678873458a5f
     endpoint = http://192.168.1.10:8080
     project = user_personal
     launch_name = AnyLaunchName
     launch_attributes = Slow Smoke
     launch_description = Smoke test
 
 The following parameters are optional:
```

### Comparing `behave-reportportal-2.0.3/behave_reportportal/__init__.py` & `behave-reportportal-2.0.4/behave_reportportal/__init__.py`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.3/behave_reportportal/behave_agent.py` & `behave-reportportal-2.0.4/behave_reportportal/behave_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 def create_rp_service(cfg):
     """Create instance of ReportPortalService."""
     if cfg.enabled:
         return RPClient(
             endpoint=cfg.endpoint,
             project=cfg.project,
-            token=cfg.token,
+            api_key=cfg.api_key,
             is_skipped_an_issue=cfg.is_skipped_an_issue,
             launch_id=cfg.launch_id,
             retries=cfg.retries,
             mode="DEBUG" if cfg.debug_mode else "DEFAULT",
             log_batch_size=cfg.log_batch_size,
             log_batch_payload_size=cfg.log_batch_payload_size
         )
@@ -243,16 +243,17 @@
             level=level,
             attachment=attachment,
             item_id=item_id,
         )
 
     def _get_launch_attributes(self):
         """Return launch attributes in the format supported by the rp."""
-        attributes = gen_attributes(self._cfg.launch_attributes) \
-            if self._cfg.launch_attributes else []
+        launch_attributes = self._cfg.launch_attributes
+        attributes = gen_attributes(
+            launch_attributes) if launch_attributes else []
         system_attributes = get_launch_sys_attrs()
         system_attributes["agent"] = f"{self.agent_name}|{self.agent_version}"
         return attributes + dict_to_payload(system_attributes)
 
     @staticmethod
     def _build_step_content(step):
         txt = ""
```

### Comparing `behave-reportportal-2.0.3/behave_reportportal/behave_agent.pyi` & `behave-reportportal-2.0.4/behave_reportportal/behave_agent.pyi`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.3/behave_reportportal/config.py` & `behave-reportportal-2.0.4/behave_reportportal/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License
 
 from configparser import ConfigParser
 from enum import Enum
-from warnings import simplefilter, warn
+from warnings import warn
 
 from reportportal_client.logs.log_manager import MAX_LOG_BATCH_PAYLOAD_SIZE
 
 RP_CFG_SECTION = "report_portal"
 DEFAULT_LAUNCH_NAME = "Python Behave Launch"
 DEFAULT_CFG_FILE = "behave.ini"
 
@@ -44,15 +44,15 @@
 class Config(object):
     """Class for configuration of behave Report Portal agent."""
 
     def __init__(
             self,
             endpoint=None,
             project=None,
-            token=None,
+            api_key=None,
             launch_id=None,
             launch_name=None,
             launch_description=None,
             launch_attributes=None,
             debug_mode=None,
             log_layout=None,
             step_based=None,
@@ -63,16 +63,14 @@
             log_batch_size=None,
             log_batch_payload_size=None,
             **kwargs
     ):
         """Initialize instance attributes."""
         self.endpoint = endpoint
         self.project = project
-        self.token = token
-        self.enabled = all([self.endpoint, self.project, self.token])
         self.launch_id = launch_id
         self.launch_name = launch_name or DEFAULT_LAUNCH_NAME
         self.launch_description = launch_description
         self.launch_attributes = launch_attributes and launch_attributes.split(
             " "
         )
         self.debug_mode = get_bool(debug_mode) or False
@@ -82,37 +80,59 @@
         self.rerun_of = rerun_of
         self.log_batch_size = (log_batch_size and int(
             log_batch_size)) or 20
         self.log_batch_payload_size = (log_batch_payload_size and int(
             log_batch_payload_size)) or MAX_LOG_BATCH_PAYLOAD_SIZE
 
         if step_based and not log_layout:
-            simplefilter("default")
             warn(
                 "'step_based' config setting has been deprecated"
                 "in favor of the new log_layout configuration.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             self.log_layout = (
                 LogLayout.STEP if get_bool(step_based) else LogLayout.SCENARIO
             )
         else:
             self.log_layout = LogLayout(log_layout)
 
+        self.api_key = api_key
+        if not self.api_key:
+            if 'token' in kwargs:
+                warn(
+                    message="Argument `token` is deprecated since 2.0.4 and "
+                            "will be subject for removing in the next major "
+                            "version. Use `api_key` argument instead.",
+                    category=DeprecationWarning,
+                    stacklevel=2
+                )
+                self.api_key = kwargs['token']
+
+            if not self.api_key:
+                warn(
+                    message="Argument `api_key` is `None` or empty string, "
+                            "that's not supposed to happen because Report "
+                            "Portal is usually requires an authorization key. "
+                            "Please check your code.",
+                    category=RuntimeWarning,
+                    stacklevel=2
+                )
+        self.enabled = all([self.endpoint, self.project, self.api_key])
+
 
 def read_config(context):
     """Read config from file and return instance of Config."""
     cp = ConfigParser()
     cmd_data = context._config.userdata
     path = cmd_data.get("config_file")
     cp.read(path or DEFAULT_CFG_FILE)
     rp_cfg = {}
     if cp.has_section(RP_CFG_SECTION):
-        rp_cfg = cp[RP_CFG_SECTION]
+        rp_cfg.update(cp[RP_CFG_SECTION])
     rp_cfg.update(cmd_data)
 
     return Config(**rp_cfg)
 
 
 def get_bool(value):
     """Convert string value to bool."""
```

### Comparing `behave-reportportal-2.0.3/behave_reportportal/config.pyi` & `behave-reportportal-2.0.4/behave_reportportal/config.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     STEP = ...
     NESTED = ...
 
 
 class Config(object):
     endpoint: Optional[str]
     project: Optional[str]
-    token: Optional[str]
+    api_key: Optional[str]
     enabled: bool
     launch_id: Optional[str]
     launch_name: str
     launch_description: Optional[str]
     launch_attributes: Optional[List[str]]
     debug_mode: bool
     is_skipped_an_issue: bool
@@ -44,15 +44,15 @@
     log_batch_payload_size: int
     log_layout: LogLayout
 
     def __init__(
             self,
             endpoint: Optional[str] = ...,
             project: Optional[str] = ...,
-            token: Optional[str] = ...,
+            api_key: Optional[str] = ...,
             launch_id: Optional[str] = ...,
             launch_name: Optional[str] = ...,
             launch_description: Optional[str] = ...,
             launch_attributes: Optional[str] = ...,
             debug_mode: Optional[Union[str, bool]] = ...,
             log_layout: Optional[Union[str, LogLayout]] = ...,
             step_based: Optional[str] = ...,
```

### Comparing `behave-reportportal-2.0.3/behave_reportportal/utils.py` & `behave-reportportal-2.0.4/behave_reportportal/utils.py`

 * *Files identical despite different names*

### Comparing `behave-reportportal-2.0.3/behave_reportportal.egg-info/PKG-INFO` & `behave-reportportal-2.0.4/behave_reportportal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-reportportal
-Version: 2.0.3
+Version: 2.0.4
 Summary: Agent for reporting Behave results to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-behave
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,behave
 Classifier: Programming Language :: Python :: 3.6
@@ -68,24 +68,24 @@
 .. code-block:: bash
 
     behave -D config_file=<path_to_config_file>
 
 
 The :code:`behave.ini` file should have next mandatory fields under [report_portal] section:
 
-- :code:`token` - value could be found in the User Profile section
+- :code:`api_key` - value could be found in the User Profile section
 - :code:`project` - name of project in Report Portal
 - :code:`endpoint` - address of Report Portal Server
 
 Example of :code:`behave.ini`:
 
 .. code-block:: text
 
     [report_portal]
-    token = fb586627-32be-47dd-93c1-678873458a5f
+    api_key = fb586627-32be-47dd-93c1-678873458a5f
     endpoint = http://192.168.1.10:8080
     project = user_personal
     launch_name = AnyLaunchName
     launch_attributes = Slow Smoke
     launch_description = Smoke test
 
 The following parameters are optional:
```

### Comparing `behave-reportportal-2.0.3/setup.py` & `behave-reportportal-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Config for setup package behave agent."""
 
 import os
 
 from setuptools import setup
 
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Filename to be read
     :return: File content
```

