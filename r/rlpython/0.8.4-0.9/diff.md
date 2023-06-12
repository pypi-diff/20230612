# Comparing `tmp/rlpython-0.8.4.tar.gz` & `tmp/rlpython-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlpython-0.8.4.tar", last modified: Mon Oct 18 08:36:57 2021, max compression
+gzip compressed data, was "rlpython-0.9.tar", last modified: Sat May 14 11:14:33 2022, max compression
```

## Comparing `rlpython-0.8.4.tar` & `rlpython-0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-10-18 08:36:57.813607 rlpython-0.8.4/
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1071 2021-03-06 14:46:35.000000 rlpython-0.8.4/LICENSE.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2272 2021-10-18 08:36:57.813607 rlpython-0.8.4/PKG-INFO
--rw-r--r--   0 fsc       (1000) fsc       (1000)      990 2021-04-06 06:42:02.000000 rlpython-0.8.4/README.rst
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-10-18 08:36:57.809607 rlpython-0.8.4/bin/
--rwxr-xr-x   0 fsc       (1000) fsc       (1000)      172 2021-03-17 11:21:52.000000 rlpython-0.8.4/bin/rlpython
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-10-18 08:36:57.809607 rlpython-0.8.4/rlpython/
--rw-r--r--   0 fsc       (1000) fsc       (1000)      128 2021-10-18 08:34:59.000000 rlpython-0.8.4/rlpython/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      994 2021-05-16 08:15:48.000000 rlpython-0.8.4/rlpython/aliases.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2360 2021-04-26 07:05:49.000000 rlpython-0.8.4/rlpython/command_line.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-10-18 08:36:57.813607 rlpython-0.8.4/rlpython/commands/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-03-10 09:08:38.000000 rlpython-0.8.4/rlpython/commands/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1196 2021-04-26 07:12:16.000000 rlpython-0.8.4/rlpython/commands/aliases.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2094 2021-06-07 06:28:50.000000 rlpython-0.8.4/rlpython/commands/edit.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1198 2021-05-15 11:04:06.000000 rlpython-0.8.4/rlpython/commands/loops.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1611 2021-05-15 11:04:06.000000 rlpython-0.8.4/rlpython/commands/tasks.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2538 2021-10-14 06:48:45.000000 rlpython-0.8.4/rlpython/commands/threads.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2060 2021-04-26 07:05:49.000000 rlpython-0.8.4/rlpython/commands/unix_environment.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2043 2021-05-16 08:14:07.000000 rlpython-0.8.4/rlpython/commands/variables.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     9464 2021-10-18 08:30:48.000000 rlpython-0.8.4/rlpython/completion.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2681 2021-04-30 07:51:12.000000 rlpython-0.8.4/rlpython/embed.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      247 2021-03-17 11:21:52.000000 rlpython-0.8.4/rlpython/frontend.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      759 2021-04-30 07:51:12.000000 rlpython-0.8.4/rlpython/logging.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2533 2021-04-30 07:51:12.000000 rlpython-0.8.4/rlpython/protocol.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    10627 2021-10-13 19:14:18.000000 rlpython-0.8.4/rlpython/repl.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5434 2021-07-24 16:10:44.000000 rlpython-0.8.4/rlpython/repl_client.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     3456 2021-04-30 07:51:12.000000 rlpython-0.8.4/rlpython/repl_connection.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4452 2021-10-14 09:06:14.000000 rlpython-0.8.4/rlpython/repl_server.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-10-18 08:36:57.813607 rlpython-0.8.4/rlpython/runtimes/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-04-30 07:24:04.000000 rlpython-0.8.4/rlpython/runtimes/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2362 2021-04-26 07:12:16.000000 rlpython-0.8.4/rlpython/runtimes/command_runtime.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5987 2021-04-26 07:12:16.000000 rlpython-0.8.4/rlpython/runtimes/python_runtime.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2383 2021-04-30 07:24:04.000000 rlpython-0.8.4/rlpython/runtimes/shell_runtime.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1896 2021-04-26 07:12:16.000000 rlpython-0.8.4/rlpython/templating.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-10-18 08:36:57.813607 rlpython-0.8.4/rlpython/utils/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-03-10 09:08:38.000000 rlpython-0.8.4/rlpython/utils/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      478 2021-03-10 09:08:38.000000 rlpython-0.8.4/rlpython/utils/argument_parser.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      365 2021-04-06 06:41:51.000000 rlpython-0.8.4/rlpython/utils/asyncio_utils.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      359 2021-04-06 06:41:51.000000 rlpython-0.8.4/rlpython/utils/attribute_table.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      582 2021-03-10 09:08:38.000000 rlpython-0.8.4/rlpython/utils/editor.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      358 2021-04-06 06:41:51.000000 rlpython-0.8.4/rlpython/utils/gc_utils.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      836 2021-03-17 11:21:52.000000 rlpython-0.8.4/rlpython/utils/strings.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1890 2021-04-06 06:41:51.000000 rlpython-0.8.4/rlpython/utils/table.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      758 2021-10-14 09:09:38.000000 rlpython-0.8.4/rlpython/utils/url.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-10-18 08:36:57.809607 rlpython-0.8.4/rlpython.egg-info/
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2272 2021-10-18 08:36:57.000000 rlpython-0.8.4/rlpython.egg-info/PKG-INFO
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1093 2021-10-18 08:36:57.000000 rlpython-0.8.4/rlpython.egg-info/SOURCES.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)        1 2021-10-18 08:36:57.000000 rlpython-0.8.4/rlpython.egg-info/dependency_links.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)        9 2021-10-18 08:36:57.000000 rlpython-0.8.4/rlpython.egg-info/top_level.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)      553 2021-10-18 08:36:57.813607 rlpython-0.8.4/setup.cfg
--rwxr-xr-x   0 fsc       (1000) fsc       (1000)      458 2021-03-10 13:04:40.000000 rlpython-0.8.4/setup.py
+drwxrwxr-x   0 fls       (1000) fls       (1000)        0 2022-05-14 11:14:33.325384 rlpython-0.9/
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1071 2022-05-14 09:33:07.000000 rlpython-0.9/LICENSE.txt
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1749 2022-05-14 11:14:33.325384 rlpython-0.9/PKG-INFO
+-rw-rw-r--   0 fls       (1000) fls       (1000)      990 2022-05-14 09:33:07.000000 rlpython-0.9/README.rst
+drwxrwxr-x   0 fls       (1000) fls       (1000)        0 2022-05-14 11:14:33.317384 rlpython-0.9/bin/
+-rwxrwxr-x   0 fls       (1000) fls       (1000)      172 2022-05-14 09:33:07.000000 rlpython-0.9/bin/rlpython
+drwxrwxr-x   0 fls       (1000) fls       (1000)        0 2022-05-14 11:14:33.321384 rlpython-0.9/rlpython/
+-rw-rw-r--   0 fls       (1000) fls       (1000)      125 2022-05-14 11:13:09.000000 rlpython-0.9/rlpython/__init__.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      948 2022-05-14 11:12:25.000000 rlpython-0.9/rlpython/aliases.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2260 2022-05-14 11:12:25.000000 rlpython-0.9/rlpython/command_line.py
+drwxrwxr-x   0 fls       (1000) fls       (1000)        0 2022-05-14 11:14:33.325384 rlpython-0.9/rlpython/commands/
+-rw-rw-r--   0 fls       (1000) fls       (1000)        0 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/commands/__init__.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1196 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/commands/aliases.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2094 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/commands/edit.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1198 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/commands/loops.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1611 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/commands/tasks.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2538 2022-05-14 09:33:33.000000 rlpython-0.9/rlpython/commands/threads.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2060 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/commands/unix_environment.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2043 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/commands/variables.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     9303 2022-05-14 11:12:25.000000 rlpython-0.9/rlpython/completion.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2591 2022-05-14 11:12:25.000000 rlpython-0.9/rlpython/embed.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      247 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/frontend.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      759 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/logging.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2533 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/protocol.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)    10683 2022-05-14 11:12:25.000000 rlpython-0.9/rlpython/repl.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     5434 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/repl_client.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     3456 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/repl_connection.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     4452 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/repl_server.py
+drwxrwxr-x   0 fls       (1000) fls       (1000)        0 2022-05-14 11:14:33.325384 rlpython-0.9/rlpython/runtimes/
+-rw-rw-r--   0 fls       (1000) fls       (1000)        0 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/runtimes/__init__.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2362 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/runtimes/command_runtime.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     5997 2022-05-14 11:12:25.000000 rlpython-0.9/rlpython/runtimes/python_runtime.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     2383 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/runtimes/shell_runtime.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1896 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/templating.py
+drwxrwxr-x   0 fls       (1000) fls       (1000)        0 2022-05-14 11:14:33.325384 rlpython-0.9/rlpython/utils/
+-rw-rw-r--   0 fls       (1000) fls       (1000)        0 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/__init__.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      478 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/argument_parser.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      365 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/asyncio_utils.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      359 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/attribute_table.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      582 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/editor.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      358 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/gc_utils.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      836 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/strings.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1890 2022-05-14 09:33:07.000000 rlpython-0.9/rlpython/utils/table.py
+-rw-rw-r--   0 fls       (1000) fls       (1000)      758 2022-05-14 09:33:33.000000 rlpython-0.9/rlpython/utils/url.py
+drwxrwxr-x   0 fls       (1000) fls       (1000)        0 2022-05-14 11:14:33.321384 rlpython-0.9/rlpython.egg-info/
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1749 2022-05-14 11:14:33.000000 rlpython-0.9/rlpython.egg-info/PKG-INFO
+-rw-rw-r--   0 fls       (1000) fls       (1000)     1093 2022-05-14 11:14:33.000000 rlpython-0.9/rlpython.egg-info/SOURCES.txt
+-rw-rw-r--   0 fls       (1000) fls       (1000)        1 2022-05-14 11:14:33.000000 rlpython-0.9/rlpython.egg-info/dependency_links.txt
+-rw-rw-r--   0 fls       (1000) fls       (1000)        9 2022-05-14 11:14:33.000000 rlpython-0.9/rlpython.egg-info/top_level.txt
+-rw-rw-r--   0 fls       (1000) fls       (1000)      553 2022-05-14 11:14:33.325384 rlpython-0.9/setup.cfg
+-rwxrwxr-x   0 fls       (1000) fls       (1000)      458 2022-05-14 09:33:07.000000 rlpython-0.9/setup.py
```

### Comparing `rlpython-0.8.4/LICENSE.txt` & `rlpython-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/README.rst` & `rlpython-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/aliases.py` & `rlpython-0.9/rlpython/aliases.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,23 +22,21 @@
     def resolve(self, command):
         # check for name collisions with repl variables
         if '=' in command:
             return command
 
         _command = command.strip()
 
