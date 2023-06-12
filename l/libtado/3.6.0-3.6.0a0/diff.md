# Comparing `tmp/libtado-3.6.0.tar.gz` & `tmp/libtado-3.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libtado-3.6.0.tar", last modified: Wed May  3 06:54:09 2023, max compression
+gzip compressed data, was "dist/libtado-3.6.0a0.tar", last modified: Mon Jun 12 15:10:46 2023, max compression
```

## Comparing `libtado-3.6.0.tar` & `libtado-3.6.0a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 06:54:09.000000 libtado-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-03 06:53:53.000000 libtado-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:53:53.000000 libtado-3.6.0/libtado/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18009 2023-05-03 06:53:53.000000 libtado-3.6.0/libtado/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46255 2023-05-03 06:53:53.000000 libtado-3.6.0/libtado/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 06:54:09.000000 libtado-3.6.0/libtado.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-03 06:53:54.000000 libtado-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 06:54:09.000000 libtado-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 06:53:54.000000 libtado-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:54:09.000000 libtado-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:53:53.000000 libtado-3.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:53:53.000000 libtado-3.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:46.000000 libtado-3.6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 15:10:46.000000 libtado-3.6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-12 15:10:33.000000 libtado-3.6.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:33.000000 libtado-3.6.0a0/libtado/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18009 2023-06-12 15:10:33.000000 libtado-3.6.0a0/libtado/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48165 2023-06-12 15:10:33.000000 libtado-3.6.0a0/libtado/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 15:10:46.000000 libtado-3.6.0a0/libtado.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-12 15:10:33.000000 libtado-3.6.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 15:10:46.000000 libtado-3.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-12 15:10:33.000000 libtado-3.6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:46.000000 libtado-3.6.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:33.000000 libtado-3.6.0a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:33.000000 libtado-3.6.0a0/tests/conftest.py
```

### Comparing `libtado-3.6.0/README.md` & `libtado-3.6.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Tado python library
 
+<img src="docs/logo.png" alt="Libtado Logo" width="200px" align="center"/>
+
+---
+
 A library to control your Tado Smart Thermostat. This repository contains an actual library in `libtado/api.py` and a proof of concept command line client in `libtado/__main__.py`.
 
 **The tested version of APIs is Tado v2.**
 
 ## Installation
 
 You can download official library with `pip install libtado`.
```

### Comparing `libtado-3.6.0/libtado/__main__.py` & `libtado-3.6.0a0/libtado/__main__.py`

 * *Files identical despite different names*

### Comparing `libtado-3.6.0/libtado/api.py` & `libtado-3.6.0a0/libtado/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,45 +213,42 @@
     self.access_token = response['access_token']
     self.token_expiry = time.time() + float(response['expires_in'])
     self.refresh_token = response['refresh_token']
     self.access_headers['Authorization'] = 'Bearer ' + self.access_token
 
   def get_capabilities(self, zone):
     """
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict: The capabilities of a tado zone as dictionary.
-
-    Example
-    =======
-    ::
+      temperatures (dict): The temperature capabilities of the zone.
+      type (str): The temperature type of the zone.
 
+    Example:
+      ```json
       {
         'temperatures': {
           'celsius': {'max': 25, 'min': 5, 'step': 1.0},
           'fahrenheit': {'max': 77, 'min': 41, 'step': 1.0}
         },
         'type': 'HEATING'
       }
-
+      ```
     """
     data = self._api_call('homes/%i/zones/%i/capabilities' % (self.id, zone))
     return data
 
   def get_devices(self):
     """
     Returns:
-      list: All devices of the home as a list of dictionaries.
-
-    Example
-    =======
-    ::
+      (list): All devices of the home as a list of dictionaries.
 
+    Example:
+      ```json
       [
         {
           'characteristics': { 'capabilities': [] },
           'connectionState': {
             'timestamp': '2017-02-20T18:51:47.362Z',
             'value': True
           },
@@ -308,59 +305,68 @@
             'timestamp': '2017-01-12T13:22:11.618Z',
             'value': 'CALIBRATED'
            },
           'serialNo': 'SOME_SERIAL',
           'shortSerialNo': 'SOME_SERIAL'
         }
       ]
+      ```
     """
     data = self._api_call('homes/%i/devices' % self.id)
     return data
 
   def get_device_usage(self):
     """
     Get all devices of your home with how they are used
 
     Returns:
-      list: All devices of home as list of dictionaries
+      (list): All devices of home as list of dictionaries.
     """
 
     data = self._api_call('homes/%i/deviceList' % self.id)
     return data
 
   def get_early_start(self, zone):
     """
     Get the early start configuration of a zone.
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict: A dictionary with the early start setting of the zone. (True or False)
-
-    Example
-    =======
-    ::
+      enabled (bool): Whether early start is enabled or not.
 
-      { 'enabled': True }
+    Example:
+      ```json
+      {
+        'enabled': True
+      }
+      ```
     """
     data = self._api_call('homes/%i/zones/%i/earlyStart' % (self.id, zone))
     return data
 
   def get_home(self):
     """
     Get information about the home.
 
     Returns:
-      dict: A dictionary with information about your home.
-
-    Example
-    =======
-    ::
+      id (int): The ID of your home.
+      address (dict): The address of your home.
+      contactDetails (dict): The contact details of your home.
+      dateTimeZone (str): The timezone of your home.
+      geolocation (dict): The geolocation of your home.
+      installationCompleted (bool): Whether the installation is completed or not.
+      name (str): The name of your home.
+      partner (dict): The partner of your home.
+      simpleSmartScheduleEnabled (bool): Whether simple smart schedule is enabled or not.
+      temperatureUnit (str): The temperature unit of your home.
 
+    Example:
+      ```json
       {
         'address': {
           'addressLine1': 'SOME_STREET',
           'addressLine2': None,
           'city': 'SOME_CITY',
           'country': 'SOME_COUNTRY',
           'state': None,
@@ -379,33 +385,34 @@
         'id': SOME_ID,
         'installationCompleted': True,
         'name': 'SOME_NAME',
         'partner': None,
         'simpleSmartScheduleEnabled': True,
         'temperatureUnit': 'CELSIUS'
       }
+      ```
     """
     data = self._api_call('homes/%i' % self.id)
     return data
 
   def get_home_state(self):
     """
     Get information about the status of the home.
 
     Returns:
-      dict: A dictionary with the status of the home.
+      (dict): A dictionary with the status of the home.
     """
     data = self._api_call('homes/%i/state' % self.id)
     return data
 
   def set_home_state(self, at_home):
     """
     Set at-home/away state
 
-    Args:
+    Parameters:
       at_home (bool): True for at HOME, false for AWAY.
     """
 
     if at_home:
       payload = {'homePresence': 'HOME'}
     else:
       payload = {'homePresence': 'AWAY'}
