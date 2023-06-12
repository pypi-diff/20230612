# Comparing `tmp/getRoutersConfig-0.0.5.tar.gz` & `tmp/getRoutersConfig-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getRoutersConfig-0.0.5.tar", last modified: Sat Jun 10 14:19:01 2023, max compression
+gzip compressed data, was "getRoutersConfig-0.0.6.tar", last modified: Mon Jun 12 18:56:37 2023, max compression
```

## Comparing `getRoutersConfig-0.0.5.tar` & `getRoutersConfig-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.137152 getRoutersConfig-0.0.5/
--rw-rw-rw-   0        0        0     1092 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5286 2023-06-10 14:19:01.135157 getRoutersConfig-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       50 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.091156 getRoutersConfig-0.0.5/app/
-drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.104153 getRoutersConfig-0.0.5/app/getRoutersConfig/
--rw-rw-rw-   0        0        0       48 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.132157 getRoutersConfig-0.0.5/app/getRoutersConfig/src/
--rw-rw-rw-   0        0        0    11721 2023-06-10 12:41:37.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/CiscoClass.py
--rw-rw-rw-   0        0        0     1281 2023-06-10 12:54:23.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/HuaweiClass.py
--rw-rw-rw-   0        0        0     1216 2023-06-10 12:08:16.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/RouterClass.py
--rw-rw-rw-   0        0        0        0 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-05-30 15:46:22.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/main.py
--rw-rw-rw-   0        0        0      601 2023-06-10 12:42:51.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.116157 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/
--rw-rw-rw-   0        0        0     5286 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 14:19:01.137152 getRoutersConfig-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-03 10:07:23.000000 getRoutersConfig-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.292899 getRoutersConfig-0.0.6/
+-rw-rw-rw-   0        0        0     1092 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5294 2023-06-12 18:56:37.291898 getRoutersConfig-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.250900 getRoutersConfig-0.0.6/app/
+drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.259898 getRoutersConfig-0.0.6/app/getRoutersConfig/
+-rw-rw-rw-   0        0        0       48 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.289900 getRoutersConfig-0.0.6/app/getRoutersConfig/src/
+-rw-rw-rw-   0        0        0    11727 2023-06-12 16:51:26.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/CiscoClass.py
+-rw-rw-rw-   0        0        0     9156 2023-06-12 18:56:34.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/HuaweiClass.py
+-rw-rw-rw-   0        0        0     1216 2023-06-10 12:08:16.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/RouterClass.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-05-30 15:46:22.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/main.py
+-rw-rw-rw-   0        0        0      601 2023-06-10 12:42:51.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.272900 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/
+-rw-rw-rw-   0        0        0     5294 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:56:37.292899 getRoutersConfig-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-06-10 14:20:15.000000 getRoutersConfig-0.0.6/setup.py
```

### Comparing `getRoutersConfig-0.0.5/LICENSE` & `getRoutersConfig-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.5/PKG-INFO` & `getRoutersConfig-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.5
+Version: 0.0.6
 Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -54,21 +54,21 @@
     },
     "system_image": "c800-universalk9-mz.SPA.154-3.M6.bin",
     "serial_number": "FCZ1234A5BC",
     "config_register": "0x2102"
 }
 ```
 
-# Get static routes
+# Get Ipv4 static routes
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
-static_routes = router.getStaticRoutes()
+static_routes = router.getIpv4StaticRoutes()
 
 router.disconnect()
 ```
 
 The Schema is :
 ```json
 [
@@ -173,15 +173,15 @@
 
 # Get ACL
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
-dhcp = router.getIpv4Acl()
+acl = router.getIpv4Acl()
 
 router.disconnect()
 ```
 
 The Schema is :
 ```json
```