-        if(_command in self.repl.globals or
-           _command in self.repl.locals):
-
+        if _command in self.repl.globals:
             return command
 
         # resolve aliases
         for name, value in self.aliases.items():
             if not command.startswith(name):
                 continue
 
-            if(len(command) >= len(name) and
+            if(len(command) > len(name) and
                command[len(name)] in (' ', '\n', '\t')):
 
                 return '{}{}'.format(value, command[len(name):])
 
         return command
```

### Comparing `rlpython-0.8.4/rlpython/command_line.py` & `rlpython-0.9/rlpython/command_line.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,32 +62,27 @@
             restore_pgrp()
 
         exit(0)
 
     # local mode
     repl_kwargs = {}
 
-    for key in dir(namespace):
-        if key.startswith('_'):
-            continue
+    for key, value in vars(namespace).items():
 
-        if key in ('frontend_mode'):
+        if key in ('frontend_mode',):
             continue
 
-        value = getattr(namespace, key)
-
         if value is None:
             continue
 
         repl_kwargs[key] = value
 
     try:
         embed(
             globals={},
-            locals={},
             single_threaded=True,
             started_from_cmd_line=True,
             **repl_kwargs,
         )
 
     finally:
         if namespace.frontend_mode:
```

### Comparing `rlpython-0.8.4/rlpython/commands/aliases.py` & `rlpython-0.9/rlpython/commands/aliases.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/commands/edit.py` & `rlpython-0.9/rlpython/commands/edit.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/commands/loops.py` & `rlpython-0.9/rlpython/commands/loops.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/commands/tasks.py` & `rlpython-0.9/rlpython/commands/tasks.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/commands/threads.py` & `rlpython-0.9/rlpython/commands/threads.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/commands/unix_environment.py` & `rlpython-0.9/rlpython/commands/unix_environment.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/commands/variables.py` & `rlpython-0.9/rlpython/commands/variables.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/completion.py` & `rlpython-0.9/rlpython/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,26 @@
     def items(self):
         return chain(
             self.locals.items(),
             self.globals.items(),
         )
 
     def __getitem__(self, name):
-        if name in self.locals:
-            return self.locals[name]
-
         if name in self.globals:
             return self.globals[name]
 
         raise KeyError
 
 
 class Completer:
     def __init__(self, repl):
         self.repl = repl
 
         self.rlcompleter = rlCompleter(
-            namespace=Namespace(
-                locals=self.repl.locals,
-                globals=self.repl.globals,
-            ),
+            namespace=self.repl.globals,
         )
 
         self._module_cache = []
 
     # python complete #########################################################
     def _complete_imports(self, text, state, line_buffer):
         raw_candidates = []
```

### Comparing `rlpython-0.8.4/rlpython/embed.py` & `rlpython-0.9/rlpython/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 
     # debug mode
     if debug:
         logging.basicConfig(level=logging.DEBUG)
         os.environ['RLPYTHON_DEBUG'] = 'True'
 
     # use namespace of caller instead of own if nothing is set
-    if 'globals' not in repl_kwargs and 'locals' not in repl_kwargs:
+    if 'globals' not in repl_kwargs:
         stack = inspect.stack()
         frame_info = stack[1]
 
         repl_kwargs['globals'] = frame_info.frame.f_globals
-        repl_kwargs['locals'] = frame_info.frame.f_locals
 
     # setup warnings
     if 'warnings' not in repl_kwargs:
         repl_kwargs['warnings'] = []
 
     if not started_from_cmd_line:
         repl_kwargs['warnings'].append('running single threaded: cancellation using CTRL-C will not work')  # NOQA
```

### Comparing `rlpython-0.8.4/rlpython/logging.py` & `rlpython-0.9/rlpython/logging.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/protocol.py` & `rlpython-0.9/rlpython/protocol.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/repl.py` & `rlpython-0.9/rlpython/repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,25 +67,24 @@
 
     def __init__(self, banner=DEFAULT_BANNER, warnings=[],
                  prompt_prefix=DEFAULT_PROMPT_PREFIX,
                  prompt=DEFAULT_PROMPT,
                  prompt_ps2=DEFAULT_PROMPT_PS2,
                  history_file=DEFAULT_HISTORY_FILE,
                  history_size=DEFAULT_HISTORY_SIZE,
-                 globals={}, locals={}, commands=[], **variables):
+                 globals={}, commands=[], **variables):
 
         self.banner = banner
         self.warnings = warnings
         self.prompt_prefix = prompt_prefix
         self.ps1 = prompt
         self.ps2 = prompt_ps2
         self.history_file = os.path.expanduser(history_file)
         self.history_size = history_size
         self.globals = globals
