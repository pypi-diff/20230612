# Comparing `tmp/nmap_query_tool-1.1.7.tar.gz` & `tmp/nmap_query_tool-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmap_query_tool-1.1.7.tar", last modified: Mon Jun 12 04:25:00 2023, max compression
+gzip compressed data, was "nmap_query_tool-1.1.8.tar", last modified: Mon Jun 12 21:48:10 2023, max compression
```

## Comparing `nmap_query_tool-1.1.7.tar` & `nmap_query_tool-1.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 04:25:00.205792 nmap_query_tool-1.1.7/
--rw-r--r--   0 timheard  (1000) timheard  (1000)    11357 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/LICENSE
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 04:25:00.174136 nmap_query_tool-1.1.7/NmapQueryTool/
--rw-r--r--   0 timheard  (1000) timheard  (1000)       23 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/__init__.py
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 04:25:00.174641 nmap_query_tool-1.1.7/NmapQueryTool/lib/
--rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/lib/__init__.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     7755 2023-06-12 02:42:27.000000 nmap_query_tool-1.1.7/NmapQueryTool/lib/host_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     1797 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/lib/interaction_context.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)      621 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/lib/nmap_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     1804 2023-06-12 02:41:54.000000 nmap_query_tool-1.1.7/NmapQueryTool/lib/port_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     7664 2023-06-12 04:23:38.000000 nmap_query_tool-1.1.7/NmapQueryTool/lib/scan_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)    14622 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/nmap_query.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)      239 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/run_tests.py
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 04:25:00.174641 nmap_query_tool-1.1.7/NmapQueryTool/tst/
--rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/tst/__init__.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     8571 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/NmapQueryTool/tst/integration_tests.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 04:25:00.205792 nmap_query_tool-1.1.7/PKG-INFO
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2105 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.7/README.md
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 04:25:00.205792 nmap_query_tool-1.1.7/nmap_query_tool.egg-info/
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 04:25:00.000000 nmap_query_tool-1.1.7/nmap_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 timheard  (1000) timheard  (1000)      527 2023-06-12 04:25:00.000000 nmap_query_tool-1.1.7/nmap_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)        1 2023-06-12 04:25:00.000000 nmap_query_tool-1.1.7/nmap_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)       14 2023-06-12 04:25:00.000000 nmap_query_tool-1.1.7/nmap_query_tool.egg-info/top_level.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)       38 2023-06-12 04:25:00.205792 nmap_query_tool-1.1.7/setup.cfg
--rw-r--r--   0 timheard  (1000) timheard  (1000)      605 2023-06-12 04:24:26.000000 nmap_query_tool-1.1.7/setup.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 21:48:10.714970 nmap_query_tool-1.1.8/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    11357 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/LICENSE
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 21:48:10.633328 nmap_query_tool-1.1.8/NmapQueryTool/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       23 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/__init__.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 21:48:10.662330 nmap_query_tool-1.1.8/NmapQueryTool/lib/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/lib/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     7755 2023-06-12 02:42:27.000000 nmap_query_tool-1.1.8/NmapQueryTool/lib/host_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1797 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/lib/interaction_context.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      621 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/lib/nmap_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1804 2023-06-12 02:41:54.000000 nmap_query_tool-1.1.8/NmapQueryTool/lib/port_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     7591 2023-06-12 21:48:01.000000 nmap_query_tool-1.1.8/NmapQueryTool/lib/scan_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    14622 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/nmap_query.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      239 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/run_tests.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 21:48:10.679970 nmap_query_tool-1.1.8/NmapQueryTool/tst/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/tst/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     8571 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/NmapQueryTool/tst/integration_tests.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 21:48:10.712972 nmap_query_tool-1.1.8/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2105 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.8/README.md
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 21:48:10.710936 nmap_query_tool-1.1.8/nmap_query_tool.egg-info/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 21:48:10.000000 nmap_query_tool-1.1.8/nmap_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      527 2023-06-12 21:48:10.000000 nmap_query_tool-1.1.8/nmap_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        1 2023-06-12 21:48:10.000000 nmap_query_tool-1.1.8/nmap_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       14 2023-06-12 21:48:10.000000 nmap_query_tool-1.1.8/nmap_query_tool.egg-info/top_level.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       38 2023-06-12 21:48:10.714970 nmap_query_tool-1.1.8/setup.cfg
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      605 2023-06-12 21:48:01.000000 nmap_query_tool-1.1.8/setup.py
```

### Comparing `nmap_query_tool-1.1.7/LICENSE` & `nmap_query_tool-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/NmapQueryTool/lib/host_data.py` & `nmap_query_tool-1.1.8/NmapQueryTool/lib/host_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/NmapQueryTool/lib/interaction_context.py` & `nmap_query_tool-1.1.8/NmapQueryTool/lib/interaction_context.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/NmapQueryTool/lib/nmap_data.py` & `nmap_query_tool-1.1.8/NmapQueryTool/lib/nmap_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/NmapQueryTool/lib/port_data.py` & `nmap_query_tool-1.1.8/NmapQueryTool/lib/port_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/NmapQueryTool/lib/scan_data.py` & `nmap_query_tool-1.1.8/NmapQueryTool/lib/scan_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def get_headers(self):
         headers = HostData.DEFAULT_HOST_DATA_COLUMNS + PortData.PORT_DATA_COLUMNS
         for ip in self.host_data_by_ip:
             for key in self.host_data_by_ip[ip].additional_service_info:
                 header_value = key.upper()
                 if not header_value in headers:
                     headers.append(header_value)
