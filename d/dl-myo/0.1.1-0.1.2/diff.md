# Comparing `tmp/dl_myo-0.1.1.tar.gz` & `tmp/dl_myo-0.1.2.tar.gz`

## Comparing `dl_myo-0.1.1.tar` & `dl_myo-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dl_myo-0.1.1/Dockerfile
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dl_myo-0.1.1/docker-compose.yml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.github/workflows/release-package.yml
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 dl_myo-0.1.1/examples/sample.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 dl_myo-0.1.1/examples/ws_client.py
--rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 dl_myo-0.1.1/examples/ws_server.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/__init__.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/commands.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/device.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/handle.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/types.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.gitignore
--rw-r--r--   0        0        0    35131 2020-02-02 00:00:00.000000 dl_myo-0.1.1/LICENSE
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 dl_myo-0.1.1/README.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 dl_myo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 dl_myo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dl_myo-0.1.2/Dockerfile
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dl_myo-0.1.2/docker-compose.yml
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 dl_myo-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 dl_myo-0.1.2/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 dl_myo-0.1.2/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 dl_myo-0.1.2/examples/sample.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 dl_myo-0.1.2/examples/ws_client.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 dl_myo-0.1.2/examples/ws_server.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 dl_myo-0.1.2/myo/__init__.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 dl_myo-0.1.2/myo/commands.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 dl_myo-0.1.2/myo/device.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 dl_myo-0.1.2/myo/handle.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 dl_myo-0.1.2/myo/types.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dl_myo-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35131 2020-02-02 00:00:00.000000 dl_myo-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 dl_myo-0.1.2/README.md
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dl_myo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dl_myo-0.1.2/PKG-INFO
```

### Comparing `dl_myo-0.1.1/.github/workflows/build.yml` & `dl_myo-0.1.2/.github/workflows/build.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build
+name: build
 on:
   release:
     types: [published]
 jobs:
   build-wheel:
     strategy:
       fail-fast: false
@@ -13,20 +13,15 @@
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - name: Lint
-        run: |
-          pip install flake8
-          # stop the build if there are Python syntax errors or undefined names
-          flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-          # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
-          flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics --exclude=examples,myo/handle.py
+        uses: chartboost/ruff-action@v1
       - name: Build
         run: |
           pip install hatch
           python -m hatch build
       - name: Upload wheel
         uses: actions/upload-artifact@v3
         with:
```

### Comparing `dl_myo-0.1.1/.github/workflows/python-publish.yml` & `dl_myo-0.1.2/.github/workflows/pypi.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries
 
 # This workflow uses actions that are not certified by GitHub.
 # They are provided by a third-party and are governed by
 # separate terms of service, privacy policy, and support
 # documentation.
 
-name: Upload Python Package
+name: pypi
 on:
   release:
     types: [published]
 permissions:
   contents: read
 jobs:
   deploy:
```

### Comparing `dl_myo-0.1.1/.github/workflows/release-package.yml` & `dl_myo-0.1.2/.github/workflows/docker.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-name: Release Package
+name: docker
 on:
   push:
     # Publish `main` as Docker `latest` image.
     branches:
       - main
-      - seed
     # Publish `v1.2.3` tags as releases.
     tags:
       - v*
-  # Run tests for any PRs.
-  pull_request:
 env:
   IMAGE_NAME: dl-myo
 jobs:
   # Push image to GitHub Packages.
   # See also https://docs.docker.com/docker-hub/builds/
   push:
     runs-on: ubuntu-latest
```

### Comparing `dl_myo-0.1.1/examples/sample.py` & `dl_myo-0.1.2/examples/sample.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,77 +4,87 @@
 import argparse
 import asyncio
 import logging
 
 from bleak import BleakClient
 from bleak.backends.characteristic import BleakGATTCharacteristic
 
-from myo import *
+import myo
 
 
 def callback(sender: BleakGATTCharacteristic, data: bytearray):
-    name = Handle(sender.handle).name  # pyright: ignore
-    if name == Handle.IMU_DATA.name:  # pyright: ignore
-        print(f"{name}: {IMUData(data).json()}")
+    name = myo.Handle(sender.handle).name
+    if name == myo.Handle.IMU_DATA.name:
+        print(f"{name}: {myo.IMUData(data).json()}")
     else:
