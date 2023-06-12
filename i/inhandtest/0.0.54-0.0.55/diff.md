# Comparing `tmp/inhandtest-0.0.54.tar.gz` & `tmp/inhandtest-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.54.tar", last modified: Mon Jun 12 05:26:05 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.55.tar", last modified: Mon Jun 12 09:13:43 2023, max compression
```

## Comparing `inhandtest-0.0.54.tar` & `inhandtest-0.0.55.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.54/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-06-12 05:26:05.000000 inhandtest-0.0.54/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.54/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/dm/
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.54/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.54/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.54/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.54/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.54/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.54/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.54/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    59214 2023-06-12 05:21:09.000000 inhandtest-0.0.54/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    23673 2023-06-08 06:22:30.000000 inhandtest-0.0.54/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.54/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.54/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.54/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.54/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.54/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    52197 2023-06-07 03:52:54.000000 inhandtest-0.0.54/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7820 2023-06-07 06:08:07.000000 inhandtest-0.0.54/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.54/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.54/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.54/inhandtest/ip.py
--rw-rw-rw-   0        0        0    13255 2023-06-08 01:52:07.000000 inhandtest-0.0.54/inhandtest/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.54/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3179 2023-06-12 05:22:56.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.54/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    33345 2023-06-09 09:37:50.000000 inhandtest-0.0.54/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    27509 2023-06-07 03:54:00.000000 inhandtest-0.0.54/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.54/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 05:26:05.000000 inhandtest-0.0.54/setup.cfg
--rw-rw-rw-   0        0        0     1626 2023-06-12 05:25:50.000000 inhandtest-0.0.54/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.55/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-06-12 09:13:42.000000 inhandtest-0.0.55/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.55/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/dm/
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.55/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.55/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.55/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.55/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.55/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.55/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.55/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    59214 2023-06-12 05:21:09.000000 inhandtest-0.0.55/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    23673 2023-06-08 06:22:30.000000 inhandtest-0.0.55/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.55/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.55/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.55/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.55/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.55/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    52197 2023-06-07 03:52:54.000000 inhandtest-0.0.55/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7820 2023-06-07 06:08:07.000000 inhandtest-0.0.55/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.55/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.55/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.55/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    13416 2023-06-12 09:13:16.000000 inhandtest-0.0.55/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.55/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.55/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3150 2023-06-12 08:58:41.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.55/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    33264 2023-06-12 08:58:41.000000 inhandtest-0.0.55/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    27509 2023-06-07 03:54:00.000000 inhandtest-0.0.55/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1667 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.55/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:13:42.000000 inhandtest-0.0.55/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-06-12 09:13:16.000000 inhandtest-0.0.55/setup.py
```

### Comparing `inhandtest-0.0.54/PKG-INFO` & `inhandtest-0.0.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.54
+Version: 0.0.55
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.54/README.md` & `inhandtest-0.0.55/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/dm/mqtt.py` & `inhandtest-0.0.55/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/dm/register_v1.py` & `inhandtest-0.0.55/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.55/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.55/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.55/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/base_page/base_page.py` & `inhandtest-0.0.55/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.55/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/exception.py` & `inhandtest-0.0.55/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/file.py` & `inhandtest-0.0.55/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/inmodbus.py` & `inhandtest-0.0.55/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/inmongodb.py` & `inhandtest-0.0.55/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/inmqtt.py` & `inhandtest-0.0.55/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/inrequest.py` & `inhandtest-0.0.55/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/inserial.py` & `inhandtest-0.0.55/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/insocket.py` & `inhandtest-0.0.55/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/inssh.py` & `inhandtest-0.0.55/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/ip.py` & `inhandtest-0.0.55/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/mail.py` & `inhandtest-0.0.55/inhandtest/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,25 +32,14 @@
                              host: 必填 测试主机， 10.5.24.107
                              port： 必填 分享报告端口， 63330
                              allure_results_path: 必填 报告中的/allure-results 路径
 
     :return:
     """
     port = render.get('port') if render.get('port') else 63330
-    # 杀掉端口, 防止端口占用
-    kill_windows_port(render.get('host'), [port, port + 1])  # port+1 是https端口
-    # 启动本地服务，分享报告
-    p = subprocess.Popen(f'npx anywhere -h {render.get("host")} -p {port}', cwd=render.get('allure_results_path'),
-                         shell=True,
-                         stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
-    while True:
-        output = p.stdout.readline()
-        logging.debug(output)
-        if len(re.findall(r'Running at (.*)/', output)) < 1:  # 无论是否启动成功，都会退出循环
-            break
     # 读取报告中的summary.json文件，获取测试结果
     summary = json.load(
         open(os.path.join(render.get('allure_results_path'), 'widgets', 'summary.json'), 'r', encoding='utf-8'))
     html_file_path = os.path.join(os.path.dirname(__file__), 'pytest_email.html')
     from emails.template import JinjaTemplate as Te
 
     message = emails.html(html=Te(open(html_file_path, encoding='utf-8').read()),
@@ -63,40 +52,56 @@
     render.update({'report_url': f'http://{render.get("host")}:{port}'})
     # 发送邮件
     if mail_to:
         r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
                                         'password': mail_from[1]},
                          render=render)
         assert r.status_code == 250, 'send email failed'
-        logging.info(f'send {mail_to} test result success!')
+        logging.info(f'send {mail_to} result success!')
 
 
 def start_test_notice(mail_to: str or list, mail_from: tuple or list, render: dict):
     """使用已配置好的邮件模板，发送邮件内容, 且使用node.js anywhere启动一个本地服务，用于分享报告,
 
     :param mail_to:  发送给谁
     :param mail_from: 元组($email, $password)
     :param render: 字典类型，需要将报告的内容传入 key值如下：
                              model：必填 测试设备型号， 如VG710