-        self.locals = locals
 
         self.exit_code = 0
 
         self.variables = {
             **DEFAULT_VARIABLES,
             **variables,
         }
@@ -104,15 +103,14 @@
 
         self.read_history()
 
         # setup runtimes
         self.python_runtime = PythonRuntime(
             repl=self,
             globals=globals,
-            locals=locals,
         )
 
         self.command_runtime = CommandRuntime(
             repl=self,
         )
 
         for command in commands:
@@ -188,19 +186,23 @@
                     f.write(json.dumps(item) + '\n')
 
         except Exception:
             pass
 
     # error management ########################################################
     def write_exception(self, exception, prefix=''):
-        lines = format_exception(
-            etype=type(exception),
-            value=exception,
-            tb=exception.__traceback__,
-        )
+        if sys.version_info >= (3, 10):
+            lines = format_exception(exception)
+
+        else:
+            lines = format_exception(
+                etype=type(exception),
+                value=exception,
+                tb=exception.__traceback__,
+            )
 
         text = ''.join(lines)
 
         if prefix:
             lines = text.splitlines()
 
             for index, line in enumerate(lines):
```

### Comparing `rlpython-0.8.4/rlpython/repl_client.py` & `rlpython-0.9/rlpython/repl_client.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/repl_connection.py` & `rlpython-0.9/rlpython/repl_connection.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/repl_server.py` & `rlpython-0.9/rlpython/repl_server.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/runtimes/command_runtime.py` & `rlpython-0.9/rlpython/runtimes/command_runtime.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/runtimes/python_runtime.py` & `rlpython-0.9/rlpython/runtimes/python_runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 import builtins
 import inspect
 
 from rlpython.utils.attribute_table import write_attribute_table
 
 
 class PythonRuntime:
