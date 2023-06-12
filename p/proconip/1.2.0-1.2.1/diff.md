# Comparing `tmp/proconip-1.2.0.tar.gz` & `tmp/proconip-1.2.1.tar.gz`

## Comparing `proconip-1.2.0.tar` & `proconip-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.0/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.0/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.0/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.0/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.0/src/proconip/__init__.py
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 proconip-1.2.0/src/proconip/api.py
--rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 proconip-1.2.0/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.0/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.0/LICENSE
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.0/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.1/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.1/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.1/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.1/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.1/src/proconip/__init__.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 proconip-1.2.1/src/proconip/api.py
+-rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.1/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.1/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.1/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.1/PKG-INFO
```

### Comparing `proconip-1.2.0/CODE_OF_CONDUCT.md` & `proconip-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/CONTRIBUTING.md` & `proconip-1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/.github/workflows/pylint.yml` & `proconip-1.2.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/.github/workflows/python-publish.yml` & `proconip-1.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/.github/workflows/unittest.yml` & `proconip-1.2.1/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/src/proconip/api.py` & `proconip-1.2.1/src/proconip/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     API_PATH_GET_STATE,
     API_PATH_USRCFG,
     API_PATH_COMMAND,
     ConfigObject,
     DosageTarget,
     GetStateData,
     Relay,
+    BadRelayException
 )
 
 
 async def async_get_raw_state(client_session: ClientSession, config: ConfigObject) -> str:
     """Get raw data (csv string) from the GetState.csv interface."""
     url = URL(config.base_url).with_path(API_PATH_GET_STATE)
     result = await client_session.get(url,
@@ -50,14 +51,16 @@
 
 async def async_switch_on(
         client_session: ClientSession,
         config: ConfigObject,
         current_state: GetStateData,
         relay: Relay) -> None:
     """Switch on a relay using the usrcfg.cgi interface."""
+    if current_state.is_dosage_relay(relay):
+        raise BadRelayException
     bit_state = current_state.determine_overall_relay_bit_state()
     relay_bit_mask = relay.get_bit_mask()
     bit_state[0] |= relay_bit_mask
     bit_state[1] |= relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
                                        data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
```

### Comparing `proconip-1.2.0/src/proconip/definitions.py` & `proconip-1.2.1/src/proconip/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,20 @@
             data_object.offset,
             data_object.gain,
             data_object.value)
 
     def __str__(self):
         return f"{self._name}: {self._display_value}"
 
+    @property
+    def relay_id(self) -> int:
+        """Returns the aggregated relays id (eg. 8 for the first external relay)."""
+        offset = 8 if self.category == CATEGORY_EXTERNAL_RELAY else 0
+        return self.category_id + offset
+
     def is_on(self) -> bool:
         """Returns whether the relay is on."""
         return int(self._value) & 1 == 1
 
     def is_off(self) -> bool:
         """Returns whether the relay is off."""
         return not self.is_on()
@@ -375,39 +381,61 @@
         return self._dosage_control & 256 == 256
 
     def is_ph_plus_dosage_enabled(self) -> bool:
         """Returns true if the PH+ dosage control is enabled, false otherwise."""
         return self._dosage_control & 4096 == 4096
 
     def is_dosage_enabled(self, data_entity) -> bool:
-        """Returns true if the dosage control is enabled for the given data entity,
-         false otherwise."""
+        """Returns true if the dosage control is enabled for the given data entity (canister or
+        consumption DataObject), false otherwise."""
         match data_entity.column:
             case 36 | 39:
                 return self.is_chlorine_dosage_enabled()
             case 37 | 40:
                 return self.is_ph_minus_dosage_enabled()
             case 38 | 41:
                 return self.is_ph_plus_dosage_enabled()
             case _:
                 return False
 
     def get_dosage_relay(self, data_entity) -> int:
-        """Returns the dosage relay number (equivalent to DataObject.category_id) for
-        the given data entity."""
+        """Returns the dosage relay index (i in `GetStateData.aggregated_relay_objects[i]`) for
+        the given data entity (canister or consumption DataObject)."""
         match data_entity.column:
             case 36 | 39:
                 return self._chlorine_dosage_relay_id
             case 37 | 40:
                 return self._ph_minus_dosage_relay_id
             case 38 | 41:
                 return self._ph_plus_dosage_relay_id
             case _:
                 return False
 
+    def is_dosage_relay(self,
+                        relay_object: Relay = None,
+                        data_object: DataObject = None,
+                        relay_id: int = None) -> bool:
+        """Returns true if the given relay_object OR data_object OR column refers to a dosage
+        control relay."""
+        dosage_control_relays = [
+            self._chlorine_dosage_relay_id,
+            self._ph_minus_dosage_relay_id,
+            self._ph_plus_dosage_relay_id,
+        ]
+        if relay_object is not None:
+            return relay_object.relay_id in dosage_control_relays
+        if data_object is not None:
+            if data_object.category not in (CATEGORY_RELAY, CATEGORY_EXTERNAL_RELAY):
+                raise BadRelayException
+            offset = 8 if data_object.category == CATEGORY_EXTERNAL_RELAY else 0
+            return data_object.category_id + offset in dosage_control_relays
+        if relay_id is not None:
+            return relay_id in dosage_control_relays
+        return False
+
     def get_reset_root_cause_as_str(self) -> str:
         """Returns the reason for the last reset of the controller as string."""
         if self._reset_root_cause not in RESET_ROOT_CAUSE:
             return RESET_ROOT_CAUSE[0]
         return RESET_ROOT_CAUSE[self._reset_root_cause]
 
     def get_ntp_fault_state_as_str(self) -> str:
@@ -608,7 +636,10 @@
         for relay in relays:
             relay_bit_mask = relay.get_bit_mask()
             if relay.is_auto_mode():
                 bit_state[0] &= ~relay_bit_mask
             if relay.is_on():
                 bit_state[1] |= relay_bit_mask
         return bit_state
+
+class BadRelayException(Exception):
+    """Exception to raise when an invalid relay was given as parameter."""
```

### Comparing `proconip-1.2.0/tests/helper.py` & `proconip-1.2.1/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/tests/test_definitions.py` & `proconip-1.2.1/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/.gitignore` & `proconip-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/LICENSE` & `proconip-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/README.md` & `proconip-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.0/pyproject.toml` & `proconip-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.2.0/PKG-INFO` & `proconip-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