@@ -414,36 +421,33 @@
 
 
   def get_installations(self):
     """
     It is unclear what this does.
 
     Returns:
-      list: Currently only an empty list.
-
-    Example
-    =======
-    ::
+      (list): Currently only an empty list.
 
+    Example:
+      ```json
       []
+      ```
     """
     data = self._api_call('homes/%i/installations' % self.id)
     return data
 
   def get_invitations(self):
     """
     Get active invitations.
 
     Returns:
-      list: A list of active invitations to your home.
-
-    Example
-    =======
-    ::
+      (list): A list of active invitations to your home.
 
+    Example:
+      ```json
       [
         {
           'email': 'SOME_INVITED_EMAIL',
           'firstSent': '2017-02-20T21:01:44.450Z',
           'home': {
             'address': {
               'addressLine1': 'SOME_STREET',
@@ -479,164 +483,161 @@
             'type': 'WEB_USER',
             'username': 'SOME_USERNAME'
           },
           'lastSent': '2017-02-20T21:01:44.450Z',
           'token': 'SOME_TOKEN'
         }
       ]
+      ```
     """
 
     data = self._api_call('homes/%i/invitations' % self.id)
     return data
 
   def get_me(self):
     """
     Get information about the current user.
 
     Returns:
-      dict: A dictionary with information about the current user.
-
-    Example
-    =======
-    ::
+      (dict): A dictionary with information about the current user.
 
+    Example:
+      ```json
       {
         'email': 'SOME_EMAIL',
         'homes': [
           {
             'id': SOME_ID,
             'name': 'SOME_NAME'
           }
         ],
         'locale': 'en_US',
         'mobileDevices': [],
         'name': 'SOME_NAME',
         'username': 'SOME_USERNAME',
         'secret': 'SOME_CLIENT_SECRET'
       }
+      ```
     """
 
     data = self._api_call('me')
     return data
 
   def get_mobile_devices(self):
     """Get all mobile devices."""
     data = self._api_call('homes/%i/mobileDevices' % self.id)
     return data
 
   def get_schedule_timetables(self, zone):
     """
     Gets the schedule timetables supported by the zone
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict: The schedule types
+      (dict): The schedule types.
     """
 
     data = self._api_call('homes/%i/zones/%i/schedule/timetables' % (self.id, zone))
     return data
 
   def get_schedule(self, zone):
     """
     Get the type of the currently configured schedule of a zone.
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict: A dictionary with the ID and type of the schedule of the zone.
+      (dict): A dictionary with the ID and type of the schedule of the zone.
 
     Tado allows three different types of a schedule for a zone:
 
     * The same schedule for all seven days of a week.
     * One schedule for weekdays, one for saturday and one for sunday.
     * Seven different schedules - one for every day of the week.
 
 
-    Example
-    =======
-    ::
-
+    Example:
+      ```json
       {
         'id': 1,
         'type': 'THREE_DAY'
       }
+      ```
     """
 
     data = self._api_call('homes/%i/zones/%i/schedule/activeTimetable' % (self.id, zone))
     return data
 
   def set_schedule(self, zone, schedule):
     """
     Set the type of the currently configured schedule of a zone.
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
       schedule (int): The schedule to activate.
                       The supported zones are currently
                         * 0: ONE_DAY
                         * 1: THREE_DAY
                         * 2: SEVEN_DAY
                       But the actual mapping should be retrieved via get_schedule_timetables.
 
     Returns:
-      dict: The new configuration
+      (dict): The new configuration.
     """
 
     payload = { 'id': schedule }
     return self._api_call('homes/%i/zones/%i/schedule/activeTimeTable' % (self.id, zone), payload, method='PUT')
 
   def get_schedule_blocks(self, zone, schedule):
     """
     Gets the blocks for the current schedule on a zone
 
-    Args:
+    Parameters:
       zone (int):      The zone ID.
-      schedule (int): The schedule ID to fetch
+      schedule (int): The schedule ID to fetch.
 
     Returns:
-      list: The blocks for the requested schedule
+      (list): The blocks for the requested schedule.
     """
 
     return self._api_call('homes/%i/zones/%i/schedule/timetables/%i/blocks' % (self.id, zone, schedule))
 
 
   def set_schedule_blocks(self, zone, schedule, blocks):
     """
     Sets the blocks for the current schedule on a zone
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
       schedule (int): The schedule ID.
-      blocks (list): The new blocks
+      blocks (list): The new blocks.
 
     Returns:
-      list: The new configuration
+      (list): The new configuration.
     """
 
     payload = blocks
     return self._api_call('homes/%i/zones/%i/schedule/timetables/%i/blocks' % (self.id, zone, schedule), payload, method='PUT')
 
 
   def get_state(self, zone):
     """
     Get the current state of a zone including its desired and current temperature. Check out the example output for more.
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict: A dictionary with the current settings and sensor measurements of the zone.
-
-    Example
-    =======
-    ::
+      (dict): A dictionary with the current settings and sensor measurements of the zone.
 
+    Example:
+      ```json
       {
         'activityDataPoints': {
           'heatingPower': {
             'percentage': 0.0,
             'timestamp': '2017-02-21T11:56:52.204Z',
             'type': 'PERCENTAGE'
           }
@@ -670,72 +671,70 @@
             'celsius': 20.0,
             'fahrenheit': 68.0
           },
           'type': 'HEATING'
         },
         'tadoMode': 'HOME'
       }
+      ```
     """
 
     data = self._api_call('homes/%i/zones/%i/state' % (self.id, zone))
     return data
 
   def get_measuring_device(self, zone):
     """
     Gets the active measuring device of a zone
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict: A dictionary with the current measuring informations.
+      (dict): A dictionary with the current measuring informations.
     """
 
     data = self._api_call('homes/%i/zones/%i/measuringDevice' % (self.id, zone))
     return data
 
   def get_default_overlay(self, zone):
     """
     Get the default overlay settings of a zone
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict
-
-    Example
-    =======
-    ::
+      (dict): A dictionary with the default overlay settings of the zone.
 
+    Example:
+      ```json
       {
          "terminationCondition": {
            "type": "TADO_MODE"
          }
       }
+      ```
     """
     data = self._api_call('homes/%i/zones/%i/defaultOverlay' % (self.id, zone))
     return data
 
   def get_users(self):
     """Get all users of your home."""
     data = self._api_call('homes/%i/users' % self.id)
     return data
 
   def get_weather(self):
     """
     Get the current weather of the location of your home.
 
     Returns:
-      dict: A dictionary with weather information for your home.
-
-    Example
-    =======
-    ::
+      (dict): A dictionary with weather information for your home.
 
+    Example:
+      ```json
       {
         'outsideTemperature': {
           'celsius': 8.49,
           'fahrenheit': 47.28,
           'precision': {
             'celsius': 0.01,
             'fahrenheit': 0.01
@@ -750,30 +749,29 @@
         },
         'weatherState': {
           'timestamp': '2017-02-21T12:06:11.296Z',
           'type': 'WEATHER_STATE',
           'value': 'CLOUDY_PARTLY'
         }
       }
+      ```
     """
 
     data = self._api_call('homes/%i/weather' % self.id)
     return data
 
   def get_zones(self):
     """
     Get all zones of your home.
 
     Returns:
-      list: A list of dictionaries with all your zones.
-
-    Example
-    =======
-    ::
+      (list): A list of dictionaries with all your zones.
 
+    Example:
+      ```json
       [
         { 'dateCreated': '2016-12-23T15:53:43.615Z',
           'dazzleEnabled': True,
           'deviceTypes': ['VA01'],
           'devices': [
             {
               'characteristics': {
@@ -827,97 +825,97 @@
           'id': 3,
           'name': 'SOME_NAME ',
           'reportAvailable': False,
           'supportsDazzle': True,
           'type': 'HEATING'
         }
       ]
-
+      ```
     """
 
     data = self._api_call('homes/%i/zones' % self.id)
     return data
 
   def set_zone_name(self, zone, new_name):
     """
     Sets the name of the zone
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
-      new_name (str): The new name of the zone
+      new_name (str): The new name of the zone.
 
     Returns:
-      dict
+      (dict): A dictionary with the new name of the zone.
     """
 
     payload = { 'name': new_name }
     data = self._api_call('homes/%i/zones/%i/details' % (self.id, zone), payload, method='PUT')
     return data
 
   def set_early_start(self, zone, enabled):
     """
     Enable or disable the early start feature of a zone.
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
       enabled (bool): Enable (True) or disable (False) the early start feature of the zone.
 
     Returns:
-      dict: The new configuration of the early start feature.
+      (boolean): Whether the early start feature is enabled or not.
 
-    Example
-    =======
-    ::
-
-      {'enabled': True}
+    Example:
+      ```json
+      {
+        'enabled': True
+      }
+      ```
     """
 
     if enabled:
       payload = { 'enabled': 'true' }
     else:
       payload = { 'enabled': 'false' }
 
     return self._api_call('homes/%i/zones/%i/earlyStart' % (self.id, zone), payload, method='PUT')
 
   def set_temperature(self, zone, temperature, termination='MANUAL'):
     """
     Set the desired temperature of a zone.
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
       temperature (float): The desired temperature in celsius.
       termination (str/int): The termination mode for the zone.
 
     Returns:
-      dict: A dictionary with the new zone settings.
+      (dict): A dictionary with the new zone settings.
 
     If you set a desired temperature less than 5 celsius it will turn of the zone!
 
     The termination supports three different mode:
 
     * "MANUAL": The zone will be set on the desired temperature until you change it manually.
     * "AUTO": The zone will be set on the desired temperature until the next automatic change.
     * INTEGER: The zone will be set on the desired temperature for INTEGER seconds.
 
-    Example
-    =======
-    ::
-
+    Example:
+      ```json
       {
         'setting': {
           'power': 'ON',
           'temperature': {'celsius': 12.0, 'fahrenheit': 53.6},
           'type': 'HEATING'
         },
         'termination': {
           'projectedExpiry': None,
           'type': 'MANUAL'
         },
         'type': 'MANUAL'
       }
+      ```
     """
 
     def get_termination_dict(termination):
       if termination == 'MANUAL':
         return { 'type': 'MANUAL' }
       elif termination == 'AUTO':
         return { 'type': 'TADO_MODE' }