-                             fun: 必填 测试功能
                              version: 必填 测试的版本, 如 VG7-V209bfd4(test)-2023-03-31-14-52-02.bin
                              host: 必填 测试主机， 10.5.24.107
                              port： 必填 分享报告端口， 63330
-                             allure_results_path: 必填 报告中的/allure-results 路径
 
     :return:
     """
-    message = emails.Message(subject=f'{render.get("model")}测试已开始，勿动环境',
-                             mail_from=('映翰通网络测试', mail_from[0]), text='如需强制停止运行，请修改配置文件中的force_stop_remain_unexecute_case参数值为1'.encode('utf-8'))
+    port = render.get('port') if render.get('port') else 63330
+    # 杀掉端口, 防止端口占用
+    html_file_path = os.path.join(os.path.dirname(__file__), 'notice_email.html')
+    kill_windows_port(render.get('host'), [port, port + 1])  # port+1 是https端口
+    # 启动本地服务，分享报告
+    p = subprocess.Popen(f'npx anywhere -h {render.get("host")} -p {port}', cwd=render.get('allure_results_path'),
+                         shell=True,
+                         stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
+    while True:
+        output = p.stdout.readline()
+        logging.debug(output)
+        if len(re.findall(r'Running at (.*)/', output)) < 1:  # 无论是否启动成功，都会退出循环
+            break
+    from emails.template import JinjaTemplate as Te
+
+    message = emails.html(html=Te(open(html_file_path, encoding='utf-8').read()),
+                          subject=f'{render.get("model")}测试已开始',
+                          mail_from=('映翰通网络测试', mail_from[0]))
+    render.update({'report_url': f'http://{render.get("host")}:{port}'})
     # 发送邮件
     if mail_to:
         r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
-                                        'password': mail_from[1]})
+                                        'password': mail_from[1]},
+                         render=render)
         assert r.status_code == 250, 'send email failed'
-        logging.info(f'send {mail_to} test result success!')
+        logging.info(f'send {mail_to} result success!')
 
 
 @loop_inspector('receive last email', 120, 5)
 def receive_last_mail(receiver: tuple, mail_from: tuple, subject: str, **kwargs):
     """收取符合条件的邮件做校验，如果匹配到多个邮件，只校验最近的一封邮件
        当邮箱中邮件较多时，会耗时很长，所以建议匹配未读的邮件进行分析，分析完后，将邮件标记为已读
 
