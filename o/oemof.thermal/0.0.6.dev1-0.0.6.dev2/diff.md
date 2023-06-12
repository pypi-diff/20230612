# Comparing `tmp/oemof.thermal-0.0.6.dev1.tar.gz` & `tmp/oemof.thermal-0.0.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oemof.thermal-0.0.6.dev1.tar", last modified: Mon Jan 16 10:15:23 2023, max compression
+gzip compressed data, was "oemof.thermal-0.0.6.dev2.tar", last modified: Mon Feb 20 20:40:47 2023, max compression
```

## Comparing `oemof.thermal-0.0.6.dev1.tar` & `oemof.thermal-0.0.6.dev2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-01-16 10:15:23.291886 oemof.thermal-0.0.6.dev1/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     1079 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/LICENSE
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3737 2023-01-16 10:15:23.291886 oemof.thermal-0.0.6.dev1/PKG-INFO
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3464 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/README.rst
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       80 2023-01-16 10:15:23.291886 oemof.thermal-0.0.6.dev1/setup.cfg
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      854 2023-01-16 10:12:59.000000 oemof.thermal-0.0.6.dev1/setup.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-01-16 10:15:23.283887 oemof.thermal-0.0.6.dev1/src/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-01-16 10:15:23.283887 oemof.thermal-0.0.6.dev1/src/oemof/
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-01-16 10:15:23.291886 oemof.thermal-0.0.6.dev1/src/oemof/thermal/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      554 2023-01-16 10:09:43.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/__init__.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5919 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/absorption_heatpumps_and_chillers.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3565 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/cogeneration.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     9240 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/compression_heatpumps_and_chillers.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    12865 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/concentrating_solar_power.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)    22268 2023-01-16 10:06:30.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/facades.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5019 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/solar_thermal_collector.py
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     5903 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev1/src/oemof/thermal/stratified_thermal_storage.py
-drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-01-16 10:15:23.283887 oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/
--rw-rw-r--   0 patrik    (1001) patrik    (1001)     3737 2023-01-16 10:15:23.000000 oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/PKG-INFO
--rw-rw-r--   0 patrik    (1001) patrik    (1001)      585 2023-01-16 10:15:23.000000 oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/SOURCES.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)        1 2023-01-16 10:15:23.000000 oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/dependency_links.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)       58 2023-01-16 10:15:23.000000 oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/requires.txt
--rw-rw-r--   0 patrik    (1001) patrik    (1001)        6 2023-01-16 10:15:23.000000 oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/top_level.txt
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-02-20 20:40:47.942218 oemof.thermal-0.0.6.dev2/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     1079 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/LICENSE
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3737 2023-02-20 20:40:47.942218 oemof.thermal-0.0.6.dev2/PKG-INFO
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3464 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/README.rst
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       80 2023-02-20 20:40:47.942218 oemof.thermal-0.0.6.dev2/setup.cfg
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      854 2023-02-20 20:39:24.000000 oemof.thermal-0.0.6.dev2/setup.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-02-20 20:40:47.934218 oemof.thermal-0.0.6.dev2/src/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-02-20 20:40:47.934218 oemof.thermal-0.0.6.dev2/src/oemof/
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-02-20 20:40:47.938218 oemof.thermal-0.0.6.dev2/src/oemof/thermal/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      554 2023-02-13 13:03:53.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/__init__.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5919 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/absorption_heatpumps_and_chillers.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3565 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/cogeneration.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9240 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/compression_heatpumps_and_chillers.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    12865 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/concentrating_solar_power.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    24025 2023-02-20 20:35:03.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/facades.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5019 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/solar_thermal_collector.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     5903 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/src/oemof/thermal/stratified_thermal_storage.py
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-02-20 20:40:47.938218 oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     3737 2023-02-20 20:40:47.000000 oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/PKG-INFO
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)      635 2023-02-20 20:40:47.000000 oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)        1 2023-02-20 20:40:47.000000 oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)       58 2023-02-20 20:40:47.000000 oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/requires.txt
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)        6 2023-02-20 20:40:47.000000 oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/top_level.txt
+drwxrwxr-x   0 patrik    (1001) patrik    (1001)        0 2023-02-20 20:40:47.942218 oemof.thermal-0.0.6.dev2/tests/
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)     9474 2023-02-20 20:31:02.000000 oemof.thermal-0.0.6.dev2/tests/test_constraints.py
+-rw-rw-r--   0 patrik    (1001) patrik    (1001)    21215 2022-11-21 13:20:08.000000 oemof.thermal-0.0.6.dev2/tests/test_functions.py
```

### Comparing `oemof.thermal-0.0.6.dev1/LICENSE` & `oemof.thermal-0.0.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/PKG-INFO` & `oemof.thermal-0.0.6.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oemof.thermal
-Version: 0.0.6.dev1
+Version: 0.0.6.dev2
 Summary: Thermal energy components for the open energy modelling framework.
 Home-page: https://github.com/oemof/oemof-thermal
 Author: oemof developer group
 Author-email: contact@oemof.org
 License-File: LICENSE
 
 |badge_pypi| |badge_travis| |badge_docs| |badge_coverage| |link-latest-doi|
