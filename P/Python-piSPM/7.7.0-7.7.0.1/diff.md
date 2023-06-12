# Comparing `tmp/Python-piSPM-7.7.0.tar.gz` & `tmp/Python-piSPM-7.7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-piSPM-7.7.0.tar", last modified: Mon May 15 09:08:37 2023, max compression
+gzip compressed data, was "Python-piSPM-7.7.0.1.tar", last modified: Mon Jun 12 08:50:43 2023, max compression
```

## Comparing `Python-piSPM-7.7.0.tar` & `Python-piSPM-7.7.0.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:08:37.252143 Python-piSPM-7.7.0/
--rw-rw-rw-   0        0        0     1093 2023-03-06 08:59:01.000000 Python-piSPM-7.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0     7034 2023-05-15 09:08:37.251030 Python-piSPM-7.7.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-15 09:08:37.248367 Python-piSPM-7.7.0/Python_piSPM.egg-info/
--rw-rw-rw-   0        0        0     7034 2023-05-15 09:08:37.000000 Python-piSPM-7.7.0/Python_piSPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-15 09:08:37.000000 Python-piSPM-7.7.0/Python_piSPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:08:37.000000 Python-piSPM-7.7.0/Python_piSPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:36.000000 Python-piSPM-7.7.0/Python_piSPM.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-05-15 09:08:37.000000 Python-piSPM-7.7.0/Python_piSPM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 09:08:37.000000 Python-piSPM-7.7.0/Python_piSPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5409 2023-05-12 10:24:36.000000 Python-piSPM-7.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 09:08:37.249383 Python-piSPM-7.7.0/pi_spm/
--rw-rw-rw-   0        0        0    25851 2023-05-11 10:59:00.000000 Python-piSPM-7.7.0/pi_spm/__init__.py
--rw-rw-rw-   0        0        0      380 2023-05-15 09:06:29.000000 Python-piSPM-7.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 09:08:37.253138 Python-piSPM-7.7.0/setup.cfg
--rw-rw-rw-   0        0        0      366 2022-10-27 08:25:55.000000 Python-piSPM-7.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:50:43.130282 Python-piSPM-7.7.0.1/
+-rw-rw-rw-   0        0        0     1093 2023-03-06 08:59:01.000000 Python-piSPM-7.7.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     7048 2023-06-12 08:50:43.129282 Python-piSPM-7.7.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 08:50:43.128283 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/
+-rw-rw-rw-   0        0        0     7048 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5464 2023-06-12 08:44:29.000000 Python-piSPM-7.7.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 08:50:43.128283 Python-piSPM-7.7.0.1/pi_spm/
+-rw-rw-rw-   0        0        0    25901 2023-06-12 08:42:37.000000 Python-piSPM-7.7.0.1/pi_spm/__init__.py
+-rw-rw-rw-   0        0        0      382 2023-06-12 08:46:46.000000 Python-piSPM-7.7.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 08:50:43.130282 Python-piSPM-7.7.0.1/setup.cfg
```

### Comparing `Python-piSPM-7.7.0/LICENSE.txt` & `Python-piSPM-7.7.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Python-piSPM-7.7.0/PKG-INFO` & `Python-piSPM-7.7.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: Python-piSPM
-Version: 7.7.0
+Version: 7.7.0.1
 Summary: Python piSPM is a Python wrapper for Pickering Switch Path Manager.
-Home-page: 
-Author: Pickering Interfaces
 Author-email: Pickering Interfaces <support@pickeringtest.com>
 License: Copyright (c) 2017-2023 Pickering Interfaces Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -32,15 +30,16 @@
 # Python SPM
 Python SPM is a Python wrapper for Pickering Switch Path Manager.
 
 **Pickering Switch Path Manager is needed for the wrapper to work**
 - [Switch Path Manager]https://downloads.pickeringtest.info/downloads/Switch%20Path%20Manager/
 
 ## Changelog
