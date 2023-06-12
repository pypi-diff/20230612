# Comparing `tmp/RobertCommonDriver-0.1.42.tar.gz` & `tmp/RobertCommonDriver-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.42.tar", last modified: Fri Jun  9 09:58:37 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.43.tar", last modified: Mon Jun 12 02:27:56 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.42.tar` & `RobertCommonDriver-0.1.43.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.113941 RobertCommonDriver-0.1.42/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.42/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.42/MANIFEST.in
--rw-rw-rw-   0        0        0      850 2023-06-09 09:58:37.112593 RobertCommonDriver-0.1.42/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.42/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.030483 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0      850 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-09 09:58:36.000000 RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.42/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.031483 RobertCommonDriver-0.1.42/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.42/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.032485 RobertCommonDriver-0.1.42/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.045996 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38348 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.067191 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    68887 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566106 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    61893 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-06-09 09:58:37.113941 RobertCommonDriver-0.1.42/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-06-09 09:33:34.000000 RobertCommonDriver-0.1.42/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.068615 RobertCommonDriver-0.1.42/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.42/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.068615 RobertCommonDriver-0.1.42/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.42/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.082620 RobertCommonDriver-0.1.42/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:58:37.111478 RobertCommonDriver-0.1.42/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.451947 RobertCommonDriver-0.1.43/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.43/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.43/MANIFEST.in
+-rw-rw-rw-   0        0        0      850 2023-06-12 02:27:56.450941 RobertCommonDriver-0.1.43/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-02 07:57:02.000000 RobertCommonDriver-0.1.43/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.359636 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-12 02:27:56.000000 RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.43/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.359636 RobertCommonDriver-0.1.43/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.43/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.360610 RobertCommonDriver-0.1.43/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.379169 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87436 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6074 2023-06-09 02:14:48.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38348 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60844 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17038 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15983 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33512 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16600 2023-06-08 07:41:58.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.405483 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    68907 2023-06-12 02:27:00.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    65695 2023-06-09 08:26:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566106 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46883 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    34014 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18268 2023-06-09 08:36:24.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    61893 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24773 2023-06-09 08:44:21.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43247 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51493 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41509 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32738 2023-06-09 09:05:11.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44863 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    12926 2023-06-09 08:55:51.000000 RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 02:27:56.451947 RobertCommonDriver-0.1.43/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-06-12 02:27:36.000000 RobertCommonDriver-0.1.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.407484 RobertCommonDriver-0.1.43/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.43/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.408485 RobertCommonDriver-0.1.43/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.43/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.424264 RobertCommonDriver-0.1.43/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:27:56.449940 RobertCommonDriver-0.1.43/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22758 2023-05-22 08:58:48.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15816 2023-05-23 12:02:23.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4707 2023-06-01 02:58:21.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     9628 2023-05-25 08:18:30.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.42/LICENSE` & `RobertCommonDriver-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/PKG-INFO` & `RobertCommonDriver-0.1.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.42
+Version: 0.1.43
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.42
+Version: 0.1.43
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `RobertCommonDriver-0.1.42/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.43/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1626,14 +1626,15 @@
     def get_write_result(self):
         return 'write_result'
 
     def update_results(self, names: Optional[Union[str, list]], quality: bool, result: Optional[Any], **kwargs):
         """更新结果集"""
         if quality is True and result is None:
             self.results = {'count': len(names), 'success': {}, 'error': {}, 'start': IOTBaseCommon.get_datetime()}
+            return
 
         if isinstance(names, str):
             names = [names]
         if isinstance(names, list):
             for name in names:
                 if quality is True:
                     self.results['success'][name] = result
```

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.43/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/setup.py` & `RobertCommonDriver-0.1.43/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.42'
-DATE = '2023-06-09'
+VERSION = '0.1.43'
+DATE = '2023-06-12'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.42/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.43/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

