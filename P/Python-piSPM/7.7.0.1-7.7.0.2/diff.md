# Comparing `tmp/Python-piSPM-7.7.0.1.tar.gz` & `tmp/Python-piSPM-7.7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-piSPM-7.7.0.1.tar", last modified: Mon Jun 12 08:50:43 2023, max compression
+gzip compressed data, was "Python-piSPM-7.7.0.2.tar", last modified: Mon Jun 12 10:39:29 2023, max compression
```

## Comparing `Python-piSPM-7.7.0.1.tar` & `Python-piSPM-7.7.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 08:50:43.130282 Python-piSPM-7.7.0.1/
--rw-rw-rw-   0        0        0     1093 2023-03-06 08:59:01.000000 Python-piSPM-7.7.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     7048 2023-06-12 08:50:43.129282 Python-piSPM-7.7.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 08:50:43.128283 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/
--rw-rw-rw-   0        0        0     7048 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 08:50:43.000000 Python-piSPM-7.7.0.1/Python_piSPM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5464 2023-06-12 08:44:29.000000 Python-piSPM-7.7.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 08:50:43.128283 Python-piSPM-7.7.0.1/pi_spm/
--rw-rw-rw-   0        0        0    25901 2023-06-12 08:42:37.000000 Python-piSPM-7.7.0.1/pi_spm/__init__.py
--rw-rw-rw-   0        0        0      382 2023-06-12 08:46:46.000000 Python-piSPM-7.7.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 08:50:43.130282 Python-piSPM-7.7.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 10:39:29.684503 Python-piSPM-7.7.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-03-06 08:59:01.000000 Python-piSPM-7.7.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     7058 2023-06-12 10:39:29.684503 Python-piSPM-7.7.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 10:39:29.682504 Python-piSPM-7.7.0.2/Python_piSPM.egg-info/
+-rw-rw-rw-   0        0        0     7058 2023-06-12 10:39:29.000000 Python-piSPM-7.7.0.2/Python_piSPM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-12 10:39:29.000000 Python-piSPM-7.7.0.2/Python_piSPM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:39:29.000000 Python-piSPM-7.7.0.2/Python_piSPM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 10:39:29.000000 Python-piSPM-7.7.0.2/Python_piSPM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 10:39:29.000000 Python-piSPM-7.7.0.2/Python_piSPM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5474 2023-06-12 10:38:34.000000 Python-piSPM-7.7.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:39:29.683503 Python-piSPM-7.7.0.2/pi_spm/
+-rw-rw-rw-   0        0        0    25895 2023-06-12 10:37:45.000000 Python-piSPM-7.7.0.2/pi_spm/__init__.py
+-rw-rw-rw-   0        0        0      382 2023-06-12 10:38:44.000000 Python-piSPM-7.7.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:39:29.684503 Python-piSPM-7.7.0.2/setup.cfg
```

### Comparing `Python-piSPM-7.7.0.1/LICENSE.txt` & `Python-piSPM-7.7.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Python-piSPM-7.7.0.1/PKG-INFO` & `Python-piSPM-7.7.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-piSPM
-Version: 7.7.0.1
+Version: 7.7.0.2
 Summary: Python piSPM is a Python wrapper for Pickering Switch Path Manager.
 Author-email: Pickering Interfaces <support@pickeringtest.com>
 License: Copyright (c) 2017-2023 Pickering Interfaces Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -30,15 +30,15 @@
 # Python SPM
 Python SPM is a Python wrapper for Pickering Switch Path Manager.
 
 **Pickering Switch Path Manager is needed for the wrapper to work**
 - [Switch Path Manager]https://downloads.pickeringtest.info/downloads/Switch%20Path%20Manager/
 
 ## Changelog
-> - 7.7.0.1 - Minor bugfix for protection functions
+> - 7.7.0.1 = 7.7.0.2 - Minor bugfix for protection functions
 > - 7.7.0 - Added protection functions
 
 ## Example usage
 ```python
 import pi_spm
 import os
 import sys
```

### Comparing `Python-piSPM-7.7.0.1/Python_piSPM.egg-info/PKG-INFO` & `Python-piSPM-7.7.0.2/Python_piSPM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-piSPM
-Version: 7.7.0.1
+Version: 7.7.0.2
 Summary: Python piSPM is a Python wrapper for Pickering Switch Path Manager.
 Author-email: Pickering Interfaces <support@pickeringtest.com>
 License: Copyright (c) 2017-2023 Pickering Interfaces Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -30,15 +30,15 @@
 # Python SPM
 Python SPM is a Python wrapper for Pickering Switch Path Manager.
 
 **Pickering Switch Path Manager is needed for the wrapper to work**
 - [Switch Path Manager]https://downloads.pickeringtest.info/downloads/Switch%20Path%20Manager/
 
 ## Changelog
-> - 7.7.0.1 - Minor bugfix for protection functions
+> - 7.7.0.1 = 7.7.0.2 - Minor bugfix for protection functions
 > - 7.7.0 - Added protection functions
 
 ## Example usage
 ```python
 import pi_spm
 import os
 import sys
```

### Comparing `Python-piSPM-7.7.0.1/README.md` & `Python-piSPM-7.7.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Python SPM
 Python SPM is a Python wrapper for Pickering Switch Path Manager.
 
 **Pickering Switch Path Manager is needed for the wrapper to work**
 - [Switch Path Manager]https://downloads.pickeringtest.info/downloads/Switch%20Path%20Manager/
 
 ## Changelog
-> - 7.7.0.1 - Minor bugfix for protection functions
+> - 7.7.0.1 = 7.7.0.2 - Minor bugfix for protection functions
 > - 7.7.0 - Added protection functions
 
 ## Example usage
 ```python
 import pi_spm
 import os
 import sys
```

### Comparing `Python-piSPM-7.7.0.1/pi_spm/__init__.py` & `Python-piSPM-7.7.0.2/pi_spm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,15 +537,15 @@
     def spm_getProtectionResetEnabled(self, chassisNumber):
         state = c_int(0)
         err = self.__handleSPM.SPM_GetProtectionResetEnabled(c_int(chassisNumber), byref(state))
         return err, state.value
     
     def spm_getProtectionResetTimeout(self, chassisNumber):
         timeout = c_int(0)
-        err = self.__handleSPM.SPM_GetProtectionResetTimeout(self, c_int(chassisNumber), byref(timeout))
+        err = self.__handleSPM.SPM_GetProtectionResetTimeout(c_int(chassisNumber), byref(timeout))
         return err, timeout.value
 
     # #
     # # Sequencing Functions
     # #
     def sequence_start(self, disable_notification, project_file,
                        reset, boot_online, show_endmsg, open_close_IDE, reload_prj):
```