-> - 1.1 - Added protection functions
+> - 7.7.0.1 - Minor bugfix for protection functions
+> - 7.7.0 - Added protection functions
 
 ## Example usage
 ```python
 import pi_spm
 import os
 import sys
 from msvcrt import getch
```

### Comparing `Python-piSPM-7.7.0/Python_piSPM.egg-info/PKG-INFO` & `Python-piSPM-7.7.0.1/Python_piSPM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: Python-piSPM
-Version: 7.7.0
+Version: 7.7.0.1
 Summary: Python piSPM is a Python wrapper for Pickering Switch Path Manager.
-Home-page: 
-Author: Pickering Interfaces
 Author-email: Pickering Interfaces <support@pickeringtest.com>
 License: Copyright (c) 2017-2023 Pickering Interfaces Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -32,15 +30,16 @@
 # Python SPM
 Python SPM is a Python wrapper for Pickering Switch Path Manager.
 
 **Pickering Switch Path Manager is needed for the wrapper to work**
 - [Switch Path Manager]https://downloads.pickeringtest.info/downloads/Switch%20Path%20Manager/
 
 ## Changelog
-> - 1.1 - Added protection functions
+> - 7.7.0.1 - Minor bugfix for protection functions
+> - 7.7.0 - Added protection functions
 
 ## Example usage
 ```python
 import pi_spm
 import os
 import sys
 from msvcrt import getch
```

### Comparing `Python-piSPM-7.7.0/README.md` & `Python-piSPM-7.7.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Python SPM
 Python SPM is a Python wrapper for Pickering Switch Path Manager.
 
 **Pickering Switch Path Manager is needed for the wrapper to work**
 - [Switch Path Manager]https://downloads.pickeringtest.info/downloads/Switch%20Path%20Manager/
 
 ## Changelog
-> - 1.1 - Added protection functions
+> - 7.7.0.1 - Minor bugfix for protection functions
+> - 7.7.0 - Added protection functions
 
 ## Example usage
 ```python
 import pi_spm
 import os
 import sys
 from msvcrt import getch
```

### Comparing `Python-piSPM-7.7.0/pi_spm/__init__.py` & `Python-piSPM-7.7.0.1/pi_spm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,30 +522,30 @@
         return err, int(initialState.value)
 
     # New since April 2023
     # #
     # # Protection functions
     # #
 
-    def spm_protectionResetEnable(self, chassis, timeoutInSeconds):
-        err = self.__handleSPM.SPM_ProtectionResetEnable(c_int(chassis), c_int(timeoutInSeconds))
+    def spm_protectionResetEnable(self, chassisNumber, timeoutInSeconds):
+        err = self.__handleSPM.SPM_ProtectionResetEnable(c_int(chassisNumber), c_int(timeoutInSeconds))
         return err
 
     def spm_protectionResetDisable(self, chassisNumber):
         err = self.__handleSPM.SPM_ProtectionResetDisable(c_int(chassisNumber))
         return err
     
-    def spm_getProtectionResetEnabled(self, chassis):
+    def spm_getProtectionResetEnabled(self, chassisNumber):
         state = c_int(0)
-        err = self.__handleSPM.SPM_GetProtectionResetEnabled(chassis, byref(state))
+        err = self.__handleSPM.SPM_GetProtectionResetEnabled(c_int(chassisNumber), byref(state))
         return err, state.value
     
-    def spm_getProtectionResetTimeout(self, chassis):
+    def spm_getProtectionResetTimeout(self, chassisNumber):
         timeout = c_int(0)
-        err = self.__handleSPM.SPM_GetProtectionResetTimeout(self, chassis, byref(timeout))
+        err = self.__handleSPM.SPM_GetProtectionResetTimeout(self, c_int(chassisNumber), byref(timeout))
         return err, timeout.value
 
     # #
     # # Sequencing Functions
     # #
     def sequence_start(self, disable_notification, project_file,
                        reset, boot_online, show_endmsg, open_close_IDE, reload_prj):
```

