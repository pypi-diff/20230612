# Comparing `tmp/piOLED_display_plugin-0.1.1-py3-none-any.whl.zip` & `tmp/pioled_display_plugin-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 4622 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4884 b- defN 23-Mar-24 15:31 pioled_display_plugin/__init__.py
+Zip file size: 5357 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     5392 b- defN 23-Jun-12 15:54 pioled_display_plugin/__init__.py
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-12 15:54 pioled_display_plugin/post_install.sh
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-12 15:54 pioled_display_plugin/pre_uninstall.sh
 -rw-r--r--  2.0 unx      232 b- defN 23-Mar-24 15:22 pioled_display_plugin/ui/contrib/jobs/piOLED_display.yaml
--rw-r--r--  2.0 unx     1052 b- defN 23-Mar-24 15:32 pioled_display_plugin-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      800 b- defN 23-Mar-24 15:32 pioled_display_plugin-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-24 15:32 pioled_display_plugin-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Mar-24 15:32 pioled_display_plugin-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Mar-24 15:32 pioled_display_plugin-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      771 b- defN 23-Mar-24 15:32 pioled_display_plugin-0.1.1.dist-info/RECORD
-8 files, 7920 bytes uncompressed, 3238 bytes compressed:  59.1%
+-rw-r--r--  2.0 unx     1052 b- defN 23-Jun-12 15:55 pioled_display_plugin-0.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      800 b- defN 23-Jun-12 15:55 pioled_display_plugin-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 15:55 pioled_display_plugin-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-12 15:55 pioled_display_plugin-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-12 15:55 pioled_display_plugin-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      958 b- defN 23-Jun-12 15:55 pioled_display_plugin-0.2.0.dist-info/RECORD
+10 files, 8975 bytes uncompressed, 3671 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
 Filename: pioled_display_plugin/__init__.py
 Comment: 
 
+Filename: pioled_display_plugin/post_install.sh
+Comment: 
+
+Filename: pioled_display_plugin/pre_uninstall.sh
+Comment: 
+
 Filename: pioled_display_plugin/ui/contrib/jobs/piOLED_display.yaml
 Comment: 
 
-Filename: pioled_display_plugin-0.1.1.dist-info/LICENSE.txt
+Filename: pioled_display_plugin-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.1.1.dist-info/METADATA
+Filename: pioled_display_plugin-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pioled_display_plugin-0.1.1.dist-info/WHEEL
+Filename: pioled_display_plugin-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pioled_display_plugin-0.1.1.dist-info/entry_points.txt
+Filename: pioled_display_plugin-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.1.1.dist-info/top_level.txt
+Filename: pioled_display_plugin-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pioled_display_plugin-0.1.1.dist-info/RECORD
+Filename: pioled_display_plugin-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioled_display_plugin/__init__.py

```diff
@@ -11,16 +11,17 @@
 from PIL import ImageDraw
 from PIL import ImageFont
 from pioreactor import structs
 from pioreactor import types as pt
 from pioreactor.background_jobs.base import BackgroundJobContrib
 from pioreactor.hardware import SCL
 from pioreactor.hardware import SDA
-from pioreactor.whoami import get_latest_experiment_name
+from pioreactor.utils.networking import get_ip
 from pioreactor.whoami import get_unit_name
+from pioreactor.whoami import UNIVERSAL_EXPERIMENT
 
 
 class PiOLEDDisplay(BackgroundJobContrib):
 
     job_name = "pioled_display"
 
     growth_rate: Optional[float] = None
@@ -35,14 +36,17 @@
 
         try:
             self.disp = adafruit_ssd1306.SSD1306_I2C(128, 32, i2c)
         except Exception:
             self.logger.error("Unable to find hardware")
             self.clean_up()
 
+        # get ip for displaying
+        self._ip = get_ip()
+
         # rotate the screen since we are flipping it
         self.disp.rotation = 2
 
         # Clear display.
         self.disp.fill(0)
         self.disp.show()
 
@@ -89,33 +93,40 @@
         else:
             self.temp = None
         self.update_display()
 
     def start_passive_listeners(self) -> None:
         self.subscribe_and_callback(
             self.update_od,
-            f"pioreactor/{self.unit}/{self.experiment}/growth_rate_calculating/od_filtered",
+            f"pioreactor/{self.unit}/+/growth_rate_calculating/od_filtered",
+            allow_retained=False,
         )
         self.subscribe_and_callback(
             self.update_growth_rate,
-            f"pioreactor/{self.unit}/{self.experiment}/growth_rate_calculating/growth_rate",
+            f"pioreactor/{self.unit}/+/growth_rate_calculating/growth_rate",
+            allow_retained=False,
         )
         self.subscribe_and_callback(
             self.update_temp,
-            f"pioreactor/{self.unit}/{self.experiment}/temperature_control/temperature",
+            f"pioreactor/{self.unit}/+/temperature_control/temperature",
+            allow_retained=False,
         )
 
     def clear_display(self):
         self.draw.rectangle((0, 0, self.width, self.height), outline=0, fill=0)
         self.disp.image(self.image)
         self.disp.show()
 
     def on_disconnected(self):
         self.clear_display()
 
+    def update_display_and_increment_whoami(self):
+        self._whoami_counter += 1
+        self.update_display()
+
     def update_display(self) -> None:
         # Draw a black filled box to clear the image.
         self.draw.rectangle((0, 0, self.width, self.height), outline=0, fill=0)
         # Write four lines of text.
         self.draw.text((self.x, self.top + 0), self.unit, font=self.font, fill=255)
         if self.growth_rate:
             self.draw.text(
@@ -135,19 +146,27 @@
             self.draw.text(
                 (self.x, self.top + 25),
                 f" Temperature: {self.temp:.1f} C",
                 font=self.font,
                 fill=255,
             )
 
+        if not self.temp and not self.od and not self.growth_rate:
+            self.draw.text(
+                (self.x, self.top + 8),
+                f" IP: {self._ip}",
+                font=self.font,
+                fill=255,
+            )
+
         # Display image.
         self.disp.image(self.image)
         self.disp.show()
 
 
 @click.command(name="pioled_display")
 def click_pioled_display():
     """
     Turn on the OLED display
     """
-    lg = PiOLEDDisplay(unit=get_unit_name(), experiment=get_latest_experiment_name())
+    lg = PiOLEDDisplay(unit=get_unit_name(), experiment=UNIVERSAL_EXPERIMENT)
     lg.block_until_disconnected()
```

