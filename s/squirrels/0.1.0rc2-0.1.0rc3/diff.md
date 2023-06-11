# Comparing `tmp/squirrels-0.1.0rc2.tar.gz` & `tmp/squirrels-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrels-0.1.0rc2.tar", last modified: Fri May  5 13:53:39 2023, max compression
+gzip compressed data, was "squirrels-0.1.0rc3.tar", last modified: Tue May  9 13:29:55 2023, max compression
```

## Comparing `squirrels-0.1.0rc2.tar` & `squirrels-0.1.0rc3.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.488018 squirrels-0.1.0rc2/
--rw-rw-rw-   0        0        0     1088 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/LICENSE
--rw-rw-rw-   0        0        0     2056 2023-05-05 13:53:39.486023 squirrels-0.1.0rc2/PKG-INFO
--rw-rw-rw-   0        0        0     1799 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 13:53:39.488018 squirrels-0.1.0rc2/setup.cfg
--rw-rw-rw-   0        0        0     1410 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.392023 squirrels-0.1.0rc2/squirrels/
--rw-rw-rw-   0        0        0     1007 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/__init__.py
--rw-rw-rw-   0        0        0     5737 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/_command_line.py
--rw-rw-rw-   0        0        0     6174 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/api_server.py
--rw-rw-rw-   0        0        0     2269 2023-05-05 13:20:06.000000 squirrels-0.1.0rc2/squirrels/connection_set.py
--rw-rw-rw-   0        0        0     1596 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/constants.py
--rw-rw-rw-   0        0        0     3059 2023-04-22 22:12:54.000000 squirrels-0.1.0rc2/squirrels/credentials_manager.py
--rw-rw-rw-   0        0        0     8682 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/dateutils.py
--rw-rw-rw-   0        0        0     4283 2023-04-23 00:07:17.000000 squirrels-0.1.0rc2/squirrels/initializer.py
--rw-rw-rw-   0        0        0     5209 2023-04-23 23:15:04.000000 squirrels-0.1.0rc2/squirrels/manifest.py
--rw-rw-rw-   0        0        0     1261 2023-04-10 13:37:59.000000 squirrels-0.1.0rc2/squirrels/module_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.338017 squirrels-0.1.0rc2/squirrels/package_data/
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.429019 squirrels-0.1.0rc2/squirrels/package_data/base_project/
--rw-rw-rw-   0        0        0       40 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/.gitignore
--rw-rw-rw-   0        0        0      907 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/connections.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.435025 squirrels-0.1.0rc2/squirrels/package_data/base_project/database/
--rw-rw-rw-   0        0        0     8192 2023-04-23 00:05:57.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/database/sample_database.db
--rw-rw-rw-   0        0        0   188416 2023-03-18 14:11:28.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/database/seattle_weather.db
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.335032 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.459022 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/
--rw-rw-rw-   0        0        0      296 2023-04-27 13:23:16.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/context.py
--rw-rw-rw-   0        0        0      814 2023-04-27 13:23:30.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
--rw-rw-rw-   0        0        0      281 2023-04-27 13:23:34.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
--rw-rw-rw-   0        0        0      299 2023-04-23 09:51:57.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
--rw-rw-rw-   0        0        0       31 2023-03-20 06:10:47.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/final_view.sql.j2
--rw-rw-rw-   0        0        0     1385 2023-04-27 13:22:31.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py
--rw-rw-rw-   0        0        0      142 2023-04-27 13:23:07.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/selections.cfg
--rw-rw-rw-   0        0        0       56 2023-05-05 13:20:06.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/project_vars.yaml
--rw-rw-rw-   0        0        0      264 2023-04-27 13:17:36.000000 squirrels-0.1.0rc2/squirrels/package_data/base_project/squirrels.yaml
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.466027 squirrels-0.1.0rc2/squirrels/package_data/static/
--rw-rw-rw-   0        0        0     4638 2023-03-12 05:51:40.000000 squirrels-0.1.0rc2/squirrels/package_data/static/favicon.ico
--rw-rw-rw-   0        0        0     9029 2023-04-23 18:22:58.000000 squirrels-0.1.0rc2/squirrels/package_data/static/script.js
--rw-rw-rw-   0        0        0     1841 2023-03-12 03:03:14.000000 squirrels-0.1.0rc2/squirrels/package_data/static/style.css
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.469016 squirrels-0.1.0rc2/squirrels/package_data/templates/
--rw-rw-rw-   0        0        0     1273 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/squirrels/package_data/templates/index.html
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.482024 squirrels-0.1.0rc2/squirrels/param_configs/
--rw-rw-rw-   0        0        0        0 2023-04-14 00:13:00.000000 squirrels-0.1.0rc2/squirrels/param_configs/__init__.py
--rw-rw-rw-   0        0        0    14672 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/data_sources.py
--rw-rw-rw-   0        0        0     8355 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/parameter_options.py
--rw-rw-rw-   0        0        0     1689 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/parameter_set.py
--rw-rw-rw-   0        0        0    18760 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/param_configs/parameters.py
--rw-rw-rw-   0        0        0    14047 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/renderer.py
--rw-rw-rw-   0        0        0     1148 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/timed_imports.py
--rw-rw-rw-   0        0        0     2156 2023-05-05 13:52:42.000000 squirrels-0.1.0rc2/squirrels/utils.py
--rw-rw-rw-   0        0        0       95 2023-04-24 03:56:44.000000 squirrels-0.1.0rc2/squirrels/version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:53:39.418026 squirrels-0.1.0rc2/squirrels.egg-info/
--rw-rw-rw-   0        0        0     2056 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 13:53:39.000000 squirrels-0.1.0rc2/squirrels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.513227 squirrels-0.1.0rc3/
+-rw-rw-rw-   0        0        0     1088 2023-04-24 03:56:44.000000 squirrels-0.1.0rc3/LICENSE
+-rw-rw-rw-   0        0        0     2056 2023-05-09 13:29:55.511226 squirrels-0.1.0rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-05-05 13:52:42.000000 squirrels-0.1.0rc3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 13:29:55.514228 squirrels-0.1.0rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1410 2023-05-05 14:02:43.000000 squirrels-0.1.0rc3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.331142 squirrels-0.1.0rc3/squirrels/
+-rw-rw-rw-   0        0        0      995 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/__init__.py
+-rw-rw-rw-   0        0        0     5888 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/_command_line.py
+-rw-rw-rw-   0        0        0     6174 2023-05-05 13:52:42.000000 squirrels-0.1.0rc3/squirrels/api_server.py
+-rw-rw-rw-   0        0        0     2650 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/connection_set.py
+-rw-rw-rw-   0        0        0     1837 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/constants.py
+-rw-rw-rw-   0        0        0     3059 2023-04-22 22:12:54.000000 squirrels-0.1.0rc3/squirrels/credentials_manager.py
+-rw-rw-rw-   0        0        0     9782 2023-05-07 15:29:31.000000 squirrels-0.1.0rc3/squirrels/dateutils.py
+-rw-rw-rw-   0        0        0     4799 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/initializer.py
+-rw-rw-rw-   0        0        0     6889 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/manifest.py
+-rw-rw-rw-   0        0        0     1255 2023-05-07 15:27:27.000000 squirrels-0.1.0rc3/squirrels/module_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.269137 squirrels-0.1.0rc3/squirrels/package_data/
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.400693 squirrels-0.1.0rc3/squirrels/package_data/base_project/
+-rw-rw-rw-   0        0        0       40 2023-05-05 13:52:42.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/.gitignore
+-rw-rw-rw-   0        0        0      923 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/connections.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.408693 squirrels-0.1.0rc3/squirrels/package_data/base_project/database/
+-rw-rw-rw-   0        0        0     8192 2023-04-23 00:05:57.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/database/sample_database.db
+-rw-rw-rw-   0        0        0   188416 2023-03-18 14:11:28.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/database/seattle_weather.db
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.267125 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.448228 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/
+-rw-rw-rw-   0        0        0      298 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/context.py
+-rw-rw-rw-   0        0        0      921 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
+-rw-rw-rw-   0        0        0      376 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
+-rw-rw-rw-   0        0        0      312 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
+-rw-rw-rw-   0        0        0       31 2023-03-20 06:10:47.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/final_view.sql.j2
+-rw-rw-rw-   0        0        0     1445 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py
+-rw-rw-rw-   0        0        0      142 2023-04-27 13:23:07.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/selections.cfg
+-rw-rw-rw-   0        0        0      728 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/base_project/squirrels.yaml
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.487234 squirrels-0.1.0rc3/squirrels/package_data/static/
+-rw-rw-rw-   0        0        0     4638 2023-03-12 05:51:40.000000 squirrels-0.1.0rc3/squirrels/package_data/static/favicon.ico
+-rw-rw-rw-   0        0        0     9128 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/package_data/static/script.js
+-rw-rw-rw-   0        0        0     1841 2023-03-12 03:03:14.000000 squirrels-0.1.0rc3/squirrels/package_data/static/style.css
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.491225 squirrels-0.1.0rc3/squirrels/package_data/templates/
+-rw-rw-rw-   0        0        0     1273 2023-04-24 03:56:44.000000 squirrels-0.1.0rc3/squirrels/package_data/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.508229 squirrels-0.1.0rc3/squirrels/param_configs/
+-rw-rw-rw-   0        0        0        0 2023-04-14 00:13:00.000000 squirrels-0.1.0rc3/squirrels/param_configs/__init__.py
+-rw-rw-rw-   0        0        0    14875 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/param_configs/data_sources.py
+-rw-rw-rw-   0        0        0     8355 2023-05-05 13:52:42.000000 squirrels-0.1.0rc3/squirrels/param_configs/parameter_options.py
+-rw-rw-rw-   0        0        0     1697 2023-05-07 15:28:23.000000 squirrels-0.1.0rc3/squirrels/param_configs/parameter_set.py
+-rw-rw-rw-   0        0        0    18504 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/param_configs/parameters.py
+-rw-rw-rw-   0        0        0    14392 2023-05-09 13:28:24.000000 squirrels-0.1.0rc3/squirrels/renderer.py
+-rw-rw-rw-   0        0        0     1137 2023-05-07 12:27:48.000000 squirrels-0.1.0rc3/squirrels/timed_imports.py
+-rw-rw-rw-   0        0        0     2402 2023-05-07 13:01:28.000000 squirrels-0.1.0rc3/squirrels/utils.py
+-rw-rw-rw-   0        0        0       95 2023-04-24 03:56:44.000000 squirrels-0.1.0rc3/squirrels/version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:29:55.388695 squirrels-0.1.0rc3/squirrels.egg-info/
+-rw-rw-rw-   0        0        0     2056 2023-05-09 13:29:55.000000 squirrels-0.1.0rc3/squirrels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1744 2023-05-09 13:29:55.000000 squirrels-0.1.0rc3/squirrels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 13:29:55.000000 squirrels-0.1.0rc3/squirrels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-09 13:29:55.000000 squirrels-0.1.0rc3/squirrels.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       95 2023-05-09 13:29:55.000000 squirrels-0.1.0rc3/squirrels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 13:29:55.000000 squirrels-0.1.0rc3/squirrels.egg-info/top_level.txt
```

### Comparing `squirrels-0.1.0rc2/LICENSE` & `squirrels-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/PKG-INFO` & `squirrels-0.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrels
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Python Package for Configuring SQL Generating APIs
 Author: Tim Huang
 Author-email: tim.yuting@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `squirrels-0.1.0rc2/README.md` & `squirrels-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/setup.py` & `squirrels-0.1.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             paths.append(os.path.join('..', path, filename))
     return paths
 
 extra_files = package_files(os.path.join('squirrels', 'package_data'))
 
 setup(
     name='squirrels',
-    version='0.1.0rc2',
+    version='0.1.0rc3',
     packages=find_packages(),
     description='Python Package for Configuring SQL Generating APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tim Huang',
     author_email='tim.yuting@hotmail.com',
     license='MIT',
```

