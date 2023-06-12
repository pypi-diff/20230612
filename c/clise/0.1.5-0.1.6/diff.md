# Comparing `tmp/clise-0.1.5.tar.gz` & `tmp/clise-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clise-0.1.5.tar", last modified: Tue Mar  7 20:45:33 2023, max compression
+gzip compressed data, was "clise-0.1.6.tar", last modified: Mon Jun 12 14:13:53 2023, max compression
```

## Comparing `clise-0.1.5.tar` & `clise-0.1.6.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-03-07 20:45:33.091693 clise-0.1.5/
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       43 2022-04-28 16:59:05.000000 clise-0.1.5/AUTHORS
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1079 2023-01-05 15:53:34.000000 clise-0.1.5/LICENSE
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       75 2023-01-05 15:53:08.000000 clise-0.1.5/MANIFEST.in
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     6331 2023-03-07 20:45:33.091693 clise-0.1.5/PKG-INFO
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     5874 2023-03-07 20:45:32.000000 clise-0.1.5/README.txt
-drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-03-07 20:45:33.087692 clise-0.1.5/clise/
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       49 2023-03-07 20:45:32.000000 clise-0.1.5/clise/__init__.py
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      289 2023-01-05 05:15:50.000000 clise-0.1.5/clise/__main__.py
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     8731 2023-02-01 23:24:26.000000 clise-0.1.5/clise/cmdscript.py
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      921 2023-02-15 17:30:10.000000 clise-0.1.5/clise/demo.py
-drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-03-07 20:45:33.087692 clise-0.1.5/clise/doc/
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)    49147 2023-03-07 20:45:32.000000 clise-0.1.5/clise/doc/heron.md
-drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-03-07 20:45:33.091693 clise-0.1.5/clise/examples/
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)        0 2023-01-21 16:04:35.000000 clise-0.1.5/clise/examples/cmd.sh
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      156 2023-01-03 22:20:35.000000 clise-0.1.5/clise/examples/demo_autogen_by_file.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      216 2023-01-04 03:13:05.000000 clise-0.1.5/clise/examples/demo_autogen_by_file_native.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      380 2023-01-04 03:13:00.000000 clise-0.1.5/clise/examples/demo_autogen_by_file_native_bundles.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      128 2023-01-04 03:12:52.000000 clise-0.1.5/clise/examples/demo_autogen_by_file_native_bundles_file.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      652 2023-01-03 20:59:10.000000 clise-0.1.5/clise/examples/demo_autogen_by_id.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      761 2023-01-04 03:12:44.000000 clise-0.1.5/clise/examples/demo_autogen_by_id_native.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1064 2023-01-04 03:12:39.000000 clise-0.1.5/clise/examples/demo_autogen_by_id_native_bundles.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      451 2023-01-04 03:12:33.000000 clise-0.1.5/clise/examples/demo_autogen_by_id_native_bundles_file.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       73 2023-01-03 21:49:36.000000 clise-0.1.5/clise/examples/demo_by_file.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      295 2023-01-03 22:02:11.000000 clise-0.1.5/clise/examples/demo_by_files.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      898 2023-01-03 22:02:25.000000 clise-0.1.5/clise/examples/demo_explicit_tasks.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       58 2023-01-03 20:10:50.000000 clise-0.1.5/clise/examples/demo_one_task.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      792 2023-01-04 15:24:20.000000 clise-0.1.5/clise/examples/demo_replace_pars.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      222 2023-01-05 03:56:14.000000 clise-0.1.5/clise/examples/demo_simple_dict.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      327 2023-01-04 04:47:00.000000 clise-0.1.5/clise/examples/demo_two_by_files_gen.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      479 2023-01-04 04:51:53.000000 clise-0.1.5/clise/examples/demo_two_by_files_gen_complete.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      637 2023-01-04 05:21:33.000000 clise-0.1.5/clise/examples/demo_two_by_files_gen_double.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      587 2023-01-04 03:49:31.000000 clise-0.1.5/clise/examples/demo_two_tasks.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      944 2023-01-04 04:01:11.000000 clise-0.1.5/clise/examples/demo_two_tasks_complete.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)        0 2023-01-21 16:04:35.000000 clise-0.1.5/clise/examples/test.sh
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)    24035 2023-03-07 20:23:25.000000 clise-0.1.5/clise/heron.py
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)    44898 2023-02-22 19:04:13.000000 clise-0.1.5/clise/jsontool.py
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)   118796 2023-03-07 20:40:26.000000 clise-0.1.5/clise/plottool.py
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)    28410 2023-02-15 18:08:53.000000 clise-0.1.5/clise/rabbit.py
-drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-03-07 20:45:33.091693 clise-0.1.5/clise/startup/
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      257 2023-01-03 01:59:18.000000 clise-0.1.5/clise/startup/cmdline_rabbit.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      542 2023-01-02 01:08:04.000000 clise-0.1.5/clise/startup/scan_hdus_plot1d_rabbit.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      565 2023-01-02 01:08:11.000000 clise-0.1.5/clise/startup/scan_hdus_plot1d_rabbit_noswap.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)      577 2023-01-05 20:41:19.000000 clise-0.1.5/clise/startup/startup.json5
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)    18194 2023-03-07 20:41:22.000000 clise-0.1.5/clise/tabletool.py
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)    32989 2023-03-03 21:31:07.000000 clise-0.1.5/clise/xray_mirror.py
-drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-03-07 20:45:33.087692 clise-0.1.5/clise.egg-info/
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     6331 2023-03-07 20:45:32.000000 clise-0.1.5/clise.egg-info/PKG-INFO
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1481 2023-03-07 20:45:33.000000 clise-0.1.5/clise.egg-info/SOURCES.txt
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)        1 2023-03-07 20:45:32.000000 clise-0.1.5/clise.egg-info/dependency_links.txt
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       43 2023-03-07 20:45:32.000000 clise-0.1.5/clise.egg-info/entry_points.txt
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       10 2023-03-07 20:45:32.000000 clise-0.1.5/clise.egg-info/requires.txt
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)        6 2023-03-07 20:45:32.000000 clise-0.1.5/clise.egg-info/top_level.txt
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)       38 2023-03-07 20:45:33.091693 clise-0.1.5/setup.cfg
--rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1209 2023-03-03 16:57:02.000000 clise-0.1.5/setup.py
+drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-06-12 14:13:53.921513 clise-0.1.6/
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       43 2022-04-28 16:59:05.000000 clise-0.1.6/AUTHORS
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1079 2023-01-05 15:53:34.000000 clise-0.1.6/LICENSE
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       75 2023-01-05 15:53:08.000000 clise-0.1.6/MANIFEST.in
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     6331 2023-06-12 14:13:53.921513 clise-0.1.6/PKG-INFO
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     5874 2023-06-12 14:13:53.000000 clise-0.1.6/README.txt
+drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-06-12 14:13:53.917514 clise-0.1.6/clise/
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       49 2023-06-12 14:13:53.000000 clise-0.1.6/clise/__init__.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      289 2023-01-05 05:15:50.000000 clise-0.1.6/clise/__main__.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     8731 2023-02-01 23:24:26.000000 clise-0.1.6/clise/cmdscript.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      921 2023-02-15 17:30:10.000000 clise-0.1.6/clise/demo.py
+drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-06-12 14:13:53.917514 clise-0.1.6/clise/doc/
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)    49455 2023-06-12 14:13:53.000000 clise-0.1.6/clise/doc/heron.md
+drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-06-12 14:13:53.921513 clise-0.1.6/clise/examples/
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)        0 2023-01-21 16:04:35.000000 clise-0.1.6/clise/examples/cmd.sh
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      156 2023-01-03 22:20:35.000000 clise-0.1.6/clise/examples/demo_autogen_by_file.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      216 2023-01-04 03:13:05.000000 clise-0.1.6/clise/examples/demo_autogen_by_file_native.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      380 2023-01-04 03:13:00.000000 clise-0.1.6/clise/examples/demo_autogen_by_file_native_bundles.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      128 2023-01-04 03:12:52.000000 clise-0.1.6/clise/examples/demo_autogen_by_file_native_bundles_file.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      652 2023-01-03 20:59:10.000000 clise-0.1.6/clise/examples/demo_autogen_by_id.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      761 2023-01-04 03:12:44.000000 clise-0.1.6/clise/examples/demo_autogen_by_id_native.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1064 2023-01-04 03:12:39.000000 clise-0.1.6/clise/examples/demo_autogen_by_id_native_bundles.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      451 2023-01-04 03:12:33.000000 clise-0.1.6/clise/examples/demo_autogen_by_id_native_bundles_file.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       73 2023-01-03 21:49:36.000000 clise-0.1.6/clise/examples/demo_by_file.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      295 2023-01-03 22:02:11.000000 clise-0.1.6/clise/examples/demo_by_files.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      898 2023-01-03 22:02:25.000000 clise-0.1.6/clise/examples/demo_explicit_tasks.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       58 2023-01-03 20:10:50.000000 clise-0.1.6/clise/examples/demo_one_task.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      792 2023-01-04 15:24:20.000000 clise-0.1.6/clise/examples/demo_replace_pars.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      222 2023-01-05 03:56:14.000000 clise-0.1.6/clise/examples/demo_simple_dict.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      327 2023-01-04 04:47:00.000000 clise-0.1.6/clise/examples/demo_two_by_files_gen.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      479 2023-01-04 04:51:53.000000 clise-0.1.6/clise/examples/demo_two_by_files_gen_complete.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      637 2023-01-04 05:21:33.000000 clise-0.1.6/clise/examples/demo_two_by_files_gen_double.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      587 2023-01-04 03:49:31.000000 clise-0.1.6/clise/examples/demo_two_tasks.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      944 2023-01-04 04:01:11.000000 clise-0.1.6/clise/examples/demo_two_tasks_complete.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)        0 2023-01-21 16:04:35.000000 clise-0.1.6/clise/examples/test.sh
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)    24219 2023-06-12 14:13:16.000000 clise-0.1.6/clise/heron.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)    44898 2023-02-22 19:04:13.000000 clise-0.1.6/clise/jsontool.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)   123038 2023-06-07 16:18:33.000000 clise-0.1.6/clise/plottool.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)    28458 2023-05-04 19:15:18.000000 clise-0.1.6/clise/rabbit.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      784 2023-03-24 15:40:46.000000 clise-0.1.6/clise/rebin.py
+drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-06-12 14:13:53.921513 clise-0.1.6/clise/startup/
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      257 2023-01-03 01:59:18.000000 clise-0.1.6/clise/startup/cmdline_rabbit.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      542 2023-01-02 01:08:04.000000 clise-0.1.6/clise/startup/scan_hdus_plot1d_rabbit.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      565 2023-01-02 01:08:11.000000 clise-0.1.6/clise/startup/scan_hdus_plot1d_rabbit_noswap.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)      577 2023-01-05 20:41:19.000000 clise-0.1.6/clise/startup/startup.json5
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)    18376 2023-04-13 19:18:59.000000 clise-0.1.6/clise/tabletool.py
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)    33485 2023-03-20 21:47:23.000000 clise-0.1.6/clise/xray_mirror.py
+drwxr-xr-x   0 jaesub    (1000) jaesub    (1000)        0 2023-06-12 14:13:53.917514 clise-0.1.6/clise.egg-info/
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     6331 2023-06-12 14:13:53.000000 clise-0.1.6/clise.egg-info/PKG-INFO
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1496 2023-06-12 14:13:53.000000 clise-0.1.6/clise.egg-info/SOURCES.txt
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)        1 2023-06-12 14:13:53.000000 clise-0.1.6/clise.egg-info/dependency_links.txt
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       43 2023-06-12 14:13:53.000000 clise-0.1.6/clise.egg-info/entry_points.txt
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       10 2023-06-12 14:13:53.000000 clise-0.1.6/clise.egg-info/requires.txt
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)        6 2023-06-12 14:13:53.000000 clise-0.1.6/clise.egg-info/top_level.txt
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)       38 2023-06-12 14:13:53.921513 clise-0.1.6/setup.cfg
+-rw-r--r--   0 jaesub    (1000) jaesub    (1000)     1209 2023-03-03 16:57:02.000000 clise-0.1.6/setup.py
```

### Comparing `clise-0.1.5/LICENSE` & `clise-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/PKG-INFO` & `clise-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: clise
-Version: 0.1.5
+Version: 0.1.6
 Summary: Command liner with JSON based input file
