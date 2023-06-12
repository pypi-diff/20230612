# Comparing `tmp/nmap_query_tool-1.1.2.tar.gz` & `tmp/nmap_query_tool-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nmap_query_tool-1.1.2.tar", last modified: Fri Feb 15 16:33:46 2019, max compression
+gzip compressed data, was "nmap_query_tool-1.1.3.tar", last modified: Mon Jun 12 00:33:14 2023, max compression
```

## Comparing `nmap_query_tool-1.1.2.tar` & `nmap_query_tool-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0 timheard  (1000) timheard  (1000)        0 2019-02-15 16:33:46.000000 nmap_query_tool-1.1.2/
-drwxrwxrwx   0 timheard  (1000) timheard  (1000)        0 2019-02-15 16:33:46.000000 nmap_query_tool-1.1.2/NmapQueryTool/
-drwxrwxrwx   0 timheard  (1000) timheard  (1000)        0 2019-02-15 16:33:46.000000 nmap_query_tool-1.1.2/NmapQueryTool/lib/
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)     6983 2019-02-15 16:31:09.000000 nmap_query_tool-1.1.2/NmapQueryTool/lib/host_data.py
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)     1797 2019-02-15 16:31:09.000000 nmap_query_tool-1.1.2/NmapQueryTool/lib/interaction_context.py
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)      621 2019-02-15 16:31:09.000000 nmap_query_tool-1.1.2/NmapQueryTool/lib/nmap_data.py
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)     1449 2019-02-15 16:31:09.000000 nmap_query_tool-1.1.2/NmapQueryTool/lib/port_data.py
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)     7233 2019-02-15 16:31:09.000000 nmap_query_tool-1.1.2/NmapQueryTool/lib/scan_data.py
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)        0 2019-02-15 16:31:09.000000 nmap_query_tool-1.1.2/NmapQueryTool/lib/__init__.py
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)    14622 2019-02-13 15:06:51.000000 nmap_query_tool-1.1.2/NmapQueryTool/nmap_query.py
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)       23 2018-11-16 02:55:13.000000 nmap_query_tool-1.1.2/NmapQueryTool/__init__.py
-drwxrwxrwx   0 timheard  (1000) timheard  (1000)        0 2019-02-15 16:33:46.000000 nmap_query_tool-1.1.2/nmap_query_tool.egg-info/
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)        1 2019-02-15 16:33:45.000000 nmap_query_tool-1.1.2/nmap_query_tool.egg-info/dependency_links.txt
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)     2660 2019-02-15 16:33:45.000000 nmap_query_tool-1.1.2/nmap_query_tool.egg-info/PKG-INFO
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)      423 2019-02-15 16:33:45.000000 nmap_query_tool-1.1.2/nmap_query_tool.egg-info/SOURCES.txt
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)       14 2019-02-15 16:33:45.000000 nmap_query_tool-1.1.2/nmap_query_tool.egg-info/top_level.txt
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)     2660 2019-02-15 16:33:46.000000 nmap_query_tool-1.1.2/PKG-INFO
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)     1815 2018-11-16 02:55:13.000000 nmap_query_tool-1.1.2/README.md
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)       38 2019-02-15 16:33:46.000000 nmap_query_tool-1.1.2/setup.cfg
--rwxrwxrwx   0 timheard  (1000) timheard  (1000)      605 2019-02-15 16:23:47.000000 nmap_query_tool-1.1.2/setup.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    11357 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/LICENSE
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.906946 nmap_query_tool-1.1.3/NmapQueryTool/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       23 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/__init__.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.924203 nmap_query_tool-1.1.3/NmapQueryTool/lib/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     6983 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/host_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1797 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/interaction_context.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      621 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/nmap_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     1449 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/port_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     7260 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/lib/scan_data.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)    14622 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/nmap_query.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      239 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/run_tests.py
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.924203 nmap_query_tool-1.1.3/NmapQueryTool/tst/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        0 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/tst/__init__.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     8571 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/NmapQueryTool/tst/integration_tests.py
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2105 2023-06-11 23:28:53.000000 nmap_query_tool-1.1.3/README.md
+drwxr-xr-x   0 timheard  (1000) timheard  (1000)        0 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/
+-rw-r--r--   0 timheard  (1000) timheard  (1000)     2601 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      527 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)        1 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       14 2023-06-12 00:33:14.000000 nmap_query_tool-1.1.3/nmap_query_tool.egg-info/top_level.txt
+-rw-r--r--   0 timheard  (1000) timheard  (1000)       38 2023-06-12 00:33:14.954273 nmap_query_tool-1.1.3/setup.cfg
+-rw-r--r--   0 timheard  (1000) timheard  (1000)      605 2023-06-12 00:31:19.000000 nmap_query_tool-1.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nmap_query_tool-1.1.2/NmapQueryTool/lib/host_data.py` & `nmap_query_tool-1.1.3/NmapQueryTool/lib/host_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.2/NmapQueryTool/lib/interaction_context.py` & `nmap_query_tool-1.1.3/NmapQueryTool/lib/interaction_context.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.2/NmapQueryTool/lib/nmap_data.py` & `nmap_query_tool-1.1.3/NmapQueryTool/lib/nmap_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.2/NmapQueryTool/lib/port_data.py` & `nmap_query_tool-1.1.3/NmapQueryTool/lib/port_data.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.2/NmapQueryTool/lib/scan_data.py` & `nmap_query_tool-1.1.3/NmapQueryTool/lib/scan_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         print(str(self))
 
     @staticmethod
     def create_from_nmap_data(data_source):
         scan_data = ScanData()
 
         for line in data_source:
