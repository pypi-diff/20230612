# Comparing `tmp/kiauto-2.2.5.tar.gz` & `tmp/kiauto-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiauto-2.2.5.tar", last modified: Tue Apr 18 10:46:40 2023, max compression
+gzip compressed data, was "kiauto-2.2.6.tar", last modified: Mon Jun 12 11:51:05 2023, max compression
```

## Comparing `kiauto-2.2.5.tar` & `kiauto-2.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-18 10:45:17.000000 kiauto-2.2.5/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       67 2023-04-18 10:45:17.000000 kiauto-2.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17079 2023-04-18 10:46:40.004420 kiauto-2.2.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    13874 2023-04-18 10:45:17.000000 kiauto-2.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/kiauto/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14942 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/file_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/kiauto/interposer/
--rwxrwxr-x   0 root         (0) root         (0)    27344 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/interposer/libinterposer.so
--rw-rw-r--   0 root         (0) root         (0)    28139 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/interposer.py
--rw-rw-r--   0 root         (0) root         (0)     3755 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/log.py
--rw-rw-r--   0 root         (0) root         (0)    14340 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/misc.py
--rw-rw-r--   0 root         (0) root         (0)    19007 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/ui_automation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/kiauto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17079 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 10:46:40.004420 kiauto-2.2.5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1410 2023-04-18 10:45:17.000000 kiauto-2.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/src/
--rwxrwxr-x   0 root         (0) root         (0)    43160 2023-04-18 10:45:17.000000 kiauto-2.2.5/src/eeschema_do
--rwxrwxr-x   0 root         (0) root         (0)     6979 2023-04-18 10:45:17.000000 kiauto-2.2.5/src/kicad2step_do
--rwxrwxr-x   0 root         (0) root         (0)    75176 2023-04-18 10:45:17.000000 kiauto-2.2.5/src/pcbnew_do
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-06-12 11:48:32.000000 kiauto-2.2.6/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-06-12 11:48:32.000000 kiauto-2.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-06-12 11:51:05.902936 kiauto-2.2.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    13874 2023-06-12 11:48:32.000000 kiauto-2.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/kiauto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14967 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/kiauto/interposer/
+-rwxrwxr-x   0 root         (0) root         (0)    27344 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/interposer/libinterposer.so
+-rw-rw-r--   0 root         (0) root         (0)    28139 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/interposer.py
+-rw-rw-r--   0 root         (0) root         (0)     3755 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/log.py
+-rw-rw-r--   0 root         (0) root         (0)    14389 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    19007 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/ui_automation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/kiauto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 11:51:05.902936 kiauto-2.2.6/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1410 2023-06-12 11:48:32.000000 kiauto-2.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/src/
+-rwxrwxr-x   0 root         (0) root         (0)    43858 2023-06-12 11:48:32.000000 kiauto-2.2.6/src/eeschema_do
+-rwxrwxr-x   0 root         (0) root         (0)     7104 2023-06-12 11:48:32.000000 kiauto-2.2.6/src/kicad2step_do
+-rwxrwxr-x   0 root         (0) root         (0)    76566 2023-06-12 11:48:32.000000 kiauto-2.2.6/src/pcbnew_do
```

### Comparing `kiauto-2.2.5/LICENSE` & `kiauto-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.5/PKG-INFO` & `kiauto-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.5
+Version: 2.2.6
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.5/README.md` & `kiauto-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.5/kiauto/file_util.py` & `kiauto-2.2.6/kiauto/file_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import shutil
 import atexit
 from subprocess import DEVNULL
 # python3-psutil
 import psutil
 import json
 
-from kiauto.misc import (WRONG_ARGUMENTS, KICAD_VERSION_5_99, Config, READ_ONLY_PROBLEM)
+from kiauto.misc import WRONG_ARGUMENTS, KICAD_VERSION_5_99, Config, READ_ONLY_PROBLEM, RULES_KEY
 from kiauto import log
 logger = log.get_logger(__name__)
 time_out_scale = 1.0
 
 
 def set_time_out_scale(scale):
     global time_out_scale