-Home-page: https://pypi.org/project/clise/0.1.5
+Home-page: https://pypi.org/project/clise/0.1.6
 Author: Jaesub Hong
 Author-email: jhong@cfa.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 License-File: AUTHORS
 
 ### CLISe: Command Line Input Setter
 
 Command liner for python routines using JSON based input parameter files. It
 dives into a module with CLI and execute a routine just as herons dive into
 water and catch fish. It also uses JSON text to create task lists to automatize
-multiple executions of the routine: ver 0.1.5 by Jaesub Hong
+multiple executions of the routine: ver 0.1.6 by Jaesub Hong
 (jhong@cfa.harvard.edu)
 
        Usage: clise JSON_input_file1 -options_for_file1 ... \
             [json_input_file2 -options_for_file2 ...] \
             [--with common_json_files -common_options ...] \
             [--WITH common_json_files -common_options ...]
```

### Comparing `clise-0.1.5/README.txt` & `clise-0.1.6/README.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### CLISe: Command Line Input Setter
 
 Command liner for python routines using JSON based input parameter files. It
 dives into a module with CLI and execute a routine just as herons dive into
 water and catch fish. It also uses JSON text to create task lists to automatize
-multiple executions of the routine: ver 0.1.5 by Jaesub Hong
+multiple executions of the routine: ver 0.1.6 by Jaesub Hong
 (jhong@cfa.harvard.edu)
 
        Usage: clise JSON_input_file1 -options_for_file1 ... \
             [json_input_file2 -options_for_file2 ...] \
             [--with common_json_files -common_options ...] \
             [--WITH common_json_files -common_options ...]