### Comparing `getRoutersConfig-0.0.5/app/getRoutersConfig/src/CiscoClass.py` & `getRoutersConfig-0.0.6/app/getRoutersConfig/src/CiscoClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,22 +41,22 @@
         output = self.net_connect.send_command(f"show version")
 
         re_serie_version = r'Cisco IOS Software, (?P<serie>\S+) Software (\S+), Version (?P<version>\S+), RELEASE SOFTWARE \S+'
         re_hostname_uptime = r'(?P<hostname>\S+) uptime is( (?P<years>\d+) year(s)?,)?( (?P<weeks>\d+) week(s)?,)?( (?P<days>\d+) day(s)?,)?( (?P<hours>\d+) hour(s)?,)?( (?P<minutes>\d+) minute(s)?)?'
         re_system_image = r'System image file is "flash:(?P<system_image>\S+)"'
         re_model = r'Cisco (?P<model>\S+) \(revision \S+\) with \S+ bytes of memory.'
         re_serial_number = r'Processor board ID (?P<serial_number>\S+)'
-        re_config_register = r'Configuration register is (?P<config_register>\S+)'
+        # re_config_register = r'Configuration register is (?P<config_register>\S+)'
 
         match_serie_version = re.search(re_serie_version, output, flags=re.M)
         match_hostname_uptime = re.search(re_hostname_uptime, output, flags=re.M)
         match_system_image = re.search(re_system_image, output, flags=re.M)
         match_model = re.search(re_model, output, flags=re.M)
         match_serial_number = re.search(re_serial_number, output, flags=re.M)
-        match_config_register = re.search(re_config_register, output, flags=re.M)
+        # match_config_register = re.search(re_config_register, output, flags=re.M)
 
         return {
             "serie": match_serie_version.group('serie'),
             "model": match_model.group('model'),
             "version": match_serie_version.group('version'),
             "hostname": match_hostname_uptime.group('hostname'),
             "uptime": {
@@ -64,15 +64,15 @@
                 "weeks": int(match_hostname_uptime.group('weeks')) if match_hostname_uptime.group('weeks') else 0,
                 "days": int(match_hostname_uptime.group('days')) if match_hostname_uptime.group('days') else 0,
                 "hours": int(match_hostname_uptime.group('hours')) if match_hostname_uptime.group('hours') else 0,
                 "minutes": int(match_hostname_uptime.group('minutes')),
             },
             "system_image": match_system_image.group('system_image'),
             "serial_number": match_serial_number.group('serial_number'),
-            "config_register": match_config_register.group('config_register'),
+            # "config_register": match_config_register.group('config_register'),
         }
 
     
 
     def getInterfaces(self) -> list:
         output_v4 = self.net_connect.send_command('show ip interface')
         v4_interfaces = [{
```

### Comparing `getRoutersConfig-0.0.5/app/getRoutersConfig/src/RouterClass.py` & `getRoutersConfig-0.0.6/app/getRoutersConfig/src/RouterClass.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.5/app/getRoutersConfig/src/main.py` & `getRoutersConfig-0.0.6/app/getRoutersConfig/src/main.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.5/app/getRoutersConfig/src/tools.py` & `getRoutersConfig-0.0.6/app/getRoutersConfig/src/tools.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/PKG-INFO` & `getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.5
+Version: 0.0.6
 Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -54,21 +54,21 @@
     },
     "system_image": "c800-universalk9-mz.SPA.154-3.M6.bin",
     "serial_number": "FCZ1234A5BC",
     "config_register": "0x2102"
 }
 ```
 
-# Get static routes
+# Get Ipv4 static routes
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
-static_routes = router.getStaticRoutes()
+static_routes = router.getIpv4StaticRoutes()
 
 router.disconnect()
 ```
 
 The Schema is :
 ```json
 [
@@ -173,15 +173,15 @@
 
 # Get ACL
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
-dhcp = router.getIpv4Acl()
+acl = router.getIpv4Acl()
 
 router.disconnect()
 ```
 
 The Schema is :
 ```json
```

### Comparing `getRoutersConfig-0.0.5/setup.py` & `getRoutersConfig-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="getRoutersConfig",
-    version="0.0.5",
+    version="0.0.6",
     description="get Cisco routers configuration as Json",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanielRicklin/getRoutersConfig",
     author="DanielRicklin",
```