-            if re.match('Nmap scan report for .*', line):
+            if re.match('^Nmap scan report for ([0-9]{1,3}\.){3}[0-9]{1,3}$', line):
                 host_and_ip_data = re.match('Nmap scan report for (.*)', line).group(1)
 
                 # Handles the following two types of line formats:
                 #
                 # Nmap scan report for 10.90.78.103
                 # Nmap scan report for atsva9078153.vbschools.com (10.90.78.153)
                 host_ip = None
```

### Comparing `nmap_query_tool-1.1.2/NmapQueryTool/nmap_query.py` & `nmap_query_tool-1.1.3/NmapQueryTool/nmap_query.py`

 * *Files identical despite different names*

### Comparing `nmap_query_tool-1.1.2/nmap_query_tool.egg-info/PKG-INFO` & `nmap_query_tool-1.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,53 @@
-Metadata-Version: 2.1
-Name: nmap-query-tool
-Version: 1.1.2
-Summary: A tool for parsing and dynamically querying nmap scan data
-Home-page: https://github.com/unheardof/NmapQueryTool
-Author: Timothy Heard
-License: UNKNOWN
-Description: # NMAP Query Tool
-        Post-processor for nmap output that allows fast, simple filtering of data both interactively and inline (i.e. via a bash pipe).
-        
-        ```bash
-        Usage: python nmap-query.py [-h] [-p PORTS] [-a IPS] [-os OS] [-d DEVICE_TYPE] [-c] [-i NMAP_SCAN_RESULTS_FILE] [-o OUTPUT_FILENAME] [-q]
-        
-                Note: the nmap scan results can be provided either through an input file or from STDIN (through a pipe)
-        
-                Example: nmap -sV 10.0.0.0/24 | python nmap-query.py -q
-        
-        
-        
-        [-h | --help]: Will print the help/usage message
-        
-        [-p | --ports] PORTS: specify one or more (open) ports to filter on. The following input formats are accepted:
-        
-                Single port number: -p 22
-                Set of port numbers: -p 22,80,443
-        
-        [-a | --ip-addrs] IPS: specify one or more IP addresses on which to filter. The following input formats are accepted:
-        
-                Single IP: -a 10.0.0.1
-                Set of IPs: -a 10.0.0.1,10.0.0.2,10.0.0.3
-                Single CIDR block: -a 10.0.0.0/24
-                Set of CIDR blocks: -a 10.0.0.0/24,10.0.1.0/24
-                Range of IPs: -a 10.0.0.1-4
-        
-        [-os | --operating-system] OS: specify one or more operating systems on which to filter. The following input formats are accepted:
-        
-                Single operating system: -os Windws
-                Set of operating systems: -os Windows,Linux
-        
-        [-d | --device-type] DEVICE_TYPE: specify one or more device types on which to filter. The following input formats are accepted:
-        
-                Single device type: -d router
-                Set of device types: -d router,switch
-        
-        [-c | --output-csv]: use CSV as the output format
-        
-        [-i | --input-file] NMAP_SCAN_RESULTS_FILE: specify the name of the input file (i.e. the file which contains the results of the Nmap scan)
-        
-        [-o | --output-file] OUTPUT_FILENAME: specify the name of the output file
-        
-        [-q | --query-mode]: enter the interactive query mode
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Description-Content-Type: text/markdown
+# NMAP Query Tool
+Post-processor for nmap output that allows fast, simple filtering of data both interactively and inline (i.e. via a bash pipe).
+
+```bash
+Usage: python nmap-query.py [-h] [-p PORTS] [-a IPS] [-os OS] [-d DEVICE_TYPE] [-c] [-i NMAP_SCAN_RESULTS_FILE] [-o OUTPUT_FILENAME] [-q]
+
+        Note: the nmap scan results can be provided either through an input file or from STDIN (through a pipe)
+
+        Example: nmap -sV 10.0.0.0/24 | python nmap-query.py -q
+
+
+
+[-h | --help]: Will print the help/usage message
+
+[-p | --ports] PORTS: specify one or more (open) ports to filter on. The following input formats are accepted:
+
+        Single port number: -p 22
+        Set of port numbers: -p 22,80,443
+
+[-a | --ip-addrs] IPS: specify one or more IP addresses on which to filter. The following input formats are accepted:
+
+        Single IP: -a 10.0.0.1
+        Set of IPs: -a 10.0.0.1,10.0.0.2,10.0.0.3
+        Single CIDR block: -a 10.0.0.0/24
+        Set of CIDR blocks: -a 10.0.0.0/24,10.0.1.0/24
+        Range of IPs: -a 10.0.0.1-4
+
+[-os | --operating-system] OS: specify one or more operating systems on which to filter. The following input formats are accepted:
+
+        Single operating system: -os Windws
+        Set of operating systems: -os Windows,Linux
+
+[-d | --device-type] DEVICE_TYPE: specify one or more device types on which to filter. The following input formats are accepted:
+
+        Single device type: -d router
+        Set of device types: -d router,switch
+
+[-c | --output-csv]: use CSV as the output format
+
+[-i | --input-file] NMAP_SCAN_RESULTS_FILE: specify the name of the input file (i.e. the file which contains the results of the Nmap scan)
+
+[-o | --output-file] OUTPUT_FILENAME: specify the name of the output file
+
+[-q | --query-mode]: enter the interactive query mode
+```
+
+# Locate script install location
+
+1. `pip3 show nmap-query-tool`; will show the install directory of the package
+1. `cd <INSTALL DIRECTORY>/NmapQueryTool`
+1. `python3 nmap_query_tool.py`
+
+You can also setup an alias for running the script: `alias nmap-query="python3 ${pwd}/nmap_query.py"`
```

