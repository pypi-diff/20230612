# Comparing `tmp/teslajsonpy-3.8.1.tar.gz` & `tmp/teslajsonpy-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teslajsonpy-3.8.1.tar", max compression
+gzip compressed data, was "teslajsonpy-3.9.0.tar", max compression
```

## Comparing `teslajsonpy-3.8.1.tar` & `teslajsonpy-3.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    24168 2023-04-25 05:23:35.542426 teslajsonpy-3.8.1/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-04-25 05:23:04.142299 teslajsonpy-3.8.1/LICENSE
--rw-r--r--   0        0        0     2391 2023-04-25 05:23:04.142299 teslajsonpy-3.8.1/README.md
--rw-r--r--   0        0        0     1558 2023-04-25 05:23:35.554427 teslajsonpy-3.8.1/pyproject.toml
--rw-r--r--   0        0        0      916 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/__init__.py
--rw-r--r--   0        0        0      222 2023-04-25 05:23:35.554427 teslajsonpy-3.8.1/teslajsonpy/__version__.py
--rw-r--r--   0        0        0    46764 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/car.py
--rw-r--r--   0        0        0    25716 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/connection.py
--rw-r--r--   0        0        0     1377 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/const.py
--rw-r--r--   0        0        0    53186 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/controller.py
--rw-r--r--   0        0        0    52966 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/endpoints.json
--rw-r--r--   0        0        0     9422 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/energy.py
--rw-r--r--   0        0        0     3382 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/exceptions.py
--rw-r--r--   0        0        0     7696 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/teslaproxy.py
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 teslajsonpy-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0    24411 2023-06-12 02:53:08.822636 teslajsonpy-3.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-06-12 02:52:26.086402 teslajsonpy-3.9.0/LICENSE
+-rw-r--r--   0        0        0     2391 2023-06-12 02:52:26.086402 teslajsonpy-3.9.0/README.md
+-rw-r--r--   0        0        0     1558 2023-06-12 02:53:08.838636 teslajsonpy-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0      916 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/__init__.py
+-rw-r--r--   0        0        0      222 2023-06-12 02:53:08.838636 teslajsonpy-3.9.0/teslajsonpy/__version__.py
+-rw-r--r--   0        0        0    48303 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/car.py
+-rw-r--r--   0        0        0    25716 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/connection.py
+-rw-r--r--   0        0        0     1377 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/const.py
+-rw-r--r--   0        0        0    53186 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/controller.py
+-rw-r--r--   0        0        0    53342 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/endpoints.json
+-rw-r--r--   0        0        0     9422 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/energy.py
+-rw-r--r--   0        0        0     3382 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/exceptions.py
+-rw-r--r--   0        0        0     7696 2023-06-12 02:52:26.182402 teslajsonpy-3.9.0/teslajsonpy/teslaproxy.py
+-rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 teslajsonpy-3.9.0/PKG-INFO
```

### Comparing `teslajsonpy-3.8.1/CHANGELOG.md` & `teslajsonpy-3.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v3.9.0 (2023-06-12)
+
+### Feature
+
+* Add new heated steering wheel controls ([#408](https://github.com/zabuldon/teslajsonpy/issues/408)) ([`a8ec439`](https://github.com/zabuldon/teslajsonpy/commit/a8ec439eac3215b28712ec1d3bd45e16aae9ef7a))
+
 ## v3.8.1 (2023-04-25)
 ### Fix
 * Handle missing climate_state ([#404](https://github.com/zabuldon/teslajsonpy/issues/404)) ([`342a2ef`](https://github.com/zabuldon/teslajsonpy/commit/342a2ef03c2ccd8b4281fb815107d423f3c1bddc))
 
 ## v3.8.0 (2023-03-26)
 ### Feature
 * Add energy_site_ids and vins to update to limit updating to specific devices ([#402](https://github.com/zabuldon/teslajsonpy/issues/402)) ([`e97ccaf`](https://github.com/zabuldon/teslajsonpy/commit/e97ccaf41dcc3df0dc526882a5b85c14480ac672))
```

### Comparing `teslajsonpy-3.8.1/LICENSE` & `teslajsonpy-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/README.md` & `teslajsonpy-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/pyproject.toml` & `teslajsonpy-3.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teslajsonpy"
-version = "3.8.1"
+version = "3.9.0"
 description = "A library to work with Tesla API."
 authors = ["Sergey Isachenko <sergey.isachenkol@bool.by>"]
 license = "Apache-2.0"
 repository = "https://github.com/zabuldon/teslajsonpy"
 readme = "README.md"
 homepage = "https://github.com/zabuldon/teslajsonpy"
 documentation = "https://teslajsonpy.readthedocs.io"
```

### Comparing `teslajsonpy-3.8.1/teslajsonpy/__init__.py` & `teslajsonpy-3.9.0/teslajsonpy/__init__.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/teslajsonpy/car.py` & `teslajsonpy-3.9.0/teslajsonpy/car.py`

 * *Files 5% similar despite different names*

```diff
@@ -591,14 +591,21 @@
     def is_auto_seat_climate_right(self) -> bool:
         """Return state of auto seat climate right."""
         return self._vehicle_data.get("climate_state", {}).get(
             "auto_seat_climate_right"
         )
 
     @property
+    def is_auto_steering_wheel_heat(self) -> bool:
+        """Return the state of auto steering wheel heat."""
+        return self._vehicle_data.get("climate_state", {}).get(
+            "auto_steering_wheel_heat"
+        )
+
+    @property
     def active_route_destination(self) -> Optional[str]:
         """Return active route destination."""
         if "active_route_destination" in self._vehicle_data.get("drive_state", {}):
             return self._vehicle_data.get("drive_state", {}).get(
                 "active_route_destination"
             )
         return None
@@ -965,24 +972,58 @@
             auto_seat_position=seat_id,
             auto_climate_on=enable,
         )
         if data and data["response"]["result"] is True:
             params = {f"auto_seat_climate_{SEAT_ID_MAP[seat_id]}": enable}
             self._vehicle_data["climate_state"].update(params)
 
+    async def remote_auto_steering_wheel_heat_climate_request(
+        self, enable: bool
+    ) -> None:
+        """Send command to enable or disable auto steering wheel heat.
+
+        Args
+            enable: True to enable auto steering wheel heat, False to disable.
+
+        """
+
+        data = await self._send_command(
+            "REMOTE_AUTO_STEERING_WHEEL_HEAT_CLIMATE_REQUEST",
+            on=enable
+        )
+        if data and data["response"]["result"] is True:
+            params = {"auto_steering_wheel_heat": enable}
+            self._vehicle_data["climate_state"].update(params)
+
     async def set_heated_steering_wheel(self, value: bool) -> None:
         """Send command to set heated steering wheel."""
         data = await self._send_command(
             "REMOTE_STEERING_WHEEL_HEATER_REQUEST", on=value
         )
 
         if data and data["response"]["result"] is True:
             params = {"steering_wheel_heater": value}
             self._vehicle_data["climate_state"].update(params)
 
+    async def set_heated_steering_wheel_level(self, level: int) -> None:
+        """Send command to set the heated steering wheel level."""
+        data = await self._send_command(
+            "REMOTE_STEERING_WHEEL_HEAT_LEVEL_REQUEST", level=level
+        )
+
+        if data and data["response"]["result"] is True:
+            params = {"steering_wheel_heat_level": level}
+            self._vehicle_data["climate_state"].update(params)
+
+    def get_heated_steering_wheel_level(self) -> int:
+        """Return the status of the heated steering wheel."""
+        if self.data_available:
+            return self._vehicle_data.get("climate_state", {}).get("steering_wheel_heat_level")
+        return None
+
     async def set_hvac_mode(self, value: str) -> None:
         """Send command to set HVAC mode.
 
         Args
             value: on, off
 
         """
```

### Comparing `teslajsonpy-3.8.1/teslajsonpy/connection.py` & `teslajsonpy-3.9.0/teslajsonpy/connection.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/teslajsonpy/const.py` & `teslajsonpy-3.9.0/teslajsonpy/const.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/teslajsonpy/controller.py` & `teslajsonpy-3.9.0/teslajsonpy/controller.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/teslajsonpy/endpoints.json` & `teslajsonpy-3.9.0/teslajsonpy/endpoints.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950248756218906%*

 * *Differences: {"'REMOTE_AUTO_STEERING_WHEEL_HEAT_CLIMATE_REQUEST'": "OrderedDict([('TYPE', 'POST'), ('URI', "*

 * *                                                      "'api/1/vehicles/{vehicle_id}/command/remote_auto_steering_wheel_heat_climate_request'), "*

 * *                                                      "('AUTH', True)])",*

 * * "'REMOTE_STEERING_WHEEL_HEAT_LEVEL_REQUEST'": "OrderedDict([('TYPE', 'POST'), ('URI', "*

 * *                                               "'api/1/vehicles/{vehicle_id}/command/remote_steering_wheel_h […]*

```diff
@@ -1185,14 +1185,19 @@
         "URI": "bff/v2/mobile-app/referrals/contact-list"
     },
     "REMOTE_AUTO_SEAT_CLIMATE_REQUEST": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_auto_seat_climate_request"
     },
+    "REMOTE_AUTO_STEERING_WHEEL_HEAT_CLIMATE_REQUEST": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/remote_auto_steering_wheel_heat_climate_request"
+    },
     "REMOTE_BOOMBOX": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_boombox"
     },
     "REMOTE_SEAT_COOLING_REQUEST": {
         "AUTH": true,
@@ -1210,14 +1215,19 @@
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_start_drive"
     },
     "REMOTE_STEERING_WHEEL_HEATER_REQUEST": {
         "AUTH": true,
         "TYPE": "POST",
         "URI": "api/1/vehicles/{vehicle_id}/command/remote_steering_wheel_heater_request"
     },
+    "REMOTE_STEERING_WHEEL_HEAT_LEVEL_REQUEST": {
+        "AUTH": true,
+        "TYPE": "POST",
+        "URI": "api/1/vehicles/{vehicle_id}/command/remote_steering_wheel_heat_level_request"
+    },
     "REMOVE_VEHICLE_SHARE_DRIVER": {
         "AUTH": true,
         "TYPE": "DELETE",
         "URI": "api/1/vehicles/{vehicle_id}/drivers/{share_user_id}"
     },
     "RESET_VALET_PIN": {
         "AUTH": true,
```

### Comparing `teslajsonpy-3.8.1/teslajsonpy/energy.py` & `teslajsonpy-3.9.0/teslajsonpy/energy.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/teslajsonpy/exceptions.py` & `teslajsonpy-3.9.0/teslajsonpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/teslajsonpy/teslaproxy.py` & `teslajsonpy-3.9.0/teslajsonpy/teslaproxy.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.1/PKG-INFO` & `teslajsonpy-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teslajsonpy
-Version: 3.8.1
+Version: 3.9.0
 Summary: A library to work with Tesla API.
 Home-page: https://github.com/zabuldon/teslajsonpy
 License: Apache-2.0
 Author: Sergey Isachenko
 Author-email: sergey.isachenkol@bool.by
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,16 +16,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.7.4)
 Requires-Dist: authcaptureproxy (>=1.1.3)
 Requires-Dist: beautifulsoup4 (>=4.9.3)
 Requires-Dist: httpx (>=0.17.1,<1.0)
 Requires-Dist: orjson (>=3.8.5)
 Requires-Dist: tenacity (>=8.1.0)
```

