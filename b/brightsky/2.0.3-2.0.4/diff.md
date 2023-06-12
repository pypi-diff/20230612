# Comparing `tmp/brightsky-2.0.3.tar.gz` & `tmp/brightsky-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.3.tar", last modified: Mon May 22 14:11:00 2023, max compression
+gzip compressed data, was "brightsky-2.0.4.tar", last modified: Mon Jun 12 09:38:54 2023, max compression
```

## Comparing `brightsky-2.0.3.tar` & `brightsky-2.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.779039 brightsky-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 14:10:54.000000 brightsky-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-22 14:11:00.779039 brightsky-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-22 14:10:54.000000 brightsky-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.775040 brightsky-2.0.3/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.775040 brightsky-2.0.3/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 14:10:54.000000 brightsky-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:11:00.779039 brightsky-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-22 14:10:54.000000 brightsky-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.779039 brightsky-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.229065 brightsky-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 09:38:49.000000 brightsky-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 09:38:54.229065 brightsky-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-12 09:38:49.000000 brightsky-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.225065 brightsky-2.0.4/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-12 09:38:49.000000 brightsky-2.0.4/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.229065 brightsky-2.0.4/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:38:54.000000 brightsky-2.0.4/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 09:38:49.000000 brightsky-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:38:54.229065 brightsky-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 09:38:49.000000 brightsky-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:38:54.229065 brightsky-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-12 09:38:49.000000 brightsky-2.0.4/tests/test_web.py
```

### Comparing `brightsky-2.0.3/LICENSE` & `brightsky-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/PKG-INFO` & `brightsky-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.3
+Version: 2.0.4
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.3/README.md` & `brightsky-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/__main__.py` & `brightsky-2.0.4/brightsky/__main__.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/cli.py` & `brightsky-2.0.4/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/db.py` & `brightsky-2.0.4/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/export.py` & `brightsky-2.0.4/brightsky/export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/parsers.py` & `brightsky-2.0.4/brightsky/parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,15 +130,30 @@
     pass
 
 
 class SolarRadiationObservationsParser(
     ObservationsBrightSkyMixin,
     dwdparse.parsers.SolarRadiationObservationsParser,
 ):
-    pass
+
+    def skip_timestamp(self, timestamp):
+        # We aggregate solar radiation from ten-minute data, where the values
+        # correspond to radiation for the NEXT ten minutes, i.e. the value
+        # tagged 14:30 contains the solar radiation between 14:30 - 14:40 (I
+        # have not found a place where this is officially documented, but this
+        # interpretation makes the values align with the hourly data from the
+        # 'current' sources).
+        # This makes solar radiation the only parameter where the 'recent'
+        # sources produce a data point for today, which is otherwise only
+        # served by the 'current' sources. To avoid excessive fill-up when
+        # querying today's weather, we ignore this last data point (but will
+        # pick it up on the next day).
+        if timestamp.date() == datetime.date.today():
+            return True
+        return super().skip_timestamp(timestamp)
 
 
 class VisibilityObservationsParser(
     ObservationsBrightSkyMixin,
     dwdparse.parsers.VisibilityObservationsParser,
 ):
     pass
```

### Comparing `brightsky-2.0.3/brightsky/polling.py` & `brightsky-2.0.4/brightsky/polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/query.py` & `brightsky-2.0.4/brightsky/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,17 +199,15 @@
 
 def radar(
         date, last_date=None, lat=None, lon=None, distance=200000,
         fmt='compressed', bbox=None):
     extra = {}
     if not last_date:
         last_date = date + datetime.timedelta(hours=2)
