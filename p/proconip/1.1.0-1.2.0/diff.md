# Comparing `tmp/proconip-1.1.0.tar.gz` & `tmp/proconip-1.2.0.tar.gz`

## Comparing `proconip-1.1.0.tar` & `proconip-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.1.0/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.1.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.1.0/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.1.0/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.1.0/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.1.0/src/proconip/__init__.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 proconip-1.1.0/src/proconip/api.py
--rw-r--r--   0        0        0    21918 2020-02-02 00:00:00.000000 proconip-1.1.0/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.1.0/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.1.0/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.1.0/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.1.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.1.0/LICENSE
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 proconip-1.1.0/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 proconip-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.0/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.0/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.0/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.0/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.0/src/proconip/__init__.py
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 proconip-1.2.0/src/proconip/api.py
+-rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 proconip-1.2.0/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.0/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.0/PKG-INFO
```

### Comparing `proconip-1.1.0/CODE_OF_CONDUCT.md` & `proconip-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/CONTRIBUTING.md` & `proconip-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/.github/workflows/pylint.yml` & `proconip-1.2.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/.github/workflows/python-publish.yml` & `proconip-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/.github/workflows/unittest.yml` & `proconip-1.2.0/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/src/proconip/api.py` & `proconip-1.2.0/src/proconip/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """GetState class to get data from the GetState.csv interface."""
 
 from aiohttp import BasicAuth, ClientSession
 from yarl import URL
 
