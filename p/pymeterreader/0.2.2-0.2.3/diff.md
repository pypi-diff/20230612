# Comparing `tmp/pymeterreader-0.2.2.tar.gz` & `tmp/pymeterreader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeterreader-0.2.2.tar", last modified: Sun Aug 28 09:59:29 2022, max compression
+gzip compressed data, was "pymeterreader-0.2.3.tar", last modified: Mon Jun 12 08:26:49 2023, max compression
```

## Comparing `pymeterreader-0.2.2.tar` & `pymeterreader-0.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.896629 pymeterreader-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-08-28 09:59:29.896629 pymeterreader-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/example_configuration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.892629 pymeterreader-0.2.2/pymeterreader/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.892629 pymeterreader-0.2.2/pymeterreader/core/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/core/channel_description.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/core/channel_upload_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     4903 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/core/meter_reader_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/core/meter_reader_task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.896629 pymeterreader-0.2.2/pymeterreader/device_lib/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7102 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/meter_plain.py
--rw-r--r--   0 runner    (1001) docker     (121)     7905 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/meter_sml.py
--rw-r--r--   0 runner    (1001) docker     (121)    28538 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/sensor_bme280.py
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3968 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/test_meter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4914 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/test_meter_plain.py
--rw-r--r--   0 runner    (1001) docker     (121)     7228 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/test_meter_sml.py
--rw-r--r--   0 runner    (1001) docker     (121)     8293 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/device_lib/test_sensor_bme280.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.896629 pymeterreader-0.2.2/pymeterreader/gateway/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/gateway/basegateway.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/gateway/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     7323 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/gateway/volkszaehler.py
--rw-r--r--   0 runner    (1001) docker     (121)     7765 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/meter_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.896629 pymeterreader-0.2.2/pymeterreader/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/metrics/metrics_collector.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/metrics/prefix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/test_meter_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.896629 pymeterreader-0.2.2/pymeterreader/wizard/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/wizard/detector.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/wizard/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9020 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/pymeterreader/wizard/ncui.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:59:29.892629 pymeterreader-0.2.2/pymeterreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-08-28 09:59:29.000000 pymeterreader-0.2.2/pymeterreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-08-28 09:59:29.000000 pymeterreader-0.2.2/pymeterreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 09:59:29.000000 pymeterreader-0.2.2/pymeterreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-28 09:59:29.000000 pymeterreader-0.2.2/pymeterreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-08-28 09:59:29.000000 pymeterreader-0.2.2/pymeterreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-28 09:59:29.000000 pymeterreader-0.2.2/pymeterreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-28 09:59:29.896629 pymeterreader-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-08-28 09:59:22.000000 pymeterreader-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/example_configuration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.190734 pymeterreader-0.2.3/pymeterreader/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.190734 pymeterreader-0.2.3/pymeterreader/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/channel_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/channel_upload_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/meter_reader_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/core/meter_reader_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/device_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/meter_plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/meter_sml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28538 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/sensor_bme280.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_sml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/device_lib/test_sensor_bme280.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/basegateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/gateway/volkszaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/meter_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/metrics/metrics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/metrics/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/test_meter_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/pymeterreader/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/pymeterreader/wizard/ncui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:26:49.190734 pymeterreader-0.2.3/pymeterreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 08:26:49.000000 pymeterreader-0.2.3/pymeterreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:26:49.194735 pymeterreader-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-12 08:26:38.000000 pymeterreader-0.2.3/setup.py
```

### Comparing `pymeterreader-0.2.2/LICENSE` & `pymeterreader-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/PKG-INFO` & `pymeterreader-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeterreader
-Version: 0.2.2
+Version: 0.2.3
 Summary: pymeterreader is a service to poll smart meters and sensors.It supports uploading to volkszaehler middleware via its REST API.
 Home-page: https://github.com/Schwaneberg/pymeterreader
 Author: Oliver Schwaneberg
 Author-email: Oliver.Schwaneberg@gmail.com
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pymeterreader-0.2.2/README.md` & `pymeterreader-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/example_configuration.yaml` & `pymeterreader-0.2.3/example_configuration.yaml`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/core/channel_upload_info.py` & `pymeterreader-0.2.3/pymeterreader/core/channel_upload_info.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/core/meter_reader_node.py` & `pymeterreader-0.2.3/pymeterreader/core/meter_reader_node.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/core/meter_reader_task.py` & `pymeterreader-0.2.3/pymeterreader/core/meter_reader_task.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/base.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/base.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/common.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/common.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/meter_plain.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/meter_plain.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/meter_sml.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/meter_sml.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,22 @@
             sml_reconstructed = self.__START_SEQ + payload + trailer
             # Test if SML Start is well formatted
             assert sml_reconstructed.startswith(
                 self.__START_SEQ), "Reconstructed SML sequence has malformed Start Sequence!"
             # Test if SML End Sequence is present
             assert sml_reconstructed[8:-4].endswith(
                 self.__END_SEQ), "Reconstructed SML sequence has malformed End Sequence!"
-            _, frame = SmlBase.parse_frame(sml_reconstructed)
-            if frame is not None:
-                sample = self.__parse(frame)
-                if sample is not None:
-                    return sample
-                logger.error("Parsing the SML frame did not yield a Sample!")
+            result = SmlBase.parse_frame(sml_reconstructed)
+            if len(result) == 2:
+                _, frame = result
+                if frame is not None:
+                    sample = self.__parse(frame)
+                    if sample is not None:
+                        return sample
+                    logger.error("Parsing the SML frame did not yield a Sample!")
             logger.error("Could not parse the binary SML data")
         except AssertionError as err:
             logger.error(f"SML parsing failed: {err}")
         except SmlParserError as err:
             logger.error(f"SML parsing library failed decoding the frame: {err}")
         except serial.SerialException as err:
             logger.error(f"Serial Interface error: {err}")
```

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/sensor_bme280.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/sensor_bme280.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/serial_reader.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/serial_reader.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/test_base.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/test_base.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/test_meter.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/test_meter.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/test_meter_plain.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_plain.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from pymeterreader.device_lib.common import ChannelValue, Device
 from pymeterreader.device_lib.test_meter import StaticMeterSimulator, SerialTestData
 
 
 class PlainMeterSimulator(StaticMeterSimulator):
     """
     Simulate a Plain Meter that requires a wakeup before sending a sample.
-    This implementation is not compatible with a loop:// interface since it depends on having different send/receiver buffers.
+    This implementation is not compatible with a loop:// interface since
+    it depends on having different send/receiver buffers.
     """
 
     def __init__(self) -> None:
         start_sequence = b'\x1b\x1b\x1b\x1b\x01\x01\x01\x01'
         test_frame = b'\x026.8(0006047*kWh)6.26(00428.35*m3)9.21(99999999)\r\n'
         test_data = SerialTestData(
             binary=start_sequence + test_frame,
```

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/test_meter_sml.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/test_meter_sml.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,38 +12,61 @@
 class EmhSmlMeterSimulator(StaticMeterSimulator):
     """
     Simulate a EMH ED300L SML Meter that sends a measurement unsolicited
     """
 
     def __init__(self) -> None:
         test_data = SerialTestData(
-            binary=b'\x1b\x1b\x1b\x1b\x01\x01\x01\x01v\x07\x00\x07\r\xf8\xb2\xd7b\x00b\x00rc\x01\x01v\x01\x01\x07\x00\x07\x0b?;\x9d\x0b\t\x01EMH\x00\x00K\x18\xe2\x01\x01cXk\x00v\x07\x00\x07\r\xf8\xb2\xd8b\x00b\x00rc\x07\x01w\x01\x0b\t\x01EMH\x00\x00K\x18\xe2\x07\x01\x00b\n\xff\xffrb\x01e\x0b?\xeejzw\x07\x81\x81\xc7\x82\x03\xff\x01\x01\x01\x01\x04EMH\x01w\x07\x01\x00\x00\x00\t\xff\x01\x01\x01\x01\x0b\t\x01EMH\x00\x00K\x18\xe2\x01w\x07\x01\x00\x01\x08\x00\xffd\x01\x01\xa2\x01b\x1eR\xffV\x00\x10T\xf2\xfe\x01w\x07\x01\x00\x02\x08\x00\xffd\x01\x01\xa2\x01b\x1eR\xffV\x00\x0bHz\xf0\x01w\x07\x01\x00\x01\x08\x01\xff\x01\x01b\x1eR\xffV\x00\x10T\xf2\xfe\x01w\x07\x01\x00\x02\x08\x01\xff\x01\x01b\x1eR\xffV\x00\x0bHz\xf0\x01w\x07\x01\x00\x01\x08\x02\xff\x01\x01b\x1eR\xffV\x00\x00\x00\x00\x00\x01w\x07\x01\x00\x02\x08\x02\xff\x01\x01b\x1eR\xffV\x00\x00\x00\x00\x00\x01w\x07\x01\x00\x10\x07\x00\xff\x01\x01b\x1bR\xffU\xff\xff\xf3\xfa\x01w\x07\x81\x81\xc7\x82\x05\xff\x01rb\x01e\x0b?\xeej\x01\x01\x83\x02X\xaf(\x9aa\x13R\x98L\xf8R\x95#~\xf2fp\xcb=6~!\x8bH\xd9Rx\x9f\xc4\xa5\x88\x86\x04\x01+24\x90\xce\xd3\xd9m4\x1c\x9e\x9c\xcfw\x01\x01\x01c[\x12\x00v\x07\x00\x07\r\xf8\xb2\xdbb\x00b\x00rc\x02\x01q\x01c;\x15\x00\x00\x1b\x1b\x1b\x1b\x1a\x01\x1b\xe1',
+            binary=b'\x1b\x1b\x1b\x1b\x01\x01\x01\x01v\x07\x00\x07\r\xf8\xb2\xd7b\x00b\x00rc\x01\x01v'
+                   b'\x01\x01\x07\x00\x07\x0b?;\x9d\x0b\t\x01EMH\x00\x00K\x18\xe2\x01\x01cXk\x00v\x07'
+                   b'\x00\x07\r\xf8\xb2\xd8b\x00b\x00rc\x07\x01w\x01\x0b\t\x01EMH\x00\x00K\x18\xe2\x07'
+                   b'\x01\x00b\n\xff\xffrb\x01e\x0b?\xeejzw\x07\x81\x81\xc7\x82\x03\xff\x01\x01\x01'
+                   b'\x01\x04EMH\x01w\x07\x01\x00\x00\x00\t\xff\x01\x01\x01\x01\x0b\t\x01EMH\x00\x00'
+                   b'K\x18\xe2\x01w\x07\x01\x00\x01\x08\x00\xffd\x01\x01\xa2\x01b\x1eR\xffV\x00\x10'
+                   b'T\xf2\xfe\x01w\x07\x01\x00\x02\x08\x00\xffd\x01\x01\xa2\x01b\x1eR\xffV\x00\x0b'
+                   b'Hz\xf0\x01w\x07\x01\x00\x01\x08\x01\xff\x01\x01b\x1eR\xffV\x00\x10T\xf2\xfe\x01'
+                   b'w\x07\x01\x00\x02\x08\x01\xff\x01\x01b\x1eR\xffV\x00\x0bHz\xf0\x01w\x07\x01\x00'
+                   b'\x01\x08\x02\xff\x01\x01b\x1eR\xffV\x00\x00\x00\x00\x00\x01w\x07\x01\x00\x02\x08'
+                   b'\x02\xff\x01\x01b\x1eR\xffV\x00\x00\x00\x00\x00\x01w\x07\x01\x00\x10\x07\x00\xff'
+                   b'\x01\x01b\x1bR\xffU\xff\xff\xf3\xfa\x01w\x07\x81\x81\xc7\x82\x05\xff\x01rb\x01e'
+                   b'\x0b?\xeej\x01\x01\x83\x02X\xaf(\x9aa\x13R\x98L\xf8R\x95#~\xf2fp\xcb=6~!\x8bH\xd9'
+                   b'Rx\x9f\xc4\xa5\x88\x86\x04\x01+24\x90\xce\xd3\xd9m4\x1c\x9e\x9c\xcfw\x01\x01\x01'
+                   b'c[\x12\x00v\x07\x00\x07\r\xf8\xb2\xdbb\x00b\x00rc\x02\x01q\x01c;\x15\x00\x00\x1b'
+                   b'\x1b\x1b\x1b\x1a\x01\x1b\xe1',
             meter_id='1 EMH 00 4921570',
             channels=[ChannelValue(channel_name='129-129:199.130.3*255', value='EMH', unit=None),
                       ChannelValue(channel_name='1-0:1.8.0*255', value=27400268.6, unit='Wh'),
                       ChannelValue(channel_name='1-0:2.8.0*255', value=18929944.0, unit='Wh'),
                       ChannelValue(channel_name='1-0:1.8.1*255', value=27400268.6, unit='Wh'),
                       ChannelValue(channel_name='1-0:2.8.1*255', value=18929944.0, unit='Wh'),
                       ChannelValue(channel_name='1-0:1.8.2*255', value=0, unit='Wh'),
                       ChannelValue(channel_name='1-0:2.8.2*255', value=0, unit='Wh'),
                       ChannelValue(channel_name='1-0:16.7.0*255', value=-307.8, unit='W'),
                       ChannelValue(channel_name='129-129:199.130.5*255',
-                                   value='58af289a611352984cf85295237ef26670cb3d367e218b48d952789fc4a5888604012b323490ced3d96d341c9e9ccf77',
+                                   value='58af289a611352984cf85295237ef26670cb3d367e218b48'
+                                         'd952789fc4a5888604012b323490ced3d96d341c9e9ccf77',
                                    unit=None)])
         super().__init__(test_data)
 
 
 class IskraSMLMeterSimulator(StaticMeterSimulator):
     """
     Simulate a ISKRA MT631 SML Meter that sends a measurement unsolicited
     """
 
     def __init__(self) -> None:
         test_data = SerialTestData(
-            binary=b'\x1b\x1b\x1b\x1b\x01\x01\x01\x01v\x05\tLN\x1db\x00b\x00rc\x01\x01v\x01\x01\x05\x03\x19o_\x0b\n\x01ISK\x00\x045\xa9.rb\x01e\x03\x19p#b\x01c\xfe\x90\x00v\x05\tLN\x1eb\x00b\x00rc\x07\x01w\x01\x0b\n\x01ISK\x00\x045\xa9.\x07\x01\x00b\n\xff\xffrb\x01e\x03\x19p#uw\x07\x01\x00`2\x01\x01\x01\x01\x01\x01\x04ISK\x01w\x07\x01\x00`\x01\x00\xff\x01\x01\x01\x01\x0b\n\x01ISK\x00\x045\xa9.\x01w\x07\x01\x00\x01\x08\x00\xffe\x00\x1c)\x04\x01b\x1eR\xffe\x01"\xd9\x15\x01w\x07\x01\x00\x02\x08\x00\xff\x01\x01b\x1eR\xffe\x02\x8d\x94\x85\x01w\x07\x01\x00\x10\x07\x00\xff\x01\x01b\x1bR\x00S\xfe\xe4\x01\x01\x01c\xd6\xd5\x00v\x05\tLN\x1fb\x00b\x00rc\x02\x01q\x01cW\xe6\x00\x00\x1b\x1b\x1b\x1b\x1a\x01\x0b\x83',            meter_id='1 ISK 00 70625582',
+            binary=b'\x1b\x1b\x1b\x1b\x01\x01\x01\x01v\x05\tLN\x1db\x00b\x00rc\x01\x01v\x01\x01\x05\x03\x19o_\x0b\n'
+                   b'\x01ISK\x00\x045\xa9.rb\x01e\x03\x19p#b\x01c\xfe\x90\x00v\x05\tLN\x1eb\x00b\x00rc\x07\x01w\x01'
+                   b'\x0b\n\x01ISK\x00\x045\xa9.\x07\x01\x00b\n\xff\xffrb\x01e\x03\x19p#uw\x07\x01\x00`2\x01\x01\x01'
+                   b'\x01\x01\x01\x04ISK\x01w\x07\x01\x00`\x01\x00\xff\x01\x01\x01\x01\x0b\n\x01ISK\x00\x045\xa9.\x01'
+                   b'w\x07\x01\x00\x01\x08\x00\xffe\x00\x1c)\x04\x01b\x1eR\xffe\x01"\xd9\x15\x01w\x07\x01\x00\x02\x08'
+                   b'\x00\xff\x01\x01b\x1eR\xffe\x02\x8d\x94\x85\x01w\x07\x01\x00\x10\x07\x00\xff\x01\x01b\x1bR\x00S'
+                   b'\xfe\xe4\x01\x01\x01c\xd6\xd5\x00v\x05\tLN\x1fb\x00b\x00rc\x02\x01q\x01cW\xe6\x00\x00\x1b\x1b'
+                   b'\x1b\x1b\x1a\x01\x0b\x83',            meter_id='1 ISK 00 70625582',
             channels=[ChannelValue(channel_name='1-0:96.50.1*1', value=b'ISK', unit=None),
                       ChannelValue(channel_name='1-0:1.8.0*255', value=1906101.3, unit='Wh'),
                       ChannelValue(channel_name='1-0:2.8.0*255', value=4283302.9, unit='Wh'),
                       ChannelValue(channel_name='1-0:16.7.0*255', value=-284, unit='W')])
         super().__init__(test_data)
 
 