```

### Comparing `clise-0.1.5/clise/cmdscript.py` & `clise-0.1.6/clise/cmdscript.py`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/demo.py` & `clise-0.1.6/clise/demo.py`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/doc/heron.md` & `clise-0.1.6/clise/doc/heron.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### CLISe: Command Line Input Setter
 
 Command liner for python routines using JSON based input parameter files. It
 dives into a module with CLI and execute a routine just as herons dive into
 water and catch fish. It also uses JSON text to create task lists to automatize
-multiple executions of the routine: ver 0.1.5 by Jaesub Hong
+multiple executions of the routine: ver 0.1.6 by Jaesub Hong
 (jhong@cfa.harvard.edu)
 
        Usage: clise JSON_input_file1 -options_for_file1 ... \
             [json_input_file2 -options_for_file2 ...] \
             [--with common_json_files -common_options ...] \
             [--WITH common_json_files -common_options ...]
 
@@ -1145,14 +1145,24 @@
 
        yes         yes w. end phrase   -                task generation block
        yes/no      no                  end phrase       the end of the task gen seed
        no          -                   "rabbit"         common parameter block for the task gen seed
 
 ### Changes
 
+v0.1.6 2023/06
+      - add wcs  to dplot  in plottool: 
+                        e.g., -attr wcs
+                        range set by degrees
+      - add time to plot1d in plottool: 
+                        e.g., -attr xtime,ytime
+      - add cmos.py
+
+      - add rebin.py  and update plottool.py with rebin
+
 v0.1.5 2023/03
       - add read_mca in tabletool
 
 v0.1.4 2023/03
       - adhoc fix of a bug in loading clise's own modules
 
 v0.1.3 2023/03
```

### Comparing `clise-0.1.5/clise/examples/demo_autogen_by_id.json5` & `clise-0.1.6/clise/examples/demo_autogen_by_id.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/examples/demo_autogen_by_id_native.json5` & `clise-0.1.6/clise/examples/demo_autogen_by_id_native.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/examples/demo_autogen_by_id_native_bundles.json5` & `clise-0.1.6/clise/examples/demo_autogen_by_id_native_bundles.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/examples/demo_explicit_tasks.json5` & `clise-0.1.6/clise/examples/demo_explicit_tasks.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/examples/demo_replace_pars.json5` & `clise-0.1.6/clise/examples/demo_replace_pars.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/examples/demo_two_by_files_gen_double.json5` & `clise-0.1.6/clise/examples/demo_two_by_files_gen_double.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/examples/demo_two_tasks.json5` & `clise-0.1.6/clise/examples/demo_two_tasks.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/examples/demo_two_tasks_complete.json5` & `clise-0.1.6/clise/examples/demo_two_tasks_complete.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/heron.py` & `clise-0.1.6/clise/heron.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 from os		import path, mkdir
 from pathlib	import Path
 from socket		import gethostname
 from collections  import OrderedDict
 from datetime     import datetime
 from importlib    import import_module
-# from IPython	import embed
+from IPython	import embed
 
-__version__    = '0.1.5'
+__version__    = '0.1.6'
 
 cc = jt.cc()
 
 def version():
 	return __version__
 
 # handle input parameters
@@ -251,15 +251,15 @@
 	if levels[0] not in sys.modules:
 		module = __import__(levels[0])
 	else:
 		module = sys.modules[levels[0]]
 
 	# potential class name
 	class_name_ = '.'.join(levels[0:-1])
-	global class_object, class_name
+	global class_obj, class_name
 	if "-object" in cfg:
 		if cfg["-object"] in class_obj:
 			if show_trace: print(cc.key + 'loading the requested object:', cfg["-object"], cc.reset)
 			object = class_obj[cfg["-object"]]
 			routine = getattr(object, levels[-1])
 			return routine, module
 	else:
@@ -297,30 +297,34 @@
 		if idx == nlevels - 3:  # -3 indicates the next to the last name
 
 			icfg = cfg.get('-init', OrderedDict()).copy()
 			icfg['-collect'] = icfg.get('-collect', True)  # by default, collect everything in "-init"
 			init_args, init_kwargs = set_func_parameters([], [], cfg=icfg)
 
 			# print(init_args, init_kwargs)
-			try:
+			# try:
+			if type(routine).__name__ == 'type':
 				# now we are loading a new class or attempting
 
 				class_obj_  = routine(*init_args, **init_kwargs)
 				routine     = getattr(class_obj_, levels[-1])
 
 				# if not specified, then use class_name_ for the key of the object
 				# so that the same class name will share the same object
 				# if there needs to be more than an object for the same class,
 				# one has to specify "-object" to separate them
 				objkey	= cfg.get("-object", class_name_)
 
 				# if you are here, then safe to assign these
 				class_name[objkey] = class_name_
 				class_obj [objkey] = class_obj_
-			except Exception:
+			# except Exception:
+			else:
+				# an issue with "try: .. except:" is if exception occurs due to an error in a class
+				# one ends up here as well, which will fail
 				# oops, not class
 				routine = getattr(routine, levels[-1])
 			break
 
 	return routine, module
 
 def execute_routine(routine, args, kwargs, cfg=None, show_out=False):