### Comparing `squirrels-0.1.0rc2/squirrels/__init__.py` & `squirrels-0.1.0rc3/squirrels/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .param_configs.parameter_options import SelectParameterOption, DateParameterOption, NumberParameterOption, NumRangeParameterOption
-from .param_configs.parameters import WidgetType, Parameter, SingleSelectParameter, MultiSelectParameter, DateParameter, NumberParameter, NumRangeParameter
+from .param_configs.parameters import Parameter, SingleSelectParameter, MultiSelectParameter, DateParameter, NumberParameter, NumRangeParameter
 from .param_configs.data_sources import SelectionDataSource, DateDataSource, NumberDataSource, NumRangeDataSource, DataSourceParameter
 from .param_configs.parameter_set import ParameterSet
 from .connection_set import ConnectionSet
 from .version import __version__, major_version, minor_version, patch_version
 
 def get_credential(key: str):
     """
```

### Comparing `squirrels-0.1.0rc2/squirrels/_command_line.py` & `squirrels-0.1.0rc3/squirrels/_command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,31 +29,32 @@
     parser.add_argument('-v', '--version', action='store_true', help='Show the version and exit')
     parser.add_argument('--verbose', action='store_true', help='Enable verbose output')
     subparsers = parser.add_subparsers(title='commands', dest='command')
 
     init_parser = subparsers.add_parser(c.INIT_CMD, help='Initialize a squirrels project')
     init_parser.add_argument('--no-overwrite', action='store_true', help="Don't overwrite files if they already exist")
     init_parser.add_argument('--core', action='store_true', help='Include all core files')
+    init_parser.add_argument('--db-view', type=str, choices=c.FILE_TYPE_CHOICES, help='Create database view as sql (default) or python file if "--core" is specified')
+    init_parser.add_argument('--connections', action='store_true', help=f'Include the {c.CONNECTIONS_FILE} file')
     init_parser.add_argument('--context', action='store_true', help=f'Include the {c.CONTEXT_FILE} file')
     init_parser.add_argument('--selections-cfg', action='store_true', help=f'Include the {c.SELECTIONS_CFG_FILE} file')
-    init_parser.add_argument('--db-view', type=str, choices=['sql', 'py'], help='Create database view as sql (default) or python file')
-    init_parser.add_argument('--final-view', type=str, choices=['sql', 'py'], help='Include final view as sql or python file')
-    init_parser.add_argument('--sample-db', type=str, choices=['seattle-weather'], help='Sample sqlite database to include')
+    init_parser.add_argument('--final-view', type=str, choices=c.FILE_TYPE_CHOICES, help='Include final view as sql or python file')
+    init_parser.add_argument('--sample-db', type=str, choices=c.DATABASE_CHOICES, help='Sample sqlite database to include')
 
     subparsers.add_parser(c.LOAD_MODULES_CMD, help='Load all the modules specified in squirrels.yaml from git')
 
     def _add_profile_argument(parser: ArgumentParser):
         parser.add_argument('key', type=str, help='Key to the database connection credential')
 
-    subparsers.add_parser(c.GET_CREDS_CMD, help='Get all database connection credential keys')
-
     set_cred_parser = subparsers.add_parser(c.SET_CRED_CMD, help='Set a database connection credential key')
     _add_profile_argument(set_cred_parser)
     set_cred_parser.add_argument('--values', type=str, nargs=2, help='The username and password')
 
+    subparsers.add_parser(c.GET_CREDS_CMD, help='Get all database connection credential keys')
+
     delete_cred_parser = subparsers.add_parser(c.DELETE_CRED_CMD, help='Delete a database connection credential key')
     _add_profile_argument(delete_cred_parser)
 
     test_parser = subparsers.add_parser(c.TEST_CMD, help='For a given dataset, create outputs for parameter API response and rendered sql queries')
     test_parser.add_argument('dataset', type=str, help='Name of dataset (provided in squirrels.yaml) to test. Results are written in an "outputs" folder')
     test_parser.add_argument('-c', '--cfg', type=str, help="Configuration file for parameter selections. Path is relative to the dataset's folder")
     test_parser.add_argument('-d', '--data', type=str, help="Excel file with lookup data to avoid making a database connection. Path is relative to the dataset's folder")
@@ -72,19 +73,19 @@
     if args.version:
         print(__version__)
     elif args.command == c.INIT_CMD:
         Initializer(not args.no_overwrite).init_project(args)
     elif args.command == c.LOAD_MODULES_CMD:
         manifest = mf.from_file()
         ml.load_modules(manifest)
-    elif args.command == c.GET_CREDS_CMD: 
-        cm.squirrels_config_io.print_all_credentials()
     elif args.command == c.SET_CRED_CMD:
         user, pw = _prompt_user_pw(args.values)
         cm.squirrels_config_io.set_credential(args.key, user, pw)
+    elif args.command == c.GET_CREDS_CMD: 
+        cm.squirrels_config_io.print_all_credentials()
     elif args.command == c.DELETE_CRED_CMD:
         cm.squirrels_config_io.delete_credential(args.key)
     elif args.command in [c.RUN_CMD, c.TEST_CMD]:
         manifest = mf.from_file()
         conn_set = cs.from_file(manifest)
         if args.command == c.RUN_CMD:
             server = ApiServer(manifest, conn_set, args.no_cache, args.debug)
```

### Comparing `squirrels-0.1.0rc2/squirrels/api_server.py` & `squirrels-0.1.0rc3/squirrels/api_server.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/connection_set.py` & `squirrels-0.1.0rc3/squirrels/connection_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from squirrels.utils import ConfigurationError
 
 ConnectionPool = Union[Engine, Pool]
 
 
 class ConnectionSet:
     def __init__(self, conn_pools: Dict[str, ConnectionPool]) -> None:
+        if c.DEFAULT_DB_CONN not in conn_pools:
+            raise ConfigurationError(f'Connection name "{c.DEFAULT_DB_CONN}" was not set')
         self._conn_pools = conn_pools
     
     def get_connection_pool(self, conn_name: str) -> ConnectionPool:
         try:
             connection_pool = self._conn_pools[conn_name]
         except KeyError as e:
             raise ConfigurationError(f'Connection name "{conn_name}" was not configured') from e
@@ -29,34 +31,41 @@
             conn = connector.raw_connection()
         else:
             raise TypeError(f'Type for connection name "{conn_name}" not supported')
         
         try:
             cur = conn.cursor()
             cur.execute(query)
-            data = cur.fetchall()
-            columns = [x[0] for x in cur.description]
-            df = pd.DataFrame(data, columns=columns)
+            df = pd.DataFrame(data=cur.fetchall(), columns=[x[0] for x in cur.description])
         finally:
             conn.close()
 
         return df
 
     def dispose(self) -> None:
         for pool in self._conn_pools.values():
             pool.dispose()
 
 
 def from_file(manifest: mf.Manifest) -> ConnectionSet:
-    module = SourceFileLoader(c.CONNECTIONS_FILE, c.CONNECTIONS_FILE).load_module()
-    proj_vars = manifest.get_proj_vars()
+    connections = manifest.get_db_connections()
     try:
-        return module.main(proj_vars)
-    except Exception as e:
-        raise ConfigurationError(f'Error in the {c.CONNECTIONS_FILE} file') from e
+        module = SourceFileLoader(c.CONNECTIONS_FILE, c.CONNECTIONS_FILE).load_module()
+    except FileNotFoundError:
+        module = None
+    
+    if module is not None:
+        proj_vars = manifest.get_proj_vars()
+        try:
+            conn_from_py_file = module.main(proj_vars)
+        except Exception as e:
+            raise ConfigurationError(f'Error in the {c.CONNECTIONS_FILE} file') from e
+    else:
+        conn_from_py_file = {}
+    return ConnectionSet({**connections, **conn_from_py_file})
 
 
 def sqldf(query: str, df_by_db_views: Dict[str, pd.DataFrame]) -> pd.DataFrame:
     conn = sqlite3.connect(":memory:")
     try:
         for db_view, df in df_by_db_views.items():
             df.to_sql(db_view, conn, index=False)
```

### Comparing `squirrels-0.1.0rc2/squirrels/constants.py` & `squirrels-0.1.0rc3/squirrels/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,34 +4,39 @@
 GET_CREDS_CMD = 'get-all-credentials'
 SET_CRED_CMD = 'set-credential'
 DELETE_CRED_CMD = 'delete-credential'
 TEST_CMD = 'test'
 RUN_CMD = 'run'
 
 # Manifest file keys
+PROJ_VARS_KEY = 'project_variables'
+PRODUCT_KEY = 'product'
+MAJOR_VERSION_KEY = 'major_version'
+DB_CONNECTIONS_KEY = 'db_connections'
+DB_CREDENTIALS_KEY = 'credential_key'
+URL_KEY = 'url'
 DB_CONNECTION_KEY = 'db_connection'
 MODULES_KEY = 'modules'
 DATASET_LABEL_KEY = 'label'
 DATASETS_KEY = 'datasets'
 HEADERS_KEY = 'headers'
 DATABASE_VIEWS_KEY = 'database_views'
-DB_VIEW_NAME_KEY = 'name'
-DB_VIEW_FILE_KEY = 'file'
+FILE_KEY = 'file'
 FINAL_VIEW_KEY = 'final_view'
 BASE_PATH_KEY = 'base_path'
 SETTINGS_KEY = 'settings'
 
 # Database credentials keys
 CREDENTIALS_KEY = 'credentials'
 USERNAME_KEY = 'username'
 PASSWORD_KEY = 'password'
+DEFAULT_DB_CONN = 'default'
 
 # Folder/File names
 MANIFEST_FILE = 'squirrels.yaml'
-PROJ_VARS_FILE = 'project_vars.yaml'
 CONNECTIONS_FILE = 'connections.py'
 OUTPUTS_FOLDER = 'outputs'
 MODULES_FOLDER = 'modules'
 DATASETS_FOLDER = 'datasets'
 PARAMETERS_FILE = 'parameters.py'
 PARAMETERS_OUTPUT = 'parameters.json'
 DATABASE_VIEW_SQL_FILE = 'database_view1.sql.j2'
@@ -46,8 +51,11 @@
 PARAMETERS_CACHE_SIZE_SETTING = 'parameters.cache.size'
 PARAMETERS_CACHE_TTL_SETTING = 'parameters.cache.ttl'
 RESULTS_CACHE_SIZE_SETTING = 'results.cache.size'
 RESULTS_CACHE_TTL_SETTING = 'results.cache.ttl'
 
 # Selection cfg sections
 PARAMETERS_SECTION = 'parameters'
-HEADERS_SECTION = 'headers'
+
+# Init Command Choices
+FILE_TYPE_CHOICES = ['sql', 'py']
+DATABASE_CHOICES = ['sample_database', 'seattle_weather']
```

### Comparing `squirrels-0.1.0rc2/squirrels/credentials_manager.py` & `squirrels-0.1.0rc3/squirrels/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/dateutils.py` & `squirrels-0.1.0rc3/squirrels/dateutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import Sequence
 from dataclasses import dataclass
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
 from enum import Enum
 
 from squirrels import utils
 
@@ -35,23 +35,23 @@
 class DateModifier:
     """
     Interface for all Date modification classes, and declares a "modify" method
     """
 
     def modify(self, date: datetime) -> datetime:
         """