@@ -81,15 +104,16 @@
                 # Create serial instances with unmocked import
                 unconnected_serial_instance = serial_for_url("loop://", baudrate=9600, timeout=5)
                 shared_serial_instance = serial_for_url("loop://", baudrate=9600, timeout=5)
                 # Mock serial_for_url to return an unconnected instance and one with the simulator
                 serial_for_url_mock.side_effect = [shared_serial_instance,
                                                    unconnected_serial_instance,
                                                    shared_serial_instance]
-                # Create a Simulator. The simulator makes the first call to serial_for_url() and receives the shared instance
+                # Create a Simulator. The simulator makes the first call to serial_for_url()
+                # and receives the shared instance
                 simulator = simulator_class()
                 simulator.start()
                 # Mock available serial ports
                 list_ports_mock.return_value = [ListPortInfo("/dev/ttyUSB0"), ListPortInfo("/dev/ttyUSB1")]
                 # Start device detection. This triggers the remaining two calls to serial_for_url()
                 devices = SmlReader("unused://").detect()
                 simulator.stop()
```

### Comparing `pymeterreader-0.2.2/pymeterreader/device_lib/test_sensor_bme280.py` & `pymeterreader-0.2.3/pymeterreader/device_lib/test_sensor_bme280.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 @dataclass(frozen=True)
 class I2CTestData(TestData):
     static_registers: tp.Dict[int, int]
 
 
 class MockBus:
+    # pylint: disable=unused-argument
     def __init__(self, i2c_addr: int, test_data: I2CTestData) -> None:
         self.i2c_addr = i2c_addr
         self.test_data = test_data
         self.written = []
         self.open = False
 
     def write_byte_data(self, i2c_addr, register, value, force=None) -> None:
@@ -26,16 +27,16 @@
 
     def read_byte_data(self, i2c_addr, register, force=None) -> int:
         if i2c_addr != self.i2c_addr:
             raise OSError(f"Can not access SMBus@{i2c_addr}")
         assert self.open is True
         try:
             return self.test_data.static_registers[register]
-        except KeyError:
-            raise AssertionError(f"Register address {register} is not in the I2CTestData!")
+        except KeyError as err:
+            raise AssertionError(f"Register address {register} is not in the I2CTestData!") from err
 
     def read_i2c_block_data(self, i2c_addr, register, length, force=None) -> tp.List[int]:
         output_list: tp.List[int] = []
         for offset in range(0, length):
             output_list.append(self.read_byte_data(i2c_addr, register + offset, force))
         return output_list
```

### Comparing `pymeterreader-0.2.2/pymeterreader/gateway/basegateway.py` & `pymeterreader-0.2.3/pymeterreader/gateway/basegateway.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/gateway/debug.py` & `pymeterreader-0.2.3/pymeterreader/gateway/debug.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/gateway/volkszaehler.py` & `pymeterreader-0.2.3/pymeterreader/gateway/volkszaehler.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/meter_reader.py` & `pymeterreader-0.2.3/pymeterreader/meter_reader.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/metrics/metrics_collector.py` & `pymeterreader-0.2.3/pymeterreader/metrics/metrics_collector.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/test_meter_reader.py` & `pymeterreader-0.2.3/pymeterreader/test_meter_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,17 @@
         self.meter_id = None
 
     def poll(self):
         return self.sample
 
 
 class TestMeterReader(unittest.TestCase):