```

### Comparing `clise-0.1.5/clise/jsontool.py` & `clise-0.1.6/clise/jsontool.py`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/plottool.py` & `clise-0.1.6/clise/plottool.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import astropy
 from   astropy.table import QTable
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
 from   matplotlib.colors import Normalize, LogNorm, ListedColormap
 import matplotlib.cm     as cm
 import matplotlib        as mpl
+from matplotlib.dates import DateFormatter
 # from matplotlib.patches           import Circle
 # from matplotlib             import rcParams
 # from matplotlib.ticker            import LogLocator
 # from mpl_toolkits.axes_grid1  import make_axes_locatable
 # from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 
 import numpy as np
@@ -44,14 +45,16 @@
 # from IPython    import embed
 
 # import subprocess
 from scipy.signal import savgol_filter
 import re
 from pathlib      import Path
 
+from datetime import datetime
+from time import mktime, strptime
 # ----------------------------------------------------------------------------------------
 cc = jt.cc
 
 # obsolete?
 def help_rcParams():
 	text = OrderedDict()
 	text["figure.figsize"       ] = "changes the figure size; keeps the font size the same"
@@ -205,62 +208,70 @@
 		data = np.array(data)
 		return [np.min(data[np.nonzero(data)]), np.max(data)]
 	else:       return [np.min(data), np.max(data)]
 
 # ----------------------------------------------------------------------------------------
 # regex for scientific number
 scino = re.compile(r'[+\-]?(?:0|[1-9]\d*)(?:\.\d*)?(?:[eE][+\-]?\d+)?')
-def get_number(array):
+def get_number(array, istime=''):
 	# need to vectorize this....
 	# and implement this in tabletool to separate them out
-	ans = []
 	# if type(array[0]) is not str: return array
-	for each in array:
-		# val=re.split('(\D|^\.)',each)
-		# val=re.search('^\s*([-\+][0-9.]+)',each)
-		val = re.findall(scino, each)
-		try: ans.append(float(val[0]))
-		except Exception:
-			ans.append(0.0)
-			print('cannot find a number in', each)
-	return ans
+	if istime == '':
+		ans = []
+		tformat=''
+		for each in array:
+			# val=re.split('(\D|^\.)',each)
+			# val=re.search('^\s*([-\+][0-9.]+)',each)
+			val = re.findall(scino, each)
+			try: ans.append(float(val[0]))
+			except Exception:
+				ans.append(0.0)
+				print('cannot find a number in', each)
+	else:
+		if ':' in istime: _, tformat = istime.split(':')
+		else:	tformat="%y/%m/%d"
+		ans = [datetime.strptime(v,tformat) for v in array]
+		ans = np.array(ans)
+
+	return ans, tformat
 
 # ----------------------------------------------------------------------------------------
-def read_pars(par,  data=None, nopandas=True, dataset=None, infile=None):
+def read_pars(par,  data=None, nopandas=True, dataset=None, infile=None, comment=None):
 	ans = OrderedDict()
 	if dataset is None: dataset = OrderedDict()
 	for key, val in par.items():
 		if type(val) is str:
 			ans[key] = data[val]
 		else:
 			if 'file' not in val: file = infile
 			else:			    file = val['file']
 			if not path.isfile(file):
 				print("cannot read the file:", file)
 				return None
 
 			if file not in dataset:
 				dataset[file] = tt.from_csv_or_fits(file, ftype=val.get('ftype', None),
-										hdu=val.get('hdu', 1), nopandas=nopandas)
+										hdu=val.get('hdu', 1), nopandas=nopandas, comment=comment)
 			ans[key] = dataset[file][val['column']]
 	return ans
 
 def read(infile, x="", y="", hdu=1, data=None,
 		xlabel=None, ylabel=None,
-		ftype=None, nopandas=True, attr='', columns=None):
+		ftype=None, nopandas=True, attr='', columns=None, comment=None):
 	if data is None:
 		if infile is None:
 			print(cc.err + "input data or file is required.", cc.reset)
 			return None, None, None, None, None
 
 		if not path.isfile(infile):
 			print(cc.err + "cannot read the file:", infile, cc.reset)
 			return None, None, None, None, None
 
-		data = tt.from_csv_or_fits(infile, ftype=ftype, hdu=hdu, nopandas=nopandas, columns=columns)
+		data = tt.from_csv_or_fits(infile, ftype=ftype, hdu=hdu, nopandas=nopandas, columns=columns, comment=comment)
 
 	if x == "" or y == "":
 		if   type(data) is pandas.core.frame.DataFrame: colnames = data.columns.values.tolist()
 		elif type(data) is   astropy.table.table.Table: colnames = data.colnames
 		else: print('need to know column names or provide -x and -y')
 
 		if x == "":
@@ -288,14 +299,30 @@
 					yunit = data[y].info.unit
 					if yunit is not None: ylabel = ylabel + ' (' + str(yunit) + ')'
 		else:
 			ylabel = 'counts'
 
 	return data, x, y, xlabel, ylabel
 
+def read_img(filename, hdu=None):
+	filename = str(Path(filename).expanduser())
+	basename = path.basename(filename)
+
+	# regular image
+	if bool(re.search(r'\.tif(|f)$', basename)):
+		from PIL import Image
+		return np.array(Image.open(filename))
+	else:
+		# otherwise assume it's a fits file
+		# too presumptuous, but ...
+		hdul = fits.open(filename)
+		if hdu is None: hdu = 0
+		# image=np.transpose(hdul[hdu].data)
+		return hdul[hdu].data
+
 def set_range(data, margin=None,
 			dr=None,  # data range
 			dmin=None, dmax=None,
 			scale='linear', drawdown=None):
 
 	if type(dr) is list:
 		if dr[0] is None: dr = None
@@ -473,14 +500,15 @@
 	for key, val in rcParams.items():
 		if verbose >= 2: print(key, val)
 		plt.rcParams[key] = val
 
 	for key in defaults.keys() - rcParams.keys():
 		if verbose >= 2: print(key, defaults[key])
 		plt.rcParams[key] = defaults[key]
+	# embed()
 
 # ----------------------------------------------------------------------------------------
 def wrap(plt, xr=None, yr=None, xlabel=None, ylabel=None, fig=None,
 		title="", xscale='linear', yscale='linear', outfile=None,
 		y_title=1.0, rect=[0, 0, 1, 1],
 		ax2=None, ay2=None, ax=None,
 		xlabel2=None, ylabel2=None,
@@ -489,14 +517,15 @@
 		xtickv=None, ytickv=None, grid=None,
 		text=None, text_kw=None,
 		polygon=None, polygon_kw={},
 		ellipse=None, ellipse_kw={},
 		line=None, line_kw={},
 		loc_ylabel='center',  # rcParams=None,
 		xscale2=None, yscale2=None, gwhich='major',
+		xtformat=None, ytformat=None,
 		label=True, display=True, ion=False):
 
 	# if rcParams is not None:
 	# 	set_rcParams(rcParams, force=True, name=None)
 
 	if label:
 		if xlabel is not None: ax.set_xlabel(xlabel)
@@ -554,14 +583,23 @@
 		if xtickv is None: xtickv = [float(v) for v in xticks]
 		ax.set_xticks(xtickv, xticks)
 		# ax.set_xticks(xtickv)
 	if yticks is not None and ax is not None:
 		if ytickv is None: ytickv = [float(v) for v in yticks]
 		ax.set_yticks(ytickv, yticks)
 
+	if xtformat is not None:
+		if xtformat != '':
+			date_form = DateFormatter(xtformat)
+			ax.xaxis.set_major_formatter(date_form)
+	if ytformat is not None:
+		if ytformat != '':
+			date_form = DateFormatter(ytformat)
+			ax.yaxis.set_major_formatter(date_form)
+
 	if tight:
 		plt.tight_layout(rect=rect)
 
 	if grid is not None:
 		if type(grid) is bool:
 			if grid is True:
 				ax.grid(True, which=gwhich)
@@ -842,14 +880,29 @@
 				ax2.tick_params(axis='x', colors=color)
 				ax2.tick_params(axis='x', colors=color, which='minor')
 				ax2.spines['top'].set_color(color)
 				at = ax2
 
 	# if len(x) == len(y) +1:
 	attrs = attr.split(',')
+
+	# check if the data is time
+	# xtmat = [s for s in attrs if "xtime" in s]
+	# ytmat = [s for s in attrs if "ytime" in s]
+	# if len(xtmat) >0:
+	# 	if ':' in xtmat[0]: _, tformat = xtmat[0].split(':')
+	# 	else:	tformat="%y/%m/%d"
+	# 	x = [datetime.strptime(v,tformat) for v in x]
+	# 	x = np.array(x)
+	# if len(ytmat) >0:
+	# 	if ':' in ytmat[0]: _, tformat = ytmat[0].split(':')
+	# 	else:	tformat="%y/%m/%d"
+	# 	y = [datetime.strptime(v,tformat) for v in y]
+	# 	y = np.array(y)
+	#
 	if 'hist' in attrs:
 		# we assume this is for histogram
 		if type(x).__name__ != 'ndarray': x = np.array(x)
 		if type(y).__name__ != 'ndarray': y = np.array(y)
 		if len(x) == len(y) + 1:
 			xh, yh, xc = hist2line(x, y)
 			x = xc
@@ -921,19 +974,20 @@
 					colorbar_multivertical(im, at, plt, label,
 						rect=[1.01, 0.0, 0.03, 1], gap=0.03, ticklocation='right')
 					# plt.colorbar(im, pad=0.01)
 
 			# x, y, [xerr, yerr]
 
 		else:
-			if savgol is None: savgol = [11, 2]
 			if type(y) is list: y = np.array(y)
 			if type(y) is pandas.core.series.Series: y_sm = y.copy()
 			else: y_sm = np.array([v for v in y])
 			finite = np.isfinite(y)
+
+			if savgol is None: savgol = [11, 2]
 			y_sm[finite] = savgol_filter(y[finite], savgol[0], savgol[1])
 
 			if smzorder is None: smzorder = zorder + 1
 
 			if smooth == 'replace':
 				pid, = at.plot(x, y_sm,
 					color=color, label=label, alpha=alpha,
@@ -1298,14 +1352,42 @@
 		plt.setp(mhax.get_yticklabels(), visible=False)
 		plt.setp(mhax.get_ylabel(),      visible=False)
 		mhax.set_xscale(hscale)
 
 	despine_axes(mhax, despine)
 
 # ----------------------------------------------------------------------------------------
+def set_header_for_wcs(header, x='X', y='Y'):
+	done = 0
+	for key in header:
+		if header[key] == x:
+			mat = re.search("TTYPE([0-9]+)", key)
+			if bool(mat):
+				header['CTYPE1'] = header['TCTYP' + mat[1]]
+				header['CRPIX1'] = header['TCRPX' + mat[1]]
+				header['CRVAL1'] = header['TCRVL' + mat[1]]
+				header['CDELT1'] = header['TCDLT' + mat[1]]
+				done = done + 1
+				continue
+
+		if header[key] == y:
+			mat = re.search("TTYPE([0-9]+)", key)
+			if bool(mat):
+				header['CTYPE2'] = header['TCTYP' + mat[1]]
+				header['CRPIX2'] = header['TCRPX' + mat[1]]
+				header['CRVAL2'] = header['TCRVL' + mat[1]]
+				header['CDELT2'] = header['TCDLT' + mat[1]]
+				done = done + 10
+				continue
+
+		if done == 11: break
+
+	return header
+
+# ----------------------------------------------------------------------------------------
 def prep_data_deco(func):
 	"""
 	decorator for data loader. Used for 1-d and 2-d data as well as 2-d images
 	Some nontrivial parameters:
 		attr:
 				makehist: to make a histogram on the fly
 				hist: data is a histogram
@@ -1357,77 +1439,86 @@
 				xerr=None, yerr=None, xerrexpr=None, yerrexpr=None,
 				xlerr=None, ylerr=None, xlerrexpr=None, ylerrexpr=None,
 				xerrdata=None, yerrdata=None, xlerrdata=None, ylerrdata=None,
 				xhighdata=None, xlowdata=None, xhigh=None, xlow=None,
 				xlowexpr=None, xhighexpr=None,
 				yhighdata=None, ylowdata=None, yhigh=None, ylow=None,
 				ylowexpr=None, yhighexpr=None,
-				data=None, image=None, infile=None, x="", y="", z="",
+				data=None, image=None, flip=None,
+				infile=None, x="", y="", z="",
 				xlabel=None, ylabel=None, xr=None, yr=None,
 				infile2=None, attr='', pars=None, nbin=100, binsize=None,
 				xmin=None, xmax=None, ymin=None, ymax=None,
 				margin=0.0, drawdown=None, filter=False,
 				xscale=None, yscale=None, xlog=False, ylog=False,
 				rcParams=None, clip=None,  # pixel coordinates
+				comment=None,
 				verbose=0, ftype=None, hdu=None, columns=None, help=None, **kwargs):
 
 		help_text(help)
 
 		loaded = None
 
 		if infile is not None:
 			infile = str(path.expanduser(infile))
 
 		# try loading an image
 		if type(image) is bool:
 			if image:
-				# read image
-				# assume fits image for now
-				hdul = fits.open(infile)
-				if hdu is None: hdu = 0
-				# image=np.transpose(hdul[hdu].data)
-				image = hdul[hdu].data
+				image = read_img(infile, hdu=hdu)
+
+				# # read image
+				# # assume fits image for now
+				# hdul = fits.open(infile)
+				# if hdu is None: hdu = 0
+				# image = hdul[hdu].data
+
 				loaded = 'image'
 		elif image is not None: loaded = 'image'
 
 		# make sure 2-d image and clip if requested
 		if loaded == "image":
+			# embed()
 			ndim = image.ndim
 			if ndim == 3:
 				image = image.sum(axis=0)
 			image = np.transpose(image)
+			if flip is not None:
+				image = np.flip(image, axis=flip)
 
 			if type(clip) is list:
 				# x and y seem to be swapped
 				# image=image[clip[2]:clip[3],clip[0]:clip[1]]
 				image = image[clip[0]:clip[1], clip[2]:clip[3]]
 
 			nbinx, nbiny = image.shape
 			if type(clip) is not list:
 				if xr is None: xr = [0, nbinx]
 				if yr is None: yr = [0, nbiny]
 			else:
 				if xr is None: xr = [clip[0], clip[1]]
 				if yr is None: yr = [clip[2], clip[3]]
 
+		xtformat = None
+		ytformat = None
 		# if there is no image then try loading a table
 		if xdata is None and loaded is None:
 			if hdu is None: hdu = 1
 			if infile2 is None:
 				data, x, y, xlabel, ylabel = read(infile, x=x, y=y, data=data,
-							xlabel=xlabel, ylabel=ylabel, ftype=ftype, hdu=hdu, attr=attr, columns=columns)
+							xlabel=xlabel, ylabel=ylabel, ftype=ftype, hdu=hdu, attr=attr, columns=columns, comment=comment)
 				if data is None:
 					print('No data is read. Perhaps set ftype?')
 					return False
 				data2 = data
 			else:
 				data, x, y_, xlabel, ylabel_ = read(infile, x=x, y=None, data=data,
-							xlabel=xlabel, ylabel=None, ftype=ftype, hdu=hdu, attr=attr, columns=columns)
+							xlabel=xlabel, ylabel=None, ftype=ftype, hdu=hdu, attr=attr, columns=columns, comment=comment)
 				data2, x_, y, xlabel_, ylabel = read(infile2, x=None, y=y,
-					xlabel=None, ylabel=ylabel, ftype=ftype, hdu=hdu, attr=attr, columns=columns)
+					xlabel=None, ylabel=ylabel, ftype=ftype, hdu=hdu, attr=attr, columns=columns, comment=comment)
 			ydata = data2[y]
 
 			if xerr  is not None: xerrdata  = data [xerr ]
 			if yerr  is not None: yerrdata  = data2[yerr ]
 			if xlow  is not None: xlowdata  = data [xlow ]
 			if xhigh is not None: xhighdata = data [xhigh]
 			if ylow  is not None: ylowdata  = data2[ylow ]
@@ -1436,24 +1527,38 @@
 			if ylerr is not None: ylerrdata = data2[ylerr]
 
 			if   x == '_auto_'     : xdata = np.arange(0, len(ydata))
 			elif x == '_range_'    : xdata = (xlowdata + xhighdata) * 0.5
 			elif x == '_range_log_': xdata = np.exp((np.log(xlowdata) + np.log(xhighdata)) * 0.5)
 			else: xdata = data[x]
 
-			if type(xdata[0]) is str: xdata = get_number(xdata)
-			if type(ydata[0]) is str: ydata = get_number(ydata)
+			attrs = attr.split(',')
+			xtmat = [s for s in attrs if "xtime" in s]
+			ytmat = [s for s in attrs if "ytime" in s]
+			xtmat = '' if xtmat == [] else xtmat[0]
+			ytmat = '' if ytmat == [] else ytmat[0]
+			if type(xdata[0]) is str: xdata, xtformat = get_number(xdata, istime=xtmat)
+			if type(ydata[0]) is str: ydata, ytformat = get_number(ydata, istime=ytmat)
 
 			loaded = 'table'
 
 		if xscale is None: xscale = 'log' if xlog else 'linear'
 		if yscale is None: yscale = 'log' if ylog else 'linear'
 
+		attrs = attr.split(',')
+		if 'wcs' in attr:
+			# try to grab wcs information from header, assume fits file
+			from astropy.wcs import WCS
+			header = tt.from_csv_or_fits(infile, ftype='fitshdr')
+			header = set_header_for_wcs(header, x=x, y=y)
+			wcs = WCS(header)
+			kwargs['wcs'] = wcs
+
 		# change xdata and ydata by expr
-		if pars is not None: vars = read_pars(pars, data=data, infile=infile)
+		if pars is not None: vars = read_pars(pars, data=data, infile=infile, comment=comment)
 		else:                vars = None
 
 		xdata_     = xdexpr (xexpr    ,            xdata, ydata, vars=vars)
 		ydata_     = ydexpr (yexpr    ,            xdata, ydata, vars=vars)
 		xerrdata_  = errexpr(xerrexpr , xerrdata,  xdata, ydata, vars=vars)
 		yerrdata_  = errexpr(yerrexpr , yerrdata,  xdata, ydata, vars=vars)
 		xlerrdata_ = errexpr(xlerrexpr, xlerrdata, xdata, ydata, vars=vars)
@@ -1500,14 +1605,16 @@
 		if xlowdata  is not None: kwargs['xlowdata'   ] = xlowdata
 		if ylowdata  is not None: kwargs['ylowdata'   ] = ylowdata
 		if xhighdata is not None: kwargs['xhighdata'  ] = xhighdata
 		if yhighdata is not None: kwargs['yhighdata'  ] = yhighdata
 
 		if weights   is not None: kwargs['weights'    ] = weights
 		# if data      is not None: kwargs['data'       ] = data
+		if xtformat  is not None: kwargs['xtformat'    ] = xtformat
+		if ytformat  is not None: kwargs['ytformat'    ] = ytformat
 
 		# this is for the modeling but plotting's collect data will complain?
 		# technically this shouldn't be here. 2 decorators are cross-talking...
 		if 'm' in kwargs:
 			if infile    is not None: kwargs['infile'     ] = infile
 			if hdu       is not None: kwargs['hdu'        ] = hdu
 
@@ -1552,27 +1659,28 @@
 				xscale=None, yscale=None,
 				margin=None, drawdown=None,
 				rmin=None, rmax=None,
 				rmargin=0.0, data=None,
 				xerrdata=None, yerrdata=None,
 				xlowdata=None, xhighdata=None,
 				ylowdata=None, yhighdata=None,
+				comment=None,
 				verbose=0, attr='',
 				mhdu=None, phdu=None,
 				help=None, **kwargs):
 
 		help_text(help)
 
 		loaded = None
 
 		# if there is no image then try loading a table
 		if mdata is None and loaded is None:
 			if hdu is None: hdu = 1
 			data_, m_, r_, mlabel, rlabel = read(infile, x=m, y=r, data=data,
-						xlabel=None, ylabel=rlabel, ftype=ftype, hdu=hdu, attr=attr)
+						xlabel=None, ylabel=rlabel, ftype=ftype, hdu=hdu, attr=attr, comment=comment)
 			if data_ is None: return False
 
 			if m is not None: mdata = data_[m]
 			else:             mdata = None
 			if r is not None: rdata = data_[r]
 			else:             rdata = None
 
@@ -1630,21 +1738,26 @@
 		ellipse=None, ellipse_kw={},
 		line=None, line_kw={}, gwhich='major',
 		help=None, display=True, ion=False, hold=False, verbose=0, **kwargs):
 	"""Plot 1-D from input table
 	"""
 	if 'zdata' in kwargs: zdata = kwargs['zdata']
 	else:                 zdata = None
+	if 'xtformat' in kwargs: xtformat = kwargs['xtformat']
+	else:                    xtformat = None
+	if 'ytformat' in kwargs: ytformat = kwargs['ytformat']
+	else:                    ytformat = None
 
 	def show(ion=True):
 		check_ion(ion)
 
 		nonlocal xdata, ydata, marker
 		nonlocal binsize, nbin, edges, weights, yr, margin
 		nonlocal zdata, cmap
+		nonlocal xtformat, ytformat
 
 		fig, ax = plt.subplots()
 
 		pid, ax2, ay2 = plot1d_core(xdata, ydata, z=zdata, attr=attr, xscale=xscale, yscale=yscale,
 			xlow=xlowdata, xhigh=xhighdata, ylow=ylowdata, yhigh=yhighdata, xerr=xerrdata, yerr=yerrdata,
 			color=color, label=None, alpha=alpha, errcolor=errcolor,
 			marker=marker, markersize=markersize, linestyle=linestyle, linewidth=linewidth,
@@ -1659,14 +1772,15 @@
 		wrap(plt, xr=xr, yr=yr, xlabel=xlabel, ylabel=ylabel, fig=fig,
 			xscale=xscale, yscale=yscale, outfile=outfile,
 			ax=ax, grid=grid, title=title,
 			text=text, text_kw=text_kw,
 			polygon=polygon, polygon_kw=polygon_kw,
 			ellipse=ellipse, ellipse_kw=ellipse_kw,
 			line=line, line_kw=line_kw, gwhich=gwhich,
+			xtformat=xtformat, ytformat=ytformat,
 			display=display, ion=ion)
 
 	show(ion=ion)
 	if hold: embed()
 
 	return plt
 
@@ -1692,14 +1806,15 @@
 		xslice=None, yslice=None,  # data coordinateslike xr or yr (not necessarily pixels)
 		halpha=0.3, hcolor="darkblue", hgap=0.04, hheight=0.15,
 		despine=None, margin=0.0, drawdown=None,
 		noplot=False, grid=None,
 		text=None, text_kw=None,
 		polygon=None, polygon_kw=None,
 		ellipse=None, ellipse_kw=None,
+		wcs=None,
 		help=None, display=True, ion=False, hold=False, verbose=0, **kwargs):
 	""" 2-d density plot
 	"""
 
 	if image is None:
 		# data points
 		binx, nbinx = get_bin(binsize, nbin, binx, nbinx, xr)
@@ -1762,16 +1877,23 @@
 
 		nonlocal zmin, zmax, zoff
 		nonlocal zmid
 		nonlocal zlthresh, zlscale
 		nonlocal zclip
 		nonlocal xr, yr
 		nonlocal loc_ylabel, y_title
+		nonlocal wcs
 
-		fig, ax = plt.subplots()
+		# attrs = attr.split(',')
+		# if 'wcs' in attrs:
+		if wcs is not None:
+			fig = plt.figure()
+			ax = fig.add_subplot(111, projection=wcs)
+		else:
+			fig, ax = plt.subplots()
 
 		if ion: plt.ion()
 		norm, zmin, zmax = get_norm(zlog=zlog, zmid=zmid, zmin=zmin, zmax=zmax,
 						zr=zr, zlthresh=zlthresh, zlscale=zlscale)
 
 		image, xedges, yedges, im = ax.hist2d(xdata, ydata, weights=weights,
 											norm=norm, bins=bins,  cmap=cmap)
@@ -2694,14 +2816,17 @@
 	binsize = None
 	nbin    = 100
 	edges   = None
 
 	rcParams = None
 	gwhich = 'major'
 
+	xtformat = None
+	ytformat = None
+
 	def __init__(self, **kwpars):
 		self.data = OrderedDict()
 		self.set_kwpars(kwpars)
 
 	def set_kwpars(self, kwargs):
 
 		ignored = []
@@ -2729,15 +2854,17 @@
 			ax=ax, grid=self.grid,
 			xlabel2=self.xlabel2, ylabel2=self.ylabel2, xr2=self.xr2, yr2=self.yr2,
 			loc_ylabel=self.loc_ylabel, y_title=self.y_title,
 			text=self.text, text_kw=self.text_kw,
 			polygon=self.polygon, polygon_kw=self.polygon_kw,
 			ellipse=self.ellipse, ellipse_kw=self.ellipse_kw,
 			ion=self.ion, display=self.display,
-			gwhich=self.gwhich, **kwpars)
+			gwhich=self.gwhich, 
+			xtformat=self.xtformat, ytformat=self.ytformat, 
+			**kwpars)
 
 	def set_default_range(self):
 
 		for key, data in self.data.items():
 
 			if 'xrf' not in locals(): xrf = data.xr
 			if 'yrf' not in locals(): yrf = data.yr
@@ -2767,15 +2894,15 @@
 		self.key = self.key + 1
 
 		return 1
 
 	def composite_data(self, key=None, inkeys=None,
 					xexpr=None, yexpr=None,
 					varx=None, vary=None, defkey=None, **kwpars):
-		if type(inkeys).__name__ is None: return
+		if inkeys is None: return
 		if key is None:
 			self.key = self.key + 1
 			key = self.key
 
 		nkeys_ = len(inkeys)
 
 		if varx is None:
@@ -2798,14 +2925,24 @@
 
 		xdata = eval(xexpr)
 		ydata = eval(yexpr)
 
 		self.collect_data(key=key, xdata=xdata, ydata=ydata)
 		self.set_prop(key, **kwpars)
 
+	def rebin_data(self, keys=None, inkeys=None,
+			method='fixed', bin=2):
+		if inkeys is None: return
+		if keys is None: keys=inkeys # replace
+
+		import rebin
+		for key, inkey in zip(keys, inkeys):
+			self.data[key].xdata = rebin.one(np.array(self.data[inkey].xdata), bin=bin, mean=True)
+			self.data[key].ydata = rebin.one(np.array(self.data[inkey].ydata), bin=bin)
+
 class scatter(base):
 
 	# 1-dplot with reference data set
 	refkey      = None  # for reference data
 	refer       = False
 	refset      = False
```