## Comparing `pioled_display_plugin-0.1.1.dist-info/LICENSE.txt` & `pioled_display_plugin-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pioled_display_plugin-0.1.1.dist-info/METADATA` & `pioled_display_plugin-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioled-display-plugin
-Version: 0.1.1
+Version: 0.2.0
 Summary: Use an OLED display with your Pioreactor
 Home-page: https://github.com/Pioreactor/PiOLED-display-plugin
 Author: Cameron Davidson-Pilon
 Author-email: hello@pioreactor.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: adafruit-circuitpython-ssd1306
```

## Comparing `pioled_display_plugin-0.1.1.dist-info/RECORD` & `pioled_display_plugin-0.2.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-pioled_display_plugin/__init__.py,sha256=fYrNuBHmeo3zK6neuaI1AMLWCBt01juOeOTBnJxZVFY,4884
+pioled_display_plugin/__init__.py,sha256=kbK5-nBfmKk5heGwaRjgushGZ0IZ59bA6OI53RZe4RE,5392
+pioled_display_plugin/post_install.sh,sha256=cV2Ft1Jq6uxbAgOxSfoqDRZSx0mlhKd0NlMZgcE809E,180
+pioled_display_plugin/pre_uninstall.sh,sha256=7Ya_m3QVPCIFz8_dR7ZgaO5jKuqSlaS2EwPryoSjd6g,180
 pioled_display_plugin/ui/contrib/jobs/piOLED_display.yaml,sha256=z0Wi7Zocfkl_dCHc7gcs8oJE6G5uO9f9uaNr65OXuvA,232
-pioled_display_plugin-0.1.1.dist-info/LICENSE.txt,sha256=ocekcdri6meHuZdEP-AjJ_MucbIJ6VAG-CTqTIwJa_8,1052
-pioled_display_plugin-0.1.1.dist-info/METADATA,sha256=9nljQxM_cWXlcj13q48Oj12OO0Nq2jpv5Siji15y6Ew,800
-pioled_display_plugin-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioled_display_plugin-0.1.1.dist-info/entry_points.txt,sha256=W0sMG2mMiqAyQMPvuMY0BNToztk3TH-Q4qxa6x08ogU,67
-pioled_display_plugin-0.1.1.dist-info/top_level.txt,sha256=akjKC6z5KYffEuIiQSXyXM8MgQwJqIl2ewjjV6RqLvM,22
-pioled_display_plugin-0.1.1.dist-info/RECORD,,
+pioled_display_plugin-0.2.0.dist-info/LICENSE.txt,sha256=ocekcdri6meHuZdEP-AjJ_MucbIJ6VAG-CTqTIwJa_8,1052
+pioled_display_plugin-0.2.0.dist-info/METADATA,sha256=B07gcFQjHZ6poHGSVE2FLqnuMGzMc9zpRcWa7E4-pZ0,800
+pioled_display_plugin-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioled_display_plugin-0.2.0.dist-info/entry_points.txt,sha256=W0sMG2mMiqAyQMPvuMY0BNToztk3TH-Q4qxa6x08ogU,67
+pioled_display_plugin-0.2.0.dist-info/top_level.txt,sha256=akjKC6z5KYffEuIiQSXyXM8MgQwJqIl2ewjjV6RqLvM,22
+pioled_display_plugin-0.2.0.dist-info/RECORD,,
```

