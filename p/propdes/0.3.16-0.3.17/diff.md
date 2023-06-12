# Comparing `tmp/propdes-0.3.16.tar.gz` & `tmp/propdes-0.3.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propdes-0.3.16.tar", last modified: Mon Jun 12 07:40:55 2023, max compression
+gzip compressed data, was "propdes-0.3.17.tar", last modified: Mon Jun 12 08:04:01 2023, max compression
```

## Comparing `propdes-0.3.16.tar` & `propdes-0.3.17.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:40:55.401715 propdes-0.3.16/
--rw-rw-rw-   0        0        0    35128 2023-06-12 05:45:36.000000 propdes-0.3.16/LICENSE
--rw-rw-rw-   0        0        0     1378 2023-06-12 05:45:36.000000 propdes-0.3.16/MANIFEST.in
--rw-rw-rw-   0        0        0       78 2023-06-12 07:40:55.401715 propdes-0.3.16/PKG-INFO
--rw-rw-rw-   0        0        0     9222 2023-06-12 07:31:55.000000 propdes-0.3.16/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 07:40:55.396710 propdes-0.3.16/propdes/
--rw-rw-rw-   0        0        0      374 2023-06-12 05:36:14.000000 propdes-0.3.16/propdes/__init__.py
--rw-rw-rw-   0        0        0    28174 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/airfoil.py
--rw-rw-rw-   0        0        0     4755 2023-06-12 05:47:39.000000 propdes-0.3.16/propdes/custom_opengl_classes.py
--rw-rw-rw-   0        0        0    17884 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/foil_ui_classes.py
--rw-rw-rw-   0        0        0    49090 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/funcs.py
--rw-rw-rw-   0        0        0    17339 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/helper_ui_classes.py
--rw-rw-rw-   0        0        0    15821 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      373 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/opt_ui_classes.py
--rw-rw-rw-   0        0        0    10726 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/optimizations.py
--rw-rw-rw-   0        0        0    15171 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36115 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/prop_creation_ui_classes.py
--rw-rw-rw-   0        0        0    52601 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/propeller.py
--rw-rw-rw-   0        0        0    17220 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/radialstation.py
--rw-rw-rw-   0        0        0     1624 2023-06-12 05:47:39.000000 propdes-0.3.16/propdes/science_spinbox_class.py
--rw-rw-rw-   0        0        0     3952 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/settings.py
--rw-rw-rw-   0        0        0     5590 2023-06-12 05:56:42.000000 propdes-0.3.16/propdes/user_interface.py
--rw-rw-rw-   0        0        0     2749 2023-06-12 05:47:39.000000 propdes-0.3.16/propdes/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:40:55.401715 propdes-0.3.16/propdes.egg-info/
--rw-rw-rw-   0        0        0       78 2023-06-12 07:40:55.000000 propdes-0.3.16/propdes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      606 2023-06-12 07:40:55.000000 propdes-0.3.16/propdes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:40:55.000000 propdes-0.3.16/propdes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 07:40:55.000000 propdes-0.3.16/propdes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 07:40:55.401715 propdes-0.3.16/setup.cfg
--rw-rw-rw-   0        0        0      127 2023-06-12 07:40:29.000000 propdes-0.3.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:01.426258 propdes-0.3.17/
+-rw-rw-rw-   0        0        0    35128 2023-06-12 05:45:36.000000 propdes-0.3.17/LICENSE
+-rw-rw-rw-   0        0        0     1378 2023-06-12 05:45:36.000000 propdes-0.3.17/MANIFEST.in
+-rw-rw-rw-   0        0        0       78 2023-06-12 08:04:01.426258 propdes-0.3.17/PKG-INFO
+-rw-rw-rw-   0        0        0     9222 2023-06-12 07:31:55.000000 propdes-0.3.17/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:01.415531 propdes-0.3.17/propdes/
+-rw-rw-rw-   0        0        0      374 2023-06-12 05:36:14.000000 propdes-0.3.17/propdes/__init__.py
+-rw-rw-rw-   0        0        0    28174 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/airfoil.py
+-rw-rw-rw-   0        0        0     4755 2023-06-12 05:47:39.000000 propdes-0.3.17/propdes/custom_opengl_classes.py
+-rw-rw-rw-   0        0        0    17884 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    49090 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/funcs.py
+-rw-rw-rw-   0        0        0    17339 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    15821 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      373 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    10726 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/optimizations.py
+-rw-rw-rw-   0        0        0    15171 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36115 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/prop_creation_ui_classes.py
+-rw-rw-rw-   0        0        0    52601 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/propeller.py
+-rw-rw-rw-   0        0        0    17220 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/radialstation.py
+-rw-rw-rw-   0        0        0     1624 2023-06-12 05:47:39.000000 propdes-0.3.17/propdes/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     3952 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/settings.py
+-rw-rw-rw-   0        0        0     5590 2023-06-12 05:56:42.000000 propdes-0.3.17/propdes/user_interface.py
+-rw-rw-rw-   0        0        0     2749 2023-06-12 05:47:39.000000 propdes-0.3.17/propdes/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:01.426258 propdes-0.3.17/propdes.egg-info/
+-rw-rw-rw-   0        0        0       78 2023-06-12 08:04:01.000000 propdes-0.3.17/propdes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-06-12 08:04:01.000000 propdes-0.3.17/propdes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 08:04:01.000000 propdes-0.3.17/propdes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 08:04:01.000000 propdes-0.3.17/propdes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 08:04:01.426258 propdes-0.3.17/setup.cfg
+-rw-rw-rw-   0        0        0      127 2023-06-12 08:03:19.000000 propdes-0.3.17/setup.py
```

### Comparing `propdes-0.3.16/LICENSE` & `propdes-0.3.17/LICENSE`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/MANIFEST.in` & `propdes-0.3.17/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/README.md` & `propdes-0.3.17/README.md`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/airfoil.py` & `propdes-0.3.17/propdes/airfoil.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/custom_opengl_classes.py` & `propdes-0.3.17/propdes/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/foil_ui_classes.py` & `propdes-0.3.17/propdes/foil_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/funcs.py` & `propdes-0.3.17/propdes/funcs.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/helper_ui_classes.py` & `propdes-0.3.17/propdes/helper_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/helper_ui_subclasses.py` & `propdes-0.3.17/propdes/helper_ui_subclasses.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/optimizations.py` & `propdes-0.3.17/propdes/optimizations.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/prop_analysis_ui_classes.py` & `propdes-0.3.17/propdes/prop_analysis_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/prop_creation_ui_classes.py` & `propdes-0.3.17/propdes/prop_creation_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/propeller.py` & `propdes-0.3.17/propdes/propeller.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/radialstation.py` & `propdes-0.3.17/propdes/radialstation.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/science_spinbox_class.py` & `propdes-0.3.17/propdes/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/settings.py` & `propdes-0.3.17/propdes/settings.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/user_interface.py` & `propdes-0.3.17/propdes/user_interface.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes/user_io.py` & `propdes-0.3.17/propdes/user_io.py`

 * *Files identical despite different names*

### Comparing `propdes-0.3.16/propdes.egg-info/SOURCES.txt` & `propdes-0.3.17/propdes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