@@ -259,8 +264,9 @@
 
 
 if __name__ == '__main__':
     # 设置日志
     import sys
 
     logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s', stream=sys.stdout)
-    start_test_notice('liwei@inhand.com.cn', ('test@inhand.com.cn', 'ABc124'), {'model': 'IR302'})
+    start_test_notice('liwei@inhand.com.cn', ('test@inhand.com.cn', 'ABc124'),
+                      {'model': 'IR302', 'version': '123', 'host': '10.5.24.224'})
```

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/ingateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,12 +63,12 @@
         self.system = System(host, username, password, protocol, port, model, language, self.page, self.locale)
 
 
 if __name__ == '__main__':
     from inhandtest.tools import enable_log
 
     enable_log('./log.log', console_level=logging.INFO)
-    with InGateway('10.5.24.96', 'inhand', '64391099@inhand') as device:
+    with InGateway('10.5.24.96') as device:
         device.network.cellular.config(cellular_enable=False,
                                        submit={'tip_messages': 'cellular_configuration_changed_successful'})
 
         # device.page.wait_for_timeout(3 * 1000)
```

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.55/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.55/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/pytest_email.html` & `inhandtest-0.0.55/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest/telnet.py` & `inhandtest-0.0.55/inhandtest/telnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,17 +645,16 @@
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
     from inhandtest.tools import enable_log
 
     enable_log('./log.log')
-    device = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
+    device = Telnet('IG902', '10.5.24.96')
     # device.tcpdump(expect='10.5.24.224.62227', interface='eth0.4094',)
-    device.send_cli('ifconfig', '/www #', 'super')
 
     # device = Telnet('IG902', '
     # device = Telnet('VG710', '10.5.24.206', 'inhand', '64391099@inhand')
     # a = device.send_cli('ping www.baidu.com -c 4', '/www #', 'super')
     # print(eval('1==2'))
     # device.assert_cli('ifconfig |grep wifi', expect='Local', interface_replace_type='cli_expect_last_read')
     # print(device.re_match('ifconfig eth0', r'HWaddr(.*)inet6', key_replace={'\r\n':'', ' ': ''}))
```

### Comparing `inhandtest-0.0.54/inhandtest/tools.py` & `inhandtest-0.0.55/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.54/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.55/inhandtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.54
+Version: 0.0.55
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.54/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.55/inhandtest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 inhandtest/inmqtt.py
 inhandtest/inrequest.py
 inhandtest/inserial.py
 inhandtest/insocket.py
 inhandtest/inssh.py
 inhandtest/ip.py
 inhandtest/mail.py
+inhandtest/notice_email.html
 inhandtest/pytest_email.html
 inhandtest/telnet.py
 inhandtest/tools.py
 inhandtest.egg-info/PKG-INFO
 inhandtest.egg-info/SOURCES.txt
 inhandtest.egg-info/dependency_links.txt
 inhandtest.egg-info/requires.txt
```

### Comparing `inhandtest-0.0.54/setup.py` & `inhandtest-0.0.55/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.54',
+    version='0.0.55',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
     # packages=['inhandtest', 'inhandtest.base_page', 'inhandtest.pages', 'inhandtest.pages.ingateway', ],
     packages=find_packages(),
-    package_data={'inhandtest': ['pytest_email.html'], 'inhandtest.pages.ingateway': ['*.yml']},
+    package_data={'inhandtest': ['*.html'], 'inhandtest.pages.ingateway': ['*.yml']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'pyserial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
                       'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf', 'colorlog'
```

