# Comparing `tmp/micropython-i2c-lcd-0.1.0.tar.gz` & `tmp/micropython-i2c-lcd-0.1.1.tar.gz`

## Comparing `micropython-i2c-lcd-0.1.0.tar` & `micropython-i2c-lcd-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-10 13:38:39.000000 micropython-i2c-lcd-0.1.0/lcd_i2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-10 13:38:39.000000 micropython-i2c-lcd-0.1.0/lcd_i2c/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-03-10 13:38:39.000000 micropython-i2c-lcd-0.1.0/lcd_i2c/lcd_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-10 13:38:39.000000 micropython-i2c-lcd-0.1.0/lcd_i2c/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-10 13:38:47.000000 micropython-i2c-lcd-0.1.0/lcd_i2c/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-03-10 13:38:47.000000 micropython-i2c-lcd-0.1.0/micropython_i2c_lcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 19:08:23.000000 micropython-i2c-lcd-0.1.1/lcd_i2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-12 19:08:23.000000 micropython-i2c-lcd-0.1.1/lcd_i2c/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-06-12 19:08:23.000000 micropython-i2c-lcd-0.1.1/lcd_i2c/lcd_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-12 19:08:23.000000 micropython-i2c-lcd-0.1.1/lcd_i2c/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 19:08:34.000000 micropython-i2c-lcd-0.1.1/lcd_i2c/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-12 19:08:36.000000 micropython-i2c-lcd-0.1.1/micropython_i2c_lcd.egg-info/PKG-INFO
```

### Comparing `micropython-i2c-lcd-0.1.0/lcd_i2c/const.py` & `micropython-i2c-lcd-0.1.1/lcd_i2c/const.py`

 * *Files identical despite different names*

### Comparing `micropython-i2c-lcd-0.1.0/lcd_i2c/lcd_i2c.py` & `micropython-i2c-lcd-0.1.1/lcd_i2c/lcd_i2c.py`

 * *Files identical despite different names*

### Comparing `micropython-i2c-lcd-0.1.0/lcd_i2c/typing.py` & `micropython-i2c-lcd-0.1.1/lcd_i2c/typing.py`

 * *Files identical despite different names*

### Comparing `micropython-i2c-lcd-0.1.0/micropython_i2c_lcd.egg-info/PKG-INFO` & `micropython-i2c-lcd-0.1.1/micropython_i2c_lcd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: micropython-i2c-lcd
-Version: 0.1.0
-Summary: Micropython package to control HD44780 LCD displays 1602 and 2004 
+Version: 0.1.1
+Summary: MicroPython package to control HD44780 LCD displays 1602 and 2004
 Home-page: https://github.com/brainelectronics/micropython-i2c-lcd
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-i2c-lcd/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-i2c-lcd
-Keywords: micropython,HD44780,I2C,display,LCD1602,LCD2004
+Keywords: micropython,HD44780,I2C,display,LCD1602,LCD2004,PCF8574
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # MicroPython I2C LCD
 
 [![Downloads](https://pepy.tech/badge/micropython-i2c-lcd)](https://pepy.tech/project/micropython-i2c-lcd)
 ![Release](https://img.shields.io/github/v/release/brainelectronics/micropython-i2c-lcd?include_prereleases&color=success)
 ![MicroPython](https://img.shields.io/badge/micropython-Ok-green.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![codecov](https://codecov.io/github/brainelectronics/micropython-i2c-lcd/branch/main/graph/badge.svg)](https://app.codecov.io/github/brainelectronics/micropython-i2c-lcd)
 [![CI](https://github.com/brainelectronics/micropython-i2c-lcd/actions/workflows/release.yml/badge.svg)](https://github.com/brainelectronics/micropython-i2c-lcd/actions/workflows/release.yml)
 
-Micropython package to control HD44780 LCD displays 1602 and 2004 via I2C
+MicroPython package to control HD44780 LCD displays 1602 and 2004 via I2C
 
 ---------------
 
 ## General
 
-Micropython package to control HD44780 LCD displays 1602 and 2004 via I2C
+MicroPython package to control HD44780 LCD displays 1602 and 2004 via I2C
 
 📚 The latest documentation is available at
 [MicroPython I2C LCD ReadTheDocs][ref-rtd-micropython-i2c-lcd] 📚
 
 <!-- MarkdownTOC -->
 
 - [Installation](#installation)
@@ -79,14 +80,15 @@
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
@@ -172,21 +174,22 @@
 
 ## Usage
 
 ```python
 from lcd_i2c import LCD
 from machine import I2C, Pin
 
-I2C_ADDR = 0x27
+# PCF8574 on 0x50
+I2C_ADDR = 0x27     # DEC 39, HEX 0x27
 NUM_ROWS = 2
 NUM_COLS = 16
 
 # define custom I2C interface, default is 'I2C(0)'
 # check the docs of your device for further details and pin infos
-i2c = I2C(1, scl=Pin(3), sda=Pin(2), freq=800_000)
+i2c = I2C(0, scl=Pin(13), sda=Pin(12), freq=800000)
 lcd = LCD(addr=I2C_ADDR, cols=NUM_COLS, rows=NUM_ROWS, i2c=i2c)
 
 lcd.begin()
 lcd.print("Hello World")
 ```
 
 For further examples check the `examples` folder or the Example chapter in the
```

