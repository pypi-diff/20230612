# Comparing `tmp/nmap_query_tool-1.1.5.tar.gz` & `tmp/nmap_query_tool-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmap_query_tool-1.1.5.tar", last modified: Mon Jun 12 03:06:03 2023, max compression
+gzip compressed data, was "nmap_query_tool-1.1.6.tar", last modified: Mon Jun 12 03:15:33 2023, max compression
```

## Comparing `nmap_query_tool-1.1.5.tar` & `nmap_query_tool-1.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:06:03.452044 nmap_query_tool-1.1.5/
--rw-r--r--   0 timheard  (1000) timheard  (1000)    11357 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/LICENSE
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:06:03.405173 nmap_query_tool-1.1.5/NmapQueryTool/
--rw-r--r--   0 timheard  (1000) timheard  (1000)       23 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/__init__.py
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:06:03.420786 nmap_query_tool-1.1.5/NmapQueryTool/lib/
--rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/lib/__init__.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     7755 2023-06-12 02:42:27.000000 nmap_query_tool-1.1.5/NmapQueryTool/lib/host_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     1797 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/lib/interaction_context.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)      621 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/lib/nmap_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     1804 2023-06-12 02:41:54.000000 nmap_query_tool-1.1.5/NmapQueryTool/lib/port_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     7363 2023-06-12 03:05:36.000000 nmap_query_tool-1.1.5/NmapQueryTool/lib/scan_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)    14622 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/nmap_query.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)      239 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/run_tests.py
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:06:03.420786 nmap_query_tool-1.1.5/NmapQueryTool/tst/
--rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/tst/__init__.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     8571 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/NmapQueryTool/tst/integration_tests.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 03:06:03.452044 nmap_query_tool-1.1.5/PKG-INFO
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2105 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.5/README.md
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:06:03.452044 nmap_query_tool-1.1.5/nmap_query_tool.egg-info/
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 03:06:03.000000 nmap_query_tool-1.1.5/nmap_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 timheard  (1000) timheard  (1000)      527 2023-06-12 03:06:03.000000 nmap_query_tool-1.1.5/nmap_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)        1 2023-06-12 03:06:03.000000 nmap_query_tool-1.1.5/nmap_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)       14 2023-06-12 03:06:03.000000 nmap_query_tool-1.1.5/nmap_query_tool.egg-info/top_level.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)       38 2023-06-12 03:06:03.452044 nmap_query_tool-1.1.5/setup.cfg
--rw-r--r--   0 timheard  (1000) timheard  (1000)      605 2023-06-12 03:05:47.000000 nmap_query_tool-1.1.5/setup.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:15:33.764050 nmap_query_tool-1.1.6/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    11357 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/LICENSE
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:15:33.732752 nmap_query_tool-1.1.6/NmapQueryTool/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       23 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/__init__.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:15:33.748425 nmap_query_tool-1.1.6/NmapQueryTool/lib/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/lib/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     7755 2023-06-12 02:42:27.000000 nmap_query_tool-1.1.6/NmapQueryTool/lib/host_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1797 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/lib/interaction_context.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      621 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/lib/nmap_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1804 2023-06-12 02:41:54.000000 nmap_query_tool-1.1.6/NmapQueryTool/lib/port_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     7355 2023-06-12 03:15:17.000000 nmap_query_tool-1.1.6/NmapQueryTool/lib/scan_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    14622 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/nmap_query.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      239 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/run_tests.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:15:33.748425 nmap_query_tool-1.1.6/NmapQueryTool/tst/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/tst/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     8571 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/NmapQueryTool/tst/integration_tests.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 03:15:33.764050 nmap_query_tool-1.1.6/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2105 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.6/README.md
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 03:15:33.764050 nmap_query_tool-1.1.6/nmap_query_tool.egg-info/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 03:15:33.000000 nmap_query_tool-1.1.6/nmap_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      527 2023-06-12 03:15:33.000000 nmap_query_tool-1.1.6/nmap_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        1 2023-06-12 03:15:33.000000 nmap_query_tool-1.1.6/nmap_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       14 2023-06-12 03:15:33.000000 nmap_query_tool-1.1.6/nmap_query_tool.egg-info/top_level.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       38 2023-06-12 03:15:33.764050 nmap_query_tool-1.1.6/setup.cfg
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      605 2023-06-12 03:15:28.000000 nmap_query_tool-1.1.6/setup.py
```

### Comparing `nmap_query_tool-1.1.5/LICENSE` & `nmap_query_tool-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/NmapQueryTool/lib/host_data.py` & `nmap_query_tool-1.1.6/NmapQueryTool/lib/host_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/NmapQueryTool/lib/interaction_context.py` & `nmap_query_tool-1.1.6/NmapQueryTool/lib/interaction_context.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/NmapQueryTool/lib/nmap_data.py` & `nmap_query_tool-1.1.6/NmapQueryTool/lib/nmap_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/NmapQueryTool/lib/port_data.py` & `nmap_query_tool-1.1.6/NmapQueryTool/lib/port_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/NmapQueryTool/lib/scan_data.py` & `nmap_query_tool-1.1.6/NmapQueryTool/lib/scan_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,24 +121,24 @@
 
     def print_data(self):
         print(str(self))
 
     @staticmethod
     def create_from_nmap_data(data_source):
         scan_data = ScanData()