-from proconip.definitions import (
+from .definitions import (
     API_PATH_GET_STATE,
     API_PATH_USRCFG,
+    API_PATH_COMMAND,
     ConfigObject,
+    DosageTarget,
     GetStateData,
     Relay,
 )
 
 
 async def async_get_raw_state(client_session: ClientSession, config: ConfigObject) -> str:
     """Get raw data (csv string) from the GetState.csv interface."""
@@ -133,12 +135,57 @@
         """Set relay with given id to use auto mode."""
         await async_set_auto_mode(self.client_session,
                                   self.config,
                                   current_state,
                                   current_state.get_relay(relay_id))
 
 
+async def async_start_dosage(
+        client_session: ClientSession,
+        config: ConfigObject,
+        dosage_target: DosageTarget,
+        dosage_duration: int) -> None:
+    """Start manual dosge for given target and duration."""
+    url = URL(config.base_url)\
+        .with_path(API_PATH_COMMAND)\
+        .with_query(f"MAN_DOSAGE={dosage_target},{dosage_duration}")
+    result = await client_session.get(url, auth=BasicAuth(config.username,
+                                                          password=config.password))
+    if result.status != 200:
+        raise BasStatusCodeException(f"Unexpected status code: {result.status}")
+    if result.status in [401, 403]:
+        raise BadCredentialsException
+
+
+class DosageControl:
+    """DosageControl class to start manual dosage via Command.htm endpoint."""
+    def __init__(self, client_session: ClientSession, config: ConfigObject):
+        self.client_session = client_session
+        self.config = config
+
+    async def async_chlorine_dosage(self, dosage_duration: int) -> None:
+        """Start manual chlorine dosage."""
+        await async_start_dosage(self.client_session,
+                                 self.config,
+                                 DosageTarget.CHLORINE,
+                                 dosage_duration)
+
+    async def async_ph_minus_dosage(self, dosage_duration: int) -> None:
+        """Start manual pH minus dosage."""
+        await async_start_dosage(self.client_session,
+                                 self.config,
+                                 DosageTarget.PH_MINUS,
+                                 dosage_duration)
+
+    async def async_ph_plus_dosage(self, dosage_duration: int) -> None:
+        """Start manual pH plus dosage."""
+        await async_start_dosage(self.client_session,
+                                 self.config,
+                                 DosageTarget.PH_PLUS,
+                                 dosage_duration)
+
+
 class BadCredentialsException(Exception):
     """Exception to raise when we get an 401 Unauthorized or 403 Forbidden response."""
 
 class BasStatusCodeException(Exception):
     """Exception to raise when we get an unknown response code."""
```

### Comparing `proconip-1.1.0/src/proconip/definitions.py` & `proconip-1.2.0/src/proconip/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Defines data structures for use with and used by the GetState.csv and usercfg.cgi APIs."""
 import dataclasses
+from enum import IntEnum
 
 
 API_PATH_GET_STATE = "/GetState.csv"
 API_PATH_USRCFG = "/usrcfg.cgi"
+API_PATH_COMMAND = "/Command.htm"
 
 
 CATEGORY_TIME = "time"
 CATEGORY_ANALOG = "analog"
 CATEGORY_ELECTRODE = "electrode"
 CATEGORY_TEMPERATURE = "temperature"
 CATEGORY_RELAY = "relay"
@@ -31,14 +33,21 @@
     1: "Logfile (GUI warning, green)",
     2: "Warning (GUI warning, yellow)",
     4: "Error (GUI warning, red)",
     65536: "NTP available",
 }
 
 
+class DosageTarget(IntEnum):
+    """Helper enum for async_start_dosage."""
+    CHLORINE: 0
+    PH_MINUS: 1
+    PH_PLUS: 2
+
+
 @dataclasses.dataclass
 class ConfigObject:
     """Configuration to be used with classes that interact with the pool controller."""
 
     def __init__(
         self,
         base_url: str,
```

### Comparing `proconip-1.1.0/tests/helper.py` & `proconip-1.2.0/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/tests/test_definitions.py` & `proconip-1.2.0/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/.gitignore` & `proconip-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/LICENSE` & `proconip-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.1.0/README.md` & `proconip-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Python package for the ProCon.IP Pool Controller
 
 [![Pylint](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml)
 [![Unittest](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml)
 [![PyPi Package release](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml)
 
-![PyPI](https://img.shields.io/pypi/v/proconip?label=Current%20Release)
+[![PyPI](https://img.shields.io/pypi/v/proconip?label=Current%20Release)](https://pypi.org/project/proconip/)
 
 ## Overview
 
 * [Introduction (_What is this library for?_)](#introduction)
 * [Installation](#installation)
 * [Usage](#usage-examples)
   * [Reading the current state](#reading-the-current-state)
@@ -110,14 +110,38 @@
     print(f"Relay no. 3: {data.get_relay(2).display_value}")
     await client_session.close()
 
 
 asyncio.run(relay_switching_example())
 ```
 
+### Starting manual dosage
+
+Manual dosage depends on the same factors as if started from the web interface
+of the pool control itself. 
+
+```python
+import asyncio
+import aiohttp
+from proconip.definitions import ConfigObject
+from proconip.api import DosageControl
+
+
+async def manual_dosage_example():
+    client_session = aiohttp.ClientSession()
+    config = ConfigObject("http://192.168.2.3", "admin", "admin")
+    dosage_control = DosageControl(client_session, config)
+    await dosage_control.async_chlorine_dosage(3600) # start for 1 hour
+    await dosage_control.async_ph_minus_dosage(60) # start for 1 minute
+    await client_session.close()
+
+
+asyncio.run(reading_data_example())
+```
+
 ## A brief description of the ProCon.IP pool controller
 
 ![Picture from pooldigital.de](https://www.pooldigital.de/shop/media/image/66/47/a5/ProConIP1_720x600.png)
 
 The ProCon.IP pool controller is a low budget network attached control unit for
 home swimming pools. With its software switched relays, it can control
 multiple pumps (for the pool filter and different dosage aspects) either
```

### Comparing `proconip-1.1.0/pyproject.toml` & `proconip-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.1.0/PKG-INFO` & `proconip-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # Python package for the ProCon.IP Pool Controller
 
 [![Pylint](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/pylint.yml)
 [![Unittest](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/unittest.yml)
 [![PyPi Package release](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ylabonte/proconip-pypi/actions/workflows/python-publish.yml)
 
-![PyPI](https://img.shields.io/pypi/v/proconip?label=Current%20Release)
+[![PyPI](https://img.shields.io/pypi/v/proconip?label=Current%20Release)](https://pypi.org/project/proconip/)
 
 ## Overview
 
 * [Introduction (_What is this library for?_)](#introduction)
 * [Installation](#installation)
 * [Usage](#usage-examples)
   * [Reading the current state](#reading-the-current-state)
@@ -124,14 +124,38 @@
     print(f"Relay no. 3: {data.get_relay(2).display_value}")
     await client_session.close()
 
 
 asyncio.run(relay_switching_example())
 ```
 
+### Starting manual dosage
+
+Manual dosage depends on the same factors as if started from the web interface
+of the pool control itself. 
+
+```python
+import asyncio
+import aiohttp
+from proconip.definitions import ConfigObject
+from proconip.api import DosageControl
+
+
+async def manual_dosage_example():
+    client_session = aiohttp.ClientSession()
+    config = ConfigObject("http://192.168.2.3", "admin", "admin")
+    dosage_control = DosageControl(client_session, config)
+    await dosage_control.async_chlorine_dosage(3600) # start for 1 hour
+    await dosage_control.async_ph_minus_dosage(60) # start for 1 minute
+    await client_session.close()
+
+
+asyncio.run(reading_data_example())
+```
+
 ## A brief description of the ProCon.IP pool controller
 
 ![Picture from pooldigital.de](https://www.pooldigital.de/shop/media/image/66/47/a5/ProConIP1_720x600.png)
 
 The ProCon.IP pool controller is a low budget network attached control unit for
 home swimming pools. With its software switched relays, it can control
 multiple pumps (for the pool filter and different dosage aspects) either
```

