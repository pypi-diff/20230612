# Comparing `tmp/pioled_display_plugin-0.2.1-py3-none-any.whl.zip` & `tmp/pioled_display_plugin-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4954 bytes, number of entries: 9
--rw-r--r--  2.0 unx     5392 b- defN 23-Jun-12 15:54 pioled_display_plugin/__init__.py
+Zip file size: 4964 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     5417 b- defN 23-Jun-12 16:01 pioled_display_plugin/__init__.py
 -rw-r--r--  2.0 unx      180 b- defN 23-Jun-12 15:54 pioled_display_plugin/post_install.sh
 -rw-r--r--  2.0 unx      180 b- defN 23-Jun-12 15:54 pioled_display_plugin/pre_uninstall.sh
--rw-r--r--  2.0 unx     1052 b- defN 23-Jun-12 15:57 pioled_display_plugin-0.2.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      800 b- defN 23-Jun-12 15:57 pioled_display_plugin-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 15:57 pioled_display_plugin-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Jun-12 15:57 pioled_display_plugin-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-12 15:57 pioled_display_plugin-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      845 b- defN 23-Jun-12 15:57 pioled_display_plugin-0.2.1.dist-info/RECORD
-9 files, 8630 bytes uncompressed, 3458 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     1052 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      800 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      845 b- defN 23-Jun-12 16:02 pioled_display_plugin-0.2.2.dist-info/RECORD
+9 files, 8655 bytes uncompressed, 3468 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pioled_display_plugin/post_install.sh
 Comment: 
 
 Filename: pioled_display_plugin/pre_uninstall.sh
 Comment: 
 
-Filename: pioled_display_plugin-0.2.1.dist-info/LICENSE.txt
+Filename: pioled_display_plugin-0.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.2.1.dist-info/METADATA
+Filename: pioled_display_plugin-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pioled_display_plugin-0.2.1.dist-info/WHEEL
+Filename: pioled_display_plugin-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pioled_display_plugin-0.2.1.dist-info/entry_points.txt
+Filename: pioled_display_plugin-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.2.1.dist-info/top_level.txt
+Filename: pioled_display_plugin-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.2.1.dist-info/RECORD
+Filename: pioled_display_plugin-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioled_display_plugin/__init__.py

```diff
@@ -32,17 +32,18 @@
         super().__init__(unit=unit, experiment=experiment, plugin_name="pioled_display_plugin")
 
         # Create the I2C interface.
         i2c = busio.I2C(SCL, SDA)
 
         try:
             self.disp = adafruit_ssd1306.SSD1306_I2C(128, 32, i2c)
-        except Exception:
+        except Exception as e:
             self.logger.error("Unable to find hardware")
             self.clean_up()
+            raise e
 
         # get ip for displaying
         self._ip = get_ip()
 
         # rotate the screen since we are flipping it
         self.disp.rotation = 2
```

## Comparing `pioled_display_plugin-0.2.1.dist-info/LICENSE.txt` & `pioled_display_plugin-0.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pioled_display_plugin-0.2.1.dist-info/METADATA` & `pioled_display_plugin-0.2.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioled-display-plugin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use an OLED display with your Pioreactor
 Home-page: https://github.com/Pioreactor/PiOLED-display-plugin
 Author: Cameron Davidson-Pilon
 Author-email: hello@pioreactor.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: adafruit-circuitpython-ssd1306
```

## Comparing `pioled_display_plugin-0.2.1.dist-info/RECORD` & `pioled_display_plugin-0.2.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pioled_display_plugin/__init__.py,sha256=kbK5-nBfmKk5heGwaRjgushGZ0IZ59bA6OI53RZe4RE,5392
+pioled_display_plugin/__init__.py,sha256=QvxiS-cgKzOS1K2pyuCEGZzuVf1MyV-Z_eORW8jXSaE,5417
 pioled_display_plugin/post_install.sh,sha256=cV2Ft1Jq6uxbAgOxSfoqDRZSx0mlhKd0NlMZgcE809E,180
 pioled_display_plugin/pre_uninstall.sh,sha256=7Ya_m3QVPCIFz8_dR7ZgaO5jKuqSlaS2EwPryoSjd6g,180
-pioled_display_plugin-0.2.1.dist-info/LICENSE.txt,sha256=ocekcdri6meHuZdEP-AjJ_MucbIJ6VAG-CTqTIwJa_8,1052
-pioled_display_plugin-0.2.1.dist-info/METADATA,sha256=Bce8W9qWNCQysNKsQPwcrPcyK0b-Qr_37LEwwkncYIY,800
-pioled_display_plugin-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioled_display_plugin-0.2.1.dist-info/entry_points.txt,sha256=W0sMG2mMiqAyQMPvuMY0BNToztk3TH-Q4qxa6x08ogU,67
-pioled_display_plugin-0.2.1.dist-info/top_level.txt,sha256=akjKC6z5KYffEuIiQSXyXM8MgQwJqIl2ewjjV6RqLvM,22
-pioled_display_plugin-0.2.1.dist-info/RECORD,,
+pioled_display_plugin-0.2.2.dist-info/LICENSE.txt,sha256=ocekcdri6meHuZdEP-AjJ_MucbIJ6VAG-CTqTIwJa_8,1052
+pioled_display_plugin-0.2.2.dist-info/METADATA,sha256=YfcRwh0qRyXQusSNUdzNdW73mK73GSnR6kV3i0zRURQ,800
+pioled_display_plugin-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioled_display_plugin-0.2.2.dist-info/entry_points.txt,sha256=W0sMG2mMiqAyQMPvuMY0BNToztk3TH-Q4qxa6x08ogU,67
+pioled_display_plugin-0.2.2.dist-info/top_level.txt,sha256=akjKC6z5KYffEuIiQSXyXM8MgQwJqIl2ewjjV6RqLvM,22
+pioled_display_plugin-0.2.2.dist-info/RECORD,,
```