@@ -221,16 +221,16 @@
     logger.debug('Creating a user hotkeys config')
     with open(cfg.conf_hotkeys, "wt") as text_file:
         text_file.write('common.Control.print\tCtrl+P\n')
         text_file.write('common.Control.plot\tCtrl+Shift+P\n')
         text_file.write('common.Control.show3DViewer\tAlt+3\n')
         text_file.write('eeschema.EditorControl.exportNetlist\tCtrl+Shift+N\n')
         text_file.write('eeschema.EditorControl.generateBOM\tCtrl+Shift+B\n')
-        text_file.write('eeschema.InspectionTool.runERC\tCtrl+Shift+I\n')
-        text_file.write('pcbnew.DRCTool.runDRC\tCtrl+Shift+I\n')
+        text_file.write('eeschema.InspectionTool.runERC\t{}\n'.format(RULES_KEY))
+        text_file.write('pcbnew.DRCTool.runDRC\t{}\n'.format(RULES_KEY))
         text_file.write('pcbnew.ZoneFiller.zoneFillAll\tB\n')
         text_file.write('pcbnew.EditorControl.generateD356File\tAlt+Shift+E\n')
         text_file.write('3DViewer.Control.rotateXclockwise\tAlt+X\n')
         text_file.write('3DViewer.Control.rotateXcounterclockwise\tAlt+Shift+X\n')
         text_file.write('3DViewer.Control.rotateYclockwise\tAlt+Y\n')
         text_file.write('3DViewer.Control.rotateYcounterclockwise\tAlt+Shift+Y\n')
         text_file.write('3DViewer.Control.rotateZclockwise\tAlt+Z\n')
```

### Comparing `kiauto-2.2.5/kiauto/interposer/libinterposer.so` & `kiauto-2.2.6/kiauto/interposer/libinterposer.so`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.5/kiauto/interposer.py` & `kiauto-2.2.6/kiauto/interposer.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.5/kiauto/log.py` & `kiauto-2.2.6/kiauto/log.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.5/kiauto/misc.py` & `kiauto-2.2.6/kiauto/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 
 KICAD_VERSION_5_99 = 5099000
 KICAD_VERSION_6_99 = 6099000
 KICAD_VERSION_7_99 = 7099000
 KICAD_VERSION_7_0_3 = 7000003
 KICAD_SHARE = '/usr/share/kicad/'
 KICAD_NIGHTLY_SHARE = '/usr/share/kicad-nightly/'
+RULES_KEY = 'Ctrl+Shift+A'
+# RULES_KEY = 'Alt+I'
 
 
 @contextmanager
 def hide_stderr():
     """ Low level stderr supression, used to hide KiCad bugs. """
     newstderr = os.dup(2)
     devnull = os.open('/dev/null', os.O_WRONLY)
@@ -340,8 +342,8 @@
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2018-2023, INTI/Productize SPRL'
 __credits__ = ['Salvador E. Tropea', 'Seppe Stas', 'Jesse Vincent', 'Scott Bezek']
 __license__ = 'Apache 2.0'
 __email__ = 'stropea@inti.gob.ar'
 __status__ = 'stable'
 __url__ = 'https://github.com/INTI-CMNB/KiAuto/'
-__version__ = '2.2.5'
+__version__ = '2.2.6'
```