+        host_ip = None
 
         for line in data_source:
             if re.match('^Nmap scan report for ([0-9]{1,3}\.){3}[0-9]{1,3}$', line):
                 host_and_ip_data = re.match('Nmap scan report for (.*)', line).group(1)
 
                 # Handles the following two types of line formats:
                 #
                 # Nmap scan report for 10.90.78.103
                 # Nmap scan report for atsva9078153.vbschools.com (10.90.78.153)
-                host_ip = None
                 hostname = None
                 if re.match('([0-9]{1,3}\.){3}[0-9]{1,3}', host_and_ip_data):
                     host_ip = host_and_ip_data
                 else:
                     host_ip_pair = host_and_ip_data.replace('(', '').replace(')', '').split(' ')
                     hostname = host_ip_pair[0]
                     host_ip = host_ip_pair[1]
```

### Comparing `nmap_query_tool-1.1.5/NmapQueryTool/nmap_query.py` & `nmap_query_tool-1.1.6/NmapQueryTool/nmap_query.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/NmapQueryTool/tst/integration_tests.py` & `nmap_query_tool-1.1.6/NmapQueryTool/tst/integration_tests.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/PKG-INFO` & `nmap_query_tool-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmap_query_tool
-Version: 1.1.5
+Version: 1.1.6
 Summary: A tool for parsing and dynamically querying nmap scan data
 Home-page: https://github.com/unheardof/NmapQueryTool
 Author: Timothy Heard
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `nmap_query_tool-1.1.5/README.md` & `nmap_query_tool-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/nmap_query_tool.egg-info/PKG-INFO` & `nmap_query_tool-1.1.6/nmap_query_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmap-query-tool
-Version: 1.1.5
+Version: 1.1.6
 Summary: A tool for parsing and dynamically querying nmap scan data
 Home-page: https://github.com/unheardof/NmapQueryTool
 Author: Timothy Heard
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `nmap_query_tool-1.1.5/nmap_query_tool.egg-info/SOURCES.txt` & `nmap_query_tool-1.1.6/nmap_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.5/setup.py` & `nmap_query_tool-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="nmap_query_tool",
-	version="1.1.5",
+	version="1.1.6",
 	author="Timothy Heard",
 	description="A tool for parsing and dynamically querying nmap scan data",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/unheardof/NmapQueryTool",
 	packages=setuptools.find_packages(),
 	classifiers=[
```

