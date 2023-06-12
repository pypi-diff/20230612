# Comparing `tmp/aiobiketrax-0.5.0.tar.gz` & `tmp/aiobiketrax-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobiketrax-0.5.0.tar", max compression
+gzip compressed data, was "aiobiketrax-1.0.0.tar", max compression
```

## Comparing `aiobiketrax-0.5.0.tar` & `aiobiketrax-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1057 2022-07-07 22:22:53.680609 aiobiketrax-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     2888 2022-11-16 07:27:12.410369 aiobiketrax-0.5.0/README.md
--rw-r--r--   0        0        0       53 2022-12-09 22:41:32.805679 aiobiketrax-0.5.0/aiobiketrax/__init__.py
--rw-r--r--   0        0        0    19541 2022-11-15 23:41:31.255668 aiobiketrax-0.5.0/aiobiketrax/api.py
--rw-r--r--   0        0        0     4650 2022-11-15 21:42:50.141528 aiobiketrax-0.5.0/aiobiketrax/cli.py
--rw-r--r--   0        0        0    14916 2022-11-15 21:42:50.142300 aiobiketrax-0.5.0/aiobiketrax/client.py
--rw-r--r--   0        0        0      163 2022-11-16 07:27:40.220713 aiobiketrax-0.5.0/aiobiketrax/consts.py
--rw-r--r--   0        0        0      412 2022-11-15 21:42:50.143452 aiobiketrax-0.5.0/aiobiketrax/exceptions.py
--rw-r--r--   0        0        0    30780 2022-11-15 23:26:40.138879 aiobiketrax-0.5.0/aiobiketrax/models.py
--rw-r--r--   0        0        0      983 2022-12-09 22:41:28.658365 aiobiketrax-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3879 2022-12-09 22:53:43.481705 aiobiketrax-0.5.0/setup.py
--rw-r--r--   0        0        0     3697 2022-12-09 22:53:43.482346 aiobiketrax-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-07-07 22:22:53.680609 aiobiketrax-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2888 2022-11-16 07:27:12.410369 aiobiketrax-1.0.0/README.md
+-rw-r--r--   0        0        0       53 2023-06-12 15:28:32.233050 aiobiketrax-1.0.0/aiobiketrax/__init__.py
+-rw-r--r--   0        0        0    19541 2023-06-12 10:45:12.807608 aiobiketrax-1.0.0/aiobiketrax/api.py
+-rw-r--r--   0        0        0     4697 2023-06-07 20:25:34.005496 aiobiketrax-1.0.0/aiobiketrax/cli.py
+-rw-r--r--   0        0        0    16523 2023-06-12 09:21:35.659125 aiobiketrax-1.0.0/aiobiketrax/client.py
+-rw-r--r--   0        0        0      163 2022-11-16 07:27:40.220713 aiobiketrax-1.0.0/aiobiketrax/consts.py
+-rw-r--r--   0        0        0      412 2022-11-15 21:42:50.143452 aiobiketrax-1.0.0/aiobiketrax/exceptions.py
+-rw-r--r--   0        0        0    31233 2023-06-07 20:36:18.485149 aiobiketrax-1.0.0/aiobiketrax/models.py
+-rw-r--r--   0        0        0      982 2023-06-12 15:28:24.475770 aiobiketrax-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 aiobiketrax-1.0.0/PKG-INFO
```

### Comparing `aiobiketrax-0.5.0/LICENSE.md` & `aiobiketrax-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiobiketrax-0.5.0/README.md` & `aiobiketrax-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aiobiketrax-0.5.0/aiobiketrax/api.py` & `aiobiketrax-1.0.0/aiobiketrax/api.py`

 * *Files identical despite different names*

### Comparing `aiobiketrax-0.5.0/aiobiketrax/cli.py` & `aiobiketrax-1.0.0/aiobiketrax/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             username=arguments.username, password=arguments.password, session=session
         )
 
         await account.update_devices()
 
         for device in account.devices:
             await device.update_position()
+            await device.update_subscription()
 
             sys.stdout.write(pprint.pformat(device_to_dict(device)) + "\n")
 
 
 async def command_stream(arguments: argparse.Namespace):
     event = asyncio.Event()
     history = {}
```

### Comparing `aiobiketrax-0.5.0/aiobiketrax/client.py` & `aiobiketrax-1.0.0/aiobiketrax/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -347,14 +347,21 @@
         return self._device.attributes.guarded
 
     @property
     def is_auto_guarded(self) -> Optional[bool]:
         return self._device.attributes.auto_guard
 
     @property
+    def is_charging(self) -> Optional[bool]:
+        if not self._position:
+            return None
+
+        return self._position.attributes.charge
+
+    @property
     def geofence_radius(self) -> Optional[int]:
         return self._device.attributes.geofence_radius
 
     @property
     def guard_type(self) -> Optional[str]:
         return self._device.attributes.guard_type
 
@@ -404,14 +411,60 @@
     def battery_level(self) -> Optional[float]:
         if not self._position:
             return None
 
         return self._position.attributes.battery_level
 
     @property
+    def estimated_battery_level(self) -> Optional[float]:
+        if not self._position:
+            return None
+
+        battery_level = self._position.attributes.battery_level
+
+        if battery_level is None:
+            return None
+
+        # Correct the battery level based on the last reported device time. The
+        # tracker assumes 20 days of stand-by time at 100% battery level.
+        delta = datetime.now(tzutc()) - self._position.device_time
+        correction = (delta.days / 2.0) * 10.0
+
+        estimated_battery_level = battery_level - correction
+
+        # Ensure the estimated battery level is within the valid range.
+        if estimated_battery_level < 0.0:
+            return 0.0
+        elif estimated_battery_level > 100.0:
+            return 100.0
+        else:
+            return estimated_battery_level
+
+    @property
+    def fix_time(self) -> Optional[datetime]:
+        if not self._position:
+            return None
+
+        return self._position.fix_time
+
+    @property
+    def device_time(self) -> Optional[datetime]:
+        if not self._position:
+            return None
+
+        return self._position.device_time
+
+    @property
+    def server_time(self) -> Optional[datetime]:
+        if not self._position:
+            return None
+
+        return self._position.server_time
+
+    @property
     def total_distance(self) -> Optional[float]:
         if not self._position:
             return None
 
         return self._position.attributes.total_distance / 1000.0
 
     @property
