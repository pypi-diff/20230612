# Comparing `tmp/nmap_query_tool-1.1.3.tar.gz` & `tmp/nmap_query_tool-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmap_query_tool-1.1.3.tar", last modified: Mon Jun 12 00:33:14 2023, max compression
+gzip compressed data, was "nmap_query_tool-1.1.4.tar", last modified: Mon Jun 12 02:54:13 2023, max compression
```

## Comparing `nmap_query_tool-1.1.3.tar` & `nmap_query_tool-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/
--rw-r--r--   0 timheard  (1000) timheard  (1000)    11357 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/LICENSE
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.906946 nmap_query_tool-1.1.3/NmapQueryTool/
--rw-r--r--   0 timheard  (1000) timheard  (1000)       23 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/__init__.py
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.924203 nmap_query_tool-1.1.3/NmapQueryTool/lib/
--rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/__init__.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     6983 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/host_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     1797 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/interaction_context.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)      621 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/nmap_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     1449 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/port_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     7260 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/scan_data.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)    14622 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/nmap_query.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)      239 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/run_tests.py
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.924203 nmap_query_tool-1.1.3/NmapQueryTool/tst/
--rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/tst/__init__.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     8571 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/tst/integration_tests.py
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/PKG-INFO
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2105 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/README.md
-drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/
--rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 timheard  (1000) timheard  (1000)      527 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)        1 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)       14 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/top_level.txt
--rw-r--r--   0 timheard  (1000) timheard  (1000)       38 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/setup.cfg
--rw-r--r--   0 timheard  (1000) timheard  (1000)      605 2023-06-12 00:31:19.000000 nmap_query_tool-1.1.3/setup.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 02:54:13.207090 nmap_query_tool-1.1.4/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    11357 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/LICENSE
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 02:54:13.144579 nmap_query_tool-1.1.4/NmapQueryTool/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       23 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/__init__.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 02:54:13.160217 nmap_query_tool-1.1.4/NmapQueryTool/lib/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/lib/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     7755 2023-06-12 02:42:27.000000 nmap_query_tool-1.1.4/NmapQueryTool/lib/host_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1797 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/lib/interaction_context.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      621 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/lib/nmap_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1804 2023-06-12 02:41:54.000000 nmap_query_tool-1.1.4/NmapQueryTool/lib/port_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     7268 2023-06-12 02:39:35.000000 nmap_query_tool-1.1.4/NmapQueryTool/lib/scan_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    14622 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/nmap_query.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      239 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/run_tests.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 02:54:13.175841 nmap_query_tool-1.1.4/NmapQueryTool/tst/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/tst/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     8571 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/NmapQueryTool/tst/integration_tests.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 02:54:13.191500 nmap_query_tool-1.1.4/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2105 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.4/README.md
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 02:54:13.191500 nmap_query_tool-1.1.4/nmap_query_tool.egg-info/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 02:54:12.000000 nmap_query_tool-1.1.4/nmap_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      527 2023-06-12 02:54:13.000000 nmap_query_tool-1.1.4/nmap_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        1 2023-06-12 02:54:12.000000 nmap_query_tool-1.1.4/nmap_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       14 2023-06-12 02:54:12.000000 nmap_query_tool-1.1.4/nmap_query_tool.egg-info/top_level.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       38 2023-06-12 02:54:13.207090 nmap_query_tool-1.1.4/setup.cfg
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      605 2023-06-12 02:43:16.000000 nmap_query_tool-1.1.4/setup.py
```

### Comparing `nmap_query_tool-1.1.3/LICENSE` & `nmap_query_tool-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.3/NmapQueryTool/lib/host_data.py` & `nmap_query_tool-1.1.4/NmapQueryTool/lib/host_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,20 @@
         if ip == None or ip.strip() == '':
             raise Exception('Must provide an IP address when creating a HostData object')
 
         self.ip = ip
         self.hostname = hostname
         self.os_list = []
         self.device_types = []
-        self.additional_service_info = {} # Mapping of nmap service info key to list of values
-        self.data_by_port_number = {} # Mapping of port number strings to PortData objects
+
+        # Mapping of nmap service info key to list of values
+        self.additional_service_info = {}
+
+        # Mapping of port number strings to lists of PortData objects
+        self.data_by_port_number = {}
 
     def __str__(self):
         lines = []
 
         lines.append('Host IP: %s' % self.ip)
 
         if self.hostname != None:
@@ -37,15 +41,16 @@
 
             lines.append('%s: %s' % (key, value_str))
 
         # This line is just for formatting
         lines.append('')
 
         for port_number in self.data_by_port_number:
