# Comparing `tmp/discord-rich-presence-1.0.2.tar.gz` & `tmp/discord-rich-presence-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-rich-presence-1.0.2.tar", last modified: Sat May 20 22:07:32 2023, max compression
+gzip compressed data, was "discord-rich-presence-1.0.3.tar", last modified: Mon Jun 12 18:47:02 2023, max compression
```

## Comparing `discord-rich-presence-1.0.2.tar` & `discord-rich-presence-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-05-20 22:07:32.175963 discord-rich-presence-1.0.2/
--rw-r--r--   0 maxwe      (501) staff       (20)     1064 2022-06-14 05:49:12.000000 discord-rich-presence-1.0.2/LICENSE
--rw-r--r--   0 maxwe      (501) staff       (20)     2797 2023-05-20 22:07:32.175155 discord-rich-presence-1.0.2/PKG-INFO
--rw-r--r--   0 maxwe      (501) staff       (20)     2111 2022-06-14 05:47:37.000000 discord-rich-presence-1.0.2/README.md
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-05-20 22:07:32.172821 discord-rich-presence-1.0.2/discord_rich_presence.egg-info/
--rw-r--r--   0 maxwe      (501) staff       (20)     2797 2023-05-20 22:07:32.000000 discord-rich-presence-1.0.2/discord_rich_presence.egg-info/PKG-INFO
--rw-r--r--   0 maxwe      (501) staff       (20)      250 2023-05-20 22:07:32.000000 discord-rich-presence-1.0.2/discord_rich_presence.egg-info/SOURCES.txt
--rw-r--r--   0 maxwe      (501) staff       (20)        1 2023-05-20 22:07:32.000000 discord-rich-presence-1.0.2/discord_rich_presence.egg-info/dependency_links.txt
--rw-r--r--   0 maxwe      (501) staff       (20)       10 2023-05-20 22:07:32.000000 discord-rich-presence-1.0.2/discord_rich_presence.egg-info/top_level.txt
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-05-20 22:07:32.174225 discord-rich-presence-1.0.2/discordrp/
--rw-r--r--   0 maxwe      (501) staff       (20)      260 2023-05-20 22:05:17.000000 discord-rich-presence-1.0.2/discordrp/__init__.py
--rw-r--r--   0 maxwe      (501) staff       (20)     4885 2023-05-20 22:05:17.000000 discord-rich-presence-1.0.2/discordrp/presence.py
--rw-r--r--   0 maxwe      (501) staff       (20)       38 2023-05-20 22:07:32.176160 discord-rich-presence-1.0.2/setup.cfg
--rw-r--r--   0 maxwe      (501) staff       (20)      932 2022-06-14 06:13:05.000000 discord-rich-presence-1.0.2/setup.py
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-06-12 18:47:02.323424 discord-rich-presence-1.0.3/
+-rw-r--r--   0 maxwe      (501) staff       (20)     1064 2022-06-14 05:49:12.000000 discord-rich-presence-1.0.3/LICENSE
+-rw-r--r--   0 maxwe      (501) staff       (20)     2806 2023-06-12 18:47:02.321466 discord-rich-presence-1.0.3/PKG-INFO
+-rw-r--r--   0 maxwe      (501) staff       (20)     2120 2023-06-05 02:59:38.000000 discord-rich-presence-1.0.3/README.md
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-06-12 18:47:02.316584 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/
+-rw-r--r--   0 maxwe      (501) staff       (20)     2806 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/PKG-INFO
+-rw-r--r--   0 maxwe      (501) staff       (20)      269 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/SOURCES.txt
+-rw-r--r--   0 maxwe      (501) staff       (20)        1 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/dependency_links.txt
+-rw-r--r--   0 maxwe      (501) staff       (20)       10 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/top_level.txt
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-06-12 18:47:02.320583 discord-rich-presence-1.0.3/discordrp/
+-rw-r--r--   0 maxwe      (501) staff       (20)      315 2023-06-12 18:44:46.000000 discord-rich-presence-1.0.3/discordrp/__init__.py
+-rw-r--r--   0 maxwe      (501) staff       (20)     5804 2023-06-05 02:58:18.000000 discord-rich-presence-1.0.3/discordrp/presence.py
+-rw-r--r--   0 maxwe      (501) staff       (20)        0 2023-06-05 02:46:28.000000 discord-rich-presence-1.0.3/discordrp/py.typed
+-rw-r--r--   0 maxwe      (501) staff       (20)       38 2023-06-12 18:47:02.323570 discord-rich-presence-1.0.3/setup.cfg
+-rw-r--r--   0 maxwe      (501) staff       (20)      978 2023-06-05 02:58:18.000000 discord-rich-presence-1.0.3/setup.py
```

### Comparing `discord-rich-presence-1.0.2/LICENSE` & `discord-rich-presence-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-rich-presence-1.0.2/PKG-INFO` & `discord-rich-presence-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-rich-presence
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight and safe module for creating custom rich presences on Discord.
 Home-page: https://github.com/TenType/discord-rich-presence
 Author: TenType
 License: MIT
 Keywords: discord,presence,rich presence,activity,rpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,24 +41,24 @@
 
 ### Writing the Code
 6. Create a file ending in `.py`, and paste in the following example from [examples/simple.py](examples/simple.py):
 ```py
 from discordrp import Presence
 import time
 
-client_id = '000000000000000000' # Replace this with your own client id
+client_id = "000000000000000000"  # Replace this with your own client id
 
 with Presence(client_id) as presence:
-    presence.set({
-        'state': 'In Game',
-        'details': "Summoner's Rift",
-        'timestamps': {
-            'start': int(time.time())
-        },
-    })
+    presence.set(
+        {
+            "state": "In Game",
+            "details": "Summoner's Rift",
+            "timestamps": {"start": int(time.time())},
+        }
+    )
 
     while True:
         time.sleep(15)
 ```
 Make sure you replace the `client_id` variable with your app's id that you copied earlier.
 
 7. Run the program! You should now see that you have a rich presence on your profile that will be on until you stop the program! Feel free to change the code however you want by adding images, buttons, and more. Check out [examples/complex.py](examples/complex.py) for another example.
