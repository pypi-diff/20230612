# Comparing `tmp/lnxlink-2023.6.0.tar.gz` & `tmp/lnxlink-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2023.6.0.tar", last modified: Wed May 31 20:44:02 2023, max compression
+gzip compressed data, was "lnxlink-2023.6.1.tar", last modified: Mon Jun 12 15:59:09 2023, max compression
```

## Comparing `lnxlink-2023.6.0.tar` & `lnxlink-2023.6.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.033674 lnxlink-2023.6.0/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14770 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/boot_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/nvidia_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 20:44:02.000000 lnxlink-2023.6.0/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.008688 lnxlink-2023.6.1/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14770 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/amd_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/nvidia_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 15:59:09.000000 lnxlink-2023.6.1/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 15:59:08.000000 lnxlink-2023.6.1/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-06-12 15:58:55.000000 lnxlink-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-12 15:59:09.012688 lnxlink-2023.6.1/setup.cfg
```

### Comparing `lnxlink-2023.6.0/LICENSE.md` & `lnxlink-2023.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/PKG-INFO` & `lnxlink-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
  * [Headless Installation](#headless-installation)
  * [Examples](#examples)
  * [FAQ](#faq)
 
 
 # Features
  - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive, Brightness, Boot select.
- - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
+ - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, AMD / Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
  - **Home Assistant:** Uses MQTT Autodiscovery to create entities and shows if update is required.
  - **No sudo required:** No need to be root user to install and use, unless used on server setup.
  - **Easily expanded:** Any new module is automatically imported and custom modules can be added.
 
 # Installation
 Install or update:
 ```shell
```

### Comparing `lnxlink-2023.6.0/README.md` & `lnxlink-2023.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  * [Headless Installation](#headless-installation)
  * [Examples](#examples)
  * [FAQ](#faq)
 
 
 # Features
  - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive, Brightness, Boot select.
- - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
+ - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, AMD / Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
  - **Home Assistant:** Uses MQTT Autodiscovery to create entities and shows if update is required.
  - **No sudo required:** No need to be root user to install and use, unless used on server setup.
  - **Easily expanded:** Any new module is automatically imported and custom modules can be added.
 
 # Installation
 Install or update:
 ```shell
```

### Comparing `lnxlink-2023.6.0/lnxlink/__main__.py` & `lnxlink-2023.6.1/lnxlink/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         if hasattr(addon, 'device_class'):
             discovery['device_class'] = addon.device_class
         if hasattr(addon, 'state_class'):
             discovery['state_class'] = addon.state_class
 
         sensor_type = getattr(addon, 'sensor_type', None)
         if sensor_type in ['sensor', 'binary_sensor']:
-            discovery['expire_after'] = self.config.get('update_interval', 5) * 2
+            discovery['expire_after'] = self.config.get('update_interval', 5) * 5
         if sensor_type is not None:
             self.client.publish(
                 f"homeassistant/{sensor_type}/lnxlink/{discovery['unique_id']}/config",
                 payload=json.dumps(discovery),
                 retain=self.config['mqtt']['lwt']['retain'])
 
     def setup_discovery_control(self, discovery_template, addon, service, control_name, options):
```

### Comparing `lnxlink-2023.6.0/lnxlink/config.py` & `lnxlink-2023.6.1/lnxlink/config.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/consts.py` & `lnxlink-2023.6.1/lnxlink/consts.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/__init__.py` & `lnxlink-2023.6.1/lnxlink/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/battery.py` & `lnxlink-2023.6.1/lnxlink/modules/battery.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/boot_select.py` & `lnxlink-2023.6.1/lnxlink/modules/boot_select.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/brightness.py` & `lnxlink-2023.6.1/lnxlink/modules/brightness.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/camera_used.py` & `lnxlink-2023.6.1/lnxlink/modules/camera_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/disk_usage.py` & `lnxlink-2023.6.1/lnxlink/modules/disk_usage.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/keep_alive.py` & `lnxlink-2023.6.1/lnxlink/modules/keep_alive.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/media.py` & `lnxlink-2023.6.1/lnxlink/modules/media.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/memory.py` & `lnxlink-2023.6.1/lnxlink/modules/memory.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/microphone_used.py` & `lnxlink-2023.6.1/lnxlink/modules/microphone_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/network.py` & `lnxlink-2023.6.1/lnxlink/modules/network.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/notify.py` & `lnxlink-2023.6.1/lnxlink/modules/notify.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/nvidia_gpu.py` & `lnxlink-2023.6.1/lnxlink/modules/nvidia_gpu.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/screen_onoff.py` & `lnxlink-2023.6.1/lnxlink/modules/screen_onoff.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/screenshot.py` & `lnxlink-2023.6.1/lnxlink/modules/screenshot.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/sys_updates.py` & `lnxlink-2023.6.1/lnxlink/modules/sys_updates.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/update.py` & `lnxlink-2023.6.1/lnxlink/modules/update.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/modules/webcam.py` & `lnxlink-2023.6.1/lnxlink/modules/webcam.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink/system_monitor.py` & `lnxlink-2023.6.1/lnxlink/system_monitor.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.6.0/lnxlink.egg-info/PKG-INFO` & `lnxlink-2023.6.1/lnxlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
  * [Headless Installation](#headless-installation)
  * [Examples](#examples)
  * [FAQ](#faq)
 
 
 # Features
  - **System control:** Shutdown, Restart, Suspend, Send Keys, Notify, Media, Screen On/Off, open URL/File, bash, Keep Alive, Brightness, Boot select.
- - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
+ - **System monitor:** CPU, Ram, Network, Media, Microphone, Idle, Battery, Disk usage, Required restart, AMD / Nvidia GPU, Camera, Memory, Update required, System updates, Webcam, Screenshot.
  - **Home Assistant:** Uses MQTT Autodiscovery to create entities and shows if update is required.
  - **No sudo required:** No need to be root user to install and use, unless used on server setup.
  - **Easily expanded:** Any new module is automatically imported and custom modules can be added.
 
 # Installation
 Install or update:
 ```shell
```

### Comparing `lnxlink-2023.6.0/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2023.6.1/lnxlink.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 lnxlink.egg-info/PKG-INFO
 lnxlink.egg-info/SOURCES.txt
 lnxlink.egg-info/dependency_links.txt
 lnxlink.egg-info/entry_points.txt
 lnxlink.egg-info/requires.txt
 lnxlink.egg-info/top_level.txt
 lnxlink/modules/__init__.py
+lnxlink/modules/amd_gpu.py
 lnxlink/modules/bash.py
 lnxlink/modules/battery.py
 lnxlink/modules/boot_select.py
 lnxlink/modules/brightness.py
 lnxlink/modules/camera_used.py
 lnxlink/modules/cpu.py
 lnxlink/modules/disk_usage.py
```

### Comparing `lnxlink-2023.6.0/pyproject.toml` & `lnxlink-2023.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2023.6.0"
+version           = "2023.6.1"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
@@ -27,15 +27,16 @@
     "dbus-python>=1.3.2",
     "pgi>=0.0.11.2",
     "pyOpenSSL>=22.1.0",
     "requests>=2.28.1",
     "jc>=1.23.0",
     "dbus-idle>=2023.3.2",
     "opencv-python>=4.7.0.68",
-    "mss>=7.0.1"
+    "mss>=7.0.1",
+    "pyamdgpuinfo>=2.1.4"
 ]
 
 
 [project.urls]
 "Source Code" = "https://github.com/bkbilly/lnxlink"
 "Home Page"   = "https://bkbilly.github.io/lnxlink"
```