### Comparing `clise-0.1.5/clise/rabbit.py` & `clise-0.1.6/clise/rabbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,21 +690,21 @@
 			for tkey, value in zip(tkeys, values): task[tkey]=value
 
 		if appkeys is not None:
 			for each in appkeys: task[each] = apply_tag(task[each], tag)
 
 		if outkey in seed:
 			outfile = seed.get(outkey, None)
-			print('====', outdir, outfile)
-			outfile, outdir = get_outfile(outfile, name,
+			# print('====', outdir, outfile)
+			outfile, outdir_ = get_outfile(outfile, name,
 						outdir=outdir, outsubdir=outsubdir,
 						mirror_indir=mirror_indir, switch_subdir=switch_subdir,
 						tags=tag, cfg=seed, verbose=verbose)
 			task[outkey] = Path(outfile).expanduser()
-			print('====', outdir, outfile)
+			# print('====', outdir, outfile)
 
 		# expand ~***
 		if indir is not None: task[inkey] = (Path(indir) / Path(name)).expanduser()
 		else:                 task[inkey] = Path(name).expanduser()
 
 		# update files in a directory relative to input dir
 		if rel2indir is not None:
@@ -759,14 +759,16 @@
 		if '-checkout' not in task: task['-checkout'] = []
 
 		task['-checkin'] = task['-checkin'] + checkin
 		if checkout is not None:
 			task['-checkout'] = task['-checkout'] + checkout
 
 		tasks.append(task)
+		# from IPython	import embed
+		# embed()
 
 	# here we have to sort when we have both infile and outfile
 	if before is not None:
 		if sortby  == "":   sortby  = inkey + ":mtime"
 		if reverse is None: reverse = True
 	if after is not None:
 		if sortby  == "":   sortby  = inkey + ":mtime"
@@ -879,15 +881,15 @@
 
 			if appkeys is not None:
 				for each in appkeys:
 					if each in task: task[each] = apply_tag(task[each], tag)
 
 			if outkey in eseed:
 				outfile = eseed[outkey]
-				outfile, outdir = get_outfile(outfile, name,
+				outfile, outdir_ = get_outfile(outfile, name,
 							outdir=outdir, outsubdir=outsubdir,
 							mirror_indir=mirror_indir, switch_subdir=switch_subdir,
 							tags=tag, cfg=eseed, verbose=verbose)
 				task[outkey] = Path(outfile).expanduser()
 
 			# expand ~***
 			if inkey in task:
```

### Comparing `clise-0.1.5/clise/startup/scan_hdus_plot1d_rabbit.json5` & `clise-0.1.6/clise/startup/scan_hdus_plot1d_rabbit.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/startup/scan_hdus_plot1d_rabbit_noswap.json5` & `clise-0.1.6/clise/startup/scan_hdus_plot1d_rabbit_noswap.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/startup/startup.json5` & `clise-0.1.6/clise/startup/startup.json5`

 * *Files identical despite different names*

### Comparing `clise-0.1.5/clise/tabletool.py` & `clise-0.1.6/clise/tabletool.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,32 +166,34 @@
 		if start:
 			data.append(int(line))
 		if bool(re.search(r'<<DATA>>', line)): start = True
 
 	return pd.DataFrame(data, columns=columns)
 
 # read the table from a csv or fits file or a few other formats
-def from_csv_or_fits(filename, index=False, ftype=None, hdu=1, nopandas=False, fill=-1, columns=None):
+def from_csv_or_fits(filename, index=False, ftype=None, hdu=1, nopandas=False, fill=-1, columns=None, comment=None):
 	filename = str(Path(filename).expanduser())
 	basename = path.basename(filename)
 
 	if ftype is not None:
 		if   ftype == "json": return pd.read_json(filename)
-		elif ftype == "csv" : return pd.read_csv (filename, index_col=index)
+		elif ftype == "csv" : return pd.read_csv (filename, index_col=index, comment=None)
 		elif ftype == "mca" : return read_mca (filename, columns=columns)
+		# elif ftype == "tiff": return read_img (filename)
 		elif ftype == "fits": return ast_to_pd(Table.read(filename, format='fits', hdu=hdu), nopandas)
 		elif ftype == "fitshdr": return fits.open(filename)[hdu].header
 		else:
 			try:    return ast_to_pd(Table.read(filename, format=ftype), nopandas)
 			except Exception: pass
 
 	if   bool(re.search(r'\.fits(|\.gz)$', basename)): return ast_to_pd(Table.read(filename, format='fits', hdu=hdu), nopandas)
 	elif bool(re.search( r'\.mrt(|\.gz)$', basename)): return ast_to_pd(Table.read(filename, format='ascii.mrt'),     nopandas)
-	elif bool(re.search( r'\.csv(|\.gz)$', basename)): return pd.read_csv (filename, index_col=index)
+	elif bool(re.search( r'\.csv(|\.gz)$', basename)): return pd.read_csv (filename, index_col=index, comment=comment)
 	elif bool(re.search( r'\.mca(|\.gz)$', basename)): return read_mca    (filename, columns=columns)
+	# elif bool(re.search(r'\.tiff(|\.gz)$', basename)): return read_img    (filename)
 	elif bool(re.search( r'\.xml(|\.gz)$', basename)): return pd.read_xml (filename)
 	elif bool(re.search(r'\.json(|\.gz)$', basename)): return pd.read_json(filename)
 
 # read fits as astropy
 def readfits(infile, hdu=1, hold=True):
 	infile = str(Path(infile).expanduser())
 	data = Table.read(infile, format='fits', hdu=hdu)
```

### Comparing `clise-0.1.5/clise/xray_mirror.py` & `clise-0.1.6/clise/xray_mirror.py`

 * *Files 5% similar despite different names*

```diff
@@ -882,27 +882,61 @@
 		psf  = self.calc_HPD_FWHM(radial, image)
 		self.annotate_psf(plt, self.center, xr, yr, psf=psf)
 
 		plt.savefig(outfile)
 		plt.clf()
 		plt.close("all")
 
-	# this is getting too many input parameters....
-	def get_EA_from_SDD(infile, bkgfile, mdlfile=None, winfile=None,
-				ctsplot=None, EAplot=None, EAdata=None,
-				xr_cts=None, yr_cts=None, xlog_cts=None, ylog_cts=None,
-				xr_EA=None, yr_EA=None, xlog_EA=None, ylog_EA=None,
-				srccolorfull="red",   srclabelfull="Source",
-				srccoloraper="organge", srclabelaper="Source 1am", aperexpr=None,
-				bkgcolor="black", bkglabel="Beam"):
-
-		ea = pt.plottool()
-		ea.collect_data(infile=bkgfile, key="beam",     label=bkglabel,     color=bkgcolor)
-		ea.collect_data(infile=infile,  key="src full", label=srclabelfull, color=srccolorfull)
-		ea.collect_data(infile=infile,  key="src aper", label=srclabelaper, color=srccoloraper, yexpr=aperexpr)
+# this is getting too many input parameters....
+def get_EA_from_line(srcfile, bkgfile,
+	out='csv',
+	xr=None,
+	ch2e=None,  # channel to energy conversion
+	c4ea=1.0,   # conversion to effective area
+	id="", idhdr='id',
+	verbose=0, hold=False):
+
+	src = tt.from_csv_or_fits(srcfile)
+	bkg = tt.from_csv_or_fits(bkgfile)
+
+	if xr is None: xr = [0, len(src) - 1]
+	if ch2e is not None:
+		xr[0] = round(xr[0] / ch2e)
+		xr[1] = round(xr[1] / ch2e)
+
+	srctot = float(np.sum(src[xr[0]:xr[1]]))
+	bkgtot = float(np.sum(bkg[xr[0]:xr[1]]))
+
+	err_srctot = np.sqrt(srctot)
+	err_bkgtot = np.sqrt(bkgtot)
+
+	EA = float(srctot / bkgtot * c4ea)
+	err_EA = EA * np.sqrt((err_srctot / srctot)**2 + (err_bkgtot / bkgtot)**2)
+
+	if out == 'csv':
+		if verbose > 0:
+			for each in ['EA', 'err_EA', 'src', 'bkg', 'ch2e', 'c4ea', 'xlow', 'xhigh']:
+				print(each, end=',')
+			print(idhdr)
+		for each in [EA, err_EA, srctot, bkgtot, ch2e, c4ea, xr[0], xr[1]]:
+			print(each, end=',')
+		print(id)
+	else:
+		if verbose > 1:
+			print('channel->energy:', ch2e, 'conversion 4 EA:', c4ea)
+			print('xr:', xr)
+			print('src:', srctot, 'bkgtot:', bkgtot)
+		if verbose > 0:
+			print('srcfile:', srcfile)
+		print('id', id)
+		print('EA:', EA, '+/-', err_EA)
+
+	if hold: pt.embed()
+
+
 
 # ---------------------------------------------------------------------------
 # SAORT output summary
 # read *.dat
 # apply reflectivity correction if needed
 # generate plot and table fits
```

### Comparing `clise-0.1.5/clise.egg-info/PKG-INFO` & `clise-0.1.6/clise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: clise
-Version: 0.1.5
+Version: 0.1.6
 Summary: Command liner with JSON based input file
-Home-page: https://pypi.org/project/clise/0.1.5
+Home-page: https://pypi.org/project/clise/0.1.6
 Author: Jaesub Hong
 Author-email: jhong@cfa.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 License-File: AUTHORS
 
 ### CLISe: Command Line Input Setter
 
 Command liner for python routines using JSON based input parameter files. It
 dives into a module with CLI and execute a routine just as herons dive into
 water and catch fish. It also uses JSON text to create task lists to automatize
-multiple executions of the routine: ver 0.1.5 by Jaesub Hong
+multiple executions of the routine: ver 0.1.6 by Jaesub Hong
 (jhong@cfa.harvard.edu)
 
        Usage: clise JSON_input_file1 -options_for_file1 ... \
             [json_input_file2 -options_for_file2 ...] \
             [--with common_json_files -common_options ...] \
             [--WITH common_json_files -common_options ...]
```

### Comparing `clise-0.1.5/clise.egg-info/SOURCES.txt` & `clise-0.1.6/clise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 clise/__main__.py
 clise/cmdscript.py
 clise/demo.py
 clise/heron.py
 clise/jsontool.py
 clise/plottool.py
 clise/rabbit.py
+clise/rebin.py
 clise/tabletool.py
 clise/xray_mirror.py
 clise.egg-info/PKG-INFO
 clise.egg-info/SOURCES.txt
 clise.egg-info/dependency_links.txt
 clise.egg-info/entry_points.txt
 clise.egg-info/requires.txt
```

### Comparing `clise-0.1.5/setup.py` & `clise-0.1.6/setup.py`

 * *Files identical despite different names*