-        Method to be overwritten
+        Method to be overwritten, modifies the input date
 
         Parameters:
             date: The input date to modify.
 
         Returns:
             The modified date.
         """
-        return date
+        raise utils.AbstractMethodCallError(self.__class__, "modify")
 
 
 @dataclass
 class _DayIdxOfCalendarUnit(DateModifier):
     """
     Interface for adjusting a date to some day of calendar unit
     """
@@ -219,54 +219,75 @@
 class DateModPipeline(DateModifier):
     """
     DateModifier class to apply a list of date modifiers to an input date
 
     Attributes:
         modifiers: The list of DateModifier's to apply in sequence.
     """
-    modifiers: List[DateModifier]
+    modifiers: Sequence[DateModifier]
+
+    def __post_init__(self):
+        self.modifiers = tuple(self.modifiers)
     
     def modify(self, date: datetime) -> datetime:
         for modifier in self.modifiers:
             date = modifier.modify(date)
         return date
 
 
 @dataclass
 class _DateRepresentationModifier:
-    def __init__(self, date_modifiers: List[DateModifier]):
+    """
+    Abstract class for modifying other representations of dates (such as string or unix timestemp)
+    """
+    def __init__(self, date_modifiers: Sequence[DateModifier]):
         self.date_modifier = DateModPipeline(date_modifiers)
+    
+    def _get_joined_modifiers(self, date_modifiers: Sequence[DateModifier]) -> Sequence[DateModifier]:
+        joined_modifiers = self.date_modifier.modifiers + tuple(date_modifiers)
+        return joined_modifiers
+
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        raise utils.AbstractMethodCallError(self.__class__, "with_more_modifiers")
 
 
 @dataclass
 class DateStringModifier(_DateRepresentationModifier):
     """
     Class to modify a string representation of a date given a DateModifier
 
     Attributes:
         date_modifier: The DateModifier to apply on datetime objects
         date_format: Format of the date string. Default is '%Y-%m-%d'
     """
-    def __init__(self, date_modifiers: List[DateModifier], date_format: str = '%Y-%m-%d'):
+    def __init__(self, date_modifiers: Sequence[DateModifier], date_format: str = '%Y-%m-%d'):
         super().__init__(date_modifiers)
         self.date_format = date_format
 
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        joined_modifiers = self._get_joined_modifiers(date_modifiers)
+        return DateStringModifier(joined_modifiers, self.date_format)
+
     def modify(self, date_str: str) -> str:
         date_obj = datetime.strptime(date_str, self.date_format)
         return self.date_modifier.modify(date_obj).strftime(self.date_format)
 
 
 @dataclass
 class TimestampModifier(_DateRepresentationModifier):
     """
     Class to modify a numeric representation of a date (as Unix/Epoch/POSIX timestamp) given a DateModifier
 
     Attributes:
         date_modifier: The DateModifier to apply on datetime objects
         date_format: Format of the date string. Default is '%Y-%m-%d'
     """
-    def __init__(self, date_modifiers: List[DateModifier]):
+    def __init__(self, date_modifiers: Sequence[DateModifier]):
         super().__init__(date_modifiers)
 
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        joined_modifiers = self._get_joined_modifiers(date_modifiers)
+        return TimestampModifier(joined_modifiers)
+
     def modify(self, timestamp: float) -> float:
         date_obj = datetime.fromtimestamp(timestamp)
         return self.date_modifier.modify(date_obj).timestamp()
```

### Comparing `squirrels-0.1.0rc2/squirrels/initializer.py` & `squirrels-0.1.0rc3/squirrels/initializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,51 +34,64 @@
         if not self._path_exists(filename):
             next_major_version = int(major_version) + 1
             content = f'squirrels<{next_major_version}'
             with open(filename, 'w') as f:
                 f.write(content)
 
     def init_project(self, args):
-        options = ['core', 'context', 'selections_cfg', 'db_view', 'final_view', 'sample_db']
+        options = ['core', 'db_view', 'connections', 'context', 'selections_cfg', 'final_view', 'sample_db']
         answers = { x: getattr(args, x) for x in options }
         if not any(answers.values()):
-            questions = [
-                inquirer.Confirm('core',
+            core_questions = [
+                inquirer.Confirm('core', 
                                 message="Include all core project files?",
-                                default=True),
+                                default=True)
+            ]
+            answers = inquirer.prompt(core_questions)
+            
+            if answers.get('core', False):
+                conditional_questions = [
+                    inquirer.List('db_view', 
+                                  message="What's the file format for the database view?",
+                                  choices=c.FILE_TYPE_CHOICES),
+                ]
+                answers.update(inquirer.prompt(conditional_questions))
+
+            remaining_questions = [
+                inquirer.Confirm('connections',
+                                message=f"Do you want to add a '{c.CONNECTIONS_FILE}' file?" ,
+                                default=False),
                 inquirer.Confirm('context',
-                                message="Do you want to include a 'context.py' file?" ,
+                                message=f"Do you want to add a '{c.CONTEXT_FILE}' file?" ,
                                 default=False),
                 inquirer.Confirm('selections_cfg',
-                                message="Do you want to include a 'selections.cfg' file?" ,
+                                message=f"Do you want to add a '{c.SELECTIONS_CFG_FILE}' file?" ,
                                 default=False),
-                inquirer.List('db_view', 
-                            message="What's the file format for the database view? (ignore if core project files are not included)",
-                            choices=['sql', 'py']),
                 inquirer.List('final_view', 
                             message="What's the file format for the final view (if any)?",
-                            choices=['none', 'sql', 'py']),
+                            choices=['none'] + c.FILE_TYPE_CHOICES),
                 inquirer.List('sample_db', 
                             message="What sample sqlite database do you wish to use (if any)?",
-                            choices=['none', 'sample_database', 'seattle_weather'])
+                            choices=['none'] + c.DATABASE_CHOICES)
             ]
-            answers = inquirer.prompt(questions)
+            answers.update(inquirer.prompt(remaining_questions))
 
         if answers.get('core', False):
             self._copy_file('.gitignore')
             self._copy_file(c.MANIFEST_FILE)
-            self._copy_file(c.PROJ_VARS_FILE)
-            self._copy_file(c.CONNECTIONS_FILE)
             self._create_requirements_txt()
             self._copy_dataset_file(c.PARAMETERS_FILE)
             if answers.get('db_view') == 'py':
                 self._copy_dataset_file(c.DATABASE_VIEW_PY_FILE)
             else:
                 self._copy_dataset_file(c.DATABASE_VIEW_SQL_FILE)
         
+        if answers.get('connections', False):
+            self._copy_file(c.CONNECTIONS_FILE)
+        
         if answers.get('context', False):
             self._copy_dataset_file(c.CONTEXT_FILE)
         
         if answers.get('selections_cfg', False):
             self._copy_dataset_file(c.SELECTIONS_CFG_FILE)
         
         final_view_format = answers.get('final_view')
```

### Comparing `squirrels-0.1.0rc2/squirrels/module_loader.py` & `squirrels-0.1.0rc3/squirrels/module_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Dict
+from typing import List, Tuple
 from squirrels import constants as c, manifest as mf
 import git, shutil, os, stat
 
 
 def parse_module_repo_strings(repo_strings: List[str]) -> List[Tuple[str]]:
     output = []
     for repo in repo_strings:
```

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/base_project/database/sample_database.db` & `squirrels-0.1.0rc3/squirrels/package_data/base_project/database/sample_database.db`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/base_project/database/seattle_weather.db` & `squirrels-0.1.0rc3/squirrels/package_data/base_project/database/seattle_weather.db`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py` & `squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Dict, Union, Any
-import sqlalchemy as sa
+from typing import Dict, Any
 import pandas as pd
 
 import squirrels as sq
 
 
-def main(connection_pool: Union[sa.Engine, sa.Pool], connection_set: sq.ConnectionSet,
-         prms: sq.ParameterSet, ctx: Dict[str, Any], proj: Dict[str, str], *args, **kwargs) -> pd.DataFrame:
-    # conn = connection_pool.connect() # use this to create the corresponding DBAPI2 connection
+def main(connection_set: sq.ConnectionSet, 
+         prms: sq.ParameterSet, ctx: Dict[str, Any], args: Dict[str, Any], 
+         *p_args, **kwargs) -> pd.DataFrame:
+    # pool = connection_set.get_connection_pool("default")
+    # conn = pool.connect() # use this to get a DBAPI connection from a Pool or sqlalchemy connection from an Engine
+    # conn = pool.raw_connection() # use this to get a DBAPI connection from an Engine
     
     df = pd.DataFrame({
         'dim1': ['a', 'b', 'c', 'd', 'e', 'f'], 
         'metric1': [1, 2, 3, 4, 5, 6], 
         'metric2': [2, 4, 5, 1, 7, 3]
     })
     limit_parameter: sq.NumberParameter = prms['upper_bound']
```

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py` & `squirrels-0.1.0rc3/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from typing import Dict, Any
 import squirrels as sq
 
 
-def main(*args, **kwargs) -> sq.ParameterSet:
+def main(args: Dict[str, Any], *p_args, **kwargs) -> sq.ParameterSet:
     single_select_options = (
         sq.SelectParameterOption('a0', 'Primary Colors'),
         sq.SelectParameterOption('a1', 'Secondary Colors')
     )
     
     multi_select_options = (
-        sq.SelectParameterOption('x0', 'Red', parent_option_id='a0'),
+        sq.SelectParameterOption('x0', 'Red',    parent_option_id='a0'),
         sq.SelectParameterOption('x1', 'Yellow', parent_option_id='a0'),
-        sq.SelectParameterOption('x2', 'Blue', parent_option_id='a0'),
-        sq.SelectParameterOption('x3', 'Green', parent_option_id='a1'),
+        sq.SelectParameterOption('x2', 'Blue',   parent_option_id='a0'),
+        sq.SelectParameterOption('x3', 'Green',  parent_option_id='a1'),
         sq.SelectParameterOption('x4', 'Orange', parent_option_id='a1'),
         sq.SelectParameterOption('x5', 'Purple', parent_option_id='a1')
     )
 
     single_select_example = sq.SingleSelectParameter('color_type', 'Color Type', single_select_options)
 
     multi_select_example = sq.MultiSelectParameter('colors', 'Colors', multi_select_options,
```

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/static/favicon.ico` & `squirrels-0.1.0rc3/squirrels/package_data/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/static/script.js` & `squirrels-0.1.0rc3/squirrels/package_data/static/script.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -61,23 +61,23 @@
 
             const addLabel = function() {
                 const paramLabel = document.createElement('label')
                 paramLabel.innerHTML = param.label
                 newDiv.appendChild(paramLabel)
             }
 
-            if (param.widget_type === "DateField") {
+            if (param.widget_type === "DateParameter") {
                 addLabel()
                 const dateInput = document.createElement('input')
                 dateInput.type = 'date'
                 dateInput.id = param.name
                 dateInput.value = param.selected_date
                 dateInput.onchange = updateParameter
                 newDiv.appendChild(dateInput)
-            } else if (param.widget_type === "NumberField") {
+            } else if (param.widget_type === "NumberParameter") {
                 addLabel()
                 const sliderInput = document.createElement('input')
                 sliderInput.type = 'range'
                 sliderInput.id = param.name
                 sliderInput.min = param.min_value
                 sliderInput.max = param.max_value
                 sliderInput.step = param.increment
@@ -91,32 +91,32 @@
                 sliderInput.oninput = function() {
                     sliderValue.innerText = this.value;
                 }
                 sliderInput.onchange = updateParameter
 
                 newDiv.appendChild(sliderInput)
                 newDiv.appendChild(sliderValue)
-            } else if (param.widget_type === "RangeField") {
+            } else if (param.widget_type === "NumRangeParameter") {
                 // TODO
-            } else if (param.widget_type === "SingleSelect" && param.options.length > 0) {
+            } else if (param.widget_type === "SingleSelectParameter" && param.options.length > 0) {
                 addLabel()
                 const singleSelect = document.createElement('select');
                 singleSelect.id = param.name;
                 param.options.forEach(function(option) {
                     const selectOption = document.createElement('option');
                     selectOption.value = option.id;
                     if (option.id === param.selected_id) {
                         selectOption.selected = true;
                     }
                     selectOption.innerText = option.label;
                     singleSelect.appendChild(selectOption);
                 });
                 singleSelect.onchange = updateParameter
                 newDiv.appendChild(singleSelect);
-            } else if (param.widget_type === "MultiSelect" && param.options.length > 0) {
+            } else if (param.widget_type === "MultiSelectParameter" && param.options.length > 0) {
                 addLabel()
                 const multiSelect = document.createElement('select');
                 multiSelect.id = param.name;
                 multiSelect.multiple = true;
                 param.options.forEach(function(option) {
                     const selectOption = document.createElement('option');
                     selectOption.value = option.id;
@@ -132,44 +132,44 @@
             generatedParamsDiv.appendChild(newDiv);
         }
     });
 }
 
 function updateParameter() {
     const param = parametersMap.get(this.id)
-    if (param.widget_type === "DateField") {
+    if (param.widget_type === "DateParameter") {
         param.selected_date = this.value
-    } else if (param.widget_type === "NumberField") {
+    } else if (param.widget_type === "NumberParameter") {
         param.selected_value = this.value
-    } else if (param.widget_type === "RangeField") {
+    } else if (param.widget_type === "NumRangeParameter") {
         // TODO
-    } else if (param.widget_type === "SingleSelect") {
+    } else if (param.widget_type === "SingleSelectParameter") {
         param.selected_id = this.options[this.selectedIndex].value
-    } else if (param.widget_type === "MultiSelect") {
+    } else if (param.widget_type === "MultiSelectParameter") {
         param.selected_ids = [...this.selectedOptions].map(option => option.value)
     }
 
     if (param.trigger_refresh) {
         refreshParameters(param)
     }
 }
 
 function getQueryParams(provoker = null) {
     const queryParams = {}
 
     function addToQueryParams(key, value) {
-        if (value.widget_type === "DateField") {
+        if (value.widget_type === "DateParameter") {
             queryParams[key] = value.selected_date
-        } else if (value.widget_type === "NumberField") {
+        } else if (value.widget_type === "NumberParameter") {
             queryParams[key] = value.selected_value
-        } else if (value.widget_type === "RangeField") {
+        } else if (value.widget_type === "NumRangeParameter") {
             // TODO
-        } else if (value.widget_type === "SingleSelect") {
+        } else if (value.widget_type === "SingleSelectParameter") {
             queryParams[key] = value.selected_id
-        } else if (value.widget_type === "MultiSelect") {
+        } else if (value.widget_type === "MultiSelectParameter") {
             result = value.selected_ids.join()
             if (result !== '') queryParams[key] = result
         }
     }
     if (provoker !== null) {
         addToQueryParams(provoker.name, provoker)
     } else {
```

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/static/style.css` & `squirrels-0.1.0rc3/squirrels/package_data/static/style.css`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/package_data/templates/index.html` & `squirrels-0.1.0rc3/squirrels/package_data/templates/index.html`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/param_configs/data_sources.py` & `squirrels-0.1.0rc3/squirrels/param_configs/data_sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
-from typing import Tuple, List, Dict, Optional
+from typing import Type, Tuple, List, Dict, Optional
 from dataclasses import dataclass
 
 from squirrels.param_configs import parameters as p, parameter_options as po
 from squirrels.timed_imports import pandas as pd
-from squirrels import utils
+from squirrels import utils, constants as c
 
 
 @dataclass
 class DataSource:
     """
     Abstract class for lookup tables coming from a database
     """
-    connection_name: str
     table_or_query: str
     
     def __post_init__(self) -> None:
         if not hasattr(self, 'parent_id_col'):
             self.parent_id_col = None
+        if not hasattr(self, 'connection_name'):
+            self.connection_name = c.DEFAULT_DB_CONN
 
     def get_query(self) -> str:
         """
         Get the "table_or_query" attribute as a select query
 
         Returns:
             str: The converted select query
