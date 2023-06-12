# Comparing `tmp/energyplus_launch-3.7.0.tar.gz` & `tmp/energyplus_launch-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.7.0.tar", last modified: Tue Jun  6 15:02:26 2023, max compression
+gzip compressed data, was "energyplus_launch-3.7.1.tar", last modified: Mon Jun 12 21:52:03 2023, max compression
```

## Comparing `energyplus_launch-3.7.0.tar` & `energyplus_launch-3.7.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.888975 energyplus_launch-3.7.0/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-06 15:02:26.000000 energyplus_launch-3.7.0/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.888975 energyplus_launch-3.7.0/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     5319 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    74924 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/interface/widget_group_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-06 15:02:26.892974 energyplus_launch-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-06-06 15:02:19.000000 energyplus_launch-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5319 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78204 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/widget_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5376 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/setup.py
```

### Comparing `energyplus_launch-3.7.0/LICENSE` & `energyplus_launch-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/PKG-INFO` & `energyplus_launch-3.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.7.0
+Version: 3.7.1
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
-Description: # EP-Launch3
+Description: # EnergyPlus Launch
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
         
         Cross platform replacement for EP-Launch for EnergyPlus, written in Python using the `tkinter` graphics library.
         
         ## Documentation
```

### Comparing `energyplus_launch-3.7.0/README.md` & `energyplus_launch-3.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# EP-Launch3
+# EnergyPlus Launch
 
 [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
 
 Cross platform replacement for EP-Launch for EnergyPlus, written in Python using the `tkinter` graphics library.
 
 ## Documentation
```

### Comparing `energyplus_launch-3.7.0/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.7.1/energyplus_launch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.7.0
+Version: 3.7.1
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
-Description: # EP-Launch3
+Description: # EnergyPlus Launch
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
         
         Cross platform replacement for EP-Launch for EnergyPlus, written in Python using the `tkinter` graphics library.
         
         ## Documentation
```

### Comparing `energyplus_launch-3.7.0/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.7.1/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/__init__.py` & `energyplus_launch-3.7.1/eplaunch/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/config.py` & `energyplus_launch-3.7.1/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.7.1/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.7.1/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.7.1/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.7.1/eplaunch/interface/dialog_weather.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.7.1/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/frame_main.py` & `energyplus_launch-3.7.1/eplaunch/interface/frame_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,17 @@
 
         # potentially show a welcome screen if we are on a new version
         self._open_welcome()
 
         # bind key presses for the app
         self.bind('<Key>', self._handle_keyboard_press)
 
+        # and bind the focus event for the app
+        self.bind("<FocusIn>", self._handle_focus_in)
+
     def _define_tk_variables(self):
         self._tk_var_workflow_context = StringVar(value='<context>')
         self._tk_var_workflow_instance = StringVar(value='<instance>')
         self._tk_var_output_suffix = StringVar(value='<output')
         self._tk_var_output_1 = StringVar(value='--')
         self._tk_var_output_2 = StringVar(value='--')
         self._tk_var_output_3 = StringVar(value='--')
@@ -184,14 +187,15 @@
 
     def _build_top_menu(self):
         menubar = Menu(self)
 
         menu_file = Menu(menubar, tearoff=False)
         menu_file.add_command(label="Run Current Workflow on Selection", command=self._run_workflow_on_selection)
         menu_file.add_command(label="Run Current Workflow on Current Group", command=self._run_workflow_on_group)
+        menu_file.add_separator()
         menu_file.add_command(label="Quit", command=self._window_close)
         menubar.add_cascade(label="File", menu=menu_file)
 
         menu_nav = Menu(menubar, tearoff=False)
         self.menu_nav_recent = Menu(menu_nav, tearoff=False)
         menu_nav.add_cascade(label="Recent", menu=self.menu_nav_recent)
         menu_nav.add_command(label="Navigate to previous folder", command=self._navigate_to_previous_folder)
@@ -201,26 +205,28 @@
         menu_nav.add_command(label="Add Current Folder to Favorites", command=self._add_folder_to_favorites)
         menu_nav.add_command(label="Remove Current Folder from Favorites", command=self._remove_folder_from_favorites)
         menu_nav.add_separator()
         menu_nav.add_command(label="View Keyboard Shortcuts", command=self._open_shortcuts_dialog)
         menubar.add_cascade(label="Navigation", menu=menu_nav)
 
         menu_group = Menu(menubar, tearoff=False)
-        menu_group.add_command(label="Clear Current Group", command=self._clear_group)
-        menu_group.add_command(label="Load new Group file...", command=self._load_new_group_file)
-        menu_group.add_command(label="Save Current Group to file...", command=self._save_group_file)
         menu_group.add_command(
             label="Add selected files to current group", command=self._add_current_files_to_group
         )
+        menu_group.add_command(label="Clear Current Group", command=self._clear_group)
+        menu_group.add_separator()
         menu_group.add_command(
             label="Set weather for current group", command=self._set_weather_for_current_group
         )
         menu_group.add_command(
             label="Cycle through current group entries", command=self._cycle_through_group
         )
+        menu_group.add_separator()
+        menu_group.add_command(label="Save Current Group to file...", command=self._save_group_file)
+        menu_group.add_command(label="Load File to Current Group...", command=self._load_new_group_file)
         menubar.add_cascade(label="Group", menu=menu_group)
 
         menu_settings = Menu(menubar, tearoff=False)
         menu_settings.add_command(label="Workflow Directories", command=self._open_workflow_dir_dialog)
         self._tk_var_keep_dialogs_open = BooleanVar(value=True)
         menu_settings.add_checkbutton(
             label="Keep Output Dialog Open", onvalue=True, offvalue=False, variable=self._tk_var_keep_dialogs_open
@@ -231,15 +237,15 @@
             self.conf.keep_dialog_open = self._tk_var_keep_dialogs_open.get()
 
         self._tk_var_keep_dialogs_open.trace('w', _update_keep_dialog_open)
         menu_settings.add_command(label="Viewers...", command=self._open_viewers_dialog)
         menubar.add_cascade(label="Settings", menu=menu_settings)
 
         menu_help = Menu(menubar, tearoff=False)
-        menu_help.add_command(label="EP-Launch Documentation", command=self._open_documentation)
+        menu_help.add_command(label="EnergyPlus-Launch Documentation", command=self._open_documentation)
         menu_help.add_command(label="About...", command=self._open_about)
         menubar.add_cascade(label="Help", menu=menu_help)
 
         self.config(menu=menubar)
 
     # noinspection SqlNoDataSourceInspection
     def _build_top_icon_bar(self, container: Frame):
@@ -282,32 +288,39 @@
                 lf, text="Select Weather File...", command=self._open_weather_dialog
             )
         self.button_weather_select.grid(row=1, column=0, columnspan=2, sticky=EW, **self.pad)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=2, sticky=NS, **self.pad)
 
