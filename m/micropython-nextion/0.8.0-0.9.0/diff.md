# Comparing `tmp/micropython-nextion-0.8.0.tar.gz` & `tmp/micropython-nextion-0.9.0.tar.gz`

## Comparing `micropython-nextion-0.8.0.tar` & `micropython-nextion-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0 runner    (1001) docker     (121)     3903 2022-07-30 07:30:00.000000 micropython-nextion-0.8.0/micropython_nextion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-30 07:30:00.000000 micropython-nextion-0.8.0/micropython_nextion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9138 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_dual_state_button.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_gauge.py
--rw-r--r--   0 runner    (1001) docker     (121)    10090 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_hardware.py
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_number.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_radio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_slider.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/nextion_waveform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-07-30 07:29:49.000000 micropython-nextion-0.8.0/nextion/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-30 07:30:00.000000 micropython-nextion-0.8.0/nextion/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3903 2022-07-30 08:28:55.000000 micropython-nextion-0.9.0/micropython_nextion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-30 08:28:55.000000 micropython-nextion-0.9.0/micropython_nextion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9138 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_button.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2787 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_dual_state_button.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10090 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_number.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_radio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_slider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5247 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/nextion_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-07-30 08:28:46.000000 micropython-nextion-0.9.0/nextion/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-07-30 08:28:54.000000 micropython-nextion-0.9.0/nextion/version.py
```

### Comparing `micropython-nextion-0.8.0/micropython_nextion.egg-info/PKG-INFO` & `micropython-nextion-0.9.0/micropython_nextion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-nextion
-Version: 0.8.0
+Version: 0.9.0
 Summary: MicroPython Nextion serial displays library
 Home-page: https://github.com/brainelectronics/micropython-nextion
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-nextion/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-nextion
```

### Comparing `micropython-nextion-0.8.0/nextion/__init__.py` & `micropython-nextion-0.9.0/nextion/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .version import __version__
 
 from .nextion_hardware import NexHardware, NexHardwareError
 from .nextion_button import NexButton
 from .nextion_checkbox import NexCheckbox
 from .nextion_dual_state_button import NexDSButton
 from .nextion_gauge import NexGauge
+from .nextion_gpio import NexGpio
 from .nextion_number import NexNumber
 from .nextion_page import NexPage
 from .nextion_progressbar import NexProgressBar
 from .nextion_radio import NexRadio
 from .nextion_slider import NexSlider
 from .nextion_text import NexText
 from .nextion_waveform import NexWaveform
```

### Comparing `micropython-nextion-0.8.0/nextion/common.py` & `micropython-nextion-0.9.0/nextion/common.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/const.py` & `micropython-nextion-0.9.0/nextion/const.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_button.py` & `micropython-nextion-0.9.0/nextion/nextion_button.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_checkbox.py` & `micropython-nextion-0.9.0/nextion/nextion_checkbox.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_dual_state_button.py` & `micropython-nextion-0.9.0/nextion/nextion_dual_state_button.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_gauge.py` & `micropython-nextion-0.9.0/nextion/nextion_gauge.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_hardware.py` & `micropython-nextion-0.9.0/nextion/nextion_hardware.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_number.py` & `micropython-nextion-0.9.0/nextion/nextion_number.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_page.py` & `micropython-nextion-0.9.0/nextion/nextion_page.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_progressbar.py` & `micropython-nextion-0.9.0/nextion/nextion_progressbar.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_radio.py` & `micropython-nextion-0.9.0/nextion/nextion_radio.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_slider.py` & `micropython-nextion-0.9.0/nextion/nextion_slider.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_text.py` & `micropython-nextion-0.9.0/nextion/nextion_text.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/nextion_waveform.py` & `micropython-nextion-0.9.0/nextion/nextion_waveform.py`

 * *Files identical despite different names*

### Comparing `micropython-nextion-0.8.0/nextion/typing.py` & `micropython-nextion-0.9.0/nextion/typing.py`

 * *Files identical despite different names*

