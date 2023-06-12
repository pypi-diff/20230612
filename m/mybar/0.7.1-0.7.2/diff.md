# Comparing `tmp/mybar-0.7.1.tar.gz` & `tmp/mybar-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybar-0.7.1.tar", last modified: Sat Jun 10 06:43:51 2023, max compression
+gzip compressed data, was "mybar-0.7.2.tar", last modified: Mon Jun 12 09:15:14 2023, max compression
```

## Comparing `mybar-0.7.1.tar` & `mybar-0.7.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-10 06:43:51.853762 mybar-0.7.1/
--rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.7.1/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-10 06:43:51.853762 mybar-0.7.1/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.7.1/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-10 06:43:51.853762 mybar-0.7.1/mybar/
--rw-r--r--   0 sam       (1000) sam       (1000)      601 2023-06-10 06:41:32.000000 mybar-0.7.1/mybar/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-06-01 10:53:22.000000 mybar-0.7.1/mybar/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-05-30 09:20:33.000000 mybar-0.7.1/mybar/_setups.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3846 2023-05-31 09:01:05.000000 mybar-0.7.1/mybar/_types.py
--rw-r--r--   0 sam       (1000) sam       (1000)    46651 2023-06-06 10:30:53.000000 mybar-0.7.1/mybar/bar.py
--rw-r--r--   0 sam       (1000) sam       (1000)    12944 2023-06-10 06:37:43.000000 mybar-0.7.1/mybar/cli.py
--rw-r--r--   0 sam       (1000) sam       (1000)      861 2023-06-02 05:55:18.000000 mybar-0.7.1/mybar/constants.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2112 2023-05-29 11:58:23.000000 mybar-0.7.1/mybar/defaults.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3439 2023-06-02 11:18:30.000000 mybar-0.7.1/mybar/errors.py
--rw-r--r--   0 sam       (1000) sam       (1000)    28629 2023-06-06 09:58:42.000000 mybar-0.7.1/mybar/field.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13999 2023-06-06 11:33:06.000000 mybar-0.7.1/mybar/field_funcs.py
--rw-r--r--   0 sam       (1000) sam       (1000)    28082 2023-06-06 12:01:35.000000 mybar-0.7.1/mybar/formatting.py
--rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-05-31 11:58:31.000000 mybar-0.7.1/mybar/log.py
--rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.7.1/mybar/sync.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1929 2023-05-30 10:32:04.000000 mybar-0.7.1/mybar/templates.py
--rw-r--r--   0 sam       (1000) sam       (1000)     5685 2023-05-29 15:02:35.000000 mybar-0.7.1/mybar/utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-10 06:43:51.853762 mybar-0.7.1/mybar.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      468 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-10 06:43:51.000000 mybar-0.7.1/mybar.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.7.1/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.7.1/requirements.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      892 2023-06-10 06:43:51.857095 mybar-0.7.1/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 09:15:14.052176 mybar-0.7.2/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1077 2023-03-16 08:41:11.000000 mybar-0.7.2/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-12 09:15:14.052176 mybar-0.7.2/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      155 2023-03-16 08:41:11.000000 mybar-0.7.2/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 09:15:14.052176 mybar-0.7.2/mybar/
+-rw-r--r--   0 sam       (1000) sam       (1000)      601 2023-06-12 09:13:43.000000 mybar-0.7.2/mybar/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-06-01 10:53:22.000000 mybar-0.7.2/mybar/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-05-30 09:20:33.000000 mybar-0.7.2/mybar/_setups.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3846 2023-05-31 09:01:05.000000 mybar-0.7.2/mybar/_types.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    46651 2023-06-12 09:09:56.000000 mybar-0.7.2/mybar/bar.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13417 2023-06-12 09:11:45.000000 mybar-0.7.2/mybar/cli.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      861 2023-06-02 05:55:18.000000 mybar-0.7.2/mybar/constants.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2112 2023-05-29 11:58:23.000000 mybar-0.7.2/mybar/defaults.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3439 2023-06-02 11:18:30.000000 mybar-0.7.2/mybar/errors.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    28629 2023-06-12 09:09:56.000000 mybar-0.7.2/mybar/field.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13999 2023-06-06 11:33:06.000000 mybar-0.7.2/mybar/field_funcs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    28082 2023-06-06 12:01:35.000000 mybar-0.7.2/mybar/formatting.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-05-31 11:58:31.000000 mybar-0.7.2/mybar/log.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    13368 2023-05-03 06:07:43.000000 mybar-0.7.2/mybar/sync.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1929 2023-06-12 09:09:56.000000 mybar-0.7.2/mybar/templates.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     5685 2023-05-29 15:02:35.000000 mybar-0.7.2/mybar/utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 09:15:14.052176 mybar-0.7.2/mybar.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      468 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-06-12 09:15:14.000000 mybar-0.7.2/mybar.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-03-16 08:41:11.000000 mybar-0.7.2/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-03-16 08:41:11.000000 mybar-0.7.2/requirements.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)      892 2023-06-12 09:15:14.052176 mybar-0.7.2/setup.cfg
```

### Comparing `mybar-0.7.1/LICENSE` & `mybar-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/PKG-INFO` & `mybar-0.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.7.1
+Version: 0.7.2
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.7.1/mybar/__init__.py` & `mybar-0.7.2/mybar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 :copyright: (c) 2021-present by LonelyAbsol.
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'mybar'
 __description__ = "An async status bar with a highly customizable API."
 __url__ = "https://github.com/lonelyabsol/mybar"
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 __author__ = "LonelyAbsol"
 __license__ = 'MIT'
 __copyright__ = "Copyright (c) 2021-present LonelyAbsol"
 
 
 from .constants import *
 from . import utils
