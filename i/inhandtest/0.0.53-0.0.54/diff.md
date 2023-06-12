# Comparing `tmp/inhandtest-0.0.53.tar.gz` & `tmp/inhandtest-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.53.tar", last modified: Wed Jun  7 05:18:23 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.54.tar", last modified: Mon Jun 12 05:26:05 2023, max compression
```

## Comparing `inhandtest-0.0.53.tar` & `inhandtest-0.0.54.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.53/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-06-07 05:18:23.000000 inhandtest-0.0.53/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.53/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/dm/
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.53/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.53/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.53/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.53/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    40079 2023-06-06 03:00:03.000000 inhandtest-0.0.53/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.53/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.53/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    58788 2023-06-06 05:15:22.000000 inhandtest-0.0.53/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    23364 2023-06-05 10:27:40.000000 inhandtest-0.0.53/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.53/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.53/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.53/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.53/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.53/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    52197 2023-06-07 03:52:54.000000 inhandtest-0.0.53/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7588 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.53/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11625 2023-06-01 09:15:20.000000 inhandtest-0.0.53/inhandtest/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.53/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     2393 2023-06-06 05:25:15.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     8317 2023-06-06 01:49:59.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    67781 2023-06-02 09:30:51.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86145 2023-06-02 02:13:33.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0     9556 2023-06-06 05:26:06.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    11230 2023-06-07 02:28:23.000000 inhandtest-0.0.53/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.53/inhandtest/pages/locale.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.53/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    33681 2023-06-06 05:26:30.000000 inhandtest-0.0.53/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    27509 2023-06-07 03:54:00.000000 inhandtest-0.0.53/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 05:18:23.000000 inhandtest-0.0.53/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.53/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 05:18:23.000000 inhandtest-0.0.53/setup.cfg
--rw-rw-rw-   0        0        0     1626 2023-06-07 05:16:53.000000 inhandtest-0.0.53/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.54/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-06-12 05:26:05.000000 inhandtest-0.0.54/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.54/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/dm/
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.54/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.54/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.54/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.54/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.54/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.54/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.54/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    59214 2023-06-12 05:21:09.000000 inhandtest-0.0.54/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    23673 2023-06-08 06:22:30.000000 inhandtest-0.0.54/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.54/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.54/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.54/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.54/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.54/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    52197 2023-06-07 03:52:54.000000 inhandtest-0.0.54/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7820 2023-06-07 06:08:07.000000 inhandtest-0.0.54/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.54/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.54/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.54/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    13255 2023-06-08 01:52:07.000000 inhandtest-0.0.54/inhandtest/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.54/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3179 2023-06-12 05:22:56.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.54/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.54/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    33345 2023-06-09 09:37:50.000000 inhandtest-0.0.54/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    27509 2023-06-07 03:54:00.000000 inhandtest-0.0.54/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 05:26:05.000000 inhandtest-0.0.54/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.54/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 05:26:05.000000 inhandtest-0.0.54/setup.cfg
+-rw-rw-rw-   0        0        0     1626 2023-06-12 05:25:50.000000 inhandtest-0.0.54/setup.py
```

### Comparing `inhandtest-0.0.53/PKG-INFO` & `inhandtest-0.0.54/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.53
+Version: 0.0.54
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.53/README.md` & `inhandtest-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/dm/mqtt.py` & `inhandtest-0.0.54/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/dm/register_v1.py` & `inhandtest-0.0.54/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.54/inhandtest/base_page/_ig_contents_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,15 @@
                         'attributes': {
                             self.page.locator('.ant-tabs-tab >> nth=1'): {'aria-selected': 'true'}},
                         'wait_locator': [self.page.locator('#log_to_remote_enable')],
                     }
                 },
                 'configuration_management': {
                     'menu': self.system_config_menu,
-                    'visible_locator': [self.content_target('system_config')],
+                    'visible_locator': [self.page.locator('.ant-btn.ant-btn-danger')],
                     'wait_locator': [self.content_target('system_config')],
                 },
                 'inhand_cloud': {
                     'default': 'inhand_connect_service',
                     'menu': self.system_cloud_menu,
                     'visible_locator': [self.content_target('system_cloud')],
                     'wait_locator': [self.content_target('system_cloud')],
```

### Comparing `inhandtest-0.0.53/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.54/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.54/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/base_page/base_page.py` & `inhandtest-0.0.54/inhandtest/base_page/base_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 """
 base_page
 
 """
 import os.path
 import sys
 from os import path
+
+import playwright
+
 from inhandtest.base_page._ig_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
 from inhandtest.tools import loop_inspector, replace_str
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
 from inhandtest.base_page._ir3XX_contents_locators import Ir3XXContentsLocators
@@ -332,23 +335,25 @@
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :param action: 'check'|'uncheck'| None | '是' | 'Yes'
         :param tip_messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
                             tip_messages 是支持模糊匹配
                             该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错
         :return:
         """
-
-        if action is not None:
-            if action in ('check', 'Yes', '是', 'yes', 'enable', True):
-                locator.check()
-            else:
-                locator.uncheck()
-            if log_desc:
-                logging.info(f'Device {self.host} {log_desc} {action}')
-            self.tip_messages(tip_messages)
+        try:
+            if action is not None:
+                if action in ('check', 'Yes', '是', 'yes', 'enable', True):
+                    locator.check()
+                else:
+                    locator.uncheck()
+                if log_desc:
+                    logging.info(f'Device {self.host} {log_desc} {action}')
+                self.tip_messages(tip_messages)
+        except playwright.sync_api.Error:
+            pass
 
     @allure.step('下拉选择')
     def select_option(self, locator: Locator, value: str or int, log_desc=None) -> None:
         """ 封装公共的下拉选择操作
 
         :param locator:  元素定位
         :param value: str or int, 下拉选择option的value属性值、或label
@@ -537,34 +542,37 @@
         :param locator: 下载按钮元素
         :param file_path: 下载文件的路径, 不需要跟文件名，
         :param file_name: 如果文件名
         :return:
         """
         if file_path is not None:
             if os.path.isdir(file_path) and os.path.exists(file_path):
-                with self.page.expect_download() as download_info:
-                    locator.click()
-                download = download_info.value
-                file_name = download.suggested_filename if file_name is None else file_name
-                download.save_as(path.join(file_path, file_name))
-                logging.info(
-                    f'Device {self.host} download {download.suggested_filename} to path {file_path} success')
+                if not locator.is_disabled():
+                    with self.page.expect_download() as download_info:
+                        locator.click()
+                    download = download_info.value
+                    file_name = download.suggested_filename if file_name is None else file_name
+                    download.save_as(path.join(file_path, file_name))
+                    logging.info(
+                        f'Device {self.host} download {download.suggested_filename} to path {file_path} success')
+                else:
+                    logging.warning(f'Device {self.host} {locator} is disabled')
             else:
                 logging.error(f'{file_path} Does Not Exist.')
 
     @allure.step('输入时间或日期')
     def fill_date(self, locator: Locator, date: str) -> None:
         """输入时间或日期
 
         :param locator:
         :param date: 日期，格式为 2020-01-01
         :return:
         """
         self.click(locator)
-        if locator.get_attribute('class') == 'ant-calendar-picker':   # date
+        if locator.get_attribute('class') == 'ant-calendar-picker':  # date
             locator_ = self.page.locator('.ant-calendar-input')
         else:
             locator_ = self.page.locator('.ant-time-picker-panel-input')
         locator_.fill(date)
         locator_.press('Enter')
 
     @allure.step("校验dialog message")
@@ -772,17 +780,22 @@
                         tip_messages_timeout = value.get('tip_messages_timeout') if value.get(
                             'tip_messages_timeout') is not None else 30
                     if isinstance(param_locator.get('locator'), Locator):
                         self.click(param_locator.get('locator'), param, dialog_message, tip_messages, wait_for_time,
                                    tip_messages_timeout)
                     elif isinstance(param_locator.get('locator'), list) or isinstance(param_locator.get('locator'),
                                                                                       tuple):  # 二次确认
-                        self.click(param_locator.get('locator')[0], param, dialog_message, tip_messages, wait_for_time,
-                                   tip_messages_timeout)
-                        self.click(param_locator.get('locator')[1], 'confirm', wait_for_time=1000)
+                        self.click(param_locator.get('locator')[0], param, dialog_message)
+                        try:
+                            param_locator.get('locator')[1].click(timeout=1 * 1000)
+                        except TimeoutError:
+                            pass
+                        self.tip_messages(tip_messages, tip_messages_timeout)
+                        if wait_for_time:
+                            self.page.wait_for_timeout(wait_for_time)
                     else:
                         raise Exception(f'locator {param_locator.get("locator")} is not a Locator or list or tuple')
             elif param_locator.get('type') == 'check':
                 if value:
                     value_, tip_messages = value, None
                     if isinstance(value, dict):
                         value_ = value.get('value')
@@ -920,16 +933,14 @@
                             logging.info(f'Check {option[0]} , {expression} is success')
                         else:
                             logging.info(f'Check {option[0]} , {expression} is failed')
                             return False
                     except TypeError:
                         logging.error(f'get {key} inner_text failed')
                         return False
-                else:
-                    raise KeyError(f'not support the key {key}')
         return True
 
     @allure.step("获取页面元素文本值")
     def get_text(self, keys: str or list or tuple, locators: list) -> str or dict or None:
         """获取页面元素文本值
 
         :param keys: None or str or list or tuple, 需要获取对应文本的元素的关键字
@@ -961,15 +972,15 @@
                                 if 'ant-switch-checked' in locator.first.get_attribute('class'):
                                     value = 'enable'
                                 else:
                                     value = 'disable'
                             else:
                                 value = locator.first.inner_text()
                         else:
-                            raise
+                            value = None
                     else:
                         value = str(locator)
                     result[key] = value
                 else:
                     raise KeyError(f'not support the key {key}')
         if result:
             if len(result.keys()) == 1:
```

### Comparing `inhandtest-0.0.53/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.54/inhandtest/base_page/table_tr.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,10 +452,15 @@
                 logging.info(f'table resource {value} connect success')
             else:
                 logging.debug(f'table resource {value} already connected')
 
     def delete_all(self) -> None:
         tr_locators = self.table_locator.locator('//tbody[@class="ant-table-tbody"]/tr').locator(
             '//i[@class="anticon anticon-delete"]')
-        while tr_locators.count() > 0:
+        exist_tr_number = tr_locators.count()
+        for i in range(0, exist_tr_number):
             tr_locators.first.click()
+            if isinstance(self.action_confirm, Locator):
+                self.action_confirm.click()
+            while tr_locators.count() + i + 1 != exist_tr_number:   # 等待删除完成,
+                self.table_locator.page.wait_for_timeout(500)
         logging.debug('table resource all delete')
```

### Comparing `inhandtest-0.0.53/inhandtest/exception.py` & `inhandtest-0.0.54/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/file.py` & `inhandtest-0.0.54/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/inmodbus.py` & `inhandtest-0.0.54/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/inmongodb.py` & `inhandtest-0.0.54/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/inmqtt.py` & `inhandtest-0.0.54/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/inrequest.py` & `inhandtest-0.0.54/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/inserial.py` & `inhandtest-0.0.54/inhandtest/inserial.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,27 +92,32 @@
                 raise ConnectionError
             logging.info(f'Serial Connect {self.com} Successful')
         except Exception:
             raise ConnectionError
 
     def __open(self):
         try:
-            check_windows_process('sscom', True)
-            time.sleep(2)
+            check_windows_process(['sscom', 'MobaXterm'], True)
         except:
             pass
         self.serial.port = self.com
         self.serial.baudrate = self.baud_rate
         self.serial.bytesize = self.data_bits
         self.serial.parity = self.parity
         self.serial.stopbits = self.stop_bit
         self.serial.xonxoff = self.flow_control
         self.serial.timeout = self.timeout
-        if not self.serial.is_open:
-            self.serial.open()
+        for i in range(0, 30, 3):
+            if not self.serial.is_open:
+                self.serial.open()
+                logging.debug(f"open serial {self.com} success")
+                break
+            time.sleep(3)
+        else:
+            raise SerialException(f'serial {self.com} already used')
 
     def receive_log(self, timeout=20, logs_number=1):
         """接收日志
 
         :param timeout: 接收超时时间
         :param logs_number
         :return:
```

### Comparing `inhandtest-0.0.53/inhandtest/insocket.py` & `inhandtest-0.0.54/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/inssh.py` & `inhandtest-0.0.54/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/ip.py` & `inhandtest-0.0.54/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/mail.py` & `inhandtest-0.0.54/inhandtest/mail.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     # 读取报告中的summary.json文件，获取测试结果
     summary = json.load(
         open(os.path.join(render.get('allure_results_path'), 'widgets', 'summary.json'), 'r', encoding='utf-8'))
     html_file_path = os.path.join(os.path.dirname(__file__), 'pytest_email.html')
     from emails.template import JinjaTemplate as Te
 
     message = emails.html(html=Te(open(html_file_path, encoding='utf-8').read()),
-                          subject=f'{render.get("model")}自动化测试',
+                          subject=f'{render.get("model")}测试已完成',
                           mail_from=('映翰通网络测试', mail_from[0]))
     render.update(summary.get('statistic'))
     start = datetime.datetime.fromtimestamp(summary.get('time').get("start") / 1000.0).strftime('%Y-%m-%d %H:%M:%S')
     stop = datetime.datetime.fromtimestamp(summary.get('time').get("stop") / 1000.0).strftime('%Y-%m-%d %H:%M:%S')
     render.update({'start': start, 'stop': stop})
     render.update({'report_url': f'http://{render.get("host")}:{port}'})
     # 发送邮件
@@ -66,14 +66,39 @@
         r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
                                         'password': mail_from[1]},
                          render=render)
         assert r.status_code == 250, 'send email failed'
         logging.info(f'send {mail_to} test result success!')
 
 
+def start_test_notice(mail_to: str or list, mail_from: tuple or list, render: dict):
+    """使用已配置好的邮件模板，发送邮件内容, 且使用node.js anywhere启动一个本地服务，用于分享报告,
+
+    :param mail_to:  发送给谁
+    :param mail_from: 元组($email, $password)
+    :param render: 字典类型，需要将报告的内容传入 key值如下：
+                             model：必填 测试设备型号， 如VG710
+                             fun: 必填 测试功能
+                             version: 必填 测试的版本, 如 VG7-V209bfd4(test)-2023-03-31-14-52-02.bin
+                             host: 必填 测试主机， 10.5.24.107
+                             port： 必填 分享报告端口， 63330
+                             allure_results_path: 必填 报告中的/allure-results 路径
+
+    :return:
+    """
+    message = emails.Message(subject=f'{render.get("model")}测试已开始，勿动环境',
+                             mail_from=('映翰通网络测试', mail_from[0]), text='如需强制停止运行，请修改配置文件中的force_stop_remain_unexecute_case参数值为1'.encode('utf-8'))
+    # 发送邮件
+    if mail_to:
+        r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
+                                        'password': mail_from[1]})
+        assert r.status_code == 250, 'send email failed'
+        logging.info(f'send {mail_to} test result success!')
+
+
 @loop_inspector('receive last email', 120, 5)
 def receive_last_mail(receiver: tuple, mail_from: tuple, subject: str, **kwargs):
     """收取符合条件的邮件做校验，如果匹配到多个邮件，只校验最近的一封邮件
        当邮箱中邮件较多时，会耗时很长，所以建议匹配未读的邮件进行分析，分析完后，将邮件标记为已读
 
     :param receiver: 接收者('test@inhand.com.cn', '1111124') email, password
     :param mail_from: 发送者('映翰通网络', 'iot_console@inhand.com.cn') name, email
@@ -232,9 +257,10 @@
     imap_server.close()
     imap_server.logout()
 
 
 if __name__ == '__main__':
     # 设置日志
     import sys
+
     logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s', stream=sys.stdout)
-    # pass
+    start_test_notice('liwei@inhand.com.cn', ('test@inhand.com.cn', 'ABc124'), {'model': 'IR302'})
```

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.54/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.54/inhandtest/pages/ingateway/locale.yml`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,20 @@
   alarm: Alarm
   serious: Serious
   error: Error
   warning: Warning
   notice: Notice
   information: Information
   debug: Debug
+  registering_: Registering
+  connecting: Connecting
+  custom: Custom
+  current_version: Current Version
+  start_capture: Start Capture
+  download_capture_file: Download Capture File
 cn:
   client: 客户端
   server: 服务器
   ap: 接入端
   connect: 已连接
   disconnect: 未连接
   enable: 启用
@@ -278,8 +284,14 @@
   alarm: 警报
   serious: 严重
   error: 错误
   warning: 警告
   notice: 通知
   information: 信息
   debug: 调试
+  registering_: 正在注册
+  connecting: 正在连接
+  custom: 自定义
+  current_version: 当前版本
+  start_capture: 开始抓包
+  download_capture_file: 下载抓包文件
```

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.54/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.54/inhandtest/pages/ingateway/network/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,14 @@
                lcp_interval: 10 ex: lcp_interval=10
                lcp_max_retries: 10 ex: lcp_max_retries=10
                infinitely_dial_retry: enable,disable ex: infinitely_dial_retry="enable"
                debug: enable,disable ex: debug="enable"
                expert_options: 'AT+CPIN?'
                error_text: str or list or tuple ex: error_text="Please enter an integer for 1 ~ 604800"
                submit: True or False ex: submit=True  or  submit={'tip_messages': 'cellular_configuration_changed_successful'}
-               profile_save_ok: True or False ex: profile_save_ok=True 点击submit后是否弹出保存成功的提示框
                reset: True or False ex: reset=True
         :return:
         """
         self.access_menu('network.network_interface.cellular')
         self.agg_in(self.network_locators.cellular_locators, kwargs)
```

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.54/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,18 +175,17 @@
             ('infinitely_dial_retry', {'locator': self.page.locator('#infinitely_dial_retry'), 'type': 'switch_button',
                                        'relation': [('cellular_enable', 'enable'), ('advanced_settings', 'expand')]}),
             ('debug', {'locator': self.page.locator('#debug'), 'type': 'switch_button',
                        'relation': [('cellular_enable', 'enable'), ('advanced_settings', 'expand')]}),
             ('expert_options', {'locator': self.page.locator('#expert_options'), 'type': 'text',
                                 'relation': [('cellular_enable', 'enable'), ('advanced_settings', 'expand')]}),
             ('submit',
-             {'locator': self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
-              'type': 'button'}),
-            ('profile_save_ok',
-             {'locator': self.page.locator('.ant-modal-content').locator('//button[@class="ant-btn ant-btn-primary"]'),
+             {'locator': [self.page.locator('//button[@class="ant-btn ant-btn-primary"]', has_text=self.locale.submit),
+                          self.page.locator('.ant-modal-content').locator(
+                              '//button[@class="ant-btn ant-btn-primary"]')],
               'type': 'button'}),
             ('errors_text', {'type': 'text_messages'}),
             ('success_tip', {'type': 'tip_messages'}),
             ('reset', {'locator': self.page.locator('//button[@class="ant-btn" and @type="reset"]'),
                        'type': 'button'}),
         ]
```

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.54/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/pytest_email.html` & `inhandtest-0.0.54/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest/telnet.py` & `inhandtest-0.0.54/inhandtest/telnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class Telnet:
     __doc__ = '使用telnet连接设备，封装下面命令'
 
     def __init__(self, model: str, host: str, super_user: str, super_password: str, user='adm', password='123456',
                  port=23, **kwargs):
         """使用telnet连接设备
 
-        :param model: 设备型号，VG710'|'IR302'|'ER805'|'ER605'|'IG902'|'IG502'|'IR915'|'ODU2002'
+        :param model: 设备型号，VG710'|'IR302'|'ER805'|'ER605'|'IG902'|'IG502'|'IR915'|'ODU2002'|'IR305'|'IR615'
         :param host: 设备lan ip， 192.168.2.1
         :param super_user: 超级管理员的用户名称
         :param super_password:  超级管理员的密码
         :param user: 用户名
         :param password: 用户密码
         :param port: 端口
         :param kwargs: interface_replace, 字典类型，只替换输入命令 {'wan': 'wan0', 'wifi_sta': 'wan2', 'cellular1': 'wwan0'}
@@ -47,15 +47,15 @@
         self.config_tag = '(config)#'
         self.user_tag = '#'    # 特权模式
         self.normal_tag = '>'
         self.factory_tag = '(factory)#'  # 仅部分设备支持工厂模式
         self.factory_username = kwargs.get('factory_username')
         self.factory_password = kwargs.get('factory_password')
         self.interface_replace: dict = kwargs.get('interface_replace')
-        if self.model not in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
+        if self.model not in ['VG710', 'IR302', 'IR305', 'IR615', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
             raise Exception(f'Not support this device model {self.model}')
         self.tn: telnetlib.Telnet
         self.__login()
 
     def update_hostname(self, hostname: str) -> None:
         """更新hostname 后对应的telnet也需要更新
 
@@ -69,15 +69,15 @@
     def __login(self):
         """
 
 
         :return:
         """
         login_spe = {"VG710": '#', 'IR302': '>', 'ER805': '#', 'ER605': '#', 'IG902': '#', 'IG502': '#', 'IR915': '#',
-                     'ODU2002': '>'}
+                     'ODU2002': '>', 'IR305': '>', 'IR615': '>'}
         try:
             # 连接telnet服务器
             logging.debug("Start telnet 【%s:%s】" % (self.host, self.port))
             self.tn = telnetlib.Telnet(self.host, self.port, timeout=10)
         except:
             raise ConnectionError(f'Device【{self.host}:{self.port} connect failed】')
         logging.debug("Telnet 【%s:%s】 connected" % (self.host, self.port))
@@ -127,32 +127,32 @@
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.debug(read_contents)
         if self.config_tag in read_contents:
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["exit", self.super_user + " " + self.super_password])
-            elif self.model == 'IR302':
+            elif self.model in ('IR302', 'IR305', 'IR615'):
                 self.send_cli(["exit", "exit", "support enable", self.super_user, self.super_password])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             self.send_cli(['cd /www'])
         elif self.user_tag in read_contents:
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli([self.super_user + " " + self.super_password])
-            elif self.model == 'IR302':
+            elif self.model in ('IR302', 'IR305', 'IR615'):
                 self.send_cli(["exit", "support enable", self.super_user, self.super_password])
         elif self.normal_tag in read_contents:
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["enable", self.password, self.super_user + ' ' + self.super_password])
-            elif self.model == 'IR302':
+            elif self.model in ('IR302', 'IR305', 'IR615'):
                 self.send_cli(["support enable", self.super_user, self.super_password])
         elif self.factory_tag in read_contents:
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(["exit", self.super_user + " " + self.super_password])
-            elif self.model == 'IR302':
+            elif self.model in ('IR302', 'IR305', 'IR615'):
                 self.send_cli(["exit", "exit", "support enable", self.super_user, self.super_password])
         else:
             logging.warning(f'not support this mode. telnet return contents: {read_contents}')
             self.close()
             self.__login()
             self.super_mode()
         logging.info(f"Device {self.host} access in super mode")
@@ -168,27 +168,24 @@
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.debug(read_contents)
         if self.config_tag in read_contents:
             pass
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli", "con t"], [self.user_tag, None])
-            elif self.model == 'IR302':
+            elif self.model in ('IR302', 'IR305', 'IR615'):
                 self.send_cli(["console", "enable", self.password, 'con t'])
             elif self.model == 'ODU2002':
                 self.send_cli(["cli", "enable", self.password, "con t"], [self.normal_tag, None, None, None])
         elif self.user_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
-                self.send_cli(['con t'])
+            self.send_cli(['con t'])
         elif self.normal_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
-                self.send_cli(["enable", self.password, 'con t'])
+            self.send_cli(["enable", self.password, 'con t'])
         elif self.factory_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
-                self.send_cli(['exit', 'con t'])
+            self.send_cli(['exit', 'con t'])
         else:
             logging.warning(f'not support this mode, last content:{read_contents}')
             self.close()
             self.__login()
             self.config_mode()
         logging.info(f"Device {self.host} access in config mode")
 
@@ -199,31 +196,28 @@
         :return:
         """
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.debug(read_contents)
         if self.config_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
-                self.send_cli(['exit'])
+            self.send_cli(['exit'])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli"], [self.user_tag])
-            elif self.model in ['IR302']:
+            elif self.model in ['IR302', 'IR305', 'IR615']:
                 self.send_cli(["console", "enable", self.password])
             elif self.model == 'ODU2002':
                 self.send_cli(["cli", "enable", self.password], [self.normal_tag, None, None])
         elif self.user_tag in read_contents:
             pass
         elif self.normal_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
-                self.send_cli(["enable", self.password])
+            self.send_cli(["enable", self.password])
         elif self.factory_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
-                self.send_cli(['exit'])
+            self.send_cli(['exit'])
         else:
             logging.warning(f'not support this mode. telnet return contents: {read_contents}')
             self.close()
             self.__login()
             self.user_mode()
         logging.info(f"Device {self.host} access in user mode")
 
@@ -236,34 +230,34 @@
         self.tn.write(("\003" + "\r").encode("cp936"))  # 普通模式下输入ctrl+c会返回  % Command is not supported!
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.debug(read_contents)
         if self.config_tag in read_contents:
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['exit', 'disable'])
-            elif self.model in ['IR302']:
+            elif self.model in ['IR302', 'IR305', 'IR615']:
                 self.send_cli(['exit', 'exit'])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli", "disable"], [self.user_tag, None])
-            elif self.model in ['IR302']:
+            elif self.model in ['IR302', 'IR305', 'IR615']:
                 self.send_cli(["console"])
             elif self.model == 'ODU2002':
                 self.send_cli(["cli"], [self.normal_tag])
         elif self.user_tag in read_contents:
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['disable'])
-            elif self.model in ['IR302']:
+            elif self.model in ['IR302', 'IR305', 'IR615']:
                 self.send_cli(['exit'])
         elif self.normal_tag in read_contents:
             pass
         elif self.factory_tag in read_contents:
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
                 self.send_cli(['exit', 'disable'])
-            elif self.model in ['IR302']:
+            elif self.model in ['IR302', 'IR305', 'IR615']:
                 self.send_cli(['exit', 'exit'])
         else:
             logging.warning(
                 f'not support this mode. telnet return contents: {read_contents} normal_tag: {self.normal_tag}')
             self.close()
             self.__login()
             self.normal_mode()
@@ -278,26 +272,26 @@
         if not self.factory_username or not self.factory_password:
             raise Exception("sure this device support factory mode, and init factory_username、factory_password")
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.debug(read_contents)
         if self.config_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'IR305', 'IR615', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(['exit', self.factory_username + " " + self.factory_password])
         elif self.super_tag in read_contents or (('/' in read_contents) and (' #' in read_contents)):
             if self.model in ['VG710', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["cli", self.factory_username + " " + self.factory_password], [self.user_tag, None])
-            elif self.model in ['IR302']:
+            elif self.model in ['IR302', 'IR305', 'IR615']:
                 self.send_cli(["console", "enable", self.password, self.factory_username + " " + self.factory_password])
         elif self.user_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'IR305', 'IR615', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli([self.factory_username + " " + self.factory_password])
         elif self.normal_tag in read_contents:
-            if self.model in ['VG710', 'IR302', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
+            if self.model in ['VG710', 'IR302', 'IR305', 'IR615', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
                 self.send_cli(["enable", self.password, self.factory_username + " " + self.factory_password])
         elif self.factory_tag in read_contents:
             pass
         else:
             logging.warning(f'not support this mode. telnet return contents: {read_contents}')
             self.close()
             self.__login()
```

### Comparing `inhandtest-0.0.53/inhandtest/tools.py` & `inhandtest-0.0.54/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.53/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.54/inhandtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.53
+Version: 0.0.54
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.53/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.54/inhandtest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 inhandtest/base_page/__init__.py
 inhandtest/base_page/_ig_contents_locators.py
 inhandtest/base_page/_ir3XX_contents_locators.py
 inhandtest/base_page/_vg710_contents_locators.py
 inhandtest/base_page/base_page.py
 inhandtest/base_page/table_tr.py
 inhandtest/pages/__init__.py
-inhandtest/pages/locale.py
 inhandtest/pages/ingateway/__init__.py
 inhandtest/pages/ingateway/ingateway.py
 inhandtest/pages/ingateway/locale.yml
 inhandtest/pages/ingateway/locators.py
 inhandtest/pages/ingateway/edge_computing/__init__.py
 inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
 inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
```

### Comparing `inhandtest-0.0.53/setup.py` & `inhandtest-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.53',
+    version='0.0.54',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