-        lf = LabelFrame(container, text="Quicklinks")
+        lf = LabelFrame(container, text="Open Selected File(s) or Directory")
         if self.extended_utf8:
             self.button_open_in_text = Button(
                 lf, text=u"\U0001F5B9 Open File in Text Editor", command=self._open_text_editor, state=DISABLED
             )
         else:
             self.button_open_in_text = Button(
                 lf, text="Open File in Text Editor", command=self._open_text_editor, state=DISABLED
             )
-        self.button_open_in_text.grid(row=0, column=0, columnspan=3, sticky=EW, **self.pad)
+        self.button_open_in_text.grid(row=0, column=0, sticky=EW, **self.pad)
         if self.extended_utf8:
-            Button(
+            dir_button = Button(
                 lf, text=u"\U0001F5C0 Open Dir in File Browser", command=self._open_file_browser, state=NORMAL
-            ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+            )
         else:
-            Button(
+            dir_button = Button(
                 lf, text="Open Dir in File Browser", command=self._open_file_browser, state=NORMAL
-            ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+            )
+        dir_button.grid(row=1, column=0, sticky=EW, **self.pad)
+        idf_editor_icon_path = Path(__file__).resolve().parent / 'resources' / 'idf_editor_icon.png'
+        self.idf_editor_image = PhotoImage(file=str(idf_editor_icon_path))
+        self.button_idf_editor = Button(
+            lf, image=self.idf_editor_image, command=self._open_idf_editor, state=DISABLED
+        )
+        self.button_idf_editor.grid(row=0, rowspan=2, column=1, sticky=EW, **self.pad)
         lf.grid_rowconfigure(ALL, weight=1)
         lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=3, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Open Outputs")
         sub_frame = Frame(lf)
         self.button_open_output_1 = Button(
@@ -461,14 +474,28 @@
         elif event.keysym == 'g' and mod_control & event.state:
             self._run_workflow_on_group()
         elif event.keysym == 'm' and mod_control & event.state:
             self._cycle_through_group()
         elif event.keysym == 'z' and mod_control & event.state:
             self._navigate_to_previous_folder()
 
+    def _handle_focus_in(self, _event) -> None:
+        # This is firing twice, even on dummy hello world window examples.
+        # The event argument is supposed to have a .detail member which you
+        # can check to see if it equals NotifyAncestor and skip some callbacks.
+        # Unfortunately that is missing, so there's not much we can do.
+        # If we really needed to skip some, we could do a small timer that
+        # won't let two callbacks happen within 0.5s of each other or something.
+        # For now that's not necessary, but could be in the future.
+        # As of right now, the only reason we need this is to try to refresh
+        # the stale attribute, which should be accomplished with just the call here.
+        # It's possible we also need to check the _event.widget to make sure we are only
+        # calling this when the main window is focused.
+        self._update_file_list()
+
     @staticmethod
     def _list_keyboard_shortcuts() -> List[Tuple[str, str]]:
         # Mimic the keyboard shortcuts in the function above
         # It helps the dialog text look nice if you make sure the widths are uniform
         return [
             ("Control + F5", "Update File List"),
             ("Control + w ", "Open Weather Dialog"),
@@ -486,34 +513,39 @@
         self.conf.group_locations.clear()
         self._rebuild_group_menu()
 
     def _load_new_group_file(self):
         group_file_path = filedialog.askopenfilename(
             title="Load a new EPLaunch Group File",
             initialdir=self.conf.directory,
-            filetypes=(("EP-Launch Group Files", "*.epg3"),)
+            filetypes=(("EnergyPlus-Launch Group Files", "*.epg3"),)
         )
         if not group_file_path:
             return
         group_file_path_object = Path(group_file_path)
         entries = group_file_path_object.read_text().splitlines()
         self.conf.group_locations = []
         for e in sorted(entries):
             if e:
                 self.conf.group_locations.append(Path(e))
         self._rebuild_group_menu()
 
     def _save_group_file(self):
+        if len(self.conf.group_locations) == 0:
+            messagebox.showerror("File Selection Issue", "Group is currently empty, add files to group before saving!")
+            return
         group_file_path = filedialog.asksaveasfilename(
             title="Save EPLaunch Group File",
             initialdir=self.conf.directory,
-            filetypes=(("EP-Launch Group Files", "*.epg3"),)
+            filetypes=(("EnergyPlus-Launch Group Files", "*.epg3"),)
         )
         if not group_file_path:
             return
+        if not group_file_path.endswith('.epg3'):
+            group_file_path += '.epg3'
         group_file_path_object = Path(group_file_path)
         try:
             group_file_path_object.write_text('\n'.join([str(p) for p in self.conf.group_locations]))
         except Exception as e:  # could be permission or just about anything
             messagebox.showerror("Error", f"Could not save group file, error message:\n{str(e)}")
             return
 
@@ -793,14 +825,22 @@
         return False
 
     def _callback_file_selection_changed(self, selected_file_names: List[str]) -> None:
         """This gets called back by the file listing widget when a selection changes"""
         self.conf.file_selection = selected_file_names
         status = NORMAL if len(self.conf.file_selection) > 0 else DISABLED
         self.button_open_in_text['state'] = status
+        # disable the IDF editor button, then possibly enable it
+        self.button_idf_editor['state'] = DISABLED
+        if system() == 'Windows':
+            if self.workflow_manager.current_workflow:
+                if self.workflow_manager.current_workflow.is_energyplus:
+                    if len(self.conf.file_selection) > 0:
+                        self.button_idf_editor['state'] = NORMAL
+        # update output buttons too
         self._refresh_output_suffix_buttons_based_on_selection()
 
     # endregion
 
     # region weather operations
 
     def _set_weather_widget_state(self, weather_enabled) -> None:
@@ -1236,37 +1276,37 @@
             **viewer_dialog.extension_to_viewer, **self.conf.viewer_overrides
         }
 
     def _open_welcome(self):
         if self.conf.welcome_shown and VERSION == self.conf.latest_welcome_shown:
             return
         message = """
-EP-Launch has been around for many years as a part of the EnergyPlus distribution.
+EnergyPlus-Launch has been around for many years as a part of the EnergyPlus distribution.
 Starting with the 3.0 release, it has changed drastically, completely redesigned and rewritten.
 For full documentation or a quick start guide, click the "Open Docs" button below.
 This dialog will only be shown once, but documentation is available in the Help menu."""
         self.generic_dialogs.display_with_alt_button(
-            self, 'Welcome to EP-Launch ' + VERSION, message, 'Open Documentation', self._open_documentation
+            self, 'Welcome to EnergyPlus-Launch ' + VERSION, message, 'Open Documentation', self._open_documentation
         )
         self.conf.welcome_shown = True
         self.conf.latest_welcome_shown = VERSION
 
     def _open_shortcuts_dialog(self, *_) -> None:
         shortcuts = EPLaunchWindow._list_keyboard_shortcuts()
         text = '\n'.join([f"{r[0]}:\t{r[1]}" for r in shortcuts])
         self.generic_dialogs.display(self, "Available Keyboard Shortcuts", text)
 
     def _open_about(self) -> None:
         text = """
-EP-Launch
+EnergyPlus-Launch
 
-EP-Launch is a graphical workflow manager for EnergyPlus.
+EnergyPlus-Launch is a graphical workflow manager for EnergyPlus.
 Originally written in VB6 and released with essentially every version of EnergyPlus,
 it is now a cross platform Python tool.
-Users are encouraged to leverage EP-Launch and write their own workflow scripts
+Users are encouraged to leverage EnergyPlus-Launch and write their own workflow scripts
 to enable new capabilities.
 
 Version %s
 Copyright (c) 2023, Alliance for Sustainable Energy, LLC  and GARD Analytics, Inc
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
@@ -1292,15 +1332,15 @@
 INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
 NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
 EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         """ % VERSION
-        self.generic_dialogs.display(self, "About EP-Launch", text)
+        self.generic_dialogs.display(self, "About EnergyPlus-Launch", text)
 
     def _open_output_file_generic(self, suffix_to_open: str):
         if len(self.conf.file_selection) > 5:
             message = """More than 5 files were selected when choosing to open workflow outputs.
         This could generate many output windows and is usually not intentional.  Select up to 5 input files."""
             messagebox.showerror("File Selection Issue", message)
             return
@@ -1397,14 +1437,32 @@
                 potential_program = self._find_default_text_editor_on_windows()
                 if potential_program != '':
                     Popen([potential_program, full_path_str])
                     return
             # if neither of those work, just open with the default editor
             self._open_file_or_dir_with_default(full_path_str)
 
+    def _open_idf_editor(self) -> None:
+        # should only be able to get here if the current configuration/workflow/selection/platform allows it
+        workflow_context_dir = self.workflow_manager.current_workflow.workflow_directory
+        eplus_root_dir = workflow_context_dir.parent
+        idf_editor_dir = eplus_root_dir / 'PreProcess' / 'IDFEditor'
+        idf_editor_binary = idf_editor_dir / 'IDFEditor.exe'
+        if len(self.conf.file_selection) > 3:
+            messagebox.showerror("File Selection Issue", "Select up to 3 files to open with IDF Editor.")
+            return
+        any_skipped = False
+        for f in self.conf.file_selection:
+            if f.endswith('idf') or f.endswith('imf'):
+                Popen([idf_editor_binary, self.conf.directory / f])
+            else:
+                any_skipped = True
+        if any_skipped:
+            messagebox.showerror("File Type Issue", "At least one file was skipped because it was not an IDF/IMF")
+
     @staticmethod
     def _find_default_text_editor_on_windows() -> str:
         from winreg import OpenKey, QueryValueEx, HKEY_CLASSES_ROOT
         try:
             key = OpenKey(HKEY_CLASSES_ROOT, '.txt')
             default_value, _ = QueryValueEx(key, '')
             key.Close()
```

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.7.1/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.7.1/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/interface/widget_group_list.py` & `energyplus_launch-3.7.1/eplaunch/interface/widget_group_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/utilities/cache.py` & `energyplus_launch-3.7.1/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.7.1/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/utilities/version.py` & `energyplus_launch-3.7.1/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/base.py` & `energyplus_launch-3.7.1/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.7.1/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.7.1/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.7.1/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/manager.py` & `energyplus_launch-3.7.1/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/workflow.py` & `energyplus_launch-3.7.1/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.7.1/eplaunch/workflows/workflow_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 """
-This file is a standalone EP-Launch workflow tester.
+This file is a standalone EnergyPlus-Launch workflow tester.
 It is called using a single argument, the path to a workflow file
 """
 
 from inspect import isclass, getmembers
 from pathlib import Path
 from sys import argv, exit
 from importlib import util as import_util
```

### Comparing `energyplus_launch-3.7.0/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.7.1/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.0/setup.py` & `energyplus_launch-3.7.1/setup.py`

 * *Files identical despite different names*

