# Comparing `tmp/lab-partner-utils-0.7.55.tar.gz` & `tmp/lab-partner-utils-0.7.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-utils-0.7.55.tar", last modified: Mon Jun 12 02:02:19 2023, max compression
+gzip compressed data, was "lab-partner-utils-0.7.56.tar", last modified: Mon Jun 12 02:09:44 2023, max compression
```

## Comparing `lab-partner-utils-0.7.55.tar` & `lab-partner-utils-0.7.56.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.005402 lab-partner-utils-0.7.55/
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.001402 lab-partner-utils-0.7.55/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.001402 lab-partner-utils-0.7.55/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.github/workflows/build-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.001402 lab-partner-utils-0.7.55/.idea/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.001402 lab-partner-utils-0.7.55/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.idea/lab-partner-utils.iml
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 02:02:19.005402 lab-partner-utils-0.7.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (122)      253 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 02:02:19.005402 lab-partner-utils-0.7.55/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.001402 lab-partner-utils-0.7.55/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.005402 lab-partner-utils-0.7.55/src/lab_partner_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/src/lab_partner_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9051 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7252 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/src/lab_partner_utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 runner    (1001) docker     (122)    13028 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/src/lab_partner_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:02:19.005402 lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 02:02:18.000000 lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-12 02:02:18.000000 lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 02:02:18.000000 lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-12 02:02:18.000000 lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-12 02:02:18.000000 lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-12 02:02:18.000000 lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-12 02:01:55.000000 lab-partner-utils-0.7.55/workspace_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.github/workflows/build-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.idea/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/lab-partner-utils.iml
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      253 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.024878 lab-partner-utils-0.7.56/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/src/lab_partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9043 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7252 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13028 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 02:09:44.028878 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-12 02:09:44.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-12 02:09:43.000000 lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-12 02:09:13.000000 lab-partner-utils-0.7.56/workspace_commands.py
```

### Comparing `lab-partner-utils-0.7.55/.gitattributes` & `lab-partner-utils-0.7.56/.gitattributes`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/.github/workflows/build-deploy.yml` & `lab-partner-utils-0.7.56/.github/workflows/build-deploy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/.gitignore` & `lab-partner-utils-0.7.56/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/LICENSE.md` & `lab-partner-utils-0.7.56/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/PKG-INFO` & `lab-partner-utils-0.7.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.55
+Version: 0.7.56
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.55/pyproject.toml` & `lab-partner-utils-0.7.56/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-utils-0.7.56/src/lab_partner_utils/cli_command_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,16 @@
                         entry_point_metadata = WorkspaceEntryPointMetadata.build(entry_point_name, entry_point_value, project_name, project_version, project_path, project_data_path)
                         cli_plugins[entry_point_metadata.name] = entry_point_metadata
         return cli_plugins
 
     @staticmethod
     def check_for_entrypoint(entrypoint_name: str, project_toml: Dict[str, Any]) -> bool:
         return 'project' in project_toml \
-            and 'entry-points' not in project_toml['project'] \
-            and entrypoint_name not in project_toml['project']['entry-points']
+            and 'entry-points' in project_toml['project'] \
+            and entrypoint_name in project_toml['project']['entry-points']
 
     @staticmethod
     def _absolute_script_path(project_path: str, script_name: str) -> Optional[str]:
         """
         Walks the filesystem below the project path to resolve the absolute path of
         the script specified in the entry point
```

### Comparing `lab-partner-utils-0.7.55/src/lab_partner_utils/command_builder.py` & `lab-partner-utils-0.7.56/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/src/lab_partner_utils/commands.py` & `lab-partner-utils-0.7.56/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-utils-0.7.56/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/src/lab_partner_utils/utils.py` & `lab-partner-utils-0.7.56/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/PKG-INFO` & `lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.55
+Version: 0.7.56
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.55/src/lab_partner_utils.egg-info/SOURCES.txt` & `lab-partner-utils-0.7.56/src/lab_partner_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