-    @mock.patch("pymeterreader.meter_reader.VolkszaehlerGateway", return_value=MockedGateway('http://192.168.1.1/', True))
+    #pylint: disable=unused-argument
+    @mock.patch("pymeterreader.meter_reader.VolkszaehlerGateway", return_value=MockedGateway('http://192.168.1.1/',
+                                                                                             True))
     @mock.patch("pymeterreader.meter_reader.SmlReader", return_value=MockedReader(SAMPLE_SML))
     @mock.patch("pymeterreader.meter_reader.PlainReader", return_value=MockedReader(SAMPLE_PLAIN))
     @mock.patch("pymeterreader.meter_reader.Bme280Reader", return_value=MockedReader(SAMPLE_BME))
     def test_meter_reader(self, mock_bme, mock_plain, mock_sml, mock_gw):
         meter_reader_nodes = map_configuration(EXAMPLE_CONF)
         self.assertEqual(3, len(meter_reader_nodes))
```

### Comparing `pymeterreader-0.2.2/pymeterreader/wizard/generator.py` & `pymeterreader-0.2.3/pymeterreader/wizard/generator.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader/wizard/ncui.py` & `pymeterreader-0.2.3/pymeterreader/wizard/ncui.py`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/pymeterreader.egg-info/PKG-INFO` & `pymeterreader-0.2.3/pymeterreader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeterreader
-Version: 0.2.2
+Version: 0.2.3
 Summary: pymeterreader is a service to poll smart meters and sensors.It supports uploading to volkszaehler middleware via its REST API.
 Home-page: https://github.com/Schwaneberg/pymeterreader
 Author: Oliver Schwaneberg
 Author-email: Oliver.Schwaneberg@gmail.com
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pymeterreader-0.2.2/pymeterreader.egg-info/SOURCES.txt` & `pymeterreader-0.2.3/pymeterreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymeterreader-0.2.2/setup.py` & `pymeterreader-0.2.3/setup.py`

 * *Files identical despite different names*

