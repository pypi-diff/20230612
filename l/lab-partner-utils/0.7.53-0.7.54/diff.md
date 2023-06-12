# Comparing `tmp/lab-partner-utils-0.7.53.tar.gz` & `tmp/lab-partner-utils-0.7.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-utils-0.7.53.tar", last modified: Mon Jun 12 01:10:42 2023, max compression
+gzip compressed data, was "lab-partner-utils-0.7.54.tar", last modified: Mon Jun 12 01:25:34 2023, max compression
```

## Comparing `lab-partner-utils-0.7.53.tar` & `lab-partner-utils-0.7.54.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.629903 lab-partner-utils-0.7.53/
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.621903 lab-partner-utils-0.7.53/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.625903 lab-partner-utils-0.7.53/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.github/workflows/build-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.625903 lab-partner-utils-0.7.53/.idea/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.625903 lab-partner-utils-0.7.53/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.idea/lab-partner-utils.iml
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 01:10:42.629903 lab-partner-utils-0.7.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (122)      253 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 01:10:42.629903 lab-partner-utils-0.7.53/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.621903 lab-partner-utils-0.7.53/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.625903 lab-partner-utils-0.7.53/src/lab_partner_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/src/lab_partner_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8482 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7252 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/src/lab_partner_utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 runner    (1001) docker     (122)    13028 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/src/lab_partner_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:10:42.629903 lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 01:10:42.000000 lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-12 01:10:42.000000 lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 01:10:42.000000 lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-12 01:10:42.000000 lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-12 01:10:42.000000 lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-12 01:10:42.000000 lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-12 01:09:53.000000 lab-partner-utils-0.7.53/workspace_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.132887 lab-partner-utils-0.7.54/
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.128887 lab-partner-utils-0.7.54/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.128887 lab-partner-utils-0.7.54/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.github/workflows/build-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.128887 lab-partner-utils-0.7.54/.idea/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.132887 lab-partner-utils-0.7.54/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.idea/lab-partner-utils.iml
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 01:25:34.132887 lab-partner-utils-0.7.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      253 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-12 01:25:34.132887 lab-partner-utils-0.7.54/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.128887 lab-partner-utils-0.7.54/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.132887 lab-partner-utils-0.7.54/src/lab_partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7252 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/src/lab_partner_utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13028 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 01:25:34.132887 lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-06-12 01:25:34.000000 lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-12 01:25:34.000000 lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 01:25:34.000000 lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-12 01:25:34.000000 lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-12 01:25:34.000000 lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-12 01:25:34.000000 lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-12 01:25:06.000000 lab-partner-utils-0.7.54/workspace_commands.py
```

### Comparing `lab-partner-utils-0.7.53/.gitattributes` & `lab-partner-utils-0.7.54/.gitattributes`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/.github/workflows/build-deploy.yml` & `lab-partner-utils-0.7.54/.github/workflows/build-deploy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/.gitignore` & `lab-partner-utils-0.7.54/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/LICENSE.md` & `lab-partner-utils-0.7.54/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/PKG-INFO` & `lab-partner-utils-0.7.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.53
+Version: 0.7.54
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.53/pyproject.toml` & `lab-partner-utils-0.7.54/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-utils-0.7.54/src/lab_partner_utils/cli_command_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,23 +128,19 @@
                 continue
 
             with open(project_toml_path, "rb") as f:
                 project_toml = tomllib.load(f)
                 if 'project' not in project_toml \
                         or 'entry-points' not in project_toml['project'] \
                         or (CLI_PLUGINS_ENTRY_POINT not in project_toml['project']['entry-points']
-                            or CLI_WORKSPACE_ONLY_PLUGINS_ENTRY_POINT not in project_toml['project']['entry-points']):
+                            and CLI_WORKSPACE_ONLY_PLUGINS_ENTRY_POINT not in project_toml['project']['entry-points']):
                     logger.info(f'the project {project_name} does not have entrypoint')
                     continue
 
-                if 'version' not in project_toml['project']:
-                    logger.warning(f'The "version" attribute is required in pyproject.toml, skipping project {project_name}')
-                    continue
-
-                project_version = project_toml['project']['version']
+                project_version = "5"
                 found_entry_points = project_toml['project']['entry-points'][CLI_PLUGINS_ENTRY_POINT]
                 for entry_point_name, entry_point_value in found_entry_points.items():
                     entry_point_metadata = WorkspaceEntryPointMetadata.build(entry_point_name, entry_point_value, project_name, project_version, project_path, project_data_path)
                     cli_plugins[entry_point_metadata.name] = entry_point_metadata
         return cli_plugins
 
     @staticmethod
```

### Comparing `lab-partner-utils-0.7.53/src/lab_partner_utils/command_builder.py` & `lab-partner-utils-0.7.54/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/src/lab_partner_utils/commands.py` & `lab-partner-utils-0.7.54/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-utils-0.7.54/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/src/lab_partner_utils/utils.py` & `lab-partner-utils-0.7.54/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/PKG-INFO` & `lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.53
+Version: 0.7.54
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.53/src/lab_partner_utils.egg-info/SOURCES.txt` & `lab-partner-utils-0.7.54/src/lab_partner_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