-    if lat or lon:
-        if not lat and lon:
-            raise ValueError("Please supply either both lat and lon, or none")
+    if lat is not None and lon is not None:
         x, y = _transformer.to_xy(lat, lon)
         if not -0.5 <= x <= 1099.5 or not -0.5 <= y <= 1199.5:
             raise LookupError("lat/lon lies outside the radar data range")
         center_x = int(round(x))
         center_y = int(round(y))
         pixels = distance // 1000
         bbox = (
@@ -300,15 +298,15 @@
         return tuple(reversed(self.to_latlon(x, y)))
 
     def bbox_to_geometry(self, bbox):
         if not bbox:
             bbox = (0, 0, 1199, 1099)
         top, left, bottom, right = bbox
         return {
-            'type': 'Geometry',
+            'type': 'Polygon',
             'coordinates': [
                 self.to_lonlat(left - .5, top - .5),
                 self.to_lonlat(left - .5, bottom + .5),
                 self.to_lonlat(right + .5, bottom + .5),
                 self.to_lonlat(right + .5, top - .5),
             ],
         }
```

### Comparing `brightsky-2.0.3/brightsky/settings.py` & `brightsky-2.0.4/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/tasks.py` & `brightsky-2.0.4/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/utils.py` & `brightsky-2.0.4/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky/web.py` & `brightsky-2.0.4/brightsky/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from functools import partial
 
 import falcon
 import orjson
 from dateutil.tz import gettz
 from dwdparse.units import convert_record, CONVERTERS
 from falcon import media
-from falcon.errors import HTTPInvalidParam
 from gunicorn.app.base import BaseApplication
 from gunicorn.util import import_app
 
 import brightsky
 from brightsky import query
 from brightsky.db import fetch
 from brightsky.settings import settings
@@ -42,17 +41,21 @@
 
     def parse_location(self, req, required=False):
         lat = req.get_param_as_float(
             'lat', required=required, min_value=-90, max_value=90)
         lon = req.get_param_as_float(
             'lon', required=required, min_value=-180, max_value=180)
         if lat != lat:
-            raise HTTPInvalidParam('The value cannot be NaN', 'lat')
+            raise falcon.HTTPInvalidParam("The value cannot be NaN", 'lat')
         elif lon != lon:
-            raise HTTPInvalidParam('The value cannot be NaN', 'lon')
+            raise falcon.HTTPInvalidParam("The value cannot be NaN", 'lon')
+        if (lat is None) != (lon is None):
+            raise falcon.HTTPBadRequest(
+                description="Please supply either both lat and lon, or none",
+            )
         return lat, lon
 
     def parse_source_ids(self, req):
         return (
             self._parse_list_or_single(req, 'source_id', transform=int),
             self._parse_list_or_single(req, 'dwd_station_id'),
             self._parse_list_or_single(req, 'wmo_station_id'))
```

### Comparing `brightsky-2.0.3/brightsky/worker.py` & `brightsky-2.0.4/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/brightsky.egg-info/PKG-INFO` & `brightsky-2.0.4/brightsky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.3
+Version: 2.0.4
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.3/brightsky.egg-info/SOURCES.txt` & `brightsky-2.0.4/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/setup.py` & `brightsky-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/tests/test_export.py` & `brightsky-2.0.4/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/tests/test_polling.py` & `brightsky-2.0.4/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/tests/test_settings.py` & `brightsky-2.0.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/tests/test_tasks.py` & `brightsky-2.0.4/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/tests/test_utils.py` & `brightsky-2.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.3/tests/test_web.py` & `brightsky-2.0.4/tests/test_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,14 +447,17 @@
         assert resp.json['weather'][k] == v, k
 
 
 def test_radar_response(radar_data, api):
     resp = api.simulate_get('/radar?date=2023-05-08T11:30')
     assert resp.status_code == 200
     assert len(resp.json['radar']) == 1
+    assert api.simulate_get('/radar?lat=52').status_code == 400
+    assert api.simulate_get('/radar?lon=7.6').status_code == 400
+    assert api.simulate_get('/radar?lat=52&lon=7.6').status_code == 200
 
 
 def _get_radar_data(api, fmt, bbox=False):
     url = f'/radar?date=2023-05-08T13:30&format={fmt}'
     if bbox:
         url += '&bbox=1117,334,1121,338'
     resp = api.simulate_get(url, headers={'Accept-Encoding': 'gzip'})
@@ -523,15 +526,15 @@
     _check_radar_data(data)
     clip = _get_radar_data(api, 'plain', bbox=True)
     _check_radar_data(clip)
 
 
 def test_radar_response_geometry(radar_data, api):
     resp = api.simulate_get('/radar?date=2023-05-08T11:30')
-    assert resp.json['geometry']['type'] == 'Geometry'
+    assert resp.json['geometry']['type'] == 'Polygon'
     assert 'latlon_position' not in resp.json
     expected_coords = [
         (1.4633, 55.86209),
         (3.56699, 45.69643),
         (16.58087, 45.68461),
         (18.73162, 55.84544),
     ]
@@ -540,15 +543,15 @@
         assert p[1] == pytest.approx(exp_p[1])
 
 
 def test_radar_response_bbox_geometry(radar_data, api):
     resp = api.simulate_get(
         '/radar?date=2023-05-08T11:30&lat=52&lon=7.6&distance=200000',
     )
-    assert resp.json['geometry']['type'] == 'Geometry'
+    assert resp.json['geometry']['type'] == 'Polygon'
     expected_coords = [
         (4.54411, 53.61306),
         (5.04988, 50.17614),
         (10.37685, 50.31264),
         (10.41558, 53.76658),
     ]
     for p, exp_p in zip(resp.json['geometry']['coordinates'], expected_coords):
@@ -559,15 +562,15 @@
 
 
 def test_radar_response_bbox_geometry_near_edge(radar_data, api):
     resp = api.simulate_get(
         '/radar?date=2023-05-08T11:30&lat=52&lon=2.6&distance=200000'
         '&fmt=plain',
     )
-    assert resp.json['geometry']['type'] == 'Geometry'
+    assert resp.json['geometry']['type'] == 'Polygon'
     expected_coords = [
         (2.00507, 53.70663),
         (2.74712, 50.28395),
         (5.6003, 50.47017),
         (5.14662, 53.91603),
     ]
     for p, exp_p in zip(resp.json['geometry']['coordinates'], expected_coords):
```

