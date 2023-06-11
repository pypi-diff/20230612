# Comparing `tmp/decomp2dbg-3.4.0.tar.gz` & `tmp/decomp2dbg-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decomp2dbg-3.4.0.tar", last modified: Thu May 25 05:08:28 2023, max compression
+gzip compressed data, was "decomp2dbg-3.5.0.tar", last modified: Sun Jun 11 22:03:24 2023, max compression
```

## Comparing `decomp2dbg-3.4.0.tar` & `decomp2dbg-3.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/d2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.670799 decomp2dbg-3.4.0/decomp2dbg/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decomp2dbg/clients/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/decompiler_pane.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gdb_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gef_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/pwndbg_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/symbol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/clients/gdb/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decomp2dbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decomp2dbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 05:08:28.000000 decomp2dbg-3.4.0/decomp2dbg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_angr/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_angr/d2d_angr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_angr/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_binja/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/d2d_binja.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_binja/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_ida/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/decompilers/server_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-25 05:08:28.674800 decomp2dbg-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-25 05:08:18.000000 decomp2dbg-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/d2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.962026 decomp2dbg-3.5.0/decomp2dbg/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decomp2dbg/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/decompiler_pane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/gdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/gef_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/pwndbg_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/symbol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/clients/gdb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decomp2dbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decomp2dbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-06-11 22:03:24.000000 decomp2dbg-3.5.0/decomp2dbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-11 22:03:24.000000 decomp2dbg-3.5.0/decomp2dbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 22:03:24.000000 decomp2dbg-3.5.0/decomp2dbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-11 22:03:24.000000 decomp2dbg-3.5.0/decomp2dbg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-11 22:03:24.000000 decomp2dbg-3.5.0/decomp2dbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-11 22:03:24.000000 decomp2dbg-3.5.0/decomp2dbg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decompilers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decompilers/d2d_angr/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decompilers/d2d_angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decompilers/d2d_angr/d2d_angr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decompilers/d2d_angr/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decompilers/d2d_binja/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decompilers/d2d_binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decompilers/d2d_binja/d2d_binja.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decompilers/d2d_binja/plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-11 22:03:15.000000 decomp2dbg-3.5.0/decompilers/d2d_binja/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decompilers/d2d_ida/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:24.966027 decomp2dbg-3.5.0/decompilers/d2d_ida/d2d_ida/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 22:03:16.000000 decomp2dbg-3.5.0/decompilers/d2d_ida/d2d_ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-11 22:03:16.000000 decomp2dbg-3.5.0/decompilers/d2d_ida/d2d_ida/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-11 22:03:16.000000 decomp2dbg-3.5.0/decompilers/d2d_ida/d2d_ida/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-11 22:03:16.000000 decomp2dbg-3.5.0/decompilers/d2d_ida/d2d_ida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-11 22:03:16.000000 decomp2dbg-3.5.0/decompilers/server_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-11 22:03:24.970027 decomp2dbg-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-11 22:03:16.000000 decomp2dbg-3.5.0/setup.py
```

### Comparing `decomp2dbg-3.4.0/LICENSE` & `decomp2dbg-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/PKG-INFO` & `decomp2dbg-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.4.0
+Version: 3.5.0
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
@@ -46,15 +46,15 @@
 ## Install
 Install through pip, then use the built-in installer for decompilers:
 ```bash
 pip3 install decomp2dbg && decomp2dbg --install 
 ```
 
 This will open a prompt where you be asked to input the path to your decompiler and debugger of choice. For Ghidra installs,
