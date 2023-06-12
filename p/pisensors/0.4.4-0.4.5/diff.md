# Comparing `tmp/pisensors-0.4.4.tar.gz` & `tmp/pisensors-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisensors-0.4.4.tar", last modified: Thu Jun  8 18:23:26 2023, max compression
+gzip compressed data, was "pisensors-0.4.5.tar", last modified: Mon Jun 12 12:24:54 2023, max compression
```

## Comparing `pisensors-0.4.4.tar` & `pisensors-0.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:26.473185 pisensors-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-08 18:23:26.473185 pisensors-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 18:23:16.000000 pisensors-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:26.469185 pisensors-0.4.4/pisensors/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:26.473185 pisensors-0.4.4/pisensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:23:26.473185 pisensors-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-08 18:23:16.000000 pisensors-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:24:54.968290 pisensors-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-12 12:24:54.968290 pisensors-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 12:24:44.000000 pisensors-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:24:54.964290 pisensors-0.4.5/pisensors/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 12:24:44.000000 pisensors-0.4.5/pisensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-12 12:24:44.000000 pisensors-0.4.5/pisensors/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 12:24:44.000000 pisensors-0.4.5/pisensors/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-12 12:24:44.000000 pisensors-0.4.5/pisensors/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:24:54.968290 pisensors-0.4.5/pisensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-12 12:24:54.000000 pisensors-0.4.5/pisensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 12:24:54.000000 pisensors-0.4.5/pisensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:24:54.000000 pisensors-0.4.5/pisensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 12:24:54.000000 pisensors-0.4.5/pisensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 12:24:54.000000 pisensors-0.4.5/pisensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:24:54.968290 pisensors-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-12 12:24:44.000000 pisensors-0.4.5/setup.py
```

### Comparing `pisensors-0.4.4/PKG-INFO` & `pisensors-0.4.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.4
+Version: 0.4.5
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.4/pisensors/sensors.py` & `pisensors-0.4.5/pisensors/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
         self.config = Config(package_name=self.class_name(),
                              template_path=template_config_path,
                              config_file_name="config.yml",
-                             dry_run=True,
+                             dry_run=dry_run,
                              dry_run_abs_path=dry_run_abs_path)
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
         self.conn.open_conn(self.config['influxdbconn'])
 
     @classmethod
@@ -41,17 +41,19 @@
         Read sensors information
         """
         have_readings = False
 
         try:
             import adafruit_dht  # pylint: disable=import-outside-toplevel
 
+            self.logger.debug("Initializing DHT22 sensor...")
             dht_sensor = adafruit_dht.DHT22(self.config["pin"])
             humidity = dht_sensor.humidity
             temp_c = dht_sensor.temperature
+            dht_sensor.exit()
             have_readings = True
         except (ModuleNotFoundError, NameError):
             self.logger.warning("No adafruit supported: returning default values.")
             humidity = 50
             temp_c = 25
             have_readings = True
         except RuntimeError as ex:
@@ -68,8 +70,7 @@
                 self.conn.insert("DHT22", points)
 
                 self.logger.info("Temp: %s | Humid: %s", temp_c, humidity)
 
             except RuntimeError as ex:
                 self.logger.error("RuntimeError: %s", ex)
                 self.logger.error("influxDB conn = %s", self.config['influxdbconn'])
-
```

### Comparing `pisensors-0.4.4/pisensors.egg-info/PKG-INFO` & `pisensors-0.4.5/pisensors.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.4
+Version: 0.4.5
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.4/setup.py` & `pisensors-0.4.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pisensors",
-    version="0.4.4",
+    version="0.4.5",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Sensors script for Temperature & Humidity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/pisensors",
     packages=setuptools.find_packages(),
```

