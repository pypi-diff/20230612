# Comparing `tmp/netbox-ipv4-tools-1.0.1.tar.gz` & `tmp/netbox-ipv4-tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-ipv4-tools-1.0.1.tar", last modified: Fri Feb  3 08:15:39 2023, max compression
+gzip compressed data, was "netbox-ipv4-tools-1.0.2.tar", last modified: Mon Jun 12 07:43:56 2023, max compression
```

## Comparing `netbox-ipv4-tools-1.0.1.tar` & `netbox-ipv4-tools-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.075163 netbox-ipv4-tools-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-03 08:15:39.075163 netbox-ipv4-tools-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.071163 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.071163 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.071163 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.075163 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.071163 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.075163 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/netbox_ipv4_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 08:15:39.075163 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-03 08:15:39.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-02-03 08:15:39.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 08:15:39.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-03 08:15:39.000000 netbox-ipv4-tools-1.0.1/netbox_ipv4_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 08:15:39.075163 netbox-ipv4-tools-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-03 08:15:27.000000 netbox-ipv4-tools-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.142945 netbox-ipv4-tools-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 07:43:56.142945 netbox-ipv4-tools-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.138945 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.138945 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.138945 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.138945 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.138945 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.142945 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/netbox_ipv4_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:43:56.138945 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-12 07:43:56.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-12 07:43:56.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:43:56.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 07:43:56.000000 netbox-ipv4-tools-1.0.2/netbox_ipv4_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 07:43:56.142945 netbox-ipv4-tools-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 07:43:40.000000 netbox-ipv4-tools-1.0.2/setup.py
```

### Comparing `netbox-ipv4-tools-1.0.1/LICENSE` & `netbox-ipv4-tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/PKG-INFO` & `netbox-ipv4-tools-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-ipv4-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Work with ipv4 in NetBox
 Home-page: https://github.com/mlongo4290/netbox-ipv4-tools
 Author: Michael Longo
 License: Apache 2.0
 Project-URL: Source, https://github.com/mlongo4290/netbox-ipv4-tools
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox-ipv4-tools-1.0.1/README.md` & `netbox-ipv4-tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/navigation.py` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/navigation.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 menu = PluginMenu(
     label='IPv4 Tools',
     groups=(
         (
             'TOOLS',
             (
                 PluginMenuItem(
+                    permissions=["netbox_ipv4_tools.view_tools"],
                     link='plugins:netbox_ipv4_tools:cidr_table',
                     link_text='CIDR Conversion Table'
                 ),
                 PluginMenuItem(
+                    permissions=["netbox_ipv4_tools.view_tools"],
                     link='plugins:netbox_ipv4_tools:cidr_to_range',
                     link_text='CIDR to IP Range'
                 ),
                 PluginMenuItem(
+                    permissions=["netbox_ipv4_tools.view_tools"],
                     link='plugins:netbox_ipv4_tools:supernet_calculator',
                     link_text='Supernet calculator'
                 ),
             ),
         ),
     ),
     icon_class='mdi mdi-ip-network',
```

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/js/netmask.js`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/js/range.js`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/static/netbox_ipv4_tools/js/supernet.js`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr-to-range.html`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/netbox_ipv4_tools/cidr.html`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools/templates/netbox_ipv4_tools/supernet-calculator.html`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools.egg-info/PKG-INFO` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-ipv4-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: Work with ipv4 in NetBox
 Home-page: https://github.com/mlongo4290/netbox-ipv4-tools
 Author: Michael Longo
 License: Apache 2.0
 Project-URL: Source, https://github.com/mlongo4290/netbox-ipv4-tools
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox-ipv4-tools-1.0.1/netbox_ipv4_tools.egg-info/SOURCES.txt` & `netbox-ipv4-tools-1.0.2/netbox_ipv4_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-ipv4-tools-1.0.1/setup.py` & `netbox-ipv4-tools-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 readme = Path(__file__).parent / "README.md"
 long_description = readme.read_text()
 
 setup(
     name="netbox-ipv4-tools",
-    version="1.0.1",
+    version="1.0.2",
     description="Work with ipv4 in NetBox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mlongo4290/netbox-ipv4-tools",
     author="Michael Longo",
     license="Apache 2.0",
     install_requires=[],
```

