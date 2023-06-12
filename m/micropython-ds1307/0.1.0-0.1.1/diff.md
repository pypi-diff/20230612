# Comparing `tmp/micropython-ds1307-0.1.0.tar.gz` & `tmp/micropython-ds1307-0.1.1.tar.gz`

## Comparing `micropython-ds1307-0.1.0.tar` & `micropython-ds1307-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 16:54:10.000000 micropython-ds1307-0.1.0/ds1307/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-05 16:54:10.000000 micropython-ds1307-0.1.0/ds1307/ds1307.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 16:54:17.000000 micropython-ds1307-0.1.0/ds1307/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-05 16:54:18.000000 micropython-ds1307-0.1.0/micropython_ds1307.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 18:42:21.000000 micropython-ds1307-0.1.1/ds1307/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-12 18:42:21.000000 micropython-ds1307-0.1.1/ds1307/ds1307.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 18:42:30.000000 micropython-ds1307-0.1.1/ds1307/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-12 18:42:32.000000 micropython-ds1307-0.1.1/micropython_ds1307.egg-info/PKG-INFO
```

### Comparing `micropython-ds1307-0.1.0/ds1307/ds1307.py` & `micropython-ds1307-0.1.1/ds1307/ds1307.py`

 * *Files identical despite different names*

### Comparing `micropython-ds1307-0.1.0/micropython_ds1307.egg-info/PKG-INFO` & `micropython-ds1307-0.1.1/micropython_ds1307.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: micropython-ds1307
-Version: 0.1.0
-Summary:  MicroPython driver for DS1307 RTC 
+Version: 0.1.1
+Summary: MicroPython driver for DS1307 RTC
 Home-page: https://github.com/brainelectronics/micropython-ds1307
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-ds1307/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-ds1307
 Keywords: micropython,i2c,ds1307,driver
@@ -82,14 +82,15 @@
 ### Install package with upip
 
 Connect the MicroPython device to a network (if possible)
 
 ```python
 import network
 station = network.WLAN(network.STA_IF)
+station.active(True)
 station.connect('SSID', 'PASSWORD')
 station.isconnected()
 ```
 
 #### General
 
 Install the latest package version of this lib on the MicroPython device
@@ -175,25 +176,26 @@
 cp examples/main.py /pyboard
 cp examples/boot.py /pyboard
 ```
 
 ## Usage
 
 ```python
-from eeprom import DS1307
+from ds1307 import DS1307
 from machine import I2C, Pin
-from time import gmtime
+from time import gmtime, time
 
-I2C_ADDR = 0x68
+# DS1307 on 0x68
+I2C_ADDR = 0x68     # DEC 104, HEX 0x68
 
 # define custom I2C interface, default is 'I2C(0)'
 # check the docs of your device for further details and pin infos
 # this are the pins for the Raspberry Pi Pico adapter board
 i2c = I2C(0, scl=Pin(13), sda=Pin(12), freq=800000)
-ds1307 = DS1307(addr=I2C_ADDR, i2c=i2c)   # DS1307 on 0x68
+ds1307 = DS1307(addr=I2C_ADDR, i2c=i2c)
 
 # get the current RTC time
 print("Current RTC time: {}".format(ds1307.datetime))
 
 # set the RTC time to the current system time
 now = gmtime(time())
 ds1307.datetime = now
```

