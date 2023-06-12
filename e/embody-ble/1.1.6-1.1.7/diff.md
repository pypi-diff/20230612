# Comparing `tmp/embody_ble-1.1.6.tar.gz` & `tmp/embody_ble-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embody_ble-1.1.6.tar", max compression
+gzip compressed data, was "embody_ble-1.1.7.tar", max compression
```

## Comparing `embody_ble-1.1.6.tar` & `embody_ble-1.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-04-26 06:47:17.657046 embody_ble-1.1.6/LICENSE
--rw-r--r--   0        0        0     4413 2023-04-26 06:47:17.657046 embody_ble-1.1.6/README.md
--rw-r--r--   0        0        0     2134 2023-04-26 06:47:31.001087 embody_ble-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      249 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/__init__.py
--rw-r--r--   0        0        0      226 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/__main__.py
--rw-r--r--   0        0        0     7024 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/cli.py
--rw-r--r--   0        0        0    17921 2023-04-26 06:47:31.001087 embody_ble-1.1.6/src/embodyble/embodyble.py
--rw-r--r--   0        0        0      150 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/exceptions.py
--rw-r--r--   0        0        0     1089 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/listeners.py
--rw-r--r--   0        0        0        0 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/py.typed
--rw-r--r--   0        0        0    24909 2023-04-26 06:47:17.661046 embody_ble-1.1.6/src/embodyble/reporting.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 embody_ble-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-12 16:24:41.670549 embody_ble-1.1.7/LICENSE
+-rw-r--r--   0        0        0     4413 2023-06-12 16:24:41.670549 embody_ble-1.1.7/README.md
+-rw-r--r--   0        0        0     2134 2023-06-12 16:25:02.286432 embody_ble-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/__init__.py
+-rw-r--r--   0        0        0      226 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/__main__.py
+-rw-r--r--   0        0        0     7024 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/cli.py
+-rw-r--r--   0        0        0    17847 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/embodyble.py
+-rw-r--r--   0        0        0      150 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/exceptions.py
+-rw-r--r--   0        0        0     1089 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/listeners.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/py.typed
+-rw-r--r--   0        0        0    24909 2023-06-12 16:24:41.674549 embody_ble-1.1.7/src/embodyble/reporting.py
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 embody_ble-1.1.7/PKG-INFO
```

### Comparing `embody_ble-1.1.6/LICENSE` & `embody_ble-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.6/README.md` & `embody_ble-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.6/pyproject.toml` & `embody_ble-1.1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embody-ble"
-version = "1.1.6"
+version = "1.1.7"
 description = "Communicate with the EmBody device over BLE (bluetooth)"
 authors = ["Aidee Health AS <hello@aidee.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidee-health/embody-ble"
 repository = "https://github.com/aidee-health/embody-ble"
 documentation = "https://github.com/aidee-health/embody-ble"
```

### Comparing `embody_ble-1.1.6/src/embodyble/cli.py` & `embody_ble-1.1.7/src/embodyble/cli.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.6/src/embodyble/embodyble.py` & `embody_ble-1.1.7/src/embodyble/embodyble.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import asyncio
 import logging
 from concurrent.futures import ThreadPoolExecutor
 from threading import Thread
 from typing import Optional
 
 from bleak import BleakClient
-from bleak import BleakGATTCharacteristic
 from bleak import BleakScanner
+from bleak.backends.characteristic import BleakGATTCharacteristic
 from embodycodec import codec
 from embodyserial import embodyserial
 from embodyserial.helpers import EmbodySendHelper
 from packaging import version
 
 from .exceptions import EmbodyBleError
 from .listeners import BleMessageListener
@@ -85,15 +85,15 @@
     def connect(self, device_name: Optional[str] = None) -> None:
         asyncio.run_coroutine_threadsafe(
             self.__async_connect(device_name), self.__loop
         ).result()
 
     async def __async_connect(self, device_name: Optional[str] = None) -> None:
         """Connect to specified device (or use device name from serial port as default)."""
-        if self.__connected() and self.__client:
+        if self.__client:
             await self.__client.disconnect()
         if self.__reader:
             self.__reader.stop()
         if device_name:
             self.__device_name = device_name
         else:
             self.__device_name = self.__find_name_from_serial_port()
@@ -127,23 +127,26 @@
     def disconnect(self) -> None:
         asyncio.run_coroutine_threadsafe(
             self.__async_disconnect(), self.__loop
         ).result()
 
     async def __async_disconnect(self) -> None:
         """Disconnect from device if connected."""
-        if self.__connected() and self.__client:
+        if self.__client:
             try:
                 await self.__client.stop_notify(UART_TX_CHAR_UUID)
             except Exception as e:
                 logging.debug(f"Failed to stop notify UART_TX:: {e}")
             await self.__client.disconnect()
+            logging.info(f"Disconnected: {self.__client}")
+            self.__client = None
 
     def shutdown(self) -> None:
         """Shutdown after use."""
+        self.disconnect()
         self.__sender = None
         if self.__reader:
             self.__reader.stop()
             self.__reader = None
         self.__loop.stop()
         self.__connection_listener_executor.shutdown(wait=False, cancel_futures=False)
 
@@ -187,21 +190,17 @@
     def stop_ble_notify(self, uuid: str) -> None:
         if not self.__reader:
             raise EmbodyBleError("Reader not initialized")
         asyncio.run_coroutine_threadsafe(
             self.__reader.stop_ble_notify(uuid), self.__loop
         ).result()
 
-    def __connected(self) -> bool:
-        """Check whether BLE is connected (active handle)"""
-        return self.__client is not None and self.__client.is_connected
-
     def _on_disconnected(self, client: BleakClient) -> None:
         """Invoked by bleak when disconnected."""
-        logging.debug(f"Disconnected: {client}")
+        logging.info(f"Disconnected: {client}")
         self.__notify_connection_listeners(False)
         if self.__reader:
             self.__reader.stop()
 
     @staticmethod
     def __find_name_from_serial_port() -> str:
         """Request serial no from EmBody device."""
```

### Comparing `embody_ble-1.1.6/src/embodyble/listeners.py` & `embody_ble-1.1.7/src/embodyble/listeners.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.6/src/embodyble/reporting.py` & `embody_ble-1.1.7/src/embodyble/reporting.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.6/PKG-INFO` & `embody_ble-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embody-ble
-Version: 1.1.6
+Version: 1.1.7
 Summary: Communicate with the EmBody device over BLE (bluetooth)
 Home-page: https://github.com/aidee-health/embody-ble
 License: MIT
 Author: Aidee Health AS
 Author-email: hello@aidee.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

