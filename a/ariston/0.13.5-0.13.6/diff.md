# Comparing `tmp/ariston-0.13.5.tar.gz` & `tmp/ariston-0.13.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.13.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ariston-0.13.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ariston-0.13.5.tar` & `ariston-0.13.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-11 19:03:10.022905 ariston-0.13.5/LICENSE
--rw-r--r--   0        0        0     3495 2023-06-11 19:03:10.022905 ariston-0.13.5/README.md
--rw-r--r--   0        0        0     5975 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/__init__.py
--rw-r--r--   0        0        0    23657 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/ariston_api.py
--rw-r--r--   0        0        0    13946 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/const.py
--rw-r--r--   0        0        0    12513 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/device.py
--rw-r--r--   0        0        0     3766 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/evo_device.py
--rw-r--r--   0        0        0     1090 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/evo_lydos_device.py
--rw-r--r--   0        0        0    30576 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/galevo_device.py
--rw-r--r--   0        0        0     1487 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/lux_device.py
--rw-r--r--   0        0        0     3172 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/lydos_hybrid_device.py
--rw-r--r--   0        0        0     9836 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/nuos_split_device.py
--rw-r--r--   0        0        0     7118 2023-06-11 19:03:10.022905 ariston-0.13.5/ariston/velis_device.py
--rw-r--r--   0        0        0      361 2023-06-11 19:03:10.026905 ariston-0.13.5/pyproject.toml
--rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-11 19:33:25.984485 ariston-0.13.6/LICENSE
+-rw-r--r--   0        0        0     3495 2023-06-11 19:33:25.984485 ariston-0.13.6/README.md
+-rw-r--r--   0        0        0     5975 2023-06-11 19:33:25.984485 ariston-0.13.6/ariston/__init__.py
+-rw-r--r--   0        0        0    23657 2023-06-11 19:33:25.984485 ariston-0.13.6/ariston/ariston_api.py
+-rw-r--r--   0        0        0    13946 2023-06-11 19:33:25.984485 ariston-0.13.6/ariston/const.py
+-rw-r--r--   0        0        0    12525 2023-06-11 19:33:25.984485 ariston-0.13.6/ariston/device.py
+-rw-r--r--   0        0        0     3766 2023-06-11 19:33:25.984485 ariston-0.13.6/ariston/evo_device.py
+-rw-r--r--   0        0        0     1090 2023-06-11 19:33:25.984485 ariston-0.13.6/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0    30576 2023-06-11 19:33:25.988485 ariston-0.13.6/ariston/galevo_device.py
+-rw-r--r--   0        0        0     1487 2023-06-11 19:33:25.988485 ariston-0.13.6/ariston/lux_device.py
+-rw-r--r--   0        0        0     3172 2023-06-11 19:33:25.988485 ariston-0.13.6/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0     9836 2023-06-11 19:33:25.988485 ariston-0.13.6/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     7118 2023-06-11 19:33:25.988485 ariston-0.13.6/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2023-06-11 19:33:25.988485 ariston-0.13.6/pyproject.toml
+-rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.6/PKG-INFO
```

### Comparing `ariston-0.13.5/LICENSE` & `ariston-0.13.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/README.md` & `ariston-0.13.6/README.md`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/__init__.py` & `ariston-0.13.6/ariston/__init__.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/ariston_api.py` & `ariston-0.13.6/ariston/ariston_api.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/const.py` & `ariston-0.13.6/ariston/const.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/device.py` & `ariston-0.13.6/ariston/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     def _get_consumption_sequence_last_value(
         self,
         consumption_type: ConsumptionType,
         time_interval: ConsumptionTimeInterval,
     ) -> Any:
         """Get last value for consumption sequence"""
         for sequence in self.consumptions_sequences:
-            if sequence["k"] == consumption_type and sequence["p"] == time_interval:
+            if sequence["k"] == consumption_type.value and sequence["p"] == time_interval.value:
                 return sequence["v"][-1]
 
         return None
 
     def _update_energy(self, old_consumptions_sequences: list[dict[str, Any]]) -> None:
         """Update the device energy settings"""
         if (
```

### Comparing `ariston-0.13.5/ariston/evo_device.py` & `ariston-0.13.6/ariston/evo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/evo_lydos_device.py` & `ariston-0.13.6/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/galevo_device.py` & `ariston-0.13.6/ariston/galevo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/lux_device.py` & `ariston-0.13.6/ariston/lux_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/lydos_hybrid_device.py` & `ariston-0.13.6/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/nuos_split_device.py` & `ariston-0.13.6/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/ariston/velis_device.py` & `ariston-0.13.6/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.5/PKG-INFO` & `ariston-0.13.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.13.5
+Version: 0.13.6
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
```

