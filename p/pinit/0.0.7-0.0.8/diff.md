# Comparing `tmp/pinit-0.0.7.tar.gz` & `tmp/pinit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinit-0.0.7.tar", max compression
+gzip compressed data, was "pinit-0.0.8.tar", max compression
```

## Comparing `pinit-0.0.7.tar` & `pinit-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      425 2023-06-03 10:35:28.564339 pinit-0.0.7/README.md
--rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.7/pinit/.pinit/install.py
--rw-r--r--   0        0        0     7093 2023-06-03 13:26:18.647897 pinit-0.0.7/pinit/.pinit/main.py
--rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.7/pinit/.pinit/pinit.svg
--rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.7/pinit/.pinit/requirements.txt
--rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.7/pinit/.pinit/shortcut.py
--rw-r--r--   0        0        0    79260 2023-06-03 10:08:22.908252 pinit-0.0.7/pinit/.pinit/ui/assets/index-88a0609b.css
--rw-r--r--   0        0        0   201367 2023-06-03 10:08:22.909252 pinit-0.0.7/pinit/.pinit/ui/assets/index-a407b3b0.js
--rw-r--r--   0        0        0   128352 2023-06-03 10:08:22.907252 pinit-0.0.7/pinit/.pinit/ui/assets/w1-8265f647.woff2
--rw-r--r--   0        0        0   155276 2023-06-03 10:08:22.909252 pinit-0.0.7/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
--rwxr-xr-x   0        0        0     2210 2023-06-03 10:08:22.437250 pinit-0.0.7/pinit/.pinit/ui/icon.svg
--rw-r--r--   0        0        0      899 2023-06-03 10:08:22.909252 pinit-0.0.7/pinit/.pinit/ui/index.html
--rw-r--r--   0        0        0      255 2023-06-03 10:23:04.373699 pinit-0.0.7/pinit/.pinit/uninstall.py
--rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.7/pinit/.pinit/upgrade.py
--rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.7/pinit/__init__.py
--rw-r--r--   0        0        0     2338 2023-06-03 13:16:45.028043 pinit-0.0.7/pinit/main.py
--rw-r--r--   0        0        0      457 2023-06-03 13:27:03.905412 pinit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 pinit-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      425 2023-06-03 10:35:28.564339 pinit-0.0.8/README.md
+-rw-r--r--   0        0        0      323 2023-01-23 13:34:30.831156 pinit-0.0.8/pinit/.pinit/install.py
+-rw-r--r--   0        0        0     7174 2023-06-12 14:50:36.568359 pinit-0.0.8/pinit/.pinit/main.py
+-rwxr-xr-x   0        0        0     2210 2023-01-06 17:49:58.404041 pinit-0.0.8/pinit/.pinit/pinit.svg
+-rw-r--r--   0        0        0       52 2023-03-27 12:23:42.562490 pinit-0.0.8/pinit/.pinit/requirements.txt
+-rw-r--r--   0        0        0      897 2023-01-06 18:07:43.742132 pinit-0.0.8/pinit/.pinit/shortcut.py
+-rw-r--r--   0        0        0    79440 2023-06-12 15:02:46.186498 pinit-0.0.8/pinit/.pinit/ui/assets/index-800b0b32.css
+-rw-r--r--   0        0        0    79260 2023-06-03 10:08:22.908252 pinit-0.0.8/pinit/.pinit/ui/assets/index-88a0609b.css
+-rw-r--r--   0        0        0   201367 2023-06-12 15:02:46.186498 pinit-0.0.8/pinit/.pinit/ui/assets/index-95facd96.js
+-rw-r--r--   0        0        0   201367 2023-06-03 10:08:22.909252 pinit-0.0.8/pinit/.pinit/ui/assets/index-a407b3b0.js
+-rw-r--r--   0        0        0   128352 2023-06-12 15:02:46.186498 pinit-0.0.8/pinit/.pinit/ui/assets/w1-8265f647.woff2
+-rw-r--r--   0        0        0   155276 2023-06-12 15:02:46.183498 pinit-0.0.8/pinit/.pinit/ui/assets/w2-35dca8a7.woff2
+-rwxr-xr-x   0        0        0     2210 2023-06-12 15:02:45.564473 pinit-0.0.8/pinit/.pinit/ui/icon.svg
+-rw-r--r--   0        0        0      899 2023-06-12 15:02:46.187498 pinit-0.0.8/pinit/.pinit/ui/index.html
+-rw-r--r--   0        0        0      255 2023-06-03 10:23:04.373699 pinit-0.0.8/pinit/.pinit/uninstall.py
+-rw-r--r--   0        0        0       16 2023-01-06 18:08:51.649138 pinit-0.0.8/pinit/.pinit/upgrade.py
+-rw-r--r--   0        0        0        0 2023-01-01 08:59:18.230362 pinit-0.0.8/pinit/__init__.py
+-rw-r--r--   0        0        0     2194 2023-06-12 15:01:27.732246 pinit-0.0.8/pinit/main.py
+-rw-r--r--   0        0        0      457 2023-06-12 15:06:04.997365 pinit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 pinit-0.0.8/PKG-INFO
```

### Comparing `pinit-0.0.7/pinit/.pinit/main.py` & `pinit-0.0.8/pinit/.pinit/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,16 +225,20 @@
     return ";;;".join(desktopIcons)
 
 
 ########################################################################################################
 
 if __name__ == "__main__":
     try:
-        os.makedirs(f'{home}/.pinit/ui/menu')
+        os.makedirs(f"{home}/.pinit/ui/menu")
     except:
         pass
     try:
-        os.makedirs(f'{home}/.pinit/ui/desktop')
+        os.makedirs(f"{home}/.pinit/ui/desktop")
+    except:
+        pass
+    try:
+        os.makedirs(f"{home}/.pinit/ui/icons")
     except:
         pass
 
     eel.start("index.html", size=(300, 690), position=(800, 200))
```

### Comparing `pinit-0.0.7/pinit/.pinit/pinit.svg` & `pinit-0.0.8/pinit/.pinit/pinit.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.7/pinit/.pinit/shortcut.py` & `pinit-0.0.8/pinit/.pinit/shortcut.py`

 * *Files identical despite different names*

### Comparing `pinit-0.0.7/pinit/.pinit/ui/assets/index-88a0609b.css` & `pinit-0.0.8/pinit/.pinit/ui/assets/index-88a0609b.css`

 * *Files identical despite different names*

### Comparing `pinit-0.0.7/pinit/.pinit/ui/assets/index-a407b3b0.js` & `pinit-0.0.8/pinit/.pinit/ui/assets/index-a407b3b0.js`

 * *Files identical despite different names*

### Comparing `pinit-0.0.7/pinit/.pinit/ui/assets/w1-8265f647.woff2` & `pinit-0.0.8/pinit/.pinit/ui/assets/w1-8265f647.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.7/pinit/.pinit/ui/assets/w2-35dca8a7.woff2` & `pinit-0.0.8/pinit/.pinit/ui/assets/w2-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `pinit-0.0.7/pinit/.pinit/ui/icon.svg` & `pinit-0.0.8/pinit/.pinit/ui/icon.svg`

 * *Files identical despite different names*

### Comparing `pinit-0.0.7/pinit/.pinit/ui/index.html` & `pinit-0.0.8/pinit/.pinit/ui/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
     <script type="text/javascript" src="/eel.js"></script>
 
 
 
 
 
-    <script type="module" crossorigin src="/assets/index-a407b3b0.js"></script>
-    <link rel="stylesheet" href="/assets/index-88a0609b.css">
+    <script type="module" crossorigin src="/assets/index-95facd96.js"></script>
+    <link rel="stylesheet" href="/assets/index-800b0b32.css">
   </head>
   <body>
     <div id="app"></div>
     
   </body>
 </html>
```

### Comparing `pinit-0.0.7/pinit/main.py` & `pinit-0.0.8/pinit/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,15 @@
             shutil.rmtree(dist)
         finally:
             shutil.copytree(src, dist)
             os.chdir(dist)
             subprocess.run(['python','-m','venv','venv'])
             subprocess.run(['venv/bin/python','-m','pip','install','-r','requirements.txt'])
             subprocess.run(['venv/bin/python', 'install.py'])
-        try:
-            os.makedirs(f'{dist}'/ui/desktop)
-            os.makedirs(f'{dist}'/ui/menu)
-        except:
-            pass
+
 
 
 
 def upgrade():
     if '--force' in sys.argv or '-f' in sys.argv:
         subprocess.run(['pip', 'install', '--upgrade', 'pinit'])
         install()
@@ -61,17 +57,15 @@
 
 
 def open():
     try:
         os.chdir(dist)
         subprocess.run(['venv/bin/python', 'main.py'])
     except:
-        install()
-        os.chdir(dist)
-        subprocess.run(['venv/bin/python', 'main.py'])
+        print("pinit is not installed .\nrun 'pinit install' command to install it.")
 
 
 def help():
     print('commands .........................................')
     print('install')
     print('uninstall')
     print('upgrade')
```

### Comparing `pinit-0.0.7/PKG-INFO` & `pinit-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinit
-Version: 0.0.7
+Version: 0.0.8
 Summary: an application for creating shortcut for apps and scripts in linux
 Home-page: https://github.com/rraammiinn/pinit.git
 License: MIT
 Author: ramin
 Author-email: ramin.kishani.farahani@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