### Comparing `kiauto-2.2.5/kiauto/ui_automation.py` & `kiauto-2.2.6/kiauto/ui_automation.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.5/kiauto.egg-info/PKG-INFO` & `kiauto-2.2.6/kiauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.5
+Version: 2.2.6
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.5/setup.py` & `kiauto-2.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.5/src/eeschema_do` & `kiauto-2.2.6/src/eeschema_do`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 log.set_domain(os.path.splitext(os.path.basename(__file__))[0])
 logger = None
 
 from kiauto.file_util import (load_filters, wait_for_file_created_by_process, apply_filters, list_errors, list_warnings,
                               check_kicad_config_dir, restore_config, backup_config, check_lib_table, create_user_hotkeys,
                               check_input_file, memorize_project, restore_project, get_log_files, create_kicad_config,
                               set_time_out_scale as set_time_out_scale_f, add_filter)
-from kiauto.misc import (REC_W, REC_H, __version__, NO_SCHEMATIC, EESCHEMA_CFG_PRESENT, KICAD_CFG_PRESENT,
+from kiauto.misc import (REC_W, REC_H, __version__, NO_SCHEMATIC, EESCHEMA_CFG_PRESENT, KICAD_CFG_PRESENT, RULES_KEY,
                          WAIT_START, WRONG_SCH_NAME, EESCHEMA_ERROR, Config, KICAD_VERSION_5_99, WONT_OVERWRITE,
                          USER_HOTKEYS_PRESENT, __copyright__, __license__, TIME_OUT_MULT, get_en_locale, KICAD_CLI_ERROR,
                          KICAD_VERSION_7_0_3)
 from kiauto.interposer import (check_interposer, dump_interposer_dialog, start_queue, wait_start_by_msg,
-                               set_kicad_process, open_dialog_i,
+                               set_kicad_process, open_dialog_i, wait_kicad_ready_i,
                                paste_output_file_i, exit_kicad_i, paste_text_i, wait_queue,
                                paste_bogus_filename, setup_interposer_filename, send_keys, wait_create_i)
 from kiauto.ui_automation import (PopenContext, xdotool, wait_for_window, wait_not_focused, recorded_xvfb,
                                   wait_point, text_replace, set_time_out_scale, wait_xserver, wait_window_get_ref,
                                   wait_window_change, open_dialog_with_retry, ShowInfoAction)
 
 TITLE_CONFIRMATION = '^Confirmation$'
@@ -318,19 +318,23 @@
     for i, line in enumerate(lines):
         m = err_regex.search(line)
         if m:
             msg = '({}) {}'.format(m.group(1), m.group(2))
             if cfg.kicad_version >= KICAD_VERSION_5_99 and i < len(lines):
                 # KiCad 6 moved the severity to the next line
                 line = lines[i+1]
-                # KiCad 7.0.2 bug: a message with two extra \n
-                # Error reading simulation model from symbol '#PWR03':\nFailed to read simulation model from fields.\n
-                if '; Severity' not in line and i+3 < len(lines) and lines[i+2] == '':
+                if '; Severity' not in line and i+3 < len(lines):
+                    if lines[i+2] == '':
+                        # KiCad 7.0.2 bug: a message with two extra \n
+                        # Error reading simulation model from symbol '#PWR03':\nFailed to read simulation model from fields.\n
+                        line = lines[i+3]
+                    else:
+                        # KiCad 7.0.5 bug: a message with one extra \n
+                        line = lines[i+2]
                     msg += ' '+line
-                    line = lines[i+3]
             # Discard messages explicitly excluded using the GUI
             excluded = '(excluded)' in line
             if r'Severity: error' in line:
                 is_err = True
                 if excluded:
                     errors_excl += 1
                 else:
@@ -412,15 +416,15 @@
     wait_create_i(cfg, 'ERC')
     # Close the ERC dialog
     send_keys(cfg, 'Exit ERC', 'alt+l', closes=dialog)
 
 
 def eeschema_run_erc_schematic_6_0_n(cfg):
     # Open the ERC dialog
-    keys = ['key', 'Escape', 'ctrl+shift+i']
+    keys = ['key', 'Escape', RULES_KEY.lower()]
     erc_name = 'Electrical Rules Checker dialog'
     erc_title = 'Electrical Rules Checker'
     erc_msg = 'Open Tools->Electrical Rules Checker'
     id = open_dialog_with_retry(erc_msg, keys, erc_name, erc_title, cfg)
     wait_point(cfg)
     # Run the ERC
     logger.info('Run ERC')
@@ -485,29 +489,38 @@
 
 def eeschema_run_erc_schematic_6_0_i(cfg):
     # KiCad 7.99 particularities:
     # 1. Forces ".rpt" in the name, no matter what name was selected in the dialog and no matter if it already has an extension
     # 2. The ERC dialog isn't destroyed, most probably hidden
     # Open the ERC dialog
     title = 'Electrical Rules Checker'
-    dialog, _ = open_dialog_i(cfg, title, 'ctrl+shift+i', no_main=True)
+    dialog, _ = open_dialog_i(cfg, title, RULES_KEY.lower(), no_main=True)
     # Run the ERC
     send_keys(cfg, 'Run ERC', 'Return')
     # Wait for completion. The Close button is refreshed at the end
-    wait_queue(cfg, 'GTK:Button Label:C_lose')
+    res = wait_queue(cfg, ['GTK:Button Label:C_lose', 'GTK:Window Destroy:'+title])
+    if res.startswith('GTK:Window Destroy:'):
+        # Ugly hack for 7.99 should be removed
+        logger.error(title+' destroyed (before completion)')
+        dialog, _ = open_dialog_i(cfg, title, RULES_KEY.lower(), no_main=True)
+        time.sleep(3)
+        wait_kicad_ready_i(cfg)
+        send_keys(cfg, 'Run ERC', 'Return')
+        wait_queue(cfg, 'GTK:Button Label:C_lose')
     # Save the report
     reopen = False
     try:
         # Catch the ERC unintentional close
         file_dlg, _ = open_dialog_i(cfg, 'Save Report to File', 'alt+s', raise_if=['GTK:Window Destroy:'+title])
     except InterruptedError:
         reopen = True
     if reopen:
+        logger.error(title+' destroyed (after completion)')
         # KiCad 7.0.2 bug, in some cases the dialog is closed, we just need to open it again
-        dialog, _ = open_dialog_i(cfg, title, 'ctrl+shift+i', no_main=True)
+        dialog, _ = open_dialog_i(cfg, title, RULES_KEY.lower(), no_main=True)
         file_dlg, _ = open_dialog_i(cfg, 'Save Report to File', 'alt+s')
     # Paste the output file
     paste_bogus_filename(cfg)
     send_keys(cfg, 'Create the report', 'Return', closes=file_dlg, delay_io=True)
     # Wait until created
     wait_create_i(cfg, 'ERC', forced_ext='rpt')
     # Close the ERC dialog
```