```

### Comparing `mybar-0.7.1/mybar/_setups.py` & `mybar-0.7.2/mybar/_setups.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/_types.py` & `mybar-0.7.2/mybar/_types.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/bar.py` & `mybar-0.7.2/mybar/bar.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/cli.py` & `mybar-0.7.2/mybar/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,41 +172,41 @@
 
                     field_definitions[field_name].update({field_opt: val})
 
         return field_definitions
 
     def add_arguments(self) -> None:
         '''Equip the parser with all its arguments.'''
-        fields_or_fmt = self.add_mutually_exclusive_group()
-        fields_or_fmt.add_argument(
+        fields_or_tmpl = self.add_mutually_exclusive_group()
+        fields_or_tmpl.add_argument(
             '-t', '--template',
             metavar="'TEMPLATE'",
             dest='template',
             help=(
                 "A curly-brace-delimited format string."
                 " Not valid with --fields/-f options."
             ),
         )
 
-        fields_or_fmt.add_argument(
+        fields_or_tmpl.add_argument(
             '-f', '--fields',
             action='extend',
             nargs='+',
             metavar=('FIELDNAME1', 'FIELDNAME2'),
             dest='field_order',
             # type=ArgFormatter.SplitFirst(','),
             help=(
                 "A list of fields to be displayed."
-                " Not valid with --format/-m options."
+                " Not valid with --template/-t options."
             ),
         )
 
         fields_group = self.add_argument_group(
             title="Options for fields",
-            description="These options are not valid when using --format/-m."
+            description="These options are not valid when using --template/-t."
         )
 
         fields_group.add_argument(
             '--icons',
             action='extend',
             nargs='+',
             metavar=("FIELDNAME1='ICON1'", "FIELDNAME2='ICON2'"),
@@ -253,33 +253,47 @@
             dest='refresh_rate',
             help=(
                 "The bar's refresh rate in seconds per cycle."
             ),
         )
 
         self.add_argument(
-            '--config', '-c',
-            metavar='FILE',
-            dest='config_file',
-            help=(
-                "The config file to use for default settings."
-            ),
-        )
-
-        self.add_argument(
             '--count', '-n',
             type=int,
             metavar='TIMES',
             dest='count',
             help=(
                 "Print the bar this many times, then exit."
             ),
         )
 
         self.add_argument(
+            '--config', '-c',
+            metavar='FILE',
+            dest='config_file',
+            help=(
+                "The config file to use for default settings."
+            ),
+        )
+
+##        self.add_argument(
+##            '--dump', '-d',
+##            type=int,
+##            nargs='?',
+##            metavar='INDENT',
+##            dest='dump_config',
+##            help=(
+##                "Instead of running the bar, print a JSON config using"
+##                " options specified in the command."
+##                " Optionally pass a number of spaces to indent by,"
+##                " which defaults to 4."
+##            ),
+##        )
+
+        self.add_argument(
             '--debug',
             action='store_true',
             help="Use debug mode. (Not implemented)",
         )
 
     def quit(self, message: str = "Exiting...") -> NoReturn:
         '''Print a message and exit the program.'''
```

### Comparing `mybar-0.7.1/mybar/constants.py` & `mybar-0.7.2/mybar/constants.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/defaults.py` & `mybar-0.7.2/mybar/defaults.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/errors.py` & `mybar-0.7.2/mybar/errors.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/field.py` & `mybar-0.7.2/mybar/field.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/field_funcs.py` & `mybar-0.7.2/mybar/field_funcs.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/formatting.py` & `mybar-0.7.2/mybar/formatting.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/sync.py` & `mybar-0.7.2/mybar/sync.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/templates.py` & `mybar-0.7.2/mybar/templates.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar/utils.py` & `mybar-0.7.2/mybar/utils.py`

 * *Files identical despite different names*

### Comparing `mybar-0.7.1/mybar.egg-info/PKG-INFO` & `mybar-0.7.2/mybar.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.7.1
+Version: 0.7.2
 Summary: An async status bar with a highly customizable API.
 Home-page: https://github.com/lonelyabsol/mybar
 Author: lonelyabsol
 License: MIT
 Project-URL: GitHub: repo, https://github.com/lonelyabsol/mybar
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mybar-0.7.1/setup.cfg` & `mybar-0.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mybar
-version = 0.7.1
+version = 0.7.2
 description = An async status bar with a highly customizable API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = lonelyabsol
 url = https://github.com/lonelyabsol/mybar
 project_urls = 
 	GitHub: repo = https://github.com/lonelyabsol/mybar
```

