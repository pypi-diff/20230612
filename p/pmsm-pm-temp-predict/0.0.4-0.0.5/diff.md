# Comparing `tmp/pmsm_pm_temp_predict-0.0.4.tar.gz` & `tmp/pmsm_pm_temp_predict-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmsm_pm_temp_predict-0.0.4.tar", last modified: Sun Jun 11 19:48:55 2023, max compression
+gzip compressed data, was "pmsm_pm_temp_predict-0.0.5.tar", last modified: Sun Jun 11 22:25:13 2023, max compression
```

## Comparing `pmsm_pm_temp_predict-0.0.4.tar` & `pmsm_pm_temp_predict-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 19:48:55.635667 pmsm_pm_temp_predict-0.0.4/
--rw-rw-rw-   0        0        0      704 2023-06-11 19:48:55.635667 pmsm_pm_temp_predict-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 19:48:55.622668 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict/
--rw-rw-rw-   0        0        0       58 2023-06-11 15:57:15.000000 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict/__init__.py
--rw-rw-rw-   0        0        0     2335 2023-06-11 19:47:47.000000 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict/prediction.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:48:55.633669 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict.egg-info/
--rw-rw-rw-   0        0        0      704 2023-06-11 19:48:55.000000 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-11 19:48:55.000000 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 19:48:55.000000 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-11 19:48:55.000000 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-11 19:48:55.000000 pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 19:48:55.636668 pmsm_pm_temp_predict-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-06-11 18:14:30.000000 pmsm_pm_temp_predict-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:25:13.239526 pmsm_pm_temp_predict-0.0.5/
+-rw-rw-rw-   0        0        0      704 2023-06-11 22:25:13.237525 pmsm_pm_temp_predict-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-11 22:25:13.224525 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict/
+-rw-rw-rw-   0        0        0      119 2023-06-11 20:56:01.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict/__init__.py
+-rw-rw-rw-   0        0        0      382 2023-06-11 22:25:10.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict/prediction.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:25:13.236526 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-11 22:25:13.000000 pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 22:25:13.239526 pmsm_pm_temp_predict-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1140 2023-06-11 22:23:58.000000 pmsm_pm_temp_predict-0.0.5/setup.py
```

### Comparing `pmsm_pm_temp_predict-0.0.4/PKG-INFO` & `pmsm_pm_temp_predict-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm_pm_temp_predict
-Version: 0.0.4
+Version: 0.0.5
 Summary: Permanent magnet temperature prediction
 Home-page: UNKNOWN
 Author: Oleksandr
 Author-email: <oleksandr.ohlashennyi.knm.2020@lpnu.ua>
 License: UNKNOWN
 Keywords: python,pmsm,motor,temperatue,prediction
 Platform: UNKNOWN
```

### Comparing `pmsm_pm_temp_predict-0.0.4/pmsm_pm_temp_predict.egg-info/PKG-INFO` & `pmsm_pm_temp_predict-0.0.5/pmsm_pm_temp_predict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmsm-pm-temp-predict
-Version: 0.0.4
+Version: 0.0.5
 Summary: Permanent magnet temperature prediction
 Home-page: UNKNOWN
 Author: Oleksandr
 Author-email: <oleksandr.ohlashennyi.knm.2020@lpnu.ua>
 License: UNKNOWN
 Keywords: python,pmsm,motor,temperatue,prediction
 Platform: UNKNOWN
```

### Comparing `pmsm_pm_temp_predict-0.0.4/setup.py` & `pmsm_pm_temp_predict-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Permanent magnet temperature prediction'
 LONG_DESCRIPTION = 'This package provides an API to predict the temperature of the permanent magnet located on the rotor of the PMS motor based on the motor voltage, current, and temperature of the coolant and stator windings.'
 
 # Setting up
 setup(
         name="pmsm_pm_temp_predict", 
         version=VERSION,
```

