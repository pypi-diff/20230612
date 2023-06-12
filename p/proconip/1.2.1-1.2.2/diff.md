# Comparing `tmp/proconip-1.2.1.tar.gz` & `tmp/proconip-1.2.2.tar.gz`

## Comparing `proconip-1.2.1.tar` & `proconip-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.1/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.1/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.1/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.1/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.1/src/proconip/__init__.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 proconip-1.2.1/src/proconip/api.py
--rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.1/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.1/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.1/LICENSE
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.1/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.2/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.2/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.2/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.2/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.2/src/proconip/__init__.py
+-rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 proconip-1.2.2/src/proconip/api.py
+-rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.2/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.2/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.2/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.2/PKG-INFO
```

### Comparing `proconip-1.2.1/CODE_OF_CONDUCT.md` & `proconip-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/CONTRIBUTING.md` & `proconip-1.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/.github/workflows/pylint.yml` & `proconip-1.2.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/.github/workflows/python-publish.yml` & `proconip-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/.github/workflows/unittest.yml` & `proconip-1.2.2/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/src/proconip/api.py` & `proconip-1.2.2/src/proconip/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     bit_state[1] |= relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
                                        data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
     if result.status != 200:
-        raise BasStatusCodeException(f"Unexpected status code: {result.status}")
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
 
 
 async def async_switch_off(
         client_session: ClientSession,
         config: ConfigObject,
@@ -84,15 +84,15 @@
     bit_state[1] &= ~relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
                                        data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
     if result.status != 200:
-        raise BasStatusCodeException(f"Unexpected status code: {result.status}")
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
 
 
 async def async_set_auto_mode(
         client_session: ClientSession,
         config: ConfigObject,
@@ -105,15 +105,15 @@
     bit_state[1] &= ~relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
                                        data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
     if result.status != 200:
-        raise BasStatusCodeException(f"Unexpected status code: {result.status}")
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
 
 
 class RelaySwitch:
     """RelaySwitch class to set relay states via usrcfg.cgi interface."""
     def __init__(self, client_session: ClientSession, config: ConfigObject):
@@ -150,15 +150,15 @@
     """Start manual dosge for given target and duration."""
     url = URL(config.base_url)\
         .with_path(API_PATH_COMMAND)\
         .with_query(f"MAN_DOSAGE={dosage_target},{dosage_duration}")
     result = await client_session.get(url, auth=BasicAuth(config.username,
                                                           password=config.password))
     if result.status != 200:
-        raise BasStatusCodeException(f"Unexpected status code: {result.status}")
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
 
 
 class DosageControl:
     """DosageControl class to start manual dosage via Command.htm endpoint."""
     def __init__(self, client_session: ClientSession, config: ConfigObject):
@@ -186,9 +186,10 @@
                                  DosageTarget.PH_PLUS,
                                  dosage_duration)
 
 
 class BadCredentialsException(Exception):
     """Exception to raise when we get an 401 Unauthorized or 403 Forbidden response."""
 
-class BasStatusCodeException(Exception):
+
+class BadStatusCodeException(Exception):
     """Exception to raise when we get an unknown response code."""
```

### Comparing `proconip-1.2.1/src/proconip/definitions.py` & `proconip-1.2.2/src/proconip/definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/tests/helper.py` & `proconip-1.2.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/tests/test_definitions.py` & `proconip-1.2.2/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/.gitignore` & `proconip-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/LICENSE` & `proconip-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/README.md` & `proconip-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.1/pyproject.toml` & `proconip-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.2.1/PKG-INFO` & `proconip-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 1.2.1
+Version: 1.2.2
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

