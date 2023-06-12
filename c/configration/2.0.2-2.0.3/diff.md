# Comparing `tmp/configration-2.0.2.tar.gz` & `tmp/configration-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-2.0.2.tar", last modified: Mon May 29 11:34:47 2023, max compression
+gzip compressed data, was "configration-2.0.3.tar", last modified: Mon Jun 12 13:01:34 2023, max compression
```

## Comparing `configration-2.0.2.tar` & `configration-2.0.3.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.2/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      882 2023-05-29 11:34:47.261345 configration-2.0.2/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.2/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.258012 configration-2.0.2/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.2/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-29 11:22:41.000000 configration-2.0.2/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.2/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1951 2023-05-29 11:33:46.000000 configration-2.0.2/configration/src/config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.2/configration/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      952 2023-05-28 09:53:21.000000 configration-2.0.2/configration/src/json_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      948 2023-05-28 09:52:59.000000 configration-2.0.2/configration/src/toml_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/configration/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.2/configration/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1696 2023-05-29 09:29:59.000000 configration-2.0.2/configration/tests/test_json.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1696 2023-05-29 09:31:39.000000 configration-2.0.2/configration/tests/test_toml.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.258012 configration-2.0.2/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      882 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      498 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-29 11:34:47.261345 configration-2.0.2/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.2/setup.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      205 2023-05-26 07:00:53.000000 configration-2.0.2/tests/test_json.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.114670 configration-2.0.3/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.3/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1019 2023-06-12 13:01:34.114670 configration-2.0.3/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.3/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.108003 configration-2.0.3/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.3/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-09 06:22:46.000000 configration-2.0.3/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.114670 configration-2.0.3/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.3/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2228 2023-06-09 11:25:05.000000 configration-2.0.3/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.3/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-09 14:31:15.000000 configration-2.0.3/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2779 2023-06-09 11:37:05.000000 configration-2.0.3/configration/src/toml_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.114670 configration-2.0.3/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.3/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2848 2023-06-09 14:35:21.000000 configration-2.0.3/configration/tests/test_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.108003 configration-2.0.3/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1019 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      449 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-12 13:01:34.114670 configration-2.0.3/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.3/setup.py
```

### Comparing `configration-2.0.2/LICENSE.txt` & `configration-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.2/PKG-INFO` & `configration-2.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.2
+Version: 2.0.3
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
-Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
+Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # configration
 
 A module to validate and load config files.
 
@@ -20,20 +21,29 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.3 9 June 2023
+
+1. Implement create()
+2. Implement save()
+3. Consolidated testing into one file
+
+------
+
 Version 1.0.2 29 May 2023
 
 1. Provide __repr__
 
 ------
 
+
 Version 1.0.1 29 May 2023
 
 1. Expose TomlConfig
 
 ------
 
 Version 1.0.0 29 May 2023
@@ -50,7 +60,9 @@
 ------
 
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
+
+
```

### Comparing `configration-2.0.2/configration/src/config.py` & `configration-2.0.3/configration/src/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,19 +19,27 @@
         The path to the config file
 
     attrs: dict[str, list[type]
         The dict keys are the fields that are expected in the config json
         The dict item holds a list of allowed types for each files
 
         If there are attrs, then the config is validated.
+
+    create: bool
+        Whether or not the config should be created if missing.
+        Defaults to False.
+        (The individual sub-classes implement the function.)
     """
 
-    def __init__(self, path: str, attrs: dict[str, list[type]] = {}):
+    def __init__(self, path: str,
+                 attrs: dict[str, list[type]] = {},
+                 create: bool = False):
         self.path = path
         self.attrs = attrs
+        self.create = create
         self.config = self._get_config()
         for key, item in self.config.items():
             self.__dict__[key] = item
 
     def __repr__(self):
         if not self.attrs:
             return str(self.__dict__)
@@ -40,18 +48,18 @@
             output .append(f'{key}, {self.__dict__[key]}')
         return '\n'.join(output)
 
     def _get_config(self) -> dict[str, object]:
         # Return config, if contents are valid.
         config = self._read_config()
 
-        if not self.attrs:
+        if config and not self.attrs:
             return config
 
-        if self._validate_config(config):
+        if config and self._validate_config(config):
             return config
         return {}
 
     def _validate_config(self, config: dict[str, type]) -> bool:
         # Return True if structure and values in config are valid.
         for name, item_types in self.attrs.items():
             if name not in config:
```

### Comparing `configration-2.0.2/configration.egg-info/PKG-INFO` & `configration-2.0.3/configration.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.2
+Version: 2.0.3
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
-Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
+Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # configration
 
 A module to validate and load config files.
 
@@ -20,20 +21,29 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.3 9 June 2023
+
+1. Implement create()
+2. Implement save()
+3. Consolidated testing into one file
+
+------
+
 Version 1.0.2 29 May 2023
 
 1. Provide __repr__
 
 ------
 
+
 Version 1.0.1 29 May 2023
 
 1. Expose TomlConfig
 
 ------
 
 Version 1.0.0 29 May 2023
@@ -50,7 +60,9 @@
 ------
 
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
+
+
```

### Comparing `configration-2.0.2/setup.py` & `configration-2.0.3/setup.py`

 * *Files identical despite different names*