-            lines.append(str(self.data_by_port_number[port_number]))
+            for port_data in self.data_by_port_number[port_number]:
+                lines.append(str(port_data))
 
         # These lines are just for formatting
         lines.append(self.DIVIDER)
         lines.append('')
 
         return '\n'.join(lines)
 
@@ -57,15 +62,18 @@
         d['device_types'] = self.device_types
 
         for key in self.additional_service_info:
             d[key] = self.additional_service_info[key]
 
         serialized_port_data = {}
         for port_number in self.data_by_port_number:
-            serialized_port_data[self.value_as_str(port_number)] = self.data_by_port_number[port_number].as_dict()
+            serialized_port_data[self.value_as_str(port_number)] = [
+                port_data.as_dict()
+                for port_data in self.data_by_port_number[port_number]
+            ]
 
         d['port_data'] = serialized_port_data
 
         return d
 
     # Will return a list of dictionaries, with each dictionary containing
     # all of the data for a single row / record in the ultimate output report
@@ -84,49 +92,56 @@
                 value_str = ','.join(self.additional_service_info[key])
             else:
                 value_str = self.additional_service_info[key]
 
             base_dict[key.upper()] = value_str
 
         # 'IP', 'HOSTNAME', 'OS', 'DEVICE TYPE', 'PORT NUMBER', 'PROTOCOL', 'STATE', 'SERVICE', 'VERSION'
-        for port in self.data_by_port_number:
-            # Create a copy of the base_dict to prevent editing that dictionary directly
-            data_dict = base_dict.copy()
-            port_data = self.data_by_port_number[port]
-
-            data_dict['PORT NUMBER'] = self.value_as_str(port_data.port_number)
-            data_dict['PROTOCOL'] = self.value_as_str(port_data.protocol)
-            data_dict['STATE'] = self.value_as_str(port_data.state)
-            data_dict['SERVICE'] = self.value_as_str(port_data.service)
+        for port_number in self.data_by_port_number:
+            for port_data in self.data_by_port_number[port_number]:
+                # Create a copy of the base_dict to prevent editing that dictionary directly
+                data_dict = base_dict.copy()
+                data_dict['PORT NUMBER'] = self.value_as_str(port_data.port_number)
+                data_dict['PROTOCOL'] = self.value_as_str(port_data.protocol)
+                data_dict['STATE'] = self.value_as_str(port_data.state)
+                data_dict['SERVICE'] = self.value_as_str(port_data.service)
 
-            # Escape any comma's in the service version
-            data_dict['VERSION'] = self.value_as_str(port_data.version.replace(',', ''))
+                # Escape any comma's in the service version
+                data_dict['VERSION'] = self.value_as_str(port_data.version.replace(',', ''))
 
-            records.append(data_dict)
+                records.append(data_dict)
 
         return records
 
     def clone(self):
         new_host_data = HostData(self.ip, self.hostname)
         new_host_data.os_list = self.os_list
         new_host_data.device_types = self.device_types
         new_host_data.additional_service_info = self.additional_service_info
         new_host_data.data_by_port_number = {}
 
-        for port in self.data_by_port_number:
-            new_host_data.data_by_port_number[port] = self.data_by_port_number[port].clone()
+        for port_number in self.data_by_port_number:
+            new_host_data.data_by_port_number[port_number] = [
+                port_data.clone()
+                for port_data in self.data_by_port_number[port_number]
+            ]
 
         return new_host_data
 
     def add_data(self, port_data):
         if port_data.port_number in self.data_by_port_number:
-            # TODO: Add functionality for merging PortData objects
-            raise Exception("Data already exists for port %s on host %s" % port_data.port_number, self.ip)
+            port_data_entry_exists = False
+            for existing_port_data in self.data_by_port_number[port_data.port_number]:
+                if existing_port_data == port_data:
+                    port_data_entry_exists = True
+
+            if not port_data_entry_exists:
+                self.data_by_port_number[port_data.port_number].append(port_data)
         else:
-            self.data_by_port_number[port_data.port_number] = port_data
+            self.data_by_port_number[port_data.port_number] = [port_data]
 
     def add_os_data(self, os_data):
         if os_data is None:
             print("WARNING: OS data is empty")
         if type(os_data) is list:
             self.os_list += os_data
         elif type(os_data) is str:
