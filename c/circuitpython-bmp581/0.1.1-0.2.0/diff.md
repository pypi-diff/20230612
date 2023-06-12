# Comparing `tmp/circuitpython-bmp581-0.1.1.tar.gz` & `tmp/circuitpython-bmp581-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bmp581-0.1.1.tar", last modified: Sun May  7 18:29:21 2023, max compression
+gzip compressed data, was "circuitpython-bmp581-0.2.0.tar", last modified: Mon Jun 12 01:27:52 2023, max compression
```

## Comparing `circuitpython-bmp581-0.1.1.tar` & `circuitpython-bmp581-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.750778 circuitpython-bmp581-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/bmp581.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_pressure_oversample_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_temperature_oversample_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:27:52.303500 circuitpython-bmp581-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:27:52.295500 circuitpython-bmp581-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:27:52.299500 circuitpython-bmp581-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-12 01:27:52.299500 circuitpython-bmp581-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/bmp581.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:27:52.299500 circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-12 01:27:52.000000 circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-12 01:27:52.000000 circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:27:52.000000 circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 01:27:52.000000 circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 01:27:52.000000 circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:27:52.299500 circuitpython-bmp581-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:27:52.299500 circuitpython-bmp581-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:27:52.299500 circuitpython-bmp581-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/examples/bmp581_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/examples/bmp581_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/examples/bmp581_pressure_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/examples/bmp581_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/examples/bmp581_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/examples/bmp581_temperature_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 01:27:44.000000 circuitpython-bmp581-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-12 01:27:35.000000 circuitpython-bmp581-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 01:27:52.303500 circuitpython-bmp581-0.2.0/setup.cfg
```

### Comparing `circuitpython-bmp581-0.1.1/.github/workflows/build.yml` & `circuitpython-bmp581-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/.github/workflows/release_gh.yml` & `circuitpython-bmp581-0.2.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/.gitignore` & `circuitpython-bmp581-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/.pre-commit-config.yaml` & `circuitpython-bmp581-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/.pylintrc` & `circuitpython-bmp581-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/LICENSE` & `circuitpython-bmp581-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/PKG-INFO` & `circuitpython-bmp581-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp581
-Version: 0.1.1
+Version: 0.2.0
 Summary: CircuitPython Driver for the Bosch BMP581 pressure sensor
-Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
+Author-email: JDM <jdm@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMP581
 Keywords: sensor,blinka,circuitpython,micropython,bmp581,pressure,temperature,bosch,sensor,BMP581
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
```

### Comparing `circuitpython-bmp581-0.1.1/README.rst` & `circuitpython-bmp581-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/bmp581.py` & `circuitpython-bmp581-0.2.0/bmp581.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from adafruit_register.i2c_bits import RWBits, ROBits
 
 try:
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMP581.git"
 
 _REG_WHOAMI = const(0x01)
 _OSR_CONF = const(0x36)
 _ODR_CONFIG = const(0x37)
 
 
@@ -96,25 +96,28 @@
 
     _device_id = ROUnaryStruct(_REG_WHOAMI, "B")
 
     _power_mode = RWBits(2, _ODR_CONFIG, 0)
     _temperature_oversample_rate = RWBits(3, _OSR_CONF, 0)
     _pressure_oversample_rate = RWBits(3, _OSR_CONF, 3)
     _output_data_rate = RWBits(5, _ODR_CONFIG, 2)
+    _pressure_enabled = RWBits(1, _OSR_CONF, 6)
 
     _temperature = ROBits(24, 0x1D, 0, 3)
     _pressure = ROBits(24, 0x20, 0, 3)
 
     def __init__(self, i2c_bus: I2C, address: int = 0x47) -> None:
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
 
         if self._device_id != 0x50:
             raise RuntimeError("Failed to find BMP581")
 
         self._power_mode = NORMAL
+        self._pressure_enabled = True
+        self.sea_level_pressure = 101.325
 
     @property
     def power_mode(self) -> str:
         """
         Sensor power_mode
 
         +-----------------------------+------------------+
@@ -250,25 +253,44 @@
     def temperature(self) -> float:
         """
         The temperature sensor in C
         :return: Temperature
         """
         raw_temp = self._temperature
 
-        return self._twos_comp(raw_temp, 24) / 2**16
+        return self._twos_comp(raw_temp, 24) / 2**16.0
 
     @property
     def pressure(self) -> float:
         """
         The sensor pressure in kPa
         :return: Pressure in kPa
         """
         raw_pressure = self._pressure
 
         return self._twos_comp(raw_pressure, 24) / 2**6 / 1000
 
+    @property
+    def altitude(self):
+        """
+        With the measured pressure p and the pressure at sea level p0 e.g. 1013.25hPa,
+        the altitude in meters can be calculated with the international barometric formula
+
+        With the measured pressure p and the absolute altitude the pressure at sea level
+        can be calculated too. See the altitude setter for this calculation
+        """
+
+        altitude = 44330.0 * (
+            1.0 - ((self.pressure / self.sea_level_pressure) ** 0.190284)
+        )
+        return round(altitude, 1)
+
+    @altitude.setter
+    def altitude(self, value: float) -> None:
+        self.sea_level_pressure = self.pressure / (1.0 - value / 44330.0) ** 5.255
+
     @staticmethod
     def _twos_comp(val: int, bits: int) -> int:
 
         if val & (1 << (bits - 1)) != 0:
             return val - (1 << bits)
         return val
```

### Comparing `circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/PKG-INFO` & `circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp581
-Version: 0.1.1
+Version: 0.2.0
 Summary: CircuitPython Driver for the Bosch BMP581 pressure sensor
-Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
+Author-email: JDM <jdm@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMP581
 Keywords: sensor,blinka,circuitpython,micropython,bmp581,pressure,temperature,bosch,sensor,BMP581
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
```

### Comparing `circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/SOURCES.txt` & `circuitpython-bmp581-0.2.0/circuitpython_bmp581.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/docs/_static/Logo.png` & `circuitpython-bmp581-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/docs/_static/favicon.ico` & `circuitpython-bmp581-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/docs/conf.py` & `circuitpython-bmp581-0.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 autodoc_mock_imports = ["digitalio", "busio", "adafruit_register"]
 autoclass_content = "both"
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 # General information about the project.
-project = "CircuitPython bmp581 Library"
+project = "CircuitPython BMP581 Library"
 creation_year = "2023"
 current_year = str(datetime.datetime.now().year)
 year_duration = (
     current_year
     if current_year == creation_year
     else creation_year + " - " + current_year
 )
```

### Comparing `circuitpython-bmp581-0.1.1/docs/examples.rst` & `circuitpython-bmp581-0.2.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/examples/bmp581_output_data_rate.py` & `circuitpython-bmp581-0.2.0/examples/bmp581_output_data_rate.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/examples/bmp581_power_mode.py` & `circuitpython-bmp581-0.2.0/examples/bmp581_power_mode.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/examples/bmp581_pressure_oversample_rate.py` & `circuitpython-bmp581-0.2.0/examples/bmp581_pressure_oversample_rate.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/examples/bmp581_temperature_oversample_rate.py` & `circuitpython-bmp581-0.2.0/examples/bmp581_temperature_oversample_rate.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.1/pyproject.toml` & `circuitpython-bmp581-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bmp581"
 description = "CircuitPython Driver for the Bosch BMP581 pressure sensor"
-version = "0.1.1"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
-    {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
+    {name = "JDM", email = "jdm@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMP581"}
 keywords = [
     "sensor",
     "blinka",
     "circuitpython",
     "micropython",
```

