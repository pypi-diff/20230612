# Comparing `tmp/minecraft-ForgePY-1.0.0.tar.gz` & `tmp/minecraft-forgePY-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft-ForgePY-1.0.0.tar", last modified: Mon Jun 12 13:58:03 2023, max compression
+gzip compressed data, was "minecraft-forgePY-1.0.1.tar", last modified: Mon Jun 12 14:16:30 2023, max compression
```

## Comparing `minecraft-ForgePY-1.0.0.tar` & `minecraft-forgePY-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 13:58:03.616277 minecraft-ForgePY-1.0.0/
--rw-rw-rw-   0        0        0      834 2023-06-12 13:58:03.614282 minecraft-ForgePY-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-06-12 13:26:03.000000 minecraft-ForgePY-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 13:58:03.590662 minecraft-ForgePY-1.0.0/forgepy/
--rw-rw-rw-   0        0        0       51 2023-06-12 12:54:54.000000 minecraft-ForgePY-1.0.0/forgepy/__init__.py
--rw-rw-rw-   0        0        0      748 2023-06-12 12:55:07.000000 minecraft-ForgePY-1.0.0/forgepy/forgepy.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:58:03.611913 minecraft-ForgePY-1.0.0/minecraft_ForgePY.egg-info/
--rw-rw-rw-   0        0        0      834 2023-06-12 13:58:03.000000 minecraft-ForgePY-1.0.0/minecraft_ForgePY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-12 13:58:03.000000 minecraft-ForgePY-1.0.0/minecraft_ForgePY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 13:58:03.000000 minecraft-ForgePY-1.0.0/minecraft_ForgePY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 13:58:03.000000 minecraft-ForgePY-1.0.0/minecraft_ForgePY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 13:58:03.000000 minecraft-ForgePY-1.0.0/minecraft_ForgePY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 13:58:03.616277 minecraft-ForgePY-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-06-12 13:57:54.000000 minecraft-ForgePY-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:16:30.146070 minecraft-forgePY-1.0.1/
+-rw-rw-rw-   0        0        0      844 2023-06-12 14:16:30.145069 minecraft-forgePY-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-06-12 14:16:05.000000 minecraft-forgePY-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 14:16:30.121425 minecraft-forgePY-1.0.1/forgepy/
+-rw-rw-rw-   0        0        0       51 2023-06-12 12:54:54.000000 minecraft-forgePY-1.0.1/forgepy/__init__.py
+-rw-rw-rw-   0        0        0      748 2023-06-12 12:55:07.000000 minecraft-forgePY-1.0.1/forgepy/forgepy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:16:30.143949 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/
+-rw-rw-rw-   0        0        0      844 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-12 14:16:30.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:16:30.146070 minecraft-forgePY-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-06-12 14:15:09.000000 minecraft-forgePY-1.0.1/setup.py
```

### Comparing `minecraft-ForgePY-1.0.0/PKG-INFO` & `minecraft-forgePY-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: minecraft-ForgePY
-Version: 1.0.0
+Name: minecraft-forgePY
+Version: 1.0.1
 Summary: Get Minecraft Forge download URLs.
 Author: matejmajny
 Keywords: python,minecraft,forge,API
 Description-Content-Type: text/markdown
 
 
 # 📦 ForgePY
 A simple Python package to fetch latest and recommended download URLs of [Minecraft Forge](https://files.minecraftforge.net/net/minecraftforge/forge/) website. 
 
 ## 💾 Installation 
 ```
-pip install forgepy 
+pip install minecraft-forgepy 
 ```
 
 ## 🔍 How to use
 ```
 import forgepy
 
 latest = GetLatestURL("1.19.4")
```

### Comparing `minecraft-ForgePY-1.0.0/README.md` & `minecraft-forgePY-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 📦 ForgePY
 A simple Python package to fetch latest and recommended download URLs of [Minecraft Forge](https://files.minecraftforge.net/net/minecraftforge/forge/) website. 
 
 ## 💾 Installation 
 ```
-pip install forgepy 
+pip install minecraft-forgepy 
 ```
 
 ## 🔍 How to use
 ```
 import forgepy
 
 latest = GetLatestURL("1.19.4")
```

### Comparing `minecraft-ForgePY-1.0.0/forgepy/forgepy.py` & `minecraft-forgePY-1.0.1/forgepy/forgepy.py`

 * *Files identical despite different names*

### Comparing `minecraft-ForgePY-1.0.0/minecraft_ForgePY.egg-info/PKG-INFO` & `minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: minecraft-ForgePY
-Version: 1.0.0
+Name: minecraft-forgePY
+Version: 1.0.1
 Summary: Get Minecraft Forge download URLs.
 Author: matejmajny
 Keywords: python,minecraft,forge,API
 Description-Content-Type: text/markdown
 
 
 # 📦 ForgePY
 A simple Python package to fetch latest and recommended download URLs of [Minecraft Forge](https://files.minecraftforge.net/net/minecraftforge/forge/) website. 
 
 ## 💾 Installation 
 ```
-pip install forgepy 
+pip install minecraft-forgepy 
 ```
 
 ## 🔍 How to use
 ```
 import forgepy
 
 latest = GetLatestURL("1.19.4")
```

### Comparing `minecraft-ForgePY-1.0.0/setup.py` & `minecraft-forgePY-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import codecs, os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Get Minecraft Forge download URLs.'
 LONG_DESCRIPTION = 'A package to get Forge latest and recommended download URLs.'
 
 setup(
-    name="minecraft-ForgePY",
+    name="minecraft-forgePY",
     version=VERSION,
     author="matejmajny",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=["requests", "bs4"],
```