### Comparing `kiauto-2.2.5/src/kicad2step_do` & `kiauto-2.2.6/src/kicad2step_do`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     parser.add_argument('pcb_filename', help='KiCad PCB file')
 
     parser.add_argument('--output-filename', '-o', nargs=1, help='output filename')
     parser.add_argument('--force', '-f', help='overwrite output file', action='store_true')
     parser.add_argument('--drill-origin', help='Use Drill Origin for output origin', action='store_true')
     parser.add_argument('--grid-origin', help='Use Grid Origin for output origin', action='store_true')
     parser.add_argument('--user-origin', nargs=1, help='User-specified output origin ex. 1x1in, 1x1inch, 25.4x25.4mm (default mm)')
-    parser.add_argument('--no-virtual', help="exclude 3D models for components with 'virtual' attribute", action='store_true')
+    parser.add_argument('--no-virtual', help="exclude 3D models for components with 'virtual'/'unspecified' attribute", action='store_true')
     parser.add_argument('--subst-models', help='Substitute STEP or IGS models with the same name in place of VRML models (KiCad 6)', action='store_true')
     parser.add_argument('--min-distance', nargs=1, help='Minimum distance between points to treat them as separate ones (default 0.01 mm)')
     # Our options
     parser.add_argument('--info', '-n', help='Show information about the installation', action=ShowInfoAction, nargs=0)
     parser.add_argument('--record', '-r', help='Record the UI automation', action='store_true')
     parser.add_argument('--rec_width', help='Record width ['+str(REC_W)+']', type=int, default=REC_W)
     parser.add_argument('--rec_height', help='Record height ['+str(REC_H)+']', type=int, default=REC_H)