-you must follow the extra steps to enable extensions [here](https://github.com/mahaloz/d2d-ghidra-plugin).
+you must follow the extra steps to enable extensions [here](https://github.com/mahaloz/decomp2dbg/tree/main/decompilers/d2d_ghidra/README.md).
 If you installed the decompiler-side in the Binja Plugin Manager, you still need to install the debugger side with the above.
 
 **Note**: You may need to allow inbound connections on port 3662, or the port you use, for decomp2dbg to connect
 to the decompiler. If you are installing decomp2dbg with GEF or pwndbg it's important that in your `~/.gdbinit` the
 `d2d.py` file is sourced after GEF or pwndbg.
 
 ## Manual Install 
@@ -80,15 +80,15 @@
 pip3 install . && \
 cp d2d.py ~/.d2d.py && echo "source ~/.d2d.py" >> ~/.gdbinit
 ```
 
 ## Usage 
 First, start the decompilation server on your decompiler. You may want to wait
 until your decompiler finishes its normal analysis before starting it. After normal analysis, this can be done by using the hotkey `Ctrl-Shift-D`,
-or selecting the `decomp2GEF: configure` tab in your associated plugins tab. After starting the server, you should
+or selecting the `decomp2dbg: configure` tab in your associated plugins tab. After starting the server, you should
 see a message in your decompiler
 ```
 [+] Starting XMLRPC server: localhost:3662
 [+] Registered decompilation server!
 ```
 
 Next, in your debugger, run:
```

### Comparing `decomp2dbg-3.4.0/README.md` & `decomp2dbg-3.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ## Install
 Install through pip, then use the built-in installer for decompilers:
 ```bash
 pip3 install decomp2dbg && decomp2dbg --install 
 ```
 
 This will open a prompt where you be asked to input the path to your decompiler and debugger of choice. For Ghidra installs,
-you must follow the extra steps to enable extensions [here](https://github.com/mahaloz/d2d-ghidra-plugin).
+you must follow the extra steps to enable extensions [here](https://github.com/mahaloz/decomp2dbg/tree/main/decompilers/d2d_ghidra/README.md).
 If you installed the decompiler-side in the Binja Plugin Manager, you still need to install the debugger side with the above.
 
 **Note**: You may need to allow inbound connections on port 3662, or the port you use, for decomp2dbg to connect
 to the decompiler. If you are installing decomp2dbg with GEF or pwndbg it's important that in your `~/.gdbinit` the
 `d2d.py` file is sourced after GEF or pwndbg.
 
 ## Manual Install 
@@ -67,15 +67,15 @@
 pip3 install . && \
 cp d2d.py ~/.d2d.py && echo "source ~/.d2d.py" >> ~/.gdbinit
 ```
 
 ## Usage 
 First, start the decompilation server on your decompiler. You may want to wait
 until your decompiler finishes its normal analysis before starting it. After normal analysis, this can be done by using the hotkey `Ctrl-Shift-D`,
-or selecting the `decomp2GEF: configure` tab in your associated plugins tab. After starting the server, you should
+or selecting the `decomp2dbg: configure` tab in your associated plugins tab. After starting the server, you should
 see a message in your decompiler
 ```
 [+] Starting XMLRPC server: localhost:3662
 [+] Registered decompilation server!
 ```
 
 Next, in your debugger, run:
```

### Comparing `decomp2dbg-3.4.0/d2d.py` & `decomp2dbg-3.5.0/d2d.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/__main__.py` & `decomp2dbg-3.5.0/decomp2dbg/__main__.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/clients/client.py` & `decomp2dbg-3.5.0/decomp2dbg/clients/client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/decompiler_pane.py` & `decomp2dbg-3.5.0/decomp2dbg/clients/gdb/decompiler_pane.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gdb_client.py` & `decomp2dbg-3.5.0/decomp2dbg/clients/gdb/gdb_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/gef_client.py` & `decomp2dbg-3.5.0/decomp2dbg/clients/gdb/gef_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/pwndbg_client.py` & `decomp2dbg-3.5.0/decomp2dbg/clients/gdb/pwndbg_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/symbol_mapper.py` & `decomp2dbg-3.5.0/decomp2dbg/clients/gdb/symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/clients/gdb/utils.py` & `decomp2dbg-3.5.0/decomp2dbg/clients/gdb/utils.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg/installer.py` & `decomp2dbg-3.5.0/decomp2dbg/installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
           ____/ /__  _________  ____ ___  ____ |__ \ ____/ / /_  ____ _
          / __  / _ \/ ___/ __ \/ __ `__ \/ __ \__/ // __  / __ \/ __ `/
         / /_/ /  __/ /__/ /_/ / / / / / / /_/ / __// /_/ / /_/ / /_/ / 
         \__,_/\___/\___/\____/_/ /_/ /_/ .___/____/\__,_/_.___/\__, /  
                                       /_/                     /____/   
         Now installing decomp2dbg...
         Please input decompiler/debugger install paths as prompted. Enter nothing to either use
-        the default install path if one exist, or to skip.
+        the default install path if one exists, or to skip.
         """))
 
     def install_gdb(self, path=None):
         path = super().install_gdb(path=None)
         if path is None:
             return None
```

### Comparing `decomp2dbg-3.4.0/decomp2dbg/utils.py` & `decomp2dbg-3.5.0/decomp2dbg/utils.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decomp2dbg.egg-info/PKG-INFO` & `decomp2dbg-3.5.0/decomp2dbg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.4.0
+Version: 3.5.0
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
@@ -46,15 +46,15 @@
 ## Install
 Install through pip, then use the built-in installer for decompilers:
 ```bash
 pip3 install decomp2dbg && decomp2dbg --install 
 ```
 
 This will open a prompt where you be asked to input the path to your decompiler and debugger of choice. For Ghidra installs,
-you must follow the extra steps to enable extensions [here](https://github.com/mahaloz/d2d-ghidra-plugin).
+you must follow the extra steps to enable extensions [here](https://github.com/mahaloz/decomp2dbg/tree/main/decompilers/d2d_ghidra/README.md).
 If you installed the decompiler-side in the Binja Plugin Manager, you still need to install the debugger side with the above.
 
 **Note**: You may need to allow inbound connections on port 3662, or the port you use, for decomp2dbg to connect
 to the decompiler. If you are installing decomp2dbg with GEF or pwndbg it's important that in your `~/.gdbinit` the
 `d2d.py` file is sourced after GEF or pwndbg.
 
 ## Manual Install 
@@ -80,15 +80,15 @@
 pip3 install . && \
 cp d2d.py ~/.d2d.py && echo "source ~/.d2d.py" >> ~/.gdbinit
 ```
 
 ## Usage 
 First, start the decompilation server on your decompiler. You may want to wait
 until your decompiler finishes its normal analysis before starting it. After normal analysis, this can be done by using the hotkey `Ctrl-Shift-D`,
-or selecting the `decomp2GEF: configure` tab in your associated plugins tab. After starting the server, you should
+or selecting the `decomp2dbg: configure` tab in your associated plugins tab. After starting the server, you should
 see a message in your decompiler
 ```
 [+] Starting XMLRPC server: localhost:3662
 [+] Registered decompilation server!
 ```
 
 Next, in your debugger, run:
```

### Comparing `decomp2dbg-3.4.0/decomp2dbg.egg-info/SOURCES.txt` & `decomp2dbg-3.5.0/decomp2dbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/d2d_angr/d2d_angr.py` & `decomp2dbg-3.5.0/decompilers/d2d_angr/d2d_angr.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/d2d_angr/server.py` & `decomp2dbg-3.5.0/decompilers/d2d_angr/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/d2d_binja/d2d_binja.py` & `decomp2dbg-3.5.0/decompilers/d2d_binja/d2d_binja.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/d2d_binja/plugin.json` & `decomp2dbg-3.5.0/decompilers/d2d_binja/plugin.json`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/d2d_binja/server.py` & `decomp2dbg-3.5.0/decompilers/d2d_binja/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/plugin.py` & `decomp2dbg-3.5.0/decompilers/d2d_ida/d2d_ida/plugin.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/d2d_ida/d2d_ida/server.py` & `decomp2dbg-3.5.0/decompilers/d2d_ida/d2d_ida/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/decompilers/server_template.py` & `decomp2dbg-3.5.0/decompilers/server_template.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/setup.cfg` & `decomp2dbg-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.4.0/setup.py` & `decomp2dbg-3.5.0/setup.py`

 * *Files identical despite different names*