-    def __init__(self, repl, globals={}, locals={}):
+    def __init__(self, repl, globals={}):
         self.repl = repl
         self.globals = globals
-        self.locals = locals
 
         # override print
         self.globals['print'] = self.print_function
         self.globals['_print'] = builtins.print
 
         # prepare special keywords
-        self.locals['_'] = None
-        self.locals['_rlpython'] = self.repl
-        self.locals['_exception'] = None
+        self.globals['_'] = None
+        self.globals['_rlpython'] = self.repl
+        self.globals['_exception'] = None
 
     def shutdown(self):
+
+        # restore default print
         del self.globals['print']
         del self.globals['_print']
 
-        del self.locals['_']
-        del self.locals['_rlpython']
-        del self.locals['_exception']
+        # remove special keywords
+        del self.globals['_']
+        del self.globals['_rlpython']
+        del self.globals['_exception']
 
     def print_function(self, *strings, end='\n'):
         string = ' '.join([str(i) for i in strings]) + end
 
         return self.repl.write(string)
 
     # introspection ###########################################################
@@ -161,15 +163,15 @@
 
         except Exception:
             return False
 
     # code running ############################################################
     def eval(self, source, safe=True):
         try:
-            return eval(source, self.globals, self.locals)
+            return eval(source, self.globals)
 
         except Exception:
             if not safe:
                 raise
 
             return None
 