@@ -133,15 +133,19 @@
     if args.drill_origin:
         cmd.append('--drill-origin')
     if args.grid_origin:
         cmd.append('--grid-origin')
     if args.user_origin:
         cmd.append('--user-origin='+args.user_origin[0])
     if args.no_virtual:
-        cmd.append('--no-virtual')
+        logger.error(cfg.ki8)
+        if cfg.ki8:
+            cmd.append('--no-unspecified')
+        else:
+            cmd.append('--no-virtual')
     if args.min_distance:
         cmd.append('--min-distance='+args.min_distance[0])
     if args.subst_models and cfg.kicad_version_major > 5:
         cmd.append('--subst-models')
     cmd.append(args.pcb_filename)
     logger.debug("Command: "+str(cmd))
```

### Comparing `kiauto-2.2.5/src/pcbnew_do` & `kiauto-2.2.6/src/pcbnew_do`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 logger = None
 
 from kiauto.file_util import (load_filters, wait_for_file_created_by_process, apply_filters, list_errors, list_warnings,
                               check_kicad_config_dir, restore_config, backup_config, check_lib_table, create_user_hotkeys,
                               check_input_file, memorize_project, restore_project, get_log_files, create_kicad_config,
                               set_time_out_scale as set_time_out_scale_f)
 from kiauto.misc import (REC_W, REC_H, __version__, NO_PCB, PCBNEW_CFG_PRESENT, WAIT_START, WRONG_LAYER_NAME,
-                         WRONG_PCB_NAME, PCBNEW_ERROR, WRONG_ARGUMENTS, Config, USER_HOTKEYS_PRESENT,
+                         WRONG_PCB_NAME, PCBNEW_ERROR, WRONG_ARGUMENTS, Config, USER_HOTKEYS_PRESENT, RULES_KEY,
                          CORRUPTED_PCB, __copyright__, __license__, TIME_OUT_MULT, get_en_locale, KICAD_CFG_PRESENT,
                          MISSING_TOOL, KICAD_VERSION_6_99)
 from kiauto.interposer import (check_interposer, dump_interposer_dialog, start_queue, setup_interposer_filename,
                                create_interposer_print_options_file, wait_queue, wait_start_by_msg, wait_and_show_progress,
                                set_kicad_process, open_dialog_i, wait_kicad_ready_i, paste_bogus_filename, paste_text_i,
                                paste_output_file_i, exit_kicad_i, send_keys, wait_create_i, save_interposer_print_data)
 from kiauto.ui_automation import (PopenContext, xdotool, wait_not_focused, wait_for_window, recorded_xvfb,
@@ -459,15 +459,15 @@
     xdotool(['key', 'shift+Tab', 'Return'])
     wait_pcbnew()
 
 
 def run_drc_6_0(cfg):
     logger.info('Open Inspect->DRC')
     wait_point(cfg)
-    xdotool(['key', 'ctrl+shift+i'])
+    xdotool(['key', RULES_KEY.lower()])
     # Wait dialog
     wait_for_window('DRC modal window', cfg.drc_dialog_name)
     # Run the DRC
     logger.info('Run DRC')
     wait_point(cfg)
     xdotool(['key', 'Return'])
     #
@@ -545,15 +545,15 @@
     file_dialog, _ = open_dialog_i(cfg, 'Disk File Report Completed', 'Return', no_show=True, no_main=True)
     send_keys(cfg, 'Close dialog', 'Return', closes=file_dialog)
     # Now close the DRC control
     send_keys(cfg, 'Closing the DRC dialog', 'alt+l', closes=control_dlg)
 
 
 def run_drc_6_0_i(cfg):
-    control_dlg, _ = open_dialog_i(cfg, cfg.drc_dialog_name, 'ctrl+shift+i', no_main=True)
+    control_dlg, _ = open_dialog_i(cfg, cfg.drc_dialog_name, RULES_KEY.lower(), no_main=True)
     # Run the DRC
     send_keys(cfg, 'Run DRC', 'Return')
     # Wait for the end of the DRC (at the end KiCad restores the Close button)
     wait_queue(cfg, 'GTK:Button Label:C_lose')
     wait_kicad_ready_i(cfg)
     # Save the DRC
     # We added a short-cut for Save...
@@ -812,14 +812,17 @@
         for _ in range(steps):
             logger.info('Step ({})'.format(k))
             xdotool(['key', k], id)
             logger.debug('Step '+key)
             if cfg.use_interposer:
                 if cfg.wait_after_move:
                     wait_kicad_ready_i(cfg, swaps=1)
+                    # Arbitrary, this is a problem with KiCad 5, so I won't spend too much time looking for a better solution
+                    sleep(1)
+                    wait_kicad_ready_i(cfg)
             else:
                 wait_3d_ready_n(cfg)
 
 
 def open_save_image_n(cfg, id):
     keys = ['key', 'alt+f', 'Return']
     for retry in range(10):
@@ -1183,15 +1186,20 @@
                                   "show_axis": False,
                                   "opengl_AA_mode": 0,
                                   "show_silkscreen": not cfg.hide_silkscreen,
                                   "show_soldermask": not cfg.hide_soldermask,
                                   "show_solderpaste": not cfg.hide_solderpaste,
                                   "show_zones": not cfg.hide_zones,
                                   "clip_silk_on_via_annulus": not cfg.dont_clip_silk_on_via_annulus,
-                                  "subtract_mask_from_silk": not cfg.dont_substrack_mask_from_silk}
+                                  "subtract_mask_from_silk": not cfg.dont_substrack_mask_from_silk,
+                                  "realistic": not cfg.use_layer_colors,
+                                  "show_board_body": not cfg.hide_board_body,
+                                  "show_comments": cfg.show_comments,
+                                  "show_eco": cfg.show_eco,
+                                  "show_adhesive": cfg.show_adhesive}
                 json_text = json.dumps(conf)
                 with open(cfg.conf_3dview, "wt") as viewer_file:
                     viewer_file.write(json_text)
                 logger.debug("3D Viewer:")
                 logger.debug(json_text)
         else:
             text_file.write('canvas_type=2\n')
@@ -1366,14 +1374,15 @@
     v3d_parser.add_argument('--copper_color', '-c', nargs=1, help='Copper color', default=['#B29C00'])
     v3d_parser.add_argument('--detect_rt', '-d', help='Try to detect when the ray tracing render finshes,'
                             ' wait_rt value is the time-out (experimental)', action='store_true')
     v3d_parser.add_argument('--dont_clip_silk_on_via_annulus', help="Don't clip silkscreen at via annuli (KiCad 6)",
                             action='store_true')
     v3d_parser.add_argument('--dont_substrack_mask_from_silk', help="Don't clip silkscreen at solder mask edges (KiCad 6)",
                             action='store_true')
+    v3d_parser.add_argument('--hide_board_body', help='Hide the body of the PCB board (KiCad 6)', action='store_true')
     v3d_parser.add_argument('--hide_silkscreen', help='Hide the silkscreen layers (KiCad 6)', action='store_true')
     v3d_parser.add_argument('--hide_soldermask', help='Hide the solder mask layers (KiCad 6)', action='store_true')
     v3d_parser.add_argument('--hide_solderpaste', help='Hide the solder paste layers (KiCad 6)', action='store_true')
     v3d_parser.add_argument('--hide_zones', help='Hide filled areas in zones (KiCad 6)', action='store_true')
     v3d_parser.add_argument('--move_x', '-x', nargs=1, help='Steps to move in the X axis (positive is to the right)',
                             default=[0], type=int)
     v3d_parser.add_argument('--move_y', '-y', nargs=1, help='Steps to move in the Y axis (positive is up)', default=[0],
@@ -1386,19 +1395,24 @@
                             help='Steps to rotate around the Y axis (positive is clockwise) KiCad 6', default=[0], type=int)
     v3d_parser.add_argument('--no_smd', '-S', help='Do not include surface mount components', action='store_true')
     v3d_parser.add_argument('--no_tht', '-T', help='Do not include through-hole components', action='store_true')
     v3d_parser.add_argument('--virtual', '-V', help='Include virtual components', action='store_true')
     v3d_parser.add_argument('--orthographic', '-O', help='Enable the orthographic projection', action='store_true')
     v3d_parser.add_argument('--output_name', '-o', nargs=1, help='Name of the output file (PNG)', default=['capture.png'])
     v3d_parser.add_argument('--ray_tracing', '-r', help='Enable the realistic render', action='store_true')
+    v3d_parser.add_argument('--show_adhesive', help='Show the adhesive layer', action='store_true')
+    v3d_parser.add_argument('--show_comments', help='Show the user comments layer', action='store_true')
+    v3d_parser.add_argument('--show_eco', help='Show the user eco layers', action='store_true')
     v3d_parser.add_argument('--silk_color', nargs=1,
                             help='Silk color (KiCad 6 supports color1,color2 for top/bottom)', default=['#E5E5E5'])
     v3d_parser.add_argument('--sm_color', nargs=1, help='Solder mask color (KiCad 6 supports color1,color2 for top/bottom)',
                             default=['#143324D4'])
     v3d_parser.add_argument('--sp_color', nargs=1, help='Solder paste color', default=['#808080'])
+    v3d_parser.add_argument('--use_layer_colors', help='Use the colors of the layers, not realistic colors (KiCad 6)',
+                            action='store_true')
     v3d_parser.add_argument('--use_rt_wait', '-u', help='Use the ray tracing end detection even on normal renders',
                             action='store_true')
     v3d_parser.add_argument('--view', '-v', nargs=1, help='Axis view, uppercase is reversed (i.e. Z is bottom)',
                             default=['z'], choices=['x', 'y', 'z', 'X', 'Y', 'Z'],)
     v3d_parser.add_argument('--wait_after_move', '-W', help='Wait after moving (KiCad 6 and interposer option)',
                             action='store_true')
     v3d_parser.add_argument('--wait_rt', '-w', nargs=1, help='Seconds to wait for the ray tracing render [5]', default=[5],
@@ -1559,14 +1573,19 @@
         cfg.wait_after_move = args.wait_after_move
         cfg.hide_silkscreen = args.hide_silkscreen
         cfg.hide_soldermask = args.hide_soldermask
         cfg.hide_solderpaste = args.hide_solderpaste
         cfg.hide_zones = args.hide_zones
         cfg.dont_substrack_mask_from_silk = args.dont_substrack_mask_from_silk
         cfg.dont_clip_silk_on_via_annulus = args.dont_clip_silk_on_via_annulus
+        cfg.use_layer_colors = args.use_layer_colors
+        cfg.hide_board_body = args.hide_board_body
+        cfg.show_comments = args.show_comments
+        cfg.show_eco = args.show_eco
+        cfg.show_adhesive = args.show_adhesive
     else:
         cfg.no_tht = False
         cfg.no_smd = False
         cfg.no_virtual = True
         cfg.ray_tracing = False
         cfg.bg_color_1 = cfg.bg_color_2 = cfg.board_color = None
         cfg.copper_color = cfg.silk_color = cfg.sm_color = cfg.sp_color = None
```