-        print(f"{name}: {EMGData(data).json()}")
+        print(f"{name}: {myo.EMGData(data).json()}")
 
 
 async def main(args: argparse.Namespace):
     logging.info("starting scan...")
 
     if args.mac and len(args.mac) != 0:
-        m = await Device.with_mac(args.mac)
+        m = await myo.Device.with_mac(args.mac)
     else:
-        m = await Device.with_uuid()
+        m = await myo.Device.with_uuid()
 
     if m.device is None:
         return
 
     logging.info(f"{m.name}: {m.device.address}")
     async with BleakClient(m.device) as client:
         logging.info(f"connected to device {m.device.address}")
-        await m.set_sleep_mode(client, SleepMode.NORMAL)
+        await m.set_sleep_mode(client, myo.SleepMode.NORMAL)
         # led red
         await m.led(client, [255, 0, 0], [255, 0, 0])
-        await m.vibrate(client, VibrationType.SHORT)
+        await m.vibrate(client, myo.VibrationType.SHORT)
         logging.info("sleep 0.25")
         await asyncio.sleep(0.25)
         # led green
         await m.led(client, [0, 255, 0], [0, 255, 0])
-        await m.vibrate(client, VibrationType.SHORT)
+        await m.vibrate(client, myo.VibrationType.SHORT)
         logging.info("sleep 0.25")
         await asyncio.sleep(0.25)
         # led cyan
         await m.led(client, [0, 255, 255], [0, 255, 255])
 
-        await client.start_notify(Handle.EMG0_DATA.value, callback)  # pyright: ignore
-        await client.start_notify(Handle.EMG1_DATA.value, callback)  # pyright: ignore
-        await client.start_notify(Handle.EMG2_DATA.value, callback)  # pyright: ignore
-        await client.start_notify(Handle.EMG3_DATA.value, callback)  # pyright: ignore
-        await client.start_notify(Handle.IMU_DATA.value, callback)  # pyright: ignore
+        await client.start_notify(myo.Handle.EMG0_DATA.value, callback)
+        await client.start_notify(myo.Handle.EMG1_DATA.value, callback)
+        await client.start_notify(myo.Handle.EMG2_DATA.value, callback)
+        await client.start_notify(myo.Handle.EMG3_DATA.value, callback)
+        await client.start_notify(myo.Handle.IMU_DATA.value, callback)
 
-        await m.vibrate(client, VibrationType.MEDIUM)
+        await m.vibrate(client, myo.VibrationType.MEDIUM)
 
         # enable emg and imu
-        await m.set_mode(client, EMGMode.SEND_EMG, IMUMode.SEND_ALL, ClassifierMode.DISABLED)
+        await m.set_mode(
+            client,
+            myo.EMGMode.SEND_EMG,
+            myo.IMUMode.SEND_ALL,
+            myo.ClassifierMode.DISABLED,
+        )
 
         logging.info("sleep 1")
         await asyncio.sleep(0.5)
 
         # disable emg and imu
-        await m.set_mode(client, EMGMode.NONE, IMUMode.NONE, ClassifierMode.DISABLED)
+        await m.set_mode(
+            client,
+            myo.EMGMode.NONE,
+            myo.IMUMode.NONE,
+            myo.ClassifierMode.DISABLED,
+        )
 
         # get the available services on the myo device
         info = await m.get_services(client)
         logging.info(info)
 
         # led purple
         await m.led(client, [100, 100, 100], [100, 100, 100])
-        await m.vibrate(client, VibrationType.LONG)
+        await m.vibrate(client, myo.VibrationType.LONG)
 
     logging.info("bye bye!")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
```

### Comparing `dl_myo-0.1.1/examples/ws_client.py` & `dl_myo-0.1.2/examples/ws_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 #!/usr/bin/env python3
 """dl-myo example ws_client.py"""
 
 import argparse
 import asyncio
 import json
-import readline  # pyright: ignore
+import readline  # noqa: F401
 
 import websockets
 
 
 async def main():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="connect to the Myo band websocket server",
     )
