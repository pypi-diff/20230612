# Comparing `tmp/micropython-eeprom-0.1.0.tar.gz` & `tmp/micropython-eeprom-0.1.1.tar.gz`

## Comparing `micropython-eeprom-0.1.0.tar` & `micropython-eeprom-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-29 11:33:48.000000 micropython-eeprom-0.1.0/eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-03-29 11:33:48.000000 micropython-eeprom-0.1.0/eeprom/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-29 11:33:58.000000 micropython-eeprom-0.1.0/eeprom/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-03-29 11:33:59.000000 micropython-eeprom-0.1.0/micropython_eeprom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 18:13:32.000000 micropython-eeprom-0.1.1/eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-06-12 18:13:32.000000 micropython-eeprom-0.1.1/eeprom/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 18:13:40.000000 micropython-eeprom-0.1.1/eeprom/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-12 18:13:41.000000 micropython-eeprom-0.1.1/micropython_eeprom.egg-info/PKG-INFO
```

### Comparing `micropython-eeprom-0.1.0/eeprom/eeprom.py` & `micropython-eeprom-0.1.1/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `micropython-eeprom-0.1.0/micropython_eeprom.egg-info/PKG-INFO` & `micropython-eeprom-0.1.1/micropython_eeprom.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-eeprom
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython driver for AT24Cxx EEPROM
 Home-page: https://github.com/brainelectronics/micropython-eeprom
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-eeprom/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-eeprom
@@ -22,39 +22,39 @@
 [![Downloads](https://pepy.tech/badge/micropython-eeprom)](https://pepy.tech/project/micropython-eeprom)
 ![Release](https://img.shields.io/github/v/release/brainelectronics/micropython-eeprom?include_prereleases&color=success)
 ![MicroPython](https://img.shields.io/badge/micropython-Ok-green.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![codecov](https://codecov.io/github/brainelectronics/micropython-eeprom/branch/main/graph/badge.svg)](https://app.codecov.io/github/brainelectronics/micropython-eeprom)
 [![CI](https://github.com/brainelectronics/micropython-eeprom/actions/workflows/release.yml/badge.svg)](https://github.com/brainelectronics/micropython-eeprom/actions/workflows/release.yml)
 
-MicroPython driveer for AT24Cxx EEPROM
+MicroPython driver for AT24Cxx EEPROM
 
 ---------------
 
 ## General
 
-MicroPython driveer for AT24Cxx EEPROM
+MicroPython driver for AT24Cxx EEPROM
 
 📚 The latest documentation is available at
 [MicroPython EEPROM ReadTheDocs][ref-rtd-micropython-eeprom] 📚
 
 <!-- MarkdownTOC -->
 
 - [Installation](#installation)
-	- [Install required tools](#install-required-tools)
+    - [Install required tools](#install-required-tools)
 - [Setup](#setup)
-	- [Install package with upip](#install-package-with-upip)
-		- [General](#general)
-		- [Specific version](#specific-version)
-		- [Test version](#test-version)
-	- [Manually](#manually)
-		- [Upload files to board](#upload-files-to-board)
+    - [Install package with upip](#install-package-with-upip)
+        - [General](#general)
+        - [Specific version](#specific-version)
+        - [Test version](#test-version)
+    - [Manually](#manually)
+        - [Upload files to board](#upload-files-to-board)
 - [Usage](#usage)
 - [Contributing](#contributing)
-	- [Unittests](#unittests)
+    - [Unittests](#unittests)
 - [Credits](#credits)
 
 <!-- /MarkdownTOC -->
 
 ## Installation
 
 ### Install required tools
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
@@ -178,16 +179,16 @@
 
 ## Usage
 
 ```python
 from eeprom import EEPROM
 from machine import I2C, Pin
 
-I2C_ADDR = 0x50
-EEPROM_SIZE = 32	# AT24C32 on 0x50
+I2C_ADDR = 0x50     # DEC 80, HEX 0x50
+EEPROM_SIZE = 32    # AT24C32 on 0x50
 
 # define custom I2C interface, default is 'I2C(0)'
 # check the docs of your device for further details and pin infos
 i2c = I2C(0, scl=Pin(13), sda=Pin(12), freq=800000)
 eeprom = EEPROM(addr=I2C_ADDR, at24x=EEPROM_SIZE, i2c=i2c)
 
 # write 'micropython' to address 10
```