@@ -197,37 +199,37 @@
                 code = compile(
                     source=source,
                     filename='<input>',
                     mode='exec',
                 )
 
             except SyntaxError as exception:
-                self.locals['_exception'] = exception
+                self.globals['_exception'] = exception
                 self.repl.write_exception(exception)
 
                 return 1
 
         # run code
         try:
-            return_value = run_code(code, self.globals, self.locals)
+            return_value = run_code(code, self.globals)
 
         except KeyboardInterrupt:
             exit_code = 1
 
             self.repl.write('\n')
 
         except Exception as exception:
             exit_code = 1
 
-            self.locals['_exception'] = exception
+            self.globals['_exception'] = exception
             self.repl.write_exception(exception)
 
         else:
             if run_code is eval:
-                self.locals['_'] = return_value
+                self.globals['_'] = return_value
 
                 if describe:
                     self.write_description(return_value, describe)
 
                 elif return_value is not None:
                     self.write_representation(return_value)
```

### Comparing `rlpython-0.8.4/rlpython/runtimes/shell_runtime.py` & `rlpython-0.9/rlpython/runtimes/shell_runtime.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/templating.py` & `rlpython-0.9/rlpython/templating.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/utils/editor.py` & `rlpython-0.9/rlpython/utils/editor.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/utils/strings.py` & `rlpython-0.9/rlpython/utils/strings.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/utils/table.py` & `rlpython-0.9/rlpython/utils/table.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython/utils/url.py` & `rlpython-0.9/rlpython/utils/url.py`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/rlpython.egg-info/SOURCES.txt` & `rlpython-0.9/rlpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlpython-0.8.4/setup.cfg` & `rlpython-0.9/setup.cfg`

 * *Files identical despite different names*