-    parser.add_argument("--address", "-a", help="the host IP address for msgpack server", default="127.0.0.1")
-    parser.add_argument("--port", "-p", help="the port for msgpack listener", default=8765)
+    parser.add_argument(
+        "--address",
+        "-a",
+        help="the host IP address for msgpack server",
+        default="127.0.0.1",
+    )
+    parser.add_argument(
+        "--port", "-p", help="the port for msgpack listener", default=8765
+    )
 
     args = parser.parse_args()
 
     uri = f"ws://{args.address}:{args.port}"
-    async with websockets.connect(uri) as websocket:  # pyright: ignore
+    async with websockets.connect(uri) as websocket:
         while True:
             action = input("[start|warmup|quit]: ")
             if action == "quit":
                 break
             payload = json.dumps({"action": action})
 
             print(f"<<< {action}")
```

### Comparing `dl_myo-0.1.1/examples/ws_server.py` & `dl_myo-0.1.2/examples/ws_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,82 @@
 #!/usr/bin/env python3
 """dl-myo example ws_host.py"""
 
 import argparse
 import asyncio
+import json
 import logging
 
 from bleak import BleakClient
 from bleak.backends.characteristic import BleakGATTCharacteristic
 from websockets.server import serve
 
-from myo import *
+import myo
 
 CONNECTIONS = set()
 MS = None
 
 
 class MyoServer:
     def __init__(self, m):
         self.myo = m
         self.emg0 = None
         self.emg1 = None
         self.emg2 = None
         self.emg3 = None
 
     async def start(self, c):
-        await c.start_notify(Handle.EMG0_DATA.value, self.on_emg)  # pyright: ignore
-        await c.start_notify(Handle.EMG1_DATA.value, self.on_emg)  # pyright: ignore
-        await c.start_notify(Handle.EMG2_DATA.value, self.on_emg)  # pyright: ignore
-        await c.start_notify(Handle.EMG3_DATA.value, self.on_emg)  # pyright: ignore
+        await c.start_notify(myo.Handle.EMG0_DATA.value, self.on_emg)
+        await c.start_notify(myo.Handle.EMG1_DATA.value, self.on_emg)
+        await c.start_notify(myo.Handle.EMG2_DATA.value, self.on_emg)
+        await c.start_notify(myo.Handle.EMG3_DATA.value, self.on_emg)
 
-        await self.myo.vibrate(c, VibrationType.MEDIUM)
+        await self.myo.vibrate(c, myo.VibrationType.MEDIUM)
 
         # enable emg and imu
-        await self.myo.set_mode(c, EMGMode.SEND_EMG, IMUMode.SEND_ALL, ClassifierMode.DISABLED)
+        await self.myo.set_mode(
+            c,
+            myo.EMGMode.SEND_EMG,
+            myo.IMUMode.SEND_ALL,
+            myo.ClassifierMode.DISABLED,
+        )
         logging.info("EMG notify ON")
 
     async def stop(self, c):
-        await self.myo.set_mode(c, EMGMode.NONE, IMUMode.NONE, ClassifierMode.DISABLED)
+        await self.myo.set_mode(
+            c, myo.EMGMode.NONE, myo.IMUMode.NONE, myo.ClassifierMode.DISABLED
+        )
         logging.info("EMG notify OFF")
 
     async def warmup(self, c):
         logging.info("warming up")
-        await self.myo.set_sleep_mode(c, SleepMode.NORMAL)
+        await self.myo.set_sleep_mode(c, myo.SleepMode.NORMAL)
         # led red
         await self.myo.led(c, [255, 0, 0], [255, 0, 0])
-        await self.myo.vibrate(c, VibrationType.SHORT)
+        await self.myo.vibrate(c, myo.VibrationType.SHORT)
         logging.info("sleep 0.25")
         await asyncio.sleep(0.25)
         # led green
         await self.myo.led(c, [0, 255, 0], [0, 255, 0])
-        await self.myo.vibrate(c, VibrationType.SHORT)
+        await self.myo.vibrate(c, myo.VibrationType.SHORT)
         logging.info("sleep 0.25")
         await asyncio.sleep(0.25)
         # led cyan
         await self.myo.led(c, [0, 255, 255], [0, 255, 255])
 
     async def on_emg(self, sender: BleakGATTCharacteristic, data: bytearray):
