# Comparing `tmp/e-data-1.1.3.tar.gz` & `tmp/e-data-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-data-1.1.3.tar", last modified: Mon Jun 12 16:04:28 2023, max compression
+gzip compressed data, was "e-data-1.1.4.tar", last modified: Mon Jun 12 16:37:40 2023, max compression
```

## Comparing `e-data-1.1.3.tar` & `e-data-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.428333 e-data-1.1.3/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    35149 2023-06-11 10:01:58.000000 e-data-1.1.3/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      193 2023-06-11 10:01:58.000000 e-data-1.1.3/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:04:28.428333 e-data-1.1.3/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4860 2023-06-11 10:01:58.000000 e-data-1.1.3/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.392333 e-data-1.1.3/e_data.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      507 2023-06-12 16:04:28.000000 e-data-1.1.3/e_data.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      134 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-06-12 16:04:27.000000 e-data-1.1.3/e_data.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.396333 e-data-1.1.3/edata/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.3/edata/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.404333 e-data-1.1.3/edata/connectors/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 12:18:54.000000 e-data-1.1.3/edata/connectors/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15204 2023-06-12 15:54:38.000000 e-data-1.1.3/edata/connectors/datadis.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1990 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/connectors/redata.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3828 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/definitions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22473 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/helpers.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:04:28.428333 e-data-1.1.3/edata/processors/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.3/edata/processors/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6224 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/billing.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2330 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/consumption.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1334 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/maximeter.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5155 2023-06-11 12:05:56.000000 e-data-1.1.3/edata/processors/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       54 2023-06-12 16:04:28.436333 e-data-1.1.3/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4283 2023-06-12 16:03:17.000000 e-data-1.1.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.095496 e-data-1.1.4/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    35149 2023-06-11 10:01:58.000000 e-data-1.1.4/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      193 2023-06-11 10:01:58.000000 e-data-1.1.4/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:37:40.095496 e-data-1.1.4/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4860 2023-06-11 10:01:58.000000 e-data-1.1.4/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.059496 e-data-1.1.4/e_data.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5703 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      507 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      120 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-06-12 16:37:39.000000 e-data-1.1.4/e_data.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.071496 e-data-1.1.4/edata/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.4/edata/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.079496 e-data-1.1.4/edata/connectors/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 12:18:54.000000 e-data-1.1.4/edata/connectors/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15204 2023-06-12 15:54:38.000000 e-data-1.1.4/edata/connectors/datadis.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1990 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/connectors/redata.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3828 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/definitions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22473 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/helpers.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-12 16:37:40.091496 e-data-1.1.4/edata/processors/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-06-11 10:01:58.000000 e-data-1.1.4/edata/processors/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/processors/base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6287 2023-06-12 16:29:42.000000 e-data-1.1.4/edata/processors/billing.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2385 2023-06-12 16:33:12.000000 e-data-1.1.4/edata/processors/consumption.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1334 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/processors/maximeter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5155 2023-06-11 12:05:56.000000 e-data-1.1.4/edata/processors/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       54 2023-06-12 16:37:40.099496 e-data-1.1.4/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4261 2023-06-12 16:36:36.000000 e-data-1.1.4/setup.py
```

### Comparing `e-data-1.1.3/LICENSE` & `e-data-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/PKG-INFO` & `e-data-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `e-data-1.1.3/README.md` & `e-data-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/e_data.egg-info/PKG-INFO` & `e-data-1.1.4/e_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-data
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python library for managing spanish energy data from various web providers
 Home-page: https://github.com/uvejota/python-edata
 Author: VMG
 Author-email: vmayorg@outlook.es
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `e-data-1.1.3/edata/connectors/datadis.py` & `e-data-1.1.4/edata/connectors/datadis.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/edata/connectors/redata.py` & `e-data-1.1.4/edata/connectors/redata.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/edata/definitions.py` & `e-data-1.1.4/edata/definitions.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/edata/helpers.py` & `e-data-1.1.4/edata/helpers.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/edata/processors/base.py` & `e-data-1.1.4/edata/processors/base.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/edata/processors/billing.py` & `e-data-1.1.4/edata/processors/billing.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,17 @@
                     {
                         "date_format": "%Y-%m-%dT00:00:00",
                         "period": "D",
                         "dictkey": "daily",
                     },
                 ):
                     _t = self._df.copy()
-                    _t = _t.groupby([_t.datetime.dt.to_period(opt["period"])]).sum()
+                    _t = _t.groupby([_t.datetime.dt.to_period(opt["period"])]).sum(
+                        numeric_only=True
+                    )
                     _t.reset_index(inplace=True)
                     _t["datetime"] = _t["datetime"].dt.strftime(opt["date_format"])
                     _t = _t.round(2)
                     self._output[opt["dictkey"]] = utils.deserialize_dict(
                         _t.to_dict("records")
                     )
             else:
```

### Comparing `e-data-1.1.3/edata/processors/consumption.py` & `e-data-1.1.4/edata/processors/consumption.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,17 @@
             ):
                 _t = self._df.copy()
                 for tariff in ("p1", "p2", "p3"):
                     _t["value_" + tariff + "_kWh"] = _t.loc[
                         _t["px"] == tariff, "value_kWh"
                     ]
                 _t.drop(["real"], axis=1, inplace=True)
-                _t = _t.groupby([_t.datetime.dt.to_period(opt["period"])]).sum()
+                _t = _t.groupby([_t.datetime.dt.to_period(opt["period"])]).sum(
+                    numeric_only=True
+                )
                 _t.reset_index(inplace=True)
                 _t["datetime"] = _t["datetime"].dt.strftime(opt["date_format"])
                 _t = _t.round(2)
                 self._output[opt["dictkey"]] = utils.deserialize_dict(
                     _t.to_dict("records")
                 )
             self._ready = True
```

### Comparing `e-data-1.1.3/edata/processors/maximeter.py` & `e-data-1.1.4/edata/processors/maximeter.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/edata/processors/utils.py` & `e-data-1.1.4/edata/processors/utils.py`

 * *Files identical despite different names*

### Comparing `e-data-1.1.3/setup.py` & `e-data-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,22 @@
 DESCRIPTION = (
     "Python library for managing spanish energy data from various web providers"
 )
 URL = "https://github.com/uvejota/python-edata"
 EMAIL = "vmayorg@outlook.es"
 AUTHOR = "VMG"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.1.3"
+VERSION = "1.1.4"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "dateparser>=1.1.2",
     "freezegun>=1.2.1",
     "holidays>=0.14.2",
-    "pandas==1.5.3",
-    "numpy==1.24.3",
+    "pandas>=2.0.2",
     "pytest>=7.1.2",
     "python_dateutil>=2.8.2",
     "requests>=2.28.1",
 ]
 
 # What packages are optional?
 EXTRAS = {
```