@@ -39,23 +40,24 @@
         Args:
             ds_param: The parameter to convert
             df: The dataframe containing the parameter options data
 
         Returns:
             The converted parameter
         """
-        raise NotImplementedError(f'Must override the "convert" method')
+        raise utils.AbstractMethodCallError(self.__class__, "convert")
     
     def _get_parent(self, row):
         return str(utils.get_row_value(row, self.parent_id_col)) if self.parent_id_col is not None else None
     
-    def _validate_widget_type(self, ds_param: DataSourceParameter, widget_types: List[p.WidgetType]) -> None:
-        if ds_param.widget_type not in widget_types:
-            class_name = self.__class__.__name__
-            raise utils.ConfigurationError(f'Invalid widget type "{ds_param.widget_type}" for {class_name}')
+    def _validate_parameter_class(self, ds_param: DataSourceParameter, parameter_classes: List[Type[p.Parameter]]) -> None:
+        if ds_param.parameter_class not in parameter_classes:
+            parameter_class_name = ds_param.parameter_class.__name__
+            datasource_class_name = self.__class__.__name__
+            raise utils.ConfigurationError(f'Invalid widget type "{parameter_class_name}" for {datasource_class_name}')
 
 
 @dataclass
 class SelectionDataSource(DataSource):
     """
     Lookup table for selection parameters (single and multi)
 
