# Comparing `tmp/wiliot-core-4.0.8.tar.gz` & `tmp/wiliot-core-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-core-4.0.8.tar", last modified: Tue Apr 25 08:27:47 2023, max compression
+gzip compressed data, was "wiliot-core-4.0.9.tar", last modified: Tue May  9 21:05:54 2023, max compression
```

## Comparing `wiliot-core-4.0.8.tar` & `wiliot-core-4.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3247 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2735 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1834 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core/
--rw-rw-rw-   0 root         (0) root         (0)     4596 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core/local_gateway/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13748 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/continuous_listener.py
--rw-rw-rw-   0 root         (0) root         (0)    12763 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/custom_energy_pattern.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core/local_gateway/examples/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/examples/local_gateway_basic_example.py
--rw-rw-rw-   0 root         (0) root         (0)    86026 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.385662 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/
--rw-rw-rw-   0 root         (0) root         (0)   253422 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   448599 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   122153 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   317338 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   229471 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   424656 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)  1242814 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
--rw-rw-rw-   0 root         (0) root         (0)  1176930 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/wiliot_core/packet_data/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26863 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/packet.py
--rw-rw-rw-   0 root         (0) root         (0)    29498 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/packet_list.py
--rw-rw-rw-   0 root         (0) root         (0)    10335 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/tag_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/wiliot_core/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)     9296 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/release_for_partners.py
--rw-rw-rw-   0 root         (0) root         (0)    14010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/update_wiliot_packages.py
--rw-rw-rw-   0 root         (0) root         (0)    12888 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3247 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-25 08:27:47.000000 wiliot-core-4.0.8/wiliot_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.965118 wiliot-core-4.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2023-05-09 21:05:54.965118 wiliot-core-4.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-09 21:05:54.965118 wiliot-core-4.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.957118 wiliot-core-4.0.9/wiliot_core/
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.957118 wiliot-core-4.0.9/wiliot_core/local_gateway/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13748 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/continuous_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)    12763 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/custom_energy_pattern.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.957118 wiliot-core-4.0.9/wiliot_core/local_gateway/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/examples/local_gateway_basic_example.py
+-rw-rw-rw-   0 root         (0) root         (0)    86162 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.965118 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/
+-rw-rw-rw-   0 root         (0) root         (0)   253422 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   448599 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   122153 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   317338 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   229471 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   424656 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)  1242814 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
+-rw-rw-rw-   0 root         (0) root         (0)  1176930 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.965118 wiliot-core-4.0.9/wiliot_core/packet_data/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/packet_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26862 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/packet_data/packet.py
+-rw-rw-rw-   0 root         (0) root         (0)    29498 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/packet_data/packet_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    10335 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/packet_data/tag_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.965118 wiliot-core-4.0.9/wiliot_core/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     9296 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/utils/release_for_partners.py
+-rw-rw-rw-   0 root         (0) root         (0)    14010 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/utils/update_wiliot_packages.py
+-rw-rw-rw-   0 root         (0) root         (0)    13980 2023-05-09 21:05:38.000000 wiliot-core-4.0.9/wiliot_core/utils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-09 21:05:54.000000 wiliot-core-4.0.9/wiliot_core/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 21:05:54.957118 wiliot-core-4.0.9/wiliot_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2023-05-09 21:05:54.000000 wiliot-core-4.0.9/wiliot_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-05-09 21:05:54.000000 wiliot-core-4.0.9/wiliot_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 21:05:54.000000 wiliot-core-4.0.9/wiliot_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 21:05:54.000000 wiliot-core-4.0.9/wiliot_core.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-05-09 21:05:54.000000 wiliot-core-4.0.9/wiliot_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-09 21:05:54.000000 wiliot-core-4.0.9/wiliot_core.egg-info/top_level.txt
```

### Comparing `wiliot-core-4.0.8/LICENSE` & `wiliot-core-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/PKG-INFO` & `wiliot-core-4.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-core
-Version: 4.0.8
+Version: 4.0.9
 Summary: A library for interacting with Wiliot's private core functions
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -56,14 +56,19 @@
 * [gateway communication](wiliot_core/local_gateway/examples)
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
+Version 4.0.9:
+-----------------
+* improve Wiliot Dir
+* add support to multiple api keys for the same owner id and environment bud different clients
+  
 Version 4.0.8:
 -----------------
 * continuous listener as multi-processes:
     * add option to specify log path and communicate reading error using event
     * connect to gw in a more robust way including printing exceptions if needed
 * local gw core:
     * connect only to “Silicon Lab”/"CP210.." ports (Wiliot's gw driver)
```

### Comparing `wiliot-core-4.0.8/README.md` & `wiliot-core-4.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 * [gateway communication](wiliot_core/local_gateway/examples)
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
+Version 4.0.9:
+-----------------
+* improve Wiliot Dir
+* add support to multiple api keys for the same owner id and environment bud different clients
+  
 Version 4.0.8:
 -----------------
 * continuous listener as multi-processes:
     * add option to specify log path and communicate reading error using event
     * connect to gw in a more robust way including printing exceptions if needed
 * local gw core:
     * connect only to “Silicon Lab”/"CP210.." ports (Wiliot's gw driver)
```

### Comparing `wiliot-core-4.0.8/bitbucket-pipelines.yml` & `wiliot-core-4.0.9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/setup.py` & `wiliot-core-4.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/__init__.py` & `wiliot-core-4.0.9/wiliot_core/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/__init__.py` & `wiliot-core-4.0.9/wiliot_core/local_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/continuous_listener.py` & `wiliot-core-4.0.9/wiliot_core/local_gateway/continuous_listener.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/custom_energy_pattern.py` & `wiliot-core-4.0.9/wiliot_core/local_gateway/custom_energy_pattern.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/examples/__init__.py` & `wiliot-core-4.0.9/wiliot_core/local_gateway/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/examples/local_gateway_basic_example.py` & `wiliot-core-4.0.9/wiliot_core/local_gateway/examples/local_gateway_basic_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_core.py` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,14 +535,16 @@
                     data_in['raw'] += '\n{}'.format(data_in_3rd_row['raw'])
                 except Exception as e:
                     print('could not found a second/third row to gw respond {}'.format(e))
 
             if "unsupported" in data_in['raw'].lower():
                 is_ack = False
             else:
+                if isinstance(cmd, bytes):
+                    cmd = cmd.decode()
                 is_ack = any([s in cmd for s in cmds_no_default_ack]) or \
                          "command complete event" in data_in['raw'].lower()
 
             return data_in, is_ack
         else:
             is_ack = True
             data = self.readline_from_buffer()
@@ -650,14 +652,17 @@
                     self.connected = self._comPortObj.isOpen()
             except Exception as e:
                 self._printing_func('Exception during close_port:{}'.format(e), 'close_port')
         else:
             self._printing_func('The gateway is already disconnected', 'close_port')
 
     def get_read_error_status(self):
+        """
+        :return True if we got error during reading
+        """
         if self.multi_process:
             self.reading_exception = self.read_error_event.is_set()
             self.read_error_event.clear()
         current_reading_exception = self.reading_exception
         self.reading_exception = False  # reset flag
         return current_reading_exception
 
@@ -1020,17 +1025,15 @@
                     self.config_param.time_profile_period = time_profile_val[1]
 
         # set Beacons Backoff:
         if beacons_backoff_val is not None:
             if combined_msg:
                 combined_msg_str += ' bb {}'.format(beacons_backoff_val)
             else:
-                gateway_response = self.write(
-                    bytes('!beacons_backoff {}\r\n'.format(beacons_backoff_val), encoding='utf-8'),
-                    with_ack=with_ack)
+                gateway_response = self.write('!beacons_backoff {}\r\n'.format(beacons_backoff_val), with_ack=with_ack)
                 gateway_response['command'] = '!beacons_backoff {}\r\n'.format(beacons_backoff_val)
                 gateway_output.append(gateway_response)
 
                 if 'unsupported' in gateway_response['raw'].lower():
                     self.config_param.beacons_backoff = None
                 else:
                     self.config_param.beacons_backoff = beacons_backoff_val
@@ -1824,10 +1827,11 @@
     print(datetime.datetime.now())
     gw = WiliotGateway(auto_connect=True, is_multi_processes=True)
     if gw.is_connected():
         # gw.start_continuous_listener()
         gw.reset_gw(reset_port=False)
         print(f'is gw alive {gw.is_gw_alive()}')
         print(gw.write('!set_tester_mode 1', with_ack=True))
-        gw.config_gw(energy_pattern_val=18, time_profile_val=[5, 15], effective_output_power_val=22)
+        gw.config_gw(energy_pattern_val=18, time_profile_val=[5, 15], effective_output_power_val=22,
+                     beacons_backoff_val=0)
     print(datetime.datetime.now())
     gw.exit_gw_api()
```

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex` & `wiliot-core-4.0.9/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/packet_data/__init__.py` & `wiliot-core-4.0.9/wiliot_core/packet_data/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/packet_data/packet.py` & `wiliot-core-4.0.9/wiliot_core/packet_data/packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,14 @@
     def get_adva(self):
         return self.packet_data['adv_address']
 
     def get_flow(self):
         flow_version = hex(int(self.packet_data['flow_ver'], 16))
         return flow_version
 
-
     def get_rssi(self):
         return str(self.gw_data['rssi'])
 
     def get_packet_data_names(self):
         """
         extract all keys name which can potentially be a column in packet df
         :return:
```

### Comparing `wiliot-core-4.0.8/wiliot_core/packet_data/packet_list.py` & `wiliot-core-4.0.9/wiliot_core/packet_data/packet_list.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/packet_data/tag_collection.py` & `wiliot-core-4.0.9/wiliot_core/packet_data/tag_collection.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/utils/get_version.py` & `wiliot-core-4.0.9/wiliot_core/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/utils/release_for_partners.py` & `wiliot-core-4.0.9/wiliot_core/utils/release_for_partners.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/utils/update_wiliot_packages.py` & `wiliot-core-4.0.9/wiliot_core/utils/update_wiliot_packages.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.8/wiliot_core/utils/utils.py` & `wiliot-core-4.0.9/wiliot_core/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,19 +88,19 @@
     def set_dir(self):
         try:
             if 'WILIOT_APP_ROOT_PATH' in os.environ.keys():
                 print(os.environ['WILIOT_APP_ROOT_PATH'])
                 self.wiliot_root_path = os.environ['WILIOT_APP_ROOT_PATH']
             else:
                 self.local_appdata_dir = user_data_dir()
-                self.wiliot_root_path = os.path.join(self.local_appdata_dir, 'wiliot')
+                self.wiliot_root_path = os.path.abspath(os.path.join(self.local_appdata_dir, 'wiliot'))
             
-            self.common_dir_path = os.path.join(self.wiliot_root_path, 'common')
-            self.config_dir_path = os.path.join(self.common_dir_path, 'configs')
-            self.user_config_path = os.path.join(self.config_dir_path, 'user_configs.json')
+            self.common_dir_path = os.path.abspath(os.path.join(self.wiliot_root_path, 'common'))
+            self.config_dir_path = os.path.abspath(os.path.join(self.common_dir_path, 'configs'))
+            self.user_config_path = os.path.abspath(os.path.join(self.config_dir_path, 'user_configs.json'))
         
         except Exception as e:
             logging.warning('Error loading environment or getting in from OS, supporting Windows, Linux and MacOS '
                             '({})'.format(e))
     
     @staticmethod
     def create_dir(path):
@@ -112,31 +112,33 @@
         self.create_dir(tester_path)
         
         for subdir in self.tester_subdirectories:
             self.create_dir(tester_path + '/' + subdir)
     
     def get_tester_dir(self, tester_name):
         wiliot_path = self.wiliot_root_path
-        tester_path = os.path.join(wiliot_path, tester_name)
+        tester_path = os.path.abspath(os.path.join(wiliot_path, tester_name))
         return tester_path
     
     def get_dir(self):
         return self.wiliot_root_path, self.common_dir_path, self.config_dir_path, self.user_config_path
     
     def get_wiliot_root_app_dir(self):
         return self.wiliot_root_path
     
     def get_common_dir(self):
         return self.common_dir_path
     
     def get_config_dir(self):
         return self.config_dir_path
     
-    def get_user_config_file(self):
-        return self.user_config_path
+    def get_user_config_file(self, client_type=None):
+        if client_type is None:
+            return self.user_config_path
+        return self.user_config_path.replace('.json', f'_{client_type}.json')
 
 
 def open_json(folder_path, file_path, default_values=None):
     """
     opens config json
     :type folder_path: string
     :param folder_path: the folder path which contains the desired file
@@ -165,20 +167,28 @@
                 json.dump(default_values, out_file)
             json_content = json.load(open(file_path, "rb"))
         else:
             json_content = json.loads(json_content)
         return json_content
 
 
-def credentials_gui():
+def credentials_gui(client_type=None):
     """
     open GUI for getting api_key from user
+    :param client_type: the cloud client type. relevant if you have different api key for several client,
+                       which will be save in different yser_config files
+    :type client_type: str
+    :return: the user input, dict with api_key, owner_id and env
+    :rtype: dict
     """
+    if client_type is None:
+        client_type = 'DEFAULT'
     layout = [
         [SimGUI.Text('Please enter your Wiliot API key')],
+        [SimGUI.Text(f'Client Type: {client_type}')],
         [SimGUI.Text('API key:'),
          SimGUI.InputText('', key='api_key')],
         [SimGUI.Text('owner id (optional):'),
          SimGUI.InputText('', key='owner_id')],
         [SimGUI.Text('environment (optional):'),
          SimGUI.InputCombo(('prod', 'non-prod'), default_value='prod', key='env')],
         [SimGUI.Submit()]]
@@ -193,32 +203,37 @@
             window.close()
             break
     
     window.close()
     return values
 
 
-def check_user_config_is_ok(owner_id=None, env=None):
+def check_user_config_is_ok(owner_id=None, env=None, client_type=None):
     """
     check user credentials
-    :param owner_id:
+    :param owner_id: use the key of the specified owner id
     :type owner_id: str or None
-    :param env:
+    :param env: use the key of the specified environment
     :type env: str or None
-    :return:
-    :rtype:
+    :param client_type: if specified the credential will be read/write from the same use config file,
+                        but with the specified suffix
+    :type client_type: str or None
+    :return: user_config_file_path - the file path,
+             api_key -the key,
+             is_success - True if the credentials we entered correctly
+    :rtype: tuple
     """
     # Create wiliot appdata directory if not exists:
     is_success = True
     auth_gui_is_needed = False
     api_key = None
     cfg_data = []
     env_dirs = WiliotDir()
     config_dir_path = env_dirs.get_config_dir()
-    user_config_file_path = env_dirs.get_user_config_file()
+    user_config_file_path = env_dirs.get_user_config_file(client_type)
     if env is not None:
         env = env.lower()
     if env == '':
         env = 'prod'
     if env is not None and ('test' in env or 'dev' in env):
         env = 'non-prod'
     
@@ -251,15 +266,15 @@
                 user_config_file_path, e))
     else:
         print("Config file user_configs.json doesn't exist at {}\n".format(config_dir_path))
         auth_gui_is_needed = True
     
     while auth_gui_is_needed:
         auth_gui_is_needed = False
-        values = credentials_gui()
+        values = credentials_gui(client_type)
         api_key = values['api_key']
         if api_key == '':
             print('api key is missing. Please try again\n')
             auth_gui_is_needed = True
         elif api_key is None:
             is_success = False
         else:
```

### Comparing `wiliot-core-4.0.8/wiliot_core.egg-info/PKG-INFO` & `wiliot-core-4.0.9/wiliot_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-core
-Version: 4.0.8
+Version: 4.0.9
 Summary: A library for interacting with Wiliot's private core functions
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -56,14 +56,19 @@
 * [gateway communication](wiliot_core/local_gateway/examples)
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
+Version 4.0.9:
+-----------------
+* improve Wiliot Dir
+* add support to multiple api keys for the same owner id and environment bud different clients
+  
 Version 4.0.8:
 -----------------
 * continuous listener as multi-processes:
     * add option to specify log path and communicate reading error using event
     * connect to gw in a more robust way including printing exceptions if needed
 * local gw core:
     * connect only to “Silicon Lab”/"CP210.." ports (Wiliot's gw driver)
```

### Comparing `wiliot-core-4.0.8/wiliot_core.egg-info/SOURCES.txt` & `wiliot-core-4.0.9/wiliot_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