```

### Comparing `oemof.thermal-0.0.6.dev1/README.rst` & `oemof.thermal-0.0.6.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/setup.py` & `oemof.thermal-0.0.6.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(name='oemof.thermal',
-      version='0.0.6.dev1',
+      version='0.0.6.dev2',
       author='oemof developer group',
       author_email='contact@oemof.org',
       description=(
           'Thermal energy components for '
           'the open energy modelling framework.'
       ),
       url='https://github.com/oemof/oemof-thermal',
```

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/__init__.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/__init__.py`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/absorption_heatpumps_and_chillers.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/absorption_heatpumps_and_chillers.py`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/cogeneration.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/cogeneration.py`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/compression_heatpumps_and_chillers.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/compression_heatpumps_and_chillers.py`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/concentrating_solar_power.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/concentrating_solar_power.py`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/facades.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/facades.py`

 * *Files 7% similar despite different names*

```diff
@@ -211,27 +211,73 @@
     ...     u_value=0.3,
     ...     initial_storage_level=0.5,
     ...     min_storage_level=0.05,
     ...     max_storage_level=0.95
     ...     capacity=1)
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(
+            self,
+            label=None,
+            inputs=None,
+            outputs=None,
+            nominal_storage_capacity=None,
+            initial_storage_level=None,
+            investment=None,
+            invest_relation_input_output=None,
+            invest_relation_input_capacity=None,
+            invest_relation_output_capacity=None,
+            min_storage_level=0.0,
+            max_storage_level=1.0,
+            balanced=True,
+            loss_rate=0,
+            fixed_losses_relative=0,
+            fixed_losses_absolute=0,
+            inflow_conversion_factor=1,
+            outflow_conversion_factor=1,
+            custom_attributes=None,
+            **kwargs
+    ):
 
-        super().__init__(
+        Facade.__init__(
+            self,
             _facade_requires_=[
                 "bus", "diameter",
                 "temp_h", "temp_c", "temp_env",
-                "u_value"], *args, **kwargs
+                "u_value"],
+            **kwargs
+        )
+
+        GenericStorage.__init__(
+            self,
+            label=label,
+            inputs=inputs,
+            outputs=outputs,
+            nominal_storage_capacity=nominal_storage_capacity,
+            initial_storage_level=initial_storage_level,
+            investment=investment,
+            invest_relation_input_output=invest_relation_input_output,
+            invest_relation_input_capacity=invest_relation_input_capacity,
+            invest_relation_output_capacity=invest_relation_output_capacity,
+            min_storage_level=min_storage_level,
+            max_storage_level=max_storage_level,
+            balanced=balanced,
+            loss_rate=loss_rate,
+            fixed_losses_relative=fixed_losses_relative,
+            fixed_losses_absolute=fixed_losses_absolute,
+            inflow_conversion_factor=inflow_conversion_factor,
+            outflow_conversion_factor=outflow_conversion_factor,
+            custom_attributes=custom_attributes,
         )
 
         self.height = kwargs.get("height")
 
         self.water_properties = {
-            'heat_capacity': kwargs.get("heat_capacity"), 'density': kwargs.get("density")
+            'heat_capacity': kwargs.get("heat_capacity"),
+            'density': kwargs.get("density")
         }
 
         self.capacity = kwargs.get("capacity")
 
         self.storage_capacity_cost = kwargs.get("storage_capacity_cost")
 
         self.capacity_cost = kwargs.get("capacity_cost")
@@ -406,15 +452,16 @@
         kwargs.update(
             {
                 "_facade_requires_": [
                     "longitude"
                 ]
             }
         )
-        super().__init__(*args, **kwargs)
+        Facade.__init__(self, *args, **kwargs)
+        Transformer.__init__(self)
 
         self.label = kwargs.get("label")
 
         self.heat_bus = kwargs.get("heat_bus")
 
         self.electrical_bus = kwargs.get("electrical_bus")
 
@@ -584,15 +631,16 @@
         kwargs.update(
             {
                 "_facade_requires_": [
                     "longitude"
                 ]
             }
         )
-        super().__init__(*args, **kwargs)
+        Facade.__init__(self, *args, **kwargs)
+        Transformer.__init__(self)
 
         self.label = kwargs.get("label")
 
         self.heat_out_bus = kwargs.get("heat_out_bus")
 
         self.electricity_in_bus = kwargs.get("electricity_in_bus")
```

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/solar_thermal_collector.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/solar_thermal_collector.py`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof/thermal/stratified_thermal_storage.py` & `oemof.thermal-0.0.6.dev2/src/oemof/thermal/stratified_thermal_storage.py`

 * *Files identical despite different names*

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/PKG-INFO` & `oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oemof.thermal
-Version: 0.0.6.dev1
+Version: 0.0.6.dev2
 Summary: Thermal energy components for the open energy modelling framework.
 Home-page: https://github.com/oemof/oemof-thermal
 Author: oemof developer group
 Author-email: contact@oemof.org
 License-File: LICENSE
 
 |badge_pypi| |badge_travis| |badge_docs| |badge_coverage| |link-latest-doi|
```

### Comparing `oemof.thermal-0.0.6.dev1/src/oemof.thermal.egg-info/SOURCES.txt` & `oemof.thermal-0.0.6.dev2/src/oemof.thermal.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 src/oemof/thermal/__init__.py
 src/oemof/thermal/absorption_heatpumps_and_chillers.py
 src/oemof/thermal/cogeneration.py
 src/oemof/thermal/compression_heatpumps_and_chillers.py
 src/oemof/thermal/concentrating_solar_power.py
 src/oemof/thermal/facades.py
 src/oemof/thermal/solar_thermal_collector.py
-src/oemof/thermal/stratified_thermal_storage.py
+src/oemof/thermal/stratified_thermal_storage.py
+tests/test_constraints.py
+tests/test_functions.py
```