@@ -69,14 +71,15 @@
         parent_id_col: The column name of the parent option id that this option belongs to
     """
     id_col: str
     options_col: str
     order_by_col: Optional[str] = None
     is_default_col: Optional[str] = None
     parent_id_col: Optional[str] = None
+    connection_name: str = c.DEFAULT_DB_CONN
 
     def __post_init__(self):
         self.order_by_col = self.order_by_col if self.order_by_col is not None else self.id_col
 
     def convert(self, ds_param: DataSourceParameter, df: pd.DataFrame) -> p.Parameter:
         """
         Method to convert the associated DataSourceParameter into a SingleSelect or MultiSelect Parameter
@@ -84,15 +87,15 @@
         Parameters:
             ds_param: The parameter to convert
             df: The dataframe containing the parameter options data
 
         Returns:
             The converted parameter
         """
-        self._validate_widget_type(ds_param, [p.WidgetType.SingleSelect, p.WidgetType.MultiSelect])
+        self._validate_parameter_class(ds_param, [p.SingleSelectParameter, p.MultiSelectParameter])
 
         def is_default(row):
             return int(utils.get_row_value(row, self.is_default_col)) == 1 if self.is_default_col is not None else False
         
         try:
             df.sort_values(self.order_by_col, inplace=True)
         except KeyError as e:
@@ -100,20 +103,15 @@
         
         options = tuple(
             po.SelectParameterOption(str(utils.get_row_value(row, self.id_col)), str(utils.get_row_value(row, self.options_col)), is_default(row), 
                                      parent_option_id=self._get_parent(row))
             for _, row in df.iterrows()
         )
         
-        if ds_param.widget_type == p.WidgetType.SingleSelect:
-            return p.SingleSelectParameter(ds_param.name, ds_param.label, options, 
-                                           is_hidden=ds_param.is_hidden, parent=ds_param.parent)
-        elif ds_param.widget_type == p.WidgetType.MultiSelect:
-            return p.MultiSelectParameter(ds_param.name, ds_param.label, options, 
-                                          is_hidden=ds_param.is_hidden, parent=ds_param.parent)
+        return ds_param.parameter_class(ds_param.name, ds_param.label, options, is_hidden=ds_param.is_hidden, parent=ds_param.parent)
 
 
 @dataclass
 class DateDataSource(DataSource):
     """
     Lookup table for date parameter default options
 
@@ -123,27 +121,28 @@
         default_date_col: The column name of the default date
         date_format: The format of the default date(s). Defaults to '%Y-%m-%d'
         parent_id_col: The column name of the parent option id that the default date belongs to
     """
     default_date_col: str
     parent_id_col: Optional[str] = None
     date_format: Optional[str] = '%Y-%m-%d'
+    connection_name: str = c.DEFAULT_DB_CONN
 
     def convert(self, ds_param: DataSourceParameter, df: pd.DataFrame) -> p.DateParameter:
         """
         Method to convert the associated DataSourceParameter into a DateParameter
 
         Parameters:
             ds_param: The parameter to convert
             df: The dataframe containing the parameter options data
 
         Returns:
             The converted parameter
         """
-        self._validate_widget_type(ds_param, [p.WidgetType.DateField])
+        self._validate_parameter_class(ds_param, [p.DateParameter])
         
         def get_date(row: pd.Series) -> str:
             return str(utils.get_row_value(row, self.default_date_col))
         
         def create_date_param_option(row: pd.Series) -> po.DateParameterOption:
             return po.DateParameterOption(get_date(row), self.date_format, self._get_parent(row))
         
@@ -162,15 +161,15 @@
     """
     Abstract class for number or number range data sources
     """
     min_value_col: str
     max_value_col: str
     increment_col: Optional[str] = None
 
-    def _convert_helper(self, row: pd.Series) -> Tuple[str]:
+    def _convert_helper(self, row: pd.Series) -> Tuple[str, str, str]:
         min_val = str(utils.get_row_value(row, self.min_value_col))
         max_val = str(utils.get_row_value(row, self.max_value_col))
         incr_val = str(utils.get_row_value(row, self.increment_col)) if self.increment_col is not None else '1'
         return min_val, max_val, incr_val
 
 @dataclass
 class NumberDataSource(_NumericDataSource):
@@ -184,27 +183,28 @@
         max_value_col: The column name of the maximum value
         increment_col: The column name of the increment value. Defaults to column of 1's if None
         default_value_col: The column name of the default value. Defaults to min_value_col if None
         parent_id_col: The column name of the parent option id that the default value belongs to
     """
     default_value_col: Optional[str] = None
     parent_id_col: Optional[str] = None