@@ -433,14 +486,18 @@
 
     @property
     def trips(self) -> list["Trip"]:
         return [
             Trip(self, (trip.start_time, trip.end_time)) for trip in self._sorted_trips
         ]
 
+    @property
+    def firmware_version(self) -> Optional[str]:
+        return self._device.attributes.fw_version
+
 
 @final
 class Trip:
     """
     A `Trip` instance is a view of `models.Trip`. It retrieves the latest
     version of the data from a `Device` instance using a key that consists of
     the start time and end time of a trip.
```

### Comparing `aiobiketrax-0.5.0/aiobiketrax/models.py` & `aiobiketrax-1.0.0/aiobiketrax/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,53 +485,61 @@
         return result
 
 
 @dataclass
 class DeviceAttributes:
     alarm: Optional[bool] = None
     auto_guard: Optional[bool] = None
+    fw_version: Optional[str] = None
     geofence_radius: Optional[int] = None
+    gps_disabled: Optional[bool] = None
     guarded: Optional[bool] = None
     guard_type: Optional[str] = None
     last_alarm: Optional[int] = None
     passport: Optional[Passport] = None
     stolen: Optional[bool] = None
     trial_end: Optional[datetime] = None
 
     @staticmethod
     def from_dict(obj: Any) -> "DeviceAttributes":
         assert isinstance(obj, dict)
         alarm = from_union([from_bool, from_none], obj.get("alarm"))
         auto_guard = from_union([from_bool, from_none], obj.get("autoGuard"))
+        fw_version = from_union([from_str, from_none], obj.get("fwVersion"))
         geofence_radius = from_union([from_int, from_none], obj.get("geofenceRadius"))
+        gps_disabled = from_union([from_bool, from_none], obj.get("gpsDisabled"))
         guarded = from_union([from_bool, from_none], obj.get("guarded"))
         guard_type = from_union([from_str, from_none], obj.get("guardType"))
         last_alarm = from_union([from_int, from_none], obj.get("lastAlarm"))
         passport = from_union([Passport.from_dict, from_none], obj.get("passport"))
         stolen = from_union([from_bool, from_none], obj.get("stolen"))
         trial_end = from_union([from_datetime, from_none], obj.get("trialEnd"))
         return DeviceAttributes(
             alarm,
             auto_guard,
+            fw_version,
             geofence_radius,
+            gps_disabled,
             guarded,
             guard_type,
             last_alarm,
             passport,
             stolen,
             trial_end,
         )
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["alarm"] = from_union([from_bool, from_none], self.alarm)
         result["autoGuard"] = from_union([from_bool, from_none], self.auto_guard)
+        result["fwVersion"] = from_union([from_str, from_none], self.fw_version)
         result["geofenceRadius"] = from_union(
             [from_int, from_none], self.geofence_radius
         )
+        result["gpsDisabled"] = from_union([from_bool, from_none], self.gps_disabled)
         result["guarded"] = from_union([from_bool, from_none], self.guarded)
         result["guardType"] = from_union([from_str, from_none], self.guard_type)
         result["lastAlarm"] = from_union([from_int, from_none], self.last_alarm)
         result["passport"] = from_union(
             [lambda x: to_class(Passport, x), from_none], self.passport
         )
         result["stolen"] = from_union([from_bool, from_none], self.stolen)
```

### Comparing `aiobiketrax-0.5.0/pyproject.toml` & `aiobiketrax-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 '''
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "aiobiketrax"
-version = "0.5.0"
+version = "1.0.0"
 description = "Python library for interacting with the PowUnity BikeTrax GPS tracker."
 authors = ["Bas Stottelaar <basstottelaar@gmail.com>"]
 keywords = ["biketrax", "powunity", "asyncio", "iot", "gps"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/basilfx/aiobiketrax"
 repository = "https://github.com/basilfx/aiobiketrax"
@@ -30,18 +30,18 @@
 aiohttp = "^3.8.1"
 auth0-python = "^3.23.1"
 python = "^3.9"
 PyJWT = "^2.4.0"
 python-dateutil = "^2.8.2"
 
 [tool.poetry.dev-dependencies]
-black = "^22.10.0"
-isort = "^5.10.1"
+black = "^23.1.0"
+isort = "^5.12.0"
 pytest = "^7.2"
-flake8 = "^5.0.4"
+flake8 = "^6.0.0"
 flake8-mypy = "^17.8.0"
 
 [tool.poetry.scripts]
 biketrax = 'aiobiketrax.cli:run'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `aiobiketrax-0.5.0/PKG-INFO` & `aiobiketrax-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: aiobiketrax
-Version: 0.5.0
+Version: 1.0.0
 Summary: Python library for interacting with the PowUnity BikeTrax GPS tracker.
 Home-page: https://github.com/basilfx/aiobiketrax
 License: MIT
 Keywords: biketrax,powunity,asyncio,iot,gps
 Author: Bas Stottelaar
 Author-email: basstottelaar@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: auth0-python (>=3.23.1,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/basilfx/aiobiketrax
 Description-Content-Type: text/markdown
```