### Comparing `nmap_query_tool-1.1.2/PKG-INFO` & `nmap_query_tool-1.1.3/nmap_query_tool.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 Metadata-Version: 2.1
-Name: nmap_query_tool
-Version: 1.1.2
+Name: nmap-query-tool
+Version: 1.1.3
 Summary: A tool for parsing and dynamically querying nmap scan data
 Home-page: https://github.com/unheardof/NmapQueryTool
 Author: Timothy Heard
 License: UNKNOWN
-Description: # NMAP Query Tool
-        Post-processor for nmap output that allows fast, simple filtering of data both interactively and inline (i.e. via a bash pipe).
-        
-        ```bash
-        Usage: python nmap-query.py [-h] [-p PORTS] [-a IPS] [-os OS] [-d DEVICE_TYPE] [-c] [-i NMAP_SCAN_RESULTS_FILE] [-o OUTPUT_FILENAME] [-q]
-        
-                Note: the nmap scan results can be provided either through an input file or from STDIN (through a pipe)
-        
-                Example: nmap -sV 10.0.0.0/24 | python nmap-query.py -q
-        
-        
-        
-        [-h | --help]: Will print the help/usage message
-        
-        [-p | --ports] PORTS: specify one or more (open) ports to filter on. The following input formats are accepted:
-        
-                Single port number: -p 22
-                Set of port numbers: -p 22,80,443
-        
-        [-a | --ip-addrs] IPS: specify one or more IP addresses on which to filter. The following input formats are accepted:
-        
-                Single IP: -a 10.0.0.1
-                Set of IPs: -a 10.0.0.1,10.0.0.2,10.0.0.3
-                Single CIDR block: -a 10.0.0.0/24
-                Set of CIDR blocks: -a 10.0.0.0/24,10.0.1.0/24
-                Range of IPs: -a 10.0.0.1-4
-        
-        [-os | --operating-system] OS: specify one or more operating systems on which to filter. The following input formats are accepted:
-        
-                Single operating system: -os Windws
-                Set of operating systems: -os Windows,Linux
-        
-        [-d | --device-type] DEVICE_TYPE: specify one or more device types on which to filter. The following input formats are accepted:
-        
-                Single device type: -d router
-                Set of device types: -d router,switch
-        
-        [-c | --output-csv]: use CSV as the output format
-        
-        [-i | --input-file] NMAP_SCAN_RESULTS_FILE: specify the name of the input file (i.e. the file which contains the results of the Nmap scan)
-        
-        [-o | --output-file] OUTPUT_FILENAME: specify the name of the output file
-        
-        [-q | --query-mode]: enter the interactive query mode
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# NMAP Query Tool
+Post-processor for nmap output that allows fast, simple filtering of data both interactively and inline (i.e. via a bash pipe).
+
+```bash
+Usage: python nmap-query.py [-h] [-p PORTS] [-a IPS] [-os OS] [-d DEVICE_TYPE] [-c] [-i NMAP_SCAN_RESULTS_FILE] [-o OUTPUT_FILENAME] [-q]
+
+        Note: the nmap scan results can be provided either through an input file or from STDIN (through a pipe)
+
+        Example: nmap -sV 10.0.0.0/24 | python nmap-query.py -q
+
+
+
+[-h | --help]: Will print the help/usage message
+
+[-p | --ports] PORTS: specify one or more (open) ports to filter on. The following input formats are accepted:
+
+        Single port number: -p 22
+        Set of port numbers: -p 22,80,443
+
+[-a | --ip-addrs] IPS: specify one or more IP addresses on which to filter. The following input formats are accepted:
+
+        Single IP: -a 10.0.0.1
+        Set of IPs: -a 10.0.0.1,10.0.0.2,10.0.0.3
+        Single CIDR block: -a 10.0.0.0/24
+        Set of CIDR blocks: -a 10.0.0.0/24,10.0.1.0/24
+        Range of IPs: -a 10.0.0.1-4
+
+[-os | --operating-system] OS: specify one or more operating systems on which to filter. The following input formats are accepted:
+
+        Single operating system: -os Windws
+        Set of operating systems: -os Windows,Linux
+
+[-d | --device-type] DEVICE_TYPE: specify one or more device types on which to filter. The following input formats are accepted:
+
+        Single device type: -d router
+        Set of device types: -d router,switch
+
+[-c | --output-csv]: use CSV as the output format
+
+[-i | --input-file] NMAP_SCAN_RESULTS_FILE: specify the name of the input file (i.e. the file which contains the results of the Nmap scan)
+
+[-o | --output-file] OUTPUT_FILENAME: specify the name of the output file
+
+[-q | --query-mode]: enter the interactive query mode
+```
+
+# Locate script install location
+
+1. `pip3 show nmap-query-tool`; will show the install directory of the package
+1. `cd <INSTALL DIRECTORY>/NmapQueryTool`
+1. `python3 nmap_query_tool.py`
+
+You can also setup an alias for running the script: `alias nmap-query="python3 ${pwd}/nmap_query.py"`
+
```

### Comparing `nmap_query_tool-1.1.2/setup.py` & `nmap_query_tool-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="nmap_query_tool",
-	version="1.1.2",
+	version="1.1.3",
 	author="Timothy Heard",
 	description="A tool for parsing and dynamically querying nmap scan data",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/unheardof/NmapQueryTool",
 	packages=setuptools.find_packages(),
 	classifiers=[
```