-                
+
         return headers
 
     def to_csv_string(self):
         rows = []
         headers = self.get_headers()
         rows.append(','.join(headers))
 
@@ -52,15 +52,15 @@
 
         return '\n'.join(rows)
 
     def ips(self):
         return self.host_data_by_ip.keys()
 
     def host_data_list(self):
-        return self.host_data_by_ip.values()        
+        return self.host_data_by_ip.values()
 
     def add_host_data(self, host_ip, host_data):
         # TODO: Add logic for merging HostData objects
         if host_ip in self.host_data_by_ip:
             raise Exception('Host data already exists for %s' % host_ip)
         else:
             self.host_data_by_ip[host_ip] = host_data
@@ -125,44 +125,46 @@
     @staticmethod
     def create_from_nmap_data(data_source):
         scan_data = ScanData()
         host_ip = None
 
         if type(data_source) is str:
             data_source = data_source.split('\n')
-        
+
         for line in data_source:
+            line = line.strip()
+
             if re.match('^Nmap scan report for ([0-9]{1,3}\.){3}[0-9]{1,3}$', line):
                 host_and_ip_data = re.match('Nmap scan report for (.*)', line).group(1)
 
                 # Handles the following two types of line formats:
                 #
                 # Nmap scan report for 10.90.78.103
                 # Nmap scan report for atsva9078153.vbschools.com (10.90.78.153)
                 hostname = None
                 if re.match('([0-9]{1,3}\.){3}[0-9]{1,3}', host_and_ip_data):
                     host_ip = host_and_ip_data
                 else:
                     host_ip_pair = host_and_ip_data.replace('(', '').replace(')', '').split(' ')
                     hostname = host_ip_pair[0]
                     host_ip = host_ip_pair[1]
-                    
+
                 if host_ip == None:
                     raise Exception('No host IP found if "%s"') % line
 
                 scan_data.add_host_data(host_ip, HostData(host_ip, hostname))
 
             # TODO: Add support for this header line format:
             #
             # Nmap scan report for www.nakatomi02.com (108.226.158.80)
-                
+
             # Skip all lines until data for a specific host is encountered
             if host_ip is None:
                 continue
-            
+
             if re.match('[0-9]+/[a-zA-Z]+[ ]+.*', line):
                 tokens = line.strip().split(' ')
                 values = [t for t in tokens if t != ''] # Filter out the whitespace tokens
 
                 # Expected format: ['port/protocol', 'state', 'service', 'version (will possibly be multiple tokens)']
                 # Example: ['22/tcp', 'open', 'ssh', 'OpenSSH', '6.2', '(protocol', '2.0;', 'Cisco', 'NX-OS)']
                 port_number = None
@@ -176,22 +178,22 @@
                 else:
                     port_number = values[0]
 
                 port_data = PortData(port_number, protocol)
                 port_data.state = values[1]
                 port_data.service = values[2]
                 port_data.version = ' '.join(values[3:])
-    
+
                 scan_data.host_data_by_ip[host_ip].add_data(port_data)
 
             elif re.match('OS details\: (.*)', line):
                 result = re.match('OS details\: (.*)', line)
                 os_info = result.group(1).replace(' or ', ' ').split(',')
                 scan_data.host_data_by_ip[host_ip].add_os_data(os_info)
-                
+
             elif re.match('Service Info: (.*)', line):
                 result = re.match('Service Info: (.*)', line)
                 service_info_str = result.group(1)
 
                 key_value_pair_strs = service_info_str.split(';')
 
                 for kv_str in key_value_pair_strs:
@@ -205,8 +207,7 @@
                     scan_data.host_data_by_ip[host_ip].add_service_info_data(service_info_key, service_info_value)
 
             else:
                 # Skip parsing lines that do not contain relevant data
                 continue
 
         return scan_data
-
```

### Comparing `nmap_query_tool-1.1.7/NmapQueryTool/nmap_query.py` & `nmap_query_tool-1.1.8/NmapQueryTool/nmap_query.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/NmapQueryTool/tst/integration_tests.py` & `nmap_query_tool-1.1.8/NmapQueryTool/tst/integration_tests.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/PKG-INFO` & `nmap_query_tool-1.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmap_query_tool
-Version: 1.1.7
+Version: 1.1.8
 Summary: A tool for parsing and dynamically querying nmap scan data
 Home-page: https://github.com/unheardof/NmapQueryTool
 Author: Timothy Heard
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `nmap_query_tool-1.1.7/README.md` & `nmap_query_tool-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/nmap_query_tool.egg-info/PKG-INFO` & `nmap_query_tool-1.1.8/nmap_query_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmap-query-tool
-Version: 1.1.7
+Version: 1.1.8
 Summary: A tool for parsing and dynamically querying nmap scan data
 Home-page: https://github.com/unheardof/NmapQueryTool
 Author: Timothy Heard
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `nmap_query_tool-1.1.7/nmap_query_tool.egg-info/SOURCES.txt` & `nmap_query_tool-1.1.8/nmap_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.7/setup.py` & `nmap_query_tool-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="nmap_query_tool",
-	version="1.1.7",
+	version="1.1.8",
 	author="Timothy Heard",
 	description="A tool for parsing and dynamically querying nmap scan data",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/unheardof/NmapQueryTool",
 	packages=setuptools.find_packages(),
 	classifiers=[
```

