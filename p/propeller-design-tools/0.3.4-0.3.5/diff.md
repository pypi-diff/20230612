# Comparing `tmp/propeller_design_tools-0.3.4.tar.gz` & `tmp/propeller_design_tools-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propeller_design_tools-0.3.4.tar", last modified: Mon Jun 12 06:07:51 2023, max compression
+gzip compressed data, was "propeller_design_tools-0.3.5.tar", last modified: Mon Jun 12 06:22:38 2023, max compression
```

## Comparing `propeller_design_tools-0.3.4.tar` & `propeller_design_tools-0.3.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:07:51.619779 propeller_design_tools-0.3.4/
--rw-rw-rw-   0        0        0    35128 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     1378 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0       92 2023-06-12 06:07:51.619779 propeller_design_tools-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     9237 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 06:07:51.599783 propeller_design_tools-0.3.4/propdes/
--rw-rw-rw-   0        0        0      374 2023-06-12 05:36:14.000000 propeller_design_tools-0.3.4/propdes/__init__.py
--rw-rw-rw-   0        0        0    28174 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/airfoil.py
--rw-rw-rw-   0        0        0     4755 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.4/propdes/custom_opengl_classes.py
--rw-rw-rw-   0        0        0    17884 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/foil_ui_classes.py
--rw-rw-rw-   0        0        0    49090 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/funcs.py
--rw-rw-rw-   0        0        0    17339 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/helper_ui_classes.py
--rw-rw-rw-   0        0        0    15821 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      373 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/opt_ui_classes.py
--rw-rw-rw-   0        0        0    10726 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/optimizations.py
--rw-rw-rw-   0        0        0    15171 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36115 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/prop_creation_ui_classes.py
--rw-rw-rw-   0        0        0    52601 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/propeller.py
--rw-rw-rw-   0        0        0    17220 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/radialstation.py
--rw-rw-rw-   0        0        0     1624 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.4/propdes/science_spinbox_class.py
--rw-rw-rw-   0        0        0     3952 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/settings.py
--rw-rw-rw-   0        0        0     5590 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.4/propdes/user_interface.py
--rw-rw-rw-   0        0        0     2749 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.4/propdes/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:07:51.609883 propeller_design_tools-0.3.4/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0       92 2023-06-12 06:07:51.000000 propeller_design_tools-0.3.4/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-12 06:07:51.000000 propeller_design_tools-0.3.4/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:07:51.000000 propeller_design_tools-0.3.4/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 06:07:51.000000 propeller_design_tools-0.3.4/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 06:07:51.619779 propeller_design_tools-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      141 2023-06-12 05:45:42.000000 propeller_design_tools-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/
+-rw-rw-rw-   0        0        0    35128 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     1378 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0       92 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9237 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 06:22:38.390107 propeller_design_tools-0.3.5/propdes/
+-rw-rw-rw-   0        0        0      374 2023-06-12 05:36:14.000000 propeller_design_tools-0.3.5/propdes/__init__.py
+-rw-rw-rw-   0        0        0    28174 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/airfoil.py
+-rw-rw-rw-   0        0        0     4755 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.5/propdes/custom_opengl_classes.py
+-rw-rw-rw-   0        0        0    17884 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    49090 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/funcs.py
+-rw-rw-rw-   0        0        0    17339 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    15821 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      373 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    10726 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/optimizations.py
+-rw-rw-rw-   0        0        0    15171 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36115 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/prop_creation_ui_classes.py
+-rw-rw-rw-   0        0        0    52601 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/propeller.py
+-rw-rw-rw-   0        0        0    17220 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/radialstation.py
+-rw-rw-rw-   0        0        0     1624 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.5/propdes/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     3952 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/settings.py
+-rw-rw-rw-   0        0        0     5590 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/user_interface.py
+-rw-rw-rw-   0        0        0     2749 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.5/propdes/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0       92 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      141 2023-06-12 06:22:18.000000 propeller_design_tools-0.3.5/setup.py
```

### Comparing `propeller_design_tools-0.3.4/LICENSE` & `propeller_design_tools-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/MANIFEST.in` & `propeller_design_tools-0.3.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/README.md` & `propeller_design_tools-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/airfoil.py` & `propeller_design_tools-0.3.5/propdes/airfoil.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/custom_opengl_classes.py` & `propeller_design_tools-0.3.5/propdes/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/foil_ui_classes.py` & `propeller_design_tools-0.3.5/propdes/foil_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/funcs.py` & `propeller_design_tools-0.3.5/propdes/funcs.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/helper_ui_classes.py` & `propeller_design_tools-0.3.5/propdes/helper_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/helper_ui_subclasses.py` & `propeller_design_tools-0.3.5/propdes/helper_ui_subclasses.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/optimizations.py` & `propeller_design_tools-0.3.5/propdes/optimizations.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/prop_analysis_ui_classes.py` & `propeller_design_tools-0.3.5/propdes/prop_analysis_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/prop_creation_ui_classes.py` & `propeller_design_tools-0.3.5/propdes/prop_creation_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/propeller.py` & `propeller_design_tools-0.3.5/propdes/propeller.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/radialstation.py` & `propeller_design_tools-0.3.5/propdes/radialstation.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/science_spinbox_class.py` & `propeller_design_tools-0.3.5/propdes/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/settings.py` & `propeller_design_tools-0.3.5/propdes/settings.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/user_interface.py` & `propeller_design_tools-0.3.5/propdes/user_interface.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propdes/user_io.py` & `propeller_design_tools-0.3.5/propdes/user_io.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.3.4/propeller_design_tools.egg-info/SOURCES.txt` & `propeller_design_tools-0.3.5/propeller_design_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