+    connection_name: str = c.DEFAULT_DB_CONN
 
     def convert(self, ds_param: DataSourceParameter, df: pd.DataFrame) -> p.NumberParameter:
         """
         Method to convert the associated DataSourceParameter into a NumberParameter
 
         Parameters:
             ds_param: The parameter to convert
             df: The dataframe containing the parameter options data
 
         Returns:
             The converted parameter
         """
-        self._validate_widget_type(ds_param, [p.WidgetType.NumberField])
+        self._validate_parameter_class(ds_param, [p.NumberParameter])
 
         def _get_default_value(row: pd.Series) -> str:
             return str(utils.get_row_value(row, self.default_value_col)) if self.default_value_col is not None \
                 else str(utils.get_row_value(row, self.min_value_col))
         
         def _create_num_param_option(row: pd.Series) -> po.NumberParameterOption:
             min_value, max_value, increment = self._convert_helper(row)
@@ -236,29 +236,30 @@
         default_lower_value_col: The column name of the default lower value. Defaults to min_value_col if None
         default_upper_value_col: The column name of the default upper value. Defaults to max_value_col if None
         parent_id_col: The column name of the parent option id that the default value belongs to
     """
     default_lower_value_col: Optional[str] = None
     default_upper_value_col: Optional[str] = None
     parent_id_col: Optional[str] = None
+    connection_name: str = c.DEFAULT_DB_CONN
 
     def convert(self, ds_param: DataSourceParameter, df: pd.DataFrame) -> p.NumRangeParameter:
         """
         Method to convert the associated DataSourceParameter into a NumRangeParameter
 
         Parameters:
             ds_param: The parameter to convert
             df: The dataframe containing the parameter options data
 
         Returns:
             The converted parameter
         """
-        self._validate_widget_type(ds_param, [p.WidgetType.RangeField])
+        self._validate_parameter_class(ds_param, [p.NumRangeParameter])
 
-        def _get_default_lower_upper_values(row: pd.Series) -> Tuple[str]:
+        def _get_default_lower_upper_values(row: pd.Series) -> Tuple[str, str]:
             lower_value_col = self.default_lower_value_col if self.default_lower_value_col is not None \
                 else self.min_value_col
             upper_value_col = self.default_upper_value_col if self.default_upper_value_col is not None \
                 else self.max_value_col
             lower_value = str(utils.get_row_value(row, lower_value_col))
             upper_value = str(utils.get_row_value(row, upper_value_col))
             return lower_value, upper_value
@@ -274,36 +275,38 @@
             min_value, max_value, increment = self._convert_helper(row)
             lower_value, upper_value = _get_default_lower_upper_values(row)
             return p.NumRangeParameter(ds_param.name, ds_param.label, min_value, max_value, increment, 
                                     lower_value, upper_value, is_hidden=ds_param.is_hidden)
         else:
             all_options = tuple(_create_range_param_option(row) for _, row in df.iterrows())
             return p.NumRangeParameter.WithParent(ds_param.name, ds_param.label, all_options, ds_param.parent,
-                                               is_hidden=ds_param.is_hidden)
+                                                  is_hidden=ds_param.is_hidden)
 
 
 @dataclass
 class DataSourceParameter(p.Parameter):
+    parameter_class: Type[p.Parameter]
     data_source: DataSource
     parent: Optional[p.Parameter] 
 
-    def __init__(self, widget_type: p.WidgetType, name: str, label: str, data_source: DataSource, *, 
+    def __init__(self, parameter_class: Type[p.Parameter], name: str, label: str, data_source: DataSource, *, 
                  is_hidden: bool = False, parent: Optional[p.Parameter] = None) -> None:
         """
         Constructor for DataSourceParameter, a Parameter that uses a DataSource to convert itself to another Parameter
 
         Parameters:
-            widget_type: The type of widget to use for this parameter
+            parameter_class: The class of widget parameter to convert to
             name: The name of the parameter
             label: The label of the parameter
             data_source: The lookup table to use for this parameter
             is_hidden: Whether or not this parameter should be hidden from parameters response
             parent: The parent parameter
         """
-        super().__init__(widget_type, name, label, None, is_hidden, None)
+        super().__init__(name, label, None, is_hidden, None)
+        self.parameter_class = parameter_class
         self.data_source = data_source
         self.parent = parent
 
     def convert(self, df: pd.DataFrame) -> p.Parameter:
         """
         Method to convert this DataSourceParameter into another parameter
 