@@ -152,22 +167,29 @@
                 self.additional_service_info[key].append(value)
 
     def filter_by_port(self, port_numbers, state = None):
         filtered_host_data = self.clone()
 
         match_found = False
         new_data_by_port_number = {}
-        for port in self.data_by_port_number:
-            if port in port_numbers:
-                port_data = self.data_by_port_number[port]
-
-                # Ignore port state unless one is provided to filter on
-                if state is None or port_data.state == state:
-                    match_found = True
-                    new_data_by_port_number[port] = port_data.clone()
+        for port_number in self.data_by_port_number:
+            if port_number not in port_numbers:
+                continue
+            
+            for port_data in self.data_by_port_number[port_number]:
+                if state is not None and port_data.state != state:
+                    # Ignore port state unless one is provided to filter on
+                    continue
+                
+                match_found = True
+
+                if port_number in new_data_by_port_number:
+                    new_data_by_port_number[port_number].append(port_data.clone())
+                else:
+                    new_data_by_port_number[port_number] = [port_data.clone()]
 
         filtered_host_data.data_by_port_number = new_data_by_port_number
 
         if match_found:
             return filtered_host_data
         else:
             return None
```

### Comparing `nmap_query_tool-1.1.3/NmapQueryTool/lib/interaction_context.py` & `nmap_query_tool-1.1.4/NmapQueryTool/lib/interaction_context.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.3/NmapQueryTool/lib/nmap_data.py` & `nmap_query_tool-1.1.4/NmapQueryTool/lib/nmap_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.3/NmapQueryTool/lib/port_data.py` & `nmap_query_tool-1.1.4/NmapQueryTool/lib/port_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,26 @@
         tokens.append(self.value_as_str(self.protocol))
         tokens.append(self.value_as_str(self.state))
         tokens.append(self.value_as_str(self.service))
         tokens.append(self.value_as_str(self.version))
 
         return ' '.join(tokens)
 
+    def __eq__(self, other):
+        if type(other) is not PortData:
+            return False
+
+        return (
+            self.port_number == other.port_number
+            and self.protocol == other.protocol
+            and self.state == other.state
+            and self.service == other.service
+            and self.version == other.version
+        )
+
     def as_dict(self):
         d = {}
         d['port_number'] = self.value_as_str(self.port_number)
         d['protocol'] = self.value_as_str(self.protocol)
         d['state'] = self.value_as_str(self.state)
         d['service'] = self.value_as_str(self.service)
         d['version'] = self.value_as_str(self.version)
```

### Comparing `nmap_query_tool-1.1.3/NmapQueryTool/lib/scan_data.py` & `nmap_query_tool-1.1.4/NmapQueryTool/lib/scan_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from .nmap_data import NmapData
 from .host_data import HostData
 from .port_data import PortData
 
 class ScanData(NmapData):
 
     def __init__(self):
-        self.host_data_by_ip = {} # Mapping of IP addresses to HostData objects
+        # Mapping of IP addresses to HostData objects
+        self.host_data_by_ip = {}
 
     def __getitem__(self, ip):
         self.host_data_by_ip[ip]
 
     def __str__(self):
         lines = []
         for ip in self.host_data_by_ip:
```

### Comparing `nmap_query_tool-1.1.3/NmapQueryTool/nmap_query.py` & `nmap_query_tool-1.1.4/NmapQueryTool/nmap_query.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.3/NmapQueryTool/tst/integration_tests.py` & `nmap_query_tool-1.1.4/NmapQueryTool/tst/integration_tests.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.3/PKG-INFO` & `nmap_query_tool-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmap_query_tool
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for parsing and dynamically querying nmap scan data
 Home-page: https://github.com/unheardof/NmapQueryTool
 Author: Timothy Heard
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `nmap_query_tool-1.1.3/README.md` & `nmap_query_tool-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.3/nmap_query_tool.egg-info/PKG-INFO` & `nmap_query_tool-1.1.4/nmap_query_tool.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmap-query-tool
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool for parsing and dynamically querying nmap scan data
 Home-page: https://github.com/unheardof/NmapQueryTool
 Author: Timothy Heard
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `nmap_query_tool-1.1.3/nmap_query_tool.egg-info/SOURCES.txt` & `nmap_query_tool-1.1.4/nmap_query_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.3/setup.py` & `nmap_query_tool-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="nmap_query_tool",
-	version="1.1.3",
+	version="1.1.4",
 	author="Timothy Heard",
 	description="A tool for parsing and dynamically querying nmap scan data",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/unheardof/NmapQueryTool",
 	packages=setuptools.find_packages(),
 	classifiers=[
```