```

### Comparing `discord-rich-presence-1.0.2/README.md` & `discord-rich-presence-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 
 ### Writing the Code
 6. Create a file ending in `.py`, and paste in the following example from [examples/simple.py](examples/simple.py):
 ```py
 from discordrp import Presence
 import time
 
-client_id = '000000000000000000' # Replace this with your own client id
+client_id = "000000000000000000"  # Replace this with your own client id
 
 with Presence(client_id) as presence:
-    presence.set({
-        'state': 'In Game',
-        'details': "Summoner's Rift",
-        'timestamps': {
-            'start': int(time.time())
-        },
-    })
+    presence.set(
+        {
+            "state": "In Game",
+            "details": "Summoner's Rift",
+            "timestamps": {"start": int(time.time())},
+        }
+    )
 
     while True:
         time.sleep(15)
 ```
 Make sure you replace the `client_id` variable with your app's id that you copied earlier.
 
 7. Run the program! You should now see that you have a rich presence on your profile that will be on until you stop the program! Feel free to change the code however you want by adding images, buttons, and more. Check out [examples/complex.py](examples/complex.py) for another example.
```

### Comparing `discord-rich-presence-1.0.2/discord_rich_presence.egg-info/PKG-INFO` & `discord-rich-presence-1.0.3/discord_rich_presence.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-rich-presence
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight and safe module for creating custom rich presences on Discord.
 Home-page: https://github.com/TenType/discord-rich-presence
 Author: TenType
 License: MIT
 Keywords: discord,presence,rich presence,activity,rpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,24 +41,24 @@
 
 ### Writing the Code
 6. Create a file ending in `.py`, and paste in the following example from [examples/simple.py](examples/simple.py):
 ```py
 from discordrp import Presence
 import time
 
-client_id = '000000000000000000' # Replace this with your own client id
+client_id = "000000000000000000"  # Replace this with your own client id
 
 with Presence(client_id) as presence:
-    presence.set({
-        'state': 'In Game',
-        'details': "Summoner's Rift",
-        'timestamps': {
-            'start': int(time.time())
-        },
-    })
+    presence.set(
+        {
+            "state": "In Game",
+            "details": "Summoner's Rift",
+            "timestamps": {"start": int(time.time())},
+        }
+    )
 
     while True:
         time.sleep(15)
 ```
 Make sure you replace the `client_id` variable with your app's id that you copied earlier.
 
 7. Run the program! You should now see that you have a rich presence on your profile that will be on until you stop the program! Feel free to change the code however you want by adding images, buttons, and more. Check out [examples/complex.py](examples/complex.py) for another example.
```

### Comparing `discord-rich-presence-1.0.2/setup.py` & `discord-rich-presence-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup
 import discordrp
 
-with open('./README.md') as file:
+with open("./README.md") as file:
     long_description = file.read()
 
 setup(
     name=discordrp.__title__,
     version=discordrp.__version__,
-    description='A lightweight and safe module for creating custom rich presences on Discord.',
+    description="A lightweight and safe module for creating custom rich presences on Discord.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/TenType/discord-rich-presence',
+    long_description_content_type="text/markdown",
+    url="https://github.com/TenType/discord-rich-presence",
     author=discordrp.__author__,
     license=discordrp.__license__,
-    keywords=['discord', 'presence', 'rich presence', 'activity', 'rpc'],
+    keywords=["discord", "presence", "rich presence", "activity", "rpc"],
     classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: End Users/Desktop',
-        'Operating System :: MacOS',
-        'Operating System :: Microsoft :: Windows',
-        'Operating System :: Unix',
-        'Typing :: Typed',
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Intended Audience :: End Users/Desktop",
+        "Operating System :: MacOS",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: Unix",
+        "Typing :: Typed",
     ],
-    python_requires='>=3.9',
+    python_requires=">=3.9",
+    package_data={"discordrp": ["py.typed"]},
 )
```