-        name = Handle(sender.handle).name  # pyright: ignore
-        if name == Handle.EMG0_DATA.name:  # pyright: ignore
-            self.emg0 = EMGData(data).to_dict()
-        elif name == Handle.EMG1_DATA.name:  # pyright: ignore
-            self.emg1 = EMGData(data).to_dict()
-        elif name == Handle.EMG2_DATA.name:  # pyright: ignore
-            self.emg2 = EMGData(data).to_dict()
-        elif name == Handle.EMG3_DATA.name:  # pyright: ignore
-            self.emg3 = EMGData(data).to_dict()
+        name = myo.Handle(sender.handle).name
+        if name == myo.Handle.EMG0_DATA.name:
+            self.emg0 = myo.EMGData(data).to_dict()
+        elif name == myo.Handle.EMG1_DATA.name:
+            self.emg1 = myo.EMGData(data).to_dict()
+        elif name == myo.Handle.EMG2_DATA.name:
+            self.emg2 = myo.EMGData(data).to_dict()
+        elif name == myo.Handle.EMG3_DATA.name:
+            self.emg3 = myo.EMGData(data).to_dict()
         if self.emg0 and self.emg1 and self.emg2 and self.emg3:
             emg = json.dumps(
                 {
                     "emg0": self.emg0,
                     "emg1": self.emg1,
                     "emg2": self.emg2,
                     "emg3": self.emg3,
@@ -84,15 +92,15 @@
 
 
 async def register(websocket):
     global CONNECTIONS, MS
 
     if MS is None:
         logging.info("initializing Myo connection")
-        m = await Device.with_uuid()
+        m = await myo.Device.with_uuid()
         if m.device is None:
             return
         logging.info(f"found {m.name}: {m.device.address}")
         MS = MyoServer(m)
 
     async with BleakClient(MS.myo.device) as c:
         try:
@@ -128,22 +136,29 @@
 
 
 async def main():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="connect to a Myo band and stream via websockets",
     )
-    parser.add_argument("-a", "--address", help="the host IP address for msgpack server", default="127.0.0.1")
+    parser.add_argument(
+        "-a",
+        "--address",
+        help="the host IP address for msgpack server",
+        default="127.0.0.1",
+    )
     parser.add_argument(
         "-d",
         "--debug",
         action="store_true",
         help="sets the log level to debug",
     )
-    parser.add_argument("-p", "--port", help="the port for msgpack listener", default=8765)
+    parser.add_argument(
+        "-p", "--port", help="the port for msgpack listener", default=8765
+    )
 
     args = parser.parse_args()
 
     log_level = logging.DEBUG if args.debug else logging.INFO
     logging.basicConfig(
         level=log_level,
         format="%(asctime)-15s %(name)-8s %(levelname)s: %(message)s",
```

### Comparing `dl_myo-0.1.1/myo/commands.py` & `dl_myo-0.1.2/myo/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,21 @@
     def __init__(self, emg_mode, imu_mode, classifier_mode):
         self.emg_mode = emg_mode
         self.imu_mode = imu_mode
         self.classifier_mode = classifier_mode
 
     @property
     def payload(self) -> bytearray:
-        return bytearray((self.emg_mode.value, self.imu_mode.value, self.classifier_mode.value))
+        return bytearray(
+            (
+                self.emg_mode.value,
+                self.imu_mode.value,
+                self.classifier_mode.value,
+            )
+        )
 
 
 # -> myohw_command_vibrate
 class Vibrate(Command):
     cmd = 0x03
 
     def __init__(self, vibration_type):
```

### Comparing `dl_myo-0.1.1/myo/device.py` & `dl_myo-0.1.2/myo/device.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 import json
 import logging
 
 from bleak import BleakClient, BleakScanner
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 
-from .commands import Command, SetMode, Vibrate, DeepSleep, LED, Vibrate2, SetSleepMode, Unlock, UserAction
+from .commands import (
+    Command,
+    SetMode,
+    Vibrate,
+    DeepSleep,
+    LED,
+    Vibrate2,
+    SetSleepMode,
+    Unlock,
+    UserAction,
+)
 from .handle import Handle, UUID
 from .types import FirmwareInfo, FirmwareVersion
 
 # from .quaternion import Quaternion
 
 logger = logging.getLogger(__name__)
 
@@ -38,15 +48,17 @@
             if mac.lower() == device.address.lower():
                 return True
             return False
 
         self = cls()
         try:
             # scan the device
-            self.__device = await BleakScanner.find_device_by_filter(match_myo_mac, cb=dict(use_bdaddr=True))
+            self.__device = await BleakScanner.find_device_by_filter(
+                match_myo_mac, cb=dict(use_bdaddr=True)
+            )
             if self.device is None:
                 logger.error(f"could not find device with address {mac}")
                 return self
         except Exception as e:
             logger.error("the mac address may be invalid", e)
             return self
 
@@ -60,15 +72,17 @@
         def match_myo_uuid(_: BLEDevice, adv: AdvertisementData):
             if str(UUID.MYO_SERVICE).lower() in adv.service_uuids:
                 return True
             return False
 
         self = cls()
         # scan the device
-        self.__device = await BleakScanner.find_device_by_filter(match_myo_uuid, cb=dict(use_bdaddr=True))
+        self.__device = await BleakScanner.find_device_by_filter(
+            match_myo_uuid, cb=dict(use_bdaddr=True)
+        )
         if self.device is None:
             logger.error(f"could not find device with service UUID {UUID.MYO_SERVICE}")
             return self
 
         # get the device name
         self.__name = str(self.device.name)
 
@@ -81,69 +95,71 @@
         val = await client.read_gatt_char(Handle.BATTERY_LEVEL)
         return ord(val)
 
     async def command(self, client: BleakClient, cmd: Command):
         """
         Command Characteristic
         """
-        await client.write_gatt_char(Handle.COMMAND.value, cmd.data, True)  # pyright: ignore
+        await client.write_gatt_char(Handle.COMMAND.value, cmd.data, True)
 
     async def deep_sleep(self, client: BleakClient):
         """
         Deep Sleep Command
         """
         await self.command(client, DeepSleep())
 
     async def emg_service(self, client):
         """
         EMG Service
         """
-        await client.write_gatt_char(Handle.EMG_SERVICE.value, b"\x01\x00", True)  # pyright: ignore
+        await client.write_gatt_char(Handle.EMG_SERVICE.value, b"\x01\x00", True)
 
-    async def get_services(self, client: BleakClient, indent=2) -> str:  # noqa: C901
+    async def get_services(self, client: BleakClient, indent=2) -> str:
         """fetch available services as dict"""
         sd = {"services": {}}
         for service in client.services:  # BleakGATTServiceCollection
             try:
-                service_name = Handle(service.handle).name  # pyright: ignore
+                service_name = Handle(service.handle).name
             except Exception as e:
                 logger.debug("unknown handle: {}", e)
                 continue
 
             sd["services"][service.handle] = {
                 "name": service_name,
                 "uuid": service.uuid,
                 "chars": {},
             }
             for char in service.characteristics:  # List[BleakGATTCharacteristic]
                 try:
-                    char_name = Handle(char.handle).name  # pyright: ignore
+                    char_name = Handle(char.handle).name
                 except Exception as e:
                     logger.debug("unknown handle: {}", e)
                     continue
 
-                sd["services"][service.handle]["chars"][char.handle] = {
-                    "name": char_name,
-                    "uuid": char.uuid,
-                }
-
-                sd["services"][service.handle]["chars"][char.handle]["properties"] = ",".join(char.properties)
+                value = None
                 if "read" in char.properties:
                     blob = await client.read_gatt_char(char.handle)
-                    if char_name == Handle.MANUFACTURER_NAME_STRING.name:  # pyright: ignore
+                    if char_name == Handle.MANUFACTURER_NAME_STRING.name:
                         value = blob.decode("utf-8")
-                    elif char_name == Handle.FIRMWARE_INFO.name:  # pyright: ignore
+                    elif char_name == Handle.FIRMWARE_INFO.name:
                         value = FirmwareInfo(blob).to_dict()
-                    elif char_name == Handle.FIRMWARE_VERSION.name:  # pyright: ignore
+                    elif char_name == Handle.FIRMWARE_VERSION.name:
                         value = str(FirmwareVersion(blob))
-                    elif char_name == Handle.BATTERY_LEVEL.name:  # pyright: ignore
+                    elif char_name == Handle.BATTERY_LEVEL.name:
                         value = ord(blob)
                     else:
                         value = binascii.b2a_hex(blob).decode("utf-8")
-                    sd["services"][service.handle]["chars"][char.handle]["value"] = value
+
+                sd["services"][service.handle]["chars"][char.handle] = {
+                    "name": char_name,
+                    "uuid": char.uuid,
+                    "properties": ",".join(char.properties),
+                    "value": value,
+                }
+
             # end char
         # end service
 
         return json.dumps(sd, indent=indent)
 
     async def led(self, client: BleakClient, *args):
         """
```

### Comparing `dl_myo-0.1.1/myo/handle.py` & `dl_myo-0.1.2/myo/handle.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,66 +57,90 @@
 
 
 class UUID:
     MYO_SERVICE = "d5060001-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 12): Device Information
     DEVICE_INFORMATION = "0000180a-0000-1000-8000-00805f9b34fb"
-    #  [Characteristic] (Handle: 13): Manufacturer Name String (read), Value: bytearray(b'Thalmic Labs')
+    #  [Characteristic] (Handle: 13): Manufacturer Name String (read)
+    #                                 Value: bytearray(b'Thalmic Labs')
     MANUFACTURER_NAME_STRING = "00002a29-0000-1000-8000-00805f9b34fb"
 
     # [Service] (Handle: 15): Battery Service
     BATTERY_SERVICE = "0000180f-0000-1000-8000-00805f9b34fb"
-    #  [Characteristic] (Handle: 16): Battery Level (read,notify), Value: bytearray(b'[')
-    #   [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 18): Client Characteristic Configuration, Value: bytearray(b'')
+    #  [Characteristic] (Handle: 16): Battery Level (read,notify)
+    #                                 Value: bytearray(b'[')
+    #   [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                (Handle: 18): Client Characteristic Configuration
+    #                              Value: bytearray(b'')
     BATTERY_LEVEL = "00002a19-0000-1000-8000-00805f9b34fb"
 
     # [Service] (Handle: 19): Control Service
     CONTROL_SERVICE = "d5060001-a904-deb9-4748-2c7f4a124842"
-    #  [Characteristic] (Handle: 20): Firmware Info (read), Value: bytearray(b'\x8e2\x94\x85;\xd2\x05\x00\x00\x00\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00')
+    #  [Characteristic] (Handle: 20): Firmware Info (read)
+    #                                 Value: bytearray
     FIRMWARE_INFO = "d5060101-a904-deb9-4748-2c7f4a124842"
-    #  [Characteristic] (Handle: 22): Firmware Version (read), Value: bytearray(b'\x01\x00\x05\x00\xb2\x07\x02\x00')
+    #  [Characteristic] (Handle: 22): Firmware Version (read)
+    #                                 Value: bytearray
     FIRMWARE_VERSION = "d5060201-a904-deb9-4748-2c7f4a124842"
     #  [Characteristic] (Handle: 24): Command (write)
     COMMAND = "d5060401-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 26): IMU Service
     IMU_SERVICE = "d5060002-a904-deb9-4748-2c7f4a124842"
     #  [Characteristic] (Handle: 27): IMU Data (notify)
-    #    [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 29): Client Characteristic Configuration, Value: bytearray(b'')
+    #    [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                 (Handle: 29): Client Characteristic Configuration
+    #                               Value: bytearray(b'')
     IMU_DATA = "d5060402-a904-deb9-4748-2c7f4a124842"
     #  [Characteristic] (Handle: 30): Motion Event (indicate)
-    #    [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 32): Client Characteristic Configuration, Value: bytearray(b'')
+    #    [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                 (Handle: 32): Client Characteristic Configuration
+    #                               Value: bytearray(b'')
     MOTION_EVENT = "d5060502-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 33): Classifier Service
     CLASSIFIER_SERVICE = "d5060003-a904-deb9-4748-2c7f4a124842"
     #  [Characteristic] (Handle: 34): Classifier Event (indicate)
-    #    [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 36): Client Characteristic Configuration, Value: bytearray(b'')
+    #    [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                 (Handle: 36): Client Characteristic Configuration
+    #                               Value: bytearray(b'')
     CLASSIFIER_EVENT = "d5060103-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 37): FV Service
     FV_SERVICE = "d5060004-a904-deb9-4748-2c7f4a124842"
     #   [Characteristic] (Handle: 38): FV Data (notify)
-    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 40): Client Characteristic Configuration, Value: bytearray(b'')
+    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                  (Handle: 40): Client Characteristic Configuration
+    #                                Value: bytearray(b'')
     FV_DATA = "d5060104-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 41): EMG Service
     EMG_SERVICE = "d5060005-a904-deb9-4748-2c7f4a124842"
     #   [Characteristic] (Handle: 42): EMG0 Data (notify)
-    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 44): Client Characteristic Configuration, Value: bytearray(b'')
+    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                  (Handle: 44): Client Characteristic Configuration
+    #                                Value: bytearray(b'')
     EMG0_DATA = "d5060105-a904-deb9-4748-2c7f4a124842"
     #   [Characteristic] (Handle: 45): EMG1 Data (notify)
-    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 47): Client Characteristic Configuration, Value: bytearray(b'')
+    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                  (Handle: 47): Client Characteristic Configuration
+    #                                Value: bytearray(b'')
     EMG1_DATA = "d5060205-a904-deb9-4748-2c7f4a124842"
     #   [Characteristic] (Handle: 48): EMG2 Data (notify)
-    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 50): Client Characteristic Configuration, Value: bytearray(b'')
+    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                  (Handle: 50): Client Characteristic Configuration
+    #                                Value: bytearray(b'')
     EMG2_DATA = "d5060305-a904-deb9-4748-2c7f4a124842"
     #   [Characteristic] (Handle: 51): EMG3 Data (notify)
-    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 53): Client Characteristic Configuration, Value: bytearray(b'')
+    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                  (Handle: 53): Client Characteristic Configuration
+    #                                Value: bytearray(b'')
     EMG3_DATA = "d5060405-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 54): Unknown Service
     UNKNOWN_SERVICE = "d5060006-a904-deb9-4748-2c7f4a124842"
     #   [Characteristic] (Handle: 55): Unknown Characteristic (indicate)
-    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb (Handle: 57): Client Characteristic Configuration, Value: bytearray(b'')
+    #     [Descriptor] 00002902-0000-1000-8000-00805f9b34fb
+    #                  (Handle: 57): Client Characteristic Configuration
+    #                                Value: bytearray(b'')
     UNKNOWN_CHAR = "d5060602-a904-deb9-4748-2c7f4a124842"
```

### Comparing `dl_myo-0.1.1/myo/types.py` & `dl_myo-0.1.2/myo/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,20 +90,20 @@
     def __init__(self, data):
         u = struct.unpack("6BH12B", data)  # 20 bytes
         assert len(u) == 19
         ser = list(u[:6])
         ser.reverse()
         ser = [hex(i)[-2:] for i in ser]
         self._serial_number = ":".join(ser).upper()
-        self._unlock_pose = Pose(u[6]).name  # pyright: ignore
-        self._active_classifier_type = ClassifierModelType(u[7]).name  # pyright: ignore
+        self._unlock_pose = Pose(u[6]).name
+        self._active_classifier_type = ClassifierModelType(u[7]).name
         self._active_classifier_index = u[8]
         self._has_custom_classifier = bool(u[9])
         self._stream_indicating = bool(u[10])
-        self._sku = SKU(u[11]).name  # pyright: ignore
+        self._sku = SKU(u[11]).name
         self._reserved = u[12:]
 
     def to_dict(self):
         return {
             "serial_number": self._serial_number,
             "unlock_pose": self._has_custom_classifier,
             "active_classifier_type": self._active_classifier_type,
@@ -120,15 +120,15 @@
         u = struct.unpack("4H", data)  # 4x uint16_t
         self._major = u[0]
         self._minor = u[1]
         self._patch = u[2]
         self._hardware_rev = HardwareRev(u[3])
 
     def __str__(self):
-        return f"{self._major}.{self._minor}.{self._patch}.{self._hardware_rev.name}"  # pyright: ignore
+        return f"{self._major}.{self._minor}.{self._patch}.{self._hardware_rev.name}"
 
 
 # -> myohw_hardware_rev_t
 class HardwareRev(aenum.Enum):
     UNKNOWN = 0
     REVC = 1
     REVD = 2
```

### Comparing `dl_myo-0.1.1/.gitignore` & `dl_myo-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.1/LICENSE` & `dl_myo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.1/README.md` & `dl_myo-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # dl-myo (Dongle-less Myo)
 
-[![Build Status](https://github.com/iomz/dl-myo/workflows/Build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3ABuild)
-[![Release Package](https://github.com/iomz/dl-myo/actions/workflows/release-package.yml/badge.svg)](https://github.com/iomz/dl-myo/actions/workflows/release-package.yml)
+[![Build Status](https://github.com/iomz/dl-myo/workflows/build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3Abuild)
 [![Image Size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=Image%20Size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
-[![PyPI Version](https://badge.fury.io/py/dl-myo.svg)](https://badge.fury.io/py/dl-myo)
+[![Python Versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![PyPI Version](https://img.shields.io/pypi/v/dl-myo.svg)](https://pypi.python.org/pypi/del-myo)
+[![License](https://img.shields.io/pypi/l/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
 
 dl-myo is a replacement to MyoConnect for Myo Armband without an official Myo dongle.
 
 If you are fed up with the dongle and still need to use Myo anyway this is the right stuff to grab.
 
 This project is a reimplementation of [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91](https://github.com/mamo91) and enhanced by [@MyrikLD](https://github.com/MyrikLD)) using [Bleak](https://github.com/hbldh/bleak) instead of [bluepy](https://github.com/IanHarvey/bluepy), and therefore supports asyncio on multiple platforms.
```

### Comparing `dl_myo-0.1.1/PKG-INFO` & `dl_myo-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-myo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A replacement middleware to MyoConnect for Myo Armband
 Project-URL: Homepage, https://github.com/iomz/dl-myo
 Project-URL: Bug Tracker, https://github.com/iomz/dl-myo/issues
 Author-email: Iori Mizutani <iori.mizutani@gmail.com>
 Maintainer-email: Iori Mizutani <iori.mizutani@gmail.com>
 License-File: LICENSE
 Classifier: Framework :: AsyncIO
@@ -17,18 +17,19 @@
 Requires-Python: >=3.11
 Requires-Dist: aenum
 Requires-Dist: bleak
 Description-Content-Type: text/markdown
 
 # dl-myo (Dongle-less Myo)
 
-[![Build Status](https://github.com/iomz/dl-myo/workflows/Build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3ABuild)
-[![Release Package](https://github.com/iomz/dl-myo/actions/workflows/release-package.yml/badge.svg)](https://github.com/iomz/dl-myo/actions/workflows/release-package.yml)
+[![Build Status](https://github.com/iomz/dl-myo/workflows/build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3Abuild)
 [![Image Size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=Image%20Size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
-[![PyPI Version](https://badge.fury.io/py/dl-myo.svg)](https://badge.fury.io/py/dl-myo)
+[![Python Versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![PyPI Version](https://img.shields.io/pypi/v/dl-myo.svg)](https://pypi.python.org/pypi/del-myo)
+[![License](https://img.shields.io/pypi/l/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
 
 dl-myo is a replacement to MyoConnect for Myo Armband without an official Myo dongle.
 
 If you are fed up with the dongle and still need to use Myo anyway this is the right stuff to grab.
 
 This project is a reimplementation of [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91](https://github.com/mamo91) and enhanced by [@MyrikLD](https://github.com/MyrikLD)) using [Bleak](https://github.com/hbldh/bleak) instead of [bluepy](https://github.com/IanHarvey/bluepy), and therefore supports asyncio on multiple platforms.
```

