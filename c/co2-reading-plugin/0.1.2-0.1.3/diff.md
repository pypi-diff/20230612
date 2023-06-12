# Comparing `tmp/co2_reading_plugin-0.1.2-py3-none-any.whl.zip` & `tmp/co2_reading_plugin-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6245 bytes, number of entries: 11
--rw-r--r--  2.0 unx     6467 b- defN 23-Apr-08 23:56 co2_reading_plugin/__init__.py
+Zip file size: 6247 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     6472 b- defN 23-Jun-12 16:46 co2_reading_plugin/__init__.py
 -rw-r--r--  2.0 unx      177 b- defN 23-Feb-02 18:01 co2_reading_plugin/additional_config.ini
 -rw-r--r--  2.0 unx      211 b- defN 22-Oct-11 18:10 co2_reading_plugin/additional_sql.sql
 -rw-r--r--  2.0 unx      270 b- defN 23-Feb-02 18:01 co2_reading_plugin/ui/contrib/charts/co2_readings.yaml
 -rw-r--r--  2.0 unx      471 b- defN 23-Feb-02 20:30 co2_reading_plugin/ui/contrib/jobs/co2_reading.yaml
--rw-r--r--  2.0 unx     1049 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1147 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1044 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/RECORD
-11 files, 11008 bytes uncompressed, 4425 bytes compressed:  59.8%
+-rw-r--r--  2.0 unx     1049 b- defN 23-Jun-12 16:50 co2_reading_plugin-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jun-12 16:50 co2_reading_plugin-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 16:50 co2_reading_plugin-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-12 16:50 co2_reading_plugin-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-12 16:50 co2_reading_plugin-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1044 b- defN 23-Jun-12 16:50 co2_reading_plugin-0.1.3.dist-info/RECORD
+11 files, 11012 bytes uncompressed, 4427 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: co2_reading_plugin/ui/contrib/charts/co2_readings.yaml
 Comment: 
 
 Filename: co2_reading_plugin/ui/contrib/jobs/co2_reading.yaml
 Comment: 
 
-Filename: co2_reading_plugin-0.1.2.dist-info/LICENSE.txt
+Filename: co2_reading_plugin-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: co2_reading_plugin-0.1.2.dist-info/METADATA
+Filename: co2_reading_plugin-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: co2_reading_plugin-0.1.2.dist-info/WHEEL
+Filename: co2_reading_plugin-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: co2_reading_plugin-0.1.2.dist-info/entry_points.txt
+Filename: co2_reading_plugin-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: co2_reading_plugin-0.1.2.dist-info/top_level.txt
+Filename: co2_reading_plugin-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: co2_reading_plugin-0.1.2.dist-info/RECORD
+Filename: co2_reading_plugin-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## co2_reading_plugin/__init__.py

```diff
@@ -52,15 +52,15 @@
         unit: str,
         experiment: str,
         interval: float,
         skip_co2: bool = False,
         skip_temperature: bool = False,
         skip_relative_humidity: bool = False,
     ) -> None:
-        super().__init__(unit=unit, experiment=experiment, source="co2_reading_plugin")
+        super().__init__(unit=unit, experiment=experiment, plugin_name="co2_reading_plugin")
 
         self.interval = interval
         self.skip_co2 = skip_co2
         self.skip_temperature = skip_temperature
         self.skip_relative_humidity = skip_relative_humidity
 
         if is_pio_job_running("co2_reading"):
```

## Comparing `co2_reading_plugin-0.1.2.dist-info/LICENSE.txt` & `co2_reading_plugin-0.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `co2_reading_plugin-0.1.2.dist-info/METADATA` & `co2_reading_plugin-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co2-reading-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Return a CO₂ reading every interval from an Adafruit CO₂ sensors SCD30, SCD40 or SCD41.
 Home-page: https://github.com/Pioreactor/co2_reading_plugin
 Author: Kelly Tran, Cameron Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -15,13 +15,12 @@
 
 Adafruit offers three CO2 sensors ([SCD30](https://www.adafruit.com/product/4867), [SCD40 and SCD41](https://learn.adafruit.com/adafruit-scd-40-and-scd-41)) that measure CO2, temperature, and humidity.
 
 This is a simple Pioreactor plugin that returns CO2 readings (or all readings) at a set duration from stemma QT connected Adafruit SCD sensors.
 
 Install with `pio install-plugin co2-reading-plugin` from the command line, or in the Pioreactor UI.
 
-
 > Important: after installation, this requires a reboot of your leader Pioreactor
 
 ### Overview chart
 
 This also adds a chart to your overview page that displays the CO2 readings per Pioreactor.
```