@@ -938,132 +936,130 @@
     """End the manual control of a zone."""
     data = self._api_call('homes/%i/zones/%i/overlay' % (self.id, zone), method='DELETE')
 
   def get_away_configuration(self, zone):
     """
     Get the away configuration for a zone
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
 
     Returns:
-      dict
+      (dict): A dictionary with the away configuration.
     """
 
     data = self._api_call('homes/%i/zones/%i/awayConfiguration' % (self.id, zone))
     return data
 
   def set_open_window_detection(self, zone, enabled, seconds):
     """
     Get the open window detection for a zone
 
-    Args:
+    Parameters:
       zone (int): The zone ID.
-      enabled (bool): If open window detection is enabled
-      seconds (int): timeout in seconds
+      enabled (bool): If open window detection is enabled.
+      seconds (int): timeout in seconds.
     """
 
     payload = { 'enabled' : enabled, 'timeoutInSeconds': timeoutInSeconds }
 
     data = self._api_call('homes/%i/zones/%i/openWindowDetection' % (self.id, zone), data=payload, method='PUT')
     return data
 
   def get_report(self, zone, date):
     """
-    Args:
+    Parameters:
       zone (int): The zone ID.
-      date (str): The date in ISO8601 format. e.g. "2019-02-14"
+      date (str): The date in ISO8601 format. e.g. "2019-02-14".
 
     Returns:
-      dict: The daily report.
+      (dict): The daily report.
 
     """
     data = self._api_call('homes/%i/zones/%i/dayReport?date=%s' % (self.id, zone, date))
     return data
 
   def get_heating_circuits(self):
     """
     Gets the heating circuits in the current home
 
     Returns:
-      list of all dictionaries for all heating circuits
+      (list): List of all dictionaries for all heating circuits.
     """
 
     data = self._api_call('homes/%i/heatingCircuits' % self.id)
     return data
 
   def get_incidents(self):
     """
     Gets the ongoing incidents in the current home
 
     Returns:
-      dict: Incident information
+      (dict): Incident information.
     """
 
     data = self._api_minder_call('homes/%i/incidents' % self.id)
     return data
 
   def get_installations(self):
     """
     Gets the ongoing installations in the current home
 
     Returns:
-      list of all current installations
+      (list): List of all current installations
     """
 
     data = self._api_call('homes/%i/installations' % self.id)
     return data
 
   def get_temperature_offset(self, device_serial):
     """
     Gets the temperature offset of a device
 
     Returns:
-      dict: A dictionary that returns the offset in 'celsius' and 'fahrenheit'
-
-    Example
-    =======
-    ::
+      (dict): A dictionary that returns the offset in 'celsius' and 'fahrenheit'.
 
+    Example:
+      ```json
       {
            "celsius": 0.0,
            "fahrenheit": 0.0
       }
+      ```
     """
 
     data = self._api_call('devices/%s/temperatureOffset' % device_serial)
     return data
 
   def set_temperature_offset(self, device_serial, offset):
     """
     Sets the temperature offset of a device
 
-    Args:
-      device_serial (Str): The serial number of the device
-      offset (float): the temperature offset to apply in celsius
+    Parameters:
+      device_serial (Str): The serial number of the device.
+      offset (float): the temperature offset to apply in celsius.
 
     Returns:
-      dict: A dictionary that returns the offset in 'celsius' and 'fahrenheit'
+      (dict): A dictionary that returns the offset in 'celsius' and 'fahrenheit'.
     """
 
     payload = { 'celsius':  offset }
 
     return self._api_call('devices/%s/temperatureOffset' % device_serial, payload, method='PUT')
 
   def get_air_comfort(self):
     """
     Get all zones of your home.
 
     Returns:
-      list: A list of dictionaries with all your zones.
-
-    Example
-    =======
-    ::
+      freshness (dict): A dictionary with the freshness of your home.
+      comfort (list): A list of dictionaries with the comfort of each zone.
 
+    Example:
+      ```json
       {
           "freshness":{
               "value":"FAIR",
               "lastOpenWindow":"2020-09-04T10:38:57Z"
           },
           "comfort":[
               {
@@ -1082,33 +1078,32 @@
                   "coordinate":{
                       "radial":0.43,
                       "angular":324
                   }
               }
           ]
       }
+      ```
     """
     data = self._api_call('homes/%i/airComfort' % self.id)
     return data
 
   def get_air_comfort_geoloc(self, latitude, longitude):
     """
     Get all zones of your home.
 
-    Args:
+    Parameters:
       latitude (float): The latitude of the home.
       longitude (float): The longitude of the home.
 
     Returns:
-      list: A dict of lists of dictionaries with all your rooms.
-
-    Example
-    =======
-    ::
+      (list): A dict of lists of dictionaries with all your rooms.
 
+    Example:
+      ```json
       {
           "roomMessages":[
               {
                   "roomId":4,
                   "message":"Bravo\u00a0! L\u2019air de cette pi\u00e8ce est proche de la perfection.",
                   "visual":"success",
                   "link":null
@@ -1252,376 +1247,367 @@
                           "value":5.76,
                           "units":"ppb"
                       }
                   }
               ]
           }
       }
+      ```
     """
     data = self._api_acme_call('homes/%i/airComfort?latitude=%f&longitude=%f' % (self.id, latitude, longitude))
     return data
 
 
   def get_heating_system(self):
     """
     Get all heating systems of your home.
-
-    Args:
-      None.
     
     Returns:
-      list: A dict of your heating systems.
-    
-    Example
-    =======
-    ::
-
-    {
-        "boiler":{
-            "present":true,
-            "id":17830,
-            "found":true
-        },
-        "underfloorHeating":{
-            "present":false
-        }
-    }
+      (list): A dict of your heating systems.
     
+    Example:
+      ```json
+      {
+          "boiler":{
+              "present":true,
+              "id":17830,
+              "found":true
+          },
+          "underfloorHeating":{
+              "present":false
+          }
+      }
+      ```
     """
     data = self._api_call('homes/%i/heatingSystem' % (self.id))
     return data
 
 
   def get_running_times(self, from_date):
     """
     Get all running times of your home.
     
-    Args:
-      None.
-    
     Returns:
-      list: A dict of your running times.
-    
-    Example
-    =======
-    ::
+      (list): A dict of your running times.
     
-    {
-        "runningTimes":[
-            {
-                "runningTimeInSeconds":0,
-                "startTime":"2022-08-18 00:00:00",
-                "endTime":"2022-08-19 00:00:00",
-                "zones":[
-                    {
-                        "id":1,
-                        "runningTimeInSeconds":0
-                    },
-                    {
-                        "id":6,
-                        "runningTimeInSeconds":0
-                    },
-                    {
-                        "id":11,
-                        "runningTimeInSeconds":0
-                    },
-                    {
-                        "id":12,
-                        "runningTimeInSeconds":0
-                    }
-                ]
-            }
-        ],
-        "summary":{
-            "startTime":"2022-08-18 00:00:00",
-            "endTime":"2022-08-19 00:00:00",
-            "totalRunningTimeInSeconds":0
-        },
-        "lastUpdated":"2022-08-18T05:07:44Z"
-    }
+    Example:
+      ```json
+      {
+          "runningTimes":[
+              {
+                  "runningTimeInSeconds":0,
+                  "startTime":"2022-08-18 00:00:00",
+                  "endTime":"2022-08-19 00:00:00",
+                  "zones":[
+                      {
+                          "id":1,
+                          "runningTimeInSeconds":0
+                      },
+                      {
+                          "id":6,
+                          "runningTimeInSeconds":0
+                      },
+                      {
+                          "id":11,
+                          "runningTimeInSeconds":0
+                      },
+                      {
+                          "id":12,
+                          "runningTimeInSeconds":0
+                      }
+                  ]
+              }
+          ],
+          "summary":{
+              "startTime":"2022-08-18 00:00:00",
+              "endTime":"2022-08-19 00:00:00",
+              "totalRunningTimeInSeconds":0
+          },
+          "lastUpdated":"2022-08-18T05:07:44Z"
+      }
+      ```
     """
     data = self._api_minder_call('homes/%i/runningTimes?from=%s' % (self.id, from_date))
     return data
 
 
   def get_zone_states(self):
     """
     Get all zone states of your home.
     
-    Args:
-      None.
-    
     Returns:
-      list: A dict of your zone states.
+      (list): A dict of your zone states.
     
-    Example
-    =======
-    ::
-    
-    {
-        "zoneStates":{
-            "1":{
-                "tadoMode":"HOME",
-                "geolocationOverride":false,
-                "geolocationOverrideDisableTime":"None",
-                "preparation":"None",
-                "setting":{
-                    "type":"HEATING",
-                    "power":"ON",
-                    "temperature":{
-                        "celsius":19.0,
-                        "fahrenheit":66.2
-                    }
-                },
-                "overlayType":"None",
-                "overlay":"None",
-                "openWindow":"None",
-                "nextScheduleChange":{
-                    "start":"2022-08-18T16:00:00Z",
-                    "setting":{
-                        "type":"HEATING",
-                        "power":"ON",
-                        "temperature":{
-                            "celsius":20.0,
-                            "fahrenheit":68.0
-                        }
-                    }
-                },
-                "nextTimeBlock":{
-                    "start":"2022-08-18T16:00:00.000Z"
-                },
-                "link":{
-                    "state":"ONLINE"
-                },
-                "activityDataPoints":{
-                    "heatingPower":{
-                        "type":"PERCENTAGE",
-                        "percentage":0.0,
-                        "timestamp":"2022-08-18T05:34:32.127Z"
-                    }
-                },
-                "sensorDataPoints":{
-                    "insideTemperature":{
-                        "celsius":24.13,
-                        "fahrenheit":75.43,
-                        "timestamp":"2022-08-18T05:36:21.241Z",
-                        "type":"TEMPERATURE",
-                        "precision":{
-                            "celsius":0.1,
-                            "fahrenheit":0.1
-                        }
-                    },
-                    "humidity":{
-                        "type":"PERCENTAGE",
-                        "percentage":62.2,
-                        "timestamp":"2022-08-18T05:36:21.241Z"
-                    }
-                }
-            },
-            "6":{
-                "tadoMode":"HOME",
-                "geolocationOverride":false,
-                "geolocationOverrideDisableTime":"None",
-                "preparation":"None",
-                "setting":{
-                    "type":"HEATING",
-                    "power":"ON",
-                    "temperature":{
-                        "celsius":19.5,
-                        "fahrenheit":67.1
-                    }
-                },
-                "overlayType":"None",
-                "overlay":"None",
-                "openWindow":"None",
-                "nextScheduleChange":{
-                    "start":"2022-08-18T07:00:00Z",
-                    "setting":{
-                        "type":"HEATING",
-                        "power":"ON",
-                        "temperature":{
-                            "celsius":18.0,
-                            "fahrenheit":64.4
-                        }
-                    }
-                },
-                "nextTimeBlock":{
-                    "start":"2022-08-18T07:00:00.000Z"
-                },
-                "link":{
-                    "state":"ONLINE"
-                },
-                "activityDataPoints":{
-                    "heatingPower":{
-                        "type":"PERCENTAGE",
-                        "percentage":0.0,
-                        "timestamp":"2022-08-18T05:47:58.505Z"
-                    }
-                },
-                "sensorDataPoints":{
-                    "insideTemperature":{
-                        "celsius":24.2,
-                        "fahrenheit":75.56,
-                        "timestamp":"2022-08-18T05:46:09.620Z",
-                        "type":"TEMPERATURE",
-                        "precision":{
-                            "celsius":0.1,
-                            "fahrenheit":0.1
-                        }
-                    },
-                    "humidity":{
-                        "type":"PERCENTAGE",
-                        "percentage":64.8,
-                        "timestamp":"2022-08-18T05:46:09.620Z"
-                    }
-                }
-            } 
-        }
-    }
+    Example:
+      ```json
+      {
+          "zoneStates":{
+              "1":{
+                  "tadoMode":"HOME",
+                  "geolocationOverride":false,
+                  "geolocationOverrideDisableTime":"None",
+                  "preparation":"None",
+                  "setting":{
+                      "type":"HEATING",
+                      "power":"ON",
+                      "temperature":{
+                          "celsius":19.0,
+                          "fahrenheit":66.2
+                      }
+                  },
+                  "overlayType":"None",
+                  "overlay":"None",
+                  "openWindow":"None",
+                  "nextScheduleChange":{
+                      "start":"2022-08-18T16:00:00Z",
+                      "setting":{
+                          "type":"HEATING",
+                          "power":"ON",
+                          "temperature":{
+                              "celsius":20.0,
+                              "fahrenheit":68.0
+                          }
+                      }
+                  },
+                  "nextTimeBlock":{
+                      "start":"2022-08-18T16:00:00.000Z"
+                  },
+                  "link":{
+                      "state":"ONLINE"
+                  },
+                  "activityDataPoints":{
+                      "heatingPower":{
+                          "type":"PERCENTAGE",
+                          "percentage":0.0,
+                          "timestamp":"2022-08-18T05:34:32.127Z"
+                      }
+                  },
+                  "sensorDataPoints":{
+                      "insideTemperature":{
+                          "celsius":24.13,
+                          "fahrenheit":75.43,
+                          "timestamp":"2022-08-18T05:36:21.241Z",
+                          "type":"TEMPERATURE",
+                          "precision":{
+                              "celsius":0.1,
+                              "fahrenheit":0.1
+                          }
+                      },
+                      "humidity":{
+                          "type":"PERCENTAGE",
+                          "percentage":62.2,
+                          "timestamp":"2022-08-18T05:36:21.241Z"
+                      }
+                  }
+              },
+              "6":{
+                  "tadoMode":"HOME",
+                  "geolocationOverride":false,
+                  "geolocationOverrideDisableTime":"None",
+                  "preparation":"None",
+                  "setting":{
+                      "type":"HEATING",
+                      "power":"ON",
+                      "temperature":{
+                          "celsius":19.5,
+                          "fahrenheit":67.1
+                      }
+                  },
+                  "overlayType":"None",
+                  "overlay":"None",
+                  "openWindow":"None",
+                  "nextScheduleChange":{
+                      "start":"2022-08-18T07:00:00Z",
+                      "setting":{
+                          "type":"HEATING",
+                          "power":"ON",
+                          "temperature":{
+                              "celsius":18.0,
+                              "fahrenheit":64.4
+                          }
+                      }
+                  },
+                  "nextTimeBlock":{
+                      "start":"2022-08-18T07:00:00.000Z"
+                  },
+                  "link":{
+                      "state":"ONLINE"
+                  },
+                  "activityDataPoints":{
+                      "heatingPower":{
+                          "type":"PERCENTAGE",
+                          "percentage":0.0,
+                          "timestamp":"2022-08-18T05:47:58.505Z"
+                      }
+                  },
+                  "sensorDataPoints":{
+                      "insideTemperature":{
+                          "celsius":24.2,
+                          "fahrenheit":75.56,
+                          "timestamp":"2022-08-18T05:46:09.620Z",
+                          "type":"TEMPERATURE",
+                          "precision":{
+                              "celsius":0.1,
+                              "fahrenheit":0.1
+                          }
+                      },
+                      "humidity":{
+                          "type":"PERCENTAGE",
+                          "percentage":64.8,
+                          "timestamp":"2022-08-18T05:46:09.620Z"
+                      }
+                  }
+              } 
+          }
+      }
+      ```
     """
     data = self._api_call('homes/%i/zoneStates' % (self.id))
     return data
 
   def get_energy_consumption(self, startDate, endDate, country, ngsw_bypass=True):
     """
     Get enery consumption of your home by range date
       
-    Args:
-      None.
+    Parameters:
+      startDate (str): Start date of the range date.
+      endDate (str): End date of the range date.
+      country (str): Country code.
+      ngsw_bypass (bool): Bypass the ngsw cache.
     
     Returns:
-      list: A dict of your energy consumption.
+      (list): A dict of your energy consumption.
     
-    Example
-    =======
-    ::
-    
-    {
-        "tariff": "0.104 €/kWh",
-        "unit": "m3",
-        "consumptionInputState": "full",
-        "customTariff": false,
-        "currency": "EUR",
-        "tariffInfo":{
-            "consumptionUnit": "kWh",
-            "customTariff": false,
-            "tariffInCents": 10.36,
-            "currencySign": "€",
-        "details":{
-            "totalCostInCents": 1762.98,
-            "totalConsumption": 16.13,
-            "perDay": [
-                {
-                    "date": "2022-09-01",
-                    "consumption": 0,
-                    "costInCents": 0
-                },{
-                    "date": "2022-09-02",
-                    "consumption": 0,
-                    "costInCents": 0
-                },{
-                    "date": "2022-09-03",
-                    "consumption": 0.04,
-                    "costInCents": 0.4144
-                }
-            ],
-        }
-    }
+    Example:
+      ```json
+      {
+          "tariff": "0.104 €/kWh",
+          "unit": "m3",
+          "consumptionInputState": "full",
+          "customTariff": false,
+          "currency": "EUR",
+          "tariffInfo":{
+              "consumptionUnit": "kWh",
+              "customTariff": false,
+              "tariffInCents": 10.36,
+              "currencySign": "€",
+          "details":{
+              "totalCostInCents": 1762.98,
+              "totalConsumption": 16.13,
+              "perDay": [
+                  {
+                      "date": "2022-09-01",
+                      "consumption": 0,
+                      "costInCents": 0
+                  },{
+                      "date": "2022-09-02",
+                      "consumption": 0,
+                      "costInCents": 0
+                  },{
+                      "date": "2022-09-03",
+                      "consumption": 0.04,
+                      "costInCents": 0.4144
+                  }
+              ],
+          }
+      }
+      `` 
     """
     data = self._api_energy_insights_call('homes/%i/consumption?startDate=%s&endDate=%s&country=%s&ngsw-bypass=%s' % (self.id, startDate, endDate, country, ngsw_bypass))
     return data
 
   def get_energy_savings(self, monthYear, country, ngsw_bypass=True):
     """
     Get energy savings of your home by month and year
       
-    Args:
-      None.
+    Parameters:
+      monthYear (str): Month and year of the range date.
+      country (str): Country code.
+      ngsw_bypass (bool): Bypass the ngsw cache.
     
     Returns:
-      list: A dict of your energy savings.
-    
-    Example
-    =======
-    ::
+      (list): A dict of your energy savings.
     
-    {
-        "coveredInterval":{
-            "start":"2022-08-31T23:48:02.675000Z",
-            "end":"2022-09-29T13:10:23.035000Z"
-        },
-        "totalSavingsAvailable":true,
-        "withAutoAssist":{
-            "detectedAwayDuration":{
-                "value":56,
-                "unit":"HOURS"
-            },
-            "openWindowDetectionTimes":9
-        },
-        "totalSavingsInThermostaticMode":{
-            "value":0,
-            "unit":"HOURS"
-        },
-        "manualControlSaving":{
-            "value":0,
-            "unit":"PERCENTAGE"
-        },
-        "totalSavings":{
-            "value":6.5,
-            "unit":"PERCENTAGE"
-        },
-        "hideSunshineDuration":false,
-        "awayDuration":{
-            "value":56,
-            "unit":"HOURS"
-        },
-        "showSavingsInThermostaticMode":false,
-        "communityNews":{
-            "type":"HOME_COMFORT_STATES",
-            "states":[
-                {
-                    "name":"humid",
-                    "value":47.3,
-                    "unit":"PERCENTAGE"
-                },
-                {
-                    "name":"ideal",
-                    "value":43.1,
-                    "unit":"PERCENTAGE"
-                },
-                {
-                    "name":"cold",
-                    "value":9.5,
-                    "unit":"PERCENTAGE"
-                },
-                {
-                    "name":"warm",
-                    "value":0.1,
-                    "unit":"PERCENTAGE"
-                },
-                {
-                    "name":"dry",
-                    "value":0,
-                    "unit":"PERCENTAGE"
-                }
-            ]
-        },
-        "sunshineDuration":{
-            "value":112,
-            "unit":"HOURS"
-        },
-        "hasAutoAssist":true,
-        "openWindowDetectionTimes":5,
-        "setbackScheduleDurationPerDay":{
-            "value":9.100000381469727,
-            "unit":"HOURS"
-        },
-        "totalSavingsInThermostaticModeAvailable":false,
-        "yearMonth":"2022-09",
-        "hideOpenWindowDetection":false,
-        "home":283787,
-        "hideCommunityNews":false
-    }
+    Example:
+      ```json
+      {
+          "coveredInterval":{
+              "start":"2022-08-31T23:48:02.675000Z",
+              "end":"2022-09-29T13:10:23.035000Z"
+          },
+          "totalSavingsAvailable":true,
+          "withAutoAssist":{
+              "detectedAwayDuration":{
+                  "value":56,
+                  "unit":"HOURS"
+              },
+              "openWindowDetectionTimes":9
+          },
+          "totalSavingsInThermostaticMode":{
+              "value":0,
+              "unit":"HOURS"
+          },
+          "manualControlSaving":{
+              "value":0,
+              "unit":"PERCENTAGE"
+          },
+          "totalSavings":{
+              "value":6.5,
+              "unit":"PERCENTAGE"
+          },
+          "hideSunshineDuration":false,
+          "awayDuration":{
+              "value":56,
+              "unit":"HOURS"
+          },
+          "showSavingsInThermostaticMode":false,
+          "communityNews":{
+              "type":"HOME_COMFORT_STATES",
+              "states":[
+                  {
+                      "name":"humid",
+                      "value":47.3,
+                      "unit":"PERCENTAGE"
+                  },
+                  {
+                      "name":"ideal",
+                      "value":43.1,
+                      "unit":"PERCENTAGE"
+                  },
+                  {
+                      "name":"cold",
+                      "value":9.5,
+                      "unit":"PERCENTAGE"
+                  },
+                  {
+                      "name":"warm",
+                      "value":0.1,
+                      "unit":"PERCENTAGE"
+                  },
+                  {
+                      "name":"dry",
+                      "value":0,
+                      "unit":"PERCENTAGE"
+                  }
+              ]
+          },
+          "sunshineDuration":{
+              "value":112,
+              "unit":"HOURS"
+          },
+          "hasAutoAssist":true,
+          "openWindowDetectionTimes":5,
+          "setbackScheduleDurationPerDay":{
+              "value":9.100000381469727,
+              "unit":"HOURS"
+          },
+          "totalSavingsInThermostaticModeAvailable":false,
+          "yearMonth":"2022-09",
+          "hideOpenWindowDetection":false,
+          "home":283787,
+          "hideCommunityNews":false
+      }
+      ```
     """
     data = self._api_energy_bob_call('%i/%s?country=%s&ngsw-bypass=%s' % (self.id, monthYear, country, ngsw_bypass))
     return data
```

### Comparing `libtado-3.6.0/setup.py` & `libtado-3.6.0a0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='libtado',
-  version='3.6.0',
+  version='3.6.0-alpha.0',
   author='Germain Lefebvre',
   author_email='germainlefebvre4@gmail.com',
   description='A library (and a command line client) to control your Tado Smart Thermostat.',
   url='https://github.com/germainlefebvre4/libtado',
   license='GPLv3+',
   packages=find_packages(),
   classifiers=[
```