@@ -321,9 +324,10 @@
 
         The field specific to this dictionary representation is "data_source".
 
         Returns:
             Dict: The dictionary representation of this DataSourceParameter
         """
         output = super().to_dict()
+        output['widget_type'] = self.parameter_class.__name__
         output['data_source'] = self.data_source.__dict__
         return output
```

### Comparing `squirrels-0.1.0rc2/squirrels/param_configs/parameter_options.py` & `squirrels-0.1.0rc3/squirrels/param_configs/parameter_options.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0rc2/squirrels/param_configs/parameter_set.py` & `squirrels-0.1.0rc3/squirrels/param_configs/parameter_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
-from typing import List, Dict
+from typing import Sequence, Dict
 from collections import OrderedDict
 
 from squirrels.param_configs import data_sources as d, parameters as p
 from squirrels.timed_imports import pandas as pd
 
 
 class ParameterSet(p.ParameterSetBase):
-    def __init__(self, parameters: List[p.Parameter]):
+    def __init__(self, parameters: Sequence[p.Parameter]):
         super().__init__()
         self._data_source_params: OrderedDict[str, d.DataSourceParameter] = OrderedDict()
         for param in parameters:
             self._parameters_dict[param.name] = param
             if isinstance(param, d.DataSourceParameter):
                 self._data_source_params[param.name] = param
```

### Comparing `squirrels-0.1.0rc2/squirrels/param_configs/parameters.py` & `squirrels-0.1.0rc3/squirrels/param_configs/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,49 @@
 from __future__ import annotations
-from typing import Iterable, Dict, List, Tuple, Iterator, Optional, Union
+from typing import Sequence, Dict, List, Iterator, Optional, Union
 from collections import OrderedDict
 from dataclasses import dataclass
 from datetime import datetime
-from enum import Enum
 from decimal import Decimal
 import copy
 
 from squirrels.param_configs import parameter_options as po
-from squirrels.utils import InvalidInputError, ConfigurationError
-
-
-class WidgetType(Enum):
-    SingleSelect = 1
-    MultiSelect = 2
-    DateField = 3
-    NumberField = 4
-    RangeField = 5
+from squirrels.utils import InvalidInputError, ConfigurationError, AbstractMethodCallError
 
 
 @dataclass
 class Parameter:
-    widget_type: WidgetType
     name: str
     label: str
-    all_options: Iterable[po.ParameterOption]
+    all_options: Sequence[po.ParameterOption]
     is_hidden: bool
     parent: Optional[_SelectionParameter]
 
-    def WithParent(all_options: Iterable[po.ParameterOption], parent: SingleSelectParameter, new_param: Parameter):
+    def WithParent(all_options: Sequence[po.ParameterOption], parent: SingleSelectParameter, new_param: Parameter):
         new_param._set_parent_and_options(parent, all_options)
         new_param.parent._add_child_mutate(new_param)
         return new_param.refresh(parent)
 
     def refresh(self, parent: Optional[_SelectionParameter] = None) -> Parameter:
         param_copy = copy.copy(self)
         if parent is not None:
             param_copy.parent = parent
         param_copy._refresh_mutate()
         return param_copy
 
     def with_selection(self, _: str) -> Parameter:
-        raise NotImplementedError(f'Must override "with_selection" method')
+        raise AbstractMethodCallError(self.__class__, "with_selection")
     
     def get_all_dependent_params(self) -> ParameterSetBase:
         dependent_params = ParameterSetBase()
         self._accum_all_dependent_params(dependent_params)
         return dependent_params
     
     def _set_default_as_selection_mutate(self) -> None:
-        raise NotImplementedError(f'Must override "_set_default_as_selection_mutate" method')
+        raise AbstractMethodCallError(self.__class__, "_set_default_as_selection_mutate")
     
     def _refresh_mutate(self) -> None:
         if self.parent is not None and hasattr(self, 'curr_option'):
             self.curr_option = next(self._get_valid_options_iterator())
         self._set_default_as_selection_mutate()
     
     def _get_valid_options_iterator(self) -> Iterator[po.ParameterOption]:
@@ -72,39 +62,39 @@
         for option in self.all_options:
             if not accum_set.isdisjoint(option.parent_option_ids):
                 raise ConfigurationError(f'For "{self.name}", it''s not a selection parameter, so no two options can share the same parent option')
             accum_set = accum_set.union(option.parent_option_ids)
         if len(accum_set) != len(self.parent.options):
             raise ConfigurationError(f'For "{self.name}", all parent option ids must exist across all options')
     
-    def _set_parent_and_options(self, parent: SingleSelectParameter, all_options: Iterable[po.ParameterOption]) -> None:
+    def _set_parent_and_options(self, parent: SingleSelectParameter, all_options: Sequence[po.ParameterOption]) -> None:
         self.parent = parent
         self.all_options = all_options
         self._verify_parent_is_single_select()
         self._verify_parent_options_have_one_child_each()
     
     def _accum_all_dependent_params(self, param_set: ParameterSetBase) -> None:
         param_set.add_parameter(self)
         
     def _enquote(self, value: str) -> str:
         return "'" + value.replace("'", "''") + "'" 
 
     def to_dict(self) -> Dict:
         return {
-            'widget_type': self.widget_type.name,
+            'widget_type': self.__class__.__name__,
             'name': self.name,
             'label': self.label
         }
 
 
 @dataclass
 class _SelectionParameter(Parameter):
     def __post_init__(self) -> None:
         self.trigger_refresh: bool = False
-        self.options: Tuple[po.SelectParameterOption] = tuple(self.all_options)
+        self.options: Sequence[po.SelectParameterOption] = tuple(self.all_options)
         self.children: List[_SelectionParameter] = list()
         if self.parent is not None:
             self.parent._add_child_mutate(self)
         self._refresh_mutate()
     
     def _add_child_mutate(self, child: Parameter) -> None:
         self.children.append(child)
@@ -112,16 +102,16 @@
     
     def _refresh_mutate(self) -> None:
         if self.parent is not None:
             self.options = tuple(self._get_valid_options_iterator())
         self._set_default_as_selection_mutate()
         self.children = [child.refresh(self) for child in self.children]
 
-    def _get_selected_ids_as_list(self) -> Tuple[str]:
-        raise NotImplementedError('Must override "_get_selected_ids_as_list"')
+    def _get_selected_ids_as_list(self) -> Sequence[str]:
+        raise AbstractMethodCallError(self.__class__, "_get_selected_ids_as_list")
 
     def _get_default_iterator(self) -> Iterator[po.ParameterOption]:
         return (x.identifier for x in self.options if x.is_default)
     
     def _validate_selected_id_in_options(self, selected_id: str) -> str:
         if selected_id in (x.identifier for x in self.options):
             return selected_id
@@ -140,17 +130,17 @@
         return output
 
 
 @dataclass
 class SingleSelectParameter(_SelectionParameter):
     selected_id: Optional[str]
 
-    def __init__(self, name: str, label: str, all_options: Iterable[po.SelectParameterOption], *, 
+    def __init__(self, name: str, label: str, all_options: Sequence[po.SelectParameterOption], *, 
                  is_hidden: bool = False, parent: Optional[_SelectionParameter] = None) -> None:
-        super().__init__(WidgetType.SingleSelect, name, label, all_options, is_hidden, parent)
+        super().__init__(name, label, all_options, is_hidden, parent)
     
     def with_selection(self, selection: str) -> SingleSelectParameter:
         param_copy = copy.copy(self)
         param_copy.selected_id = self._validate_selected_id_in_options(selection)
         param_copy.children = [child.refresh(param_copy) for child in param_copy.children]
         return param_copy
 
@@ -166,15 +156,15 @@
     def get_selected_label(self) -> str:
         return self.get_selected().label
     
     def get_selected_label_quoted(self) -> str:
         return self._enquote(self.get_selected_label())
     
     # Overriding for refresh method
-    def _get_selected_ids_as_list(self) -> Tuple[str]:
+    def _get_selected_ids_as_list(self) -> Sequence[str]:
         return (self.get_selected_id(),)
     
     def _get_default(self) -> str:
         default_id = next(self._get_default_iterator(), None)
         if default_id is None:
             default_id = self.options[0].identifier if len(self.options) > 0 else None
         return default_id
@@ -186,66 +176,66 @@
         output = super().to_dict()
         output['selected_id'] = self.selected_id
         return output
 
 
 @dataclass
 class MultiSelectParameter(_SelectionParameter):
-    selected_ids: Iterable[str]
+    selected_ids: Sequence[str]
     include_all: bool
     order_matters: bool
 
-    def __init__(self, name: str, label: str, all_options: Iterable[po.SelectParameterOption], *, is_hidden = False,
+    def __init__(self, name: str, label: str, all_options: Sequence[po.SelectParameterOption], *, is_hidden = False,
                  parent: Optional[_SelectionParameter] = None, include_all: bool = True, order_matters: bool = False) -> None:
-        super().__init__(WidgetType.MultiSelect, name, label, all_options, is_hidden, parent)
+        super().__init__(name, label, all_options, is_hidden, parent)
         self.include_all = include_all
         self.order_matters = order_matters
 
     def with_selection(self, selection: str) -> MultiSelectParameter:
         param_copy = copy.copy(self)
         selection_split = [] if (selection == '') else selection.split(',')
         param_copy.selected_ids = tuple(self._validate_selected_id_in_options(x) for x in selection_split)
         param_copy.children = [child.refresh(param_copy) for child in self.children]
         return param_copy
 
-    def get_selected_list(self) -> Tuple[po.SelectParameterOption]:
+    def get_selected_list(self) -> Sequence[po.SelectParameterOption]:
         if len(self.selected_ids) == 0 and self.include_all:
             result = tuple(self.options)
         else:
             result = tuple(x for x in self.options if x.identifier in self.selected_ids)
         return result
     
-    def get_selected_ids_as_list(self) -> Tuple[str]:
+    def get_selected_ids_as_list(self) -> Sequence[str]:
         return tuple(x.identifier for x in self.get_selected_list())
     
     def get_selected_ids_joined(self) -> str:
         return ', '.join(self.get_selected_ids_as_list())
     
-    def get_selected_ids_quoted_as_list(self) -> Tuple[str]:
+    def get_selected_ids_quoted_as_list(self) -> Sequence[str]:
         return tuple(self._enquote(x) for x in self.get_selected_ids_as_list())
     
     def get_selected_ids_quoted_joined(self) -> str:
         return ', '.join(self.get_selected_ids_quoted_as_list())
     
-    def get_selected_labels_as_list(self) -> Tuple[str]:
+    def get_selected_labels_as_list(self) -> Sequence[str]:
         return tuple(x.label for x in self.get_selected_list())
     
     def get_selected_labels_joined(self) -> str:
         return ', '.join(self.get_selected_labels_as_list())
     
-    def get_selected_labels_quoted_as_list(self) -> Tuple[str]:
+    def get_selected_labels_quoted_as_list(self) -> Sequence[str]:
         return tuple(self._enquote(x) for x in self.get_selected_labels_as_list())
     
     def get_selected_labels_quoted_joined(self) -> str:
         return ', '.join(self.get_selected_labels_quoted_as_list())
     
-    def _get_selected_ids_as_list(self) -> Tuple[str]:
+    def _get_selected_ids_as_list(self) -> Sequence[str]:
         return self.get_selected_ids_as_list()
     
-    def _get_default(self) -> Tuple[str]:
+    def _get_default(self) -> Sequence[str]:
         return tuple(self._get_default_iterator())
     
     def _set_default_as_selection_mutate(self):
         self.selected_ids = self._get_default()
 
     def to_dict(self):
         output = super().to_dict()
@@ -260,19 +250,19 @@
     curr_option: po.DateParameterOption
     selected_date: datetime
 
     def __init__(self, name: str, label: str, default_date: Union[str, datetime], date_format: str = '%Y-%m-%d', 
                  *, is_hidden: bool = False) -> None:
         self.curr_option = po.DateParameterOption(default_date, date_format)
         all_options = (self.curr_option,)
-        super().__init__(WidgetType.DateField, name, label, all_options, is_hidden, None)
+        super().__init__(name, label, all_options, is_hidden, None)
         self._set_default_as_selection_mutate()
     
     @staticmethod
-    def WithParent(name: str, label: str, all_options: Iterable[po.DateParameterOption], parent: SingleSelectParameter, *, 
+    def WithParent(name: str, label: str, all_options: Sequence[po.DateParameterOption], parent: SingleSelectParameter, *, 
                    is_hidden: bool = False) -> DateParameter:
         new_param = DateParameter(name, label, '2020-01-01', is_hidden=is_hidden) # dummy date
         return Parameter.WithParent(all_options, parent, new_param)
     
     def with_selection(self, selection: str):
         param_copy = copy.copy(self)
         try:
@@ -313,19 +303,19 @@
     selected_value: Decimal
 
     def __init__(self, name: str, label: str, min_value: po.Number, max_value: po.Number, increment: po.Number = 1, 
                  default_value: po.Number = None, *, is_hidden: bool = False) -> None:
         default_value = default_value if default_value is not None else min_value
         curr_option = po.NumberParameterOption(min_value, max_value, increment, default_value)
         all_options = (curr_option,)
-        super().__init__(WidgetType.NumberField, name, label, all_options, is_hidden, None, curr_option)
+        super().__init__(name, label, all_options, is_hidden, None, curr_option)
         self._set_default_as_selection_mutate()
     
     @staticmethod
-    def WithParent(name: str, label: str, all_options: Iterable[po.NumberParameterOption], parent: SingleSelectParameter, *, 
+    def WithParent(name: str, label: str, all_options: Sequence[po.NumberParameterOption], parent: SingleSelectParameter, *, 
                    is_hidden: bool = False) -> DateParameter:
         new_param = NumberParameter(name, label, 0, 1, is_hidden=is_hidden) # dummy values
         return Parameter.WithParent(all_options, parent, new_param)
     
     def with_selection(self, selection: str):
         param_copy = copy.copy(self)
         try:
@@ -354,19 +344,19 @@
 
     def __init__(self, name: str, label: str, min_value: po.Number, max_value: po.Number, increment: po.Number = 1, 
                  default_lower_value: po.Number = None, default_upper_value: po.Number = None, *, is_hidden: bool = False) -> None:
         default_lower_value = default_lower_value if default_lower_value is not None else min_value
         default_upper_value = default_upper_value if default_upper_value is not None else max_value
         curr_option = po.NumRangeParameterOption(min_value, max_value, increment, default_lower_value, default_upper_value)
         all_options = (curr_option,)
-        super().__init__(WidgetType.RangeField, name, label, all_options, is_hidden, None, curr_option)
+        super().__init__(name, label, all_options, is_hidden, None, curr_option)
         self._set_default_as_selection_mutate()
     
     @staticmethod
-    def WithParent(name: str, label: str, all_options: Iterable[po.NumRangeParameterOption], parent: SingleSelectParameter, *, 
+    def WithParent(name: str, label: str, all_options: Sequence[po.NumRangeParameterOption], parent: SingleSelectParameter, *, 
                    is_hidden: bool = False) -> DateParameter:
         new_param = NumRangeParameter(name, label, 0, 1, is_hidden=is_hidden) # dummy values
         return Parameter.WithParent(all_options, parent, new_param)
     
     def with_selection(self, selection: str):
         try:
             lower, upper = selection.split(',')
```

### Comparing `squirrels-0.1.0rc2/squirrels/renderer.py` & `squirrels-0.1.0rc3/squirrels/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,27 @@
                 parameter_set = parameter_set.merge(updates)
         timer.add_activity_time(f"apply selections - dataset {self.dataset}", start)
         
         return parameter_set
 
     def _render_context(self, context_func: ContextFunc, param_set: ParameterSet) -> Dict[str, Any]:
         try:
-            return context_func(param_set, self.manifest.get_proj_vars()) if context_func is not None else {}
+            return context_func(prms=param_set) if context_func is not None else {}
         except Exception as e:
             raise ConfigurationError(f'Error in the {c.CONTEXT_FILE} function for dataset "{self.dataset}"') from e
     
-    def _get_args(self, param_set: ParameterSet, context: Dict[str, Any]) -> Dict:
+    def _get_args(self, param_set: ParameterSet, context: Dict[str, Any], db_view: str = None) -> Dict:
+        if db_view is not None:
+            args = self.manifest.get_view_args(self.dataset, db_view)
+        else:
+            args = self.manifest.get_view_args(self.dataset)
         return {
             'prms': param_set,
             'ctx':  context,
-            'proj': self.manifest.get_proj_vars()
+            'args': args
         }
     
     def _render_query_from_raw(self, raw_query: Query, args: Dict) -> Query:
         if isinstance(raw_query, str):
             template = utils.j2_env.from_string(raw_query)
             return template.render(args)
         else:
@@ -141,21 +145,22 @@
         start = time.time()
         context = self._render_context(self.context_func, param_set)
         timer.add_activity_time(f"render context - dataset {self.dataset}", start)
 
         # render database view queries
         start = time.time()
         query_by_db_view = {}
-        args = self._get_args(param_set, context)
         for db_view, raw_query in self.raw_query_by_db_view.items():
+            args = self._get_args(param_set, context, db_view)
             query_by_db_view[db_view] = self._render_query_from_raw(raw_query, args)
         timer.add_activity_time(f"render database view queries - dataset {self.dataset}", start)
 
         # render final view query
         start = time.time()
+        args = self._get_args(param_set, context)
         final_view_query = self._render_query_from_raw(self.raw_final_view_query, args)
         timer.add_activity_time(f"render final view query - dataset {self.dataset}", start)
 
         # render all dataframes if "run_query" is enabled
         df_by_db_views = {}
         final_view_df = None
         if run_query:
@@ -174,38 +179,40 @@
     return {}
 
 
 class RendererIOWrapper:
     def __init__(self, dataset: str, manifest: mf.Manifest, conn_set: ConnectionSet, excel_file_name: Optional[str] = None):
         dataset_folder = manifest.get_dataset_folder(dataset)
         parameters_path = utils.join_paths(dataset_folder, c.PARAMETERS_FILE)
+        args = manifest.get_dataset_args(dataset)
         parameters_module = utils.import_file_as_module(parameters_path)
         try:
-            parameter_set = parameters_module.main()
+            parameter_set = parameters_module.main(args=args)
         except Exception as e:
             raise ConfigurationError(f'Error in the {c.PARAMETERS_FILE} function for dataset "{dataset}"') from e
 
         context_path = utils.join_paths(dataset_folder, c.CONTEXT_FILE)
         try:
-            context_func = utils.import_file_as_module(context_path).main
+            context_module = utils.import_file_as_module(context_path)
+            context_func = partial(context_module.main, args=args)
         except FileNotFoundError:
             context_func = default_context_func
         
         excel_file = None
         if excel_file_name is not None:
             excel_file_path = utils.join_paths(dataset_folder, excel_file_name)
             excel_file = pd.ExcelFile(excel_file_path)
         
         db_views = manifest.get_all_database_view_names(dataset)
         raw_query_by_db_view = {}
         for db_view in db_views:
             db_view_template_path = str(manifest.get_database_view_file(dataset, db_view))
             raw_query_by_db_view[db_view] = self._get_raw_query(db_view_template_path)
         
-        final_view_path = str(manifest.get_dataset_final_view(dataset))
+        final_view_path = str(manifest.get_dataset_final_view_file(dataset))
         if final_view_path in db_views:
             raw_final_view_query = final_view_path
         else:
             raw_final_view_query = self._get_raw_query(final_view_path)
         
         self.dataset_folder = dataset_folder
         self.output_folder = utils.join_paths(c.OUTPUTS_FOLDER, dataset)
```

### Comparing `squirrels-0.1.0rc2/squirrels/timed_imports.py` & `squirrels-0.1.0rc3/squirrels/timed_imports.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Dict, Tuple
+from typing import Dict, List
 import time
 
 
 class Timer:
     def __init__(self, verbose: bool = False):
-        self.times: Dict[str, Tuple[str, str]] = dict()
+        self.times: Dict[str, List[float]] = dict()
         self.verbose = verbose
     
     def add_activity_time(self, activity: str, start: float):
-        time_taken = (time.time()-start) * 10**3
-        total_time, count = self.times.get(activity, (0, 0))
-        self.times[activity] = (total_time+time_taken, count+1)
         if self.verbose:
+            time_taken = (time.time()-start) * 10**3
+            times_list = self.times.setdefault(activity, list())
+            times_list.append(time_taken)
             print(f'Time taken for "{activity}": {time_taken}ms')
     
     def report_times(self):
         if self.verbose:
-            for activity, time_stats in self.times.items():
-                total_time, count = time_stats
-                avg_time = total_time / count
+            for activity, times_list in self.times.items():
+                total_time = sum(times_list)
+                avg_time = total_time / len(times_list)
                 print()
                 print(f'Time statistics for "{activity}":')
                 print(f'  Total time: {total_time}ms')
                 print(f'  Average time: {avg_time}ms')
 
 timer = Timer()
```

### Comparing `squirrels-0.1.0rc2/squirrels/utils.py` & `squirrels-0.1.0rc3/squirrels/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 # Custom Exceptions
 class InvalidInputError(Exception):
     pass
 
 class ConfigurationError(Exception):
     pass
 
+class AbstractMethodCallError(NotImplementedError):
+    def __init__(self, cls, method, more_message = ""):
+        message = f"Abstract method {method}() not implemented in {cls.__name__}."
+        super().__init__(message + more_message)
+
 
 # Utility functions/variables
 j2_env = j2.Environment(loader=j2.FileSystemLoader('.'))
 
 
 def import_file_as_module(filepath: Optional[FilePath]) -> ModuleType:
     """
```

### Comparing `squirrels-0.1.0rc2/squirrels.egg-info/PKG-INFO` & `squirrels-0.1.0rc3/squirrels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrels
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Python Package for Configuring SQL Generating APIs
 Author: Tim Huang
 Author-email: tim.yuting@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `squirrels-0.1.0rc2/squirrels.egg-info/SOURCES.txt` & `squirrels-0.1.0rc3/squirrels.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 squirrels.egg-info/SOURCES.txt
 squirrels.egg-info/dependency_links.txt
 squirrels.egg-info/entry_points.txt
 squirrels.egg-info/requires.txt
 squirrels.egg-info/top_level.txt
 squirrels/package_data/base_project/.gitignore
 squirrels/package_data/base_project/connections.py
-squirrels/package_data/base_project/project_vars.yaml
 squirrels/package_data/base_project/squirrels.yaml
 squirrels/package_data/base_project/database/sample_database.db
 squirrels/package_data/base_project/database/seattle_weather.db
 squirrels/package_data/base_project/datasets/sample_dataset/context.py
 squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
 squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
 squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
```

