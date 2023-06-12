# Comparing `tmp/minecraft-forgePY-1.0.1.tar.gz` & `tmp/minecraft-forgePY-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft-forgePY-1.0.1.tar", last modified: Mon Jun 12 14:16:30 2023, max compression
+gzip compressed data, was "minecraft-forgePY-1.0.3.tar", last modified: Mon Jun 12 14:32:55 2023, max compression
```

## Comparing `minecraft-forgePY-1.0.1.tar` & `minecraft-forgePY-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:16:30.146070 minecraft-forgePY-1.0.1/
--rw-rw-rw-   0        0        0      844 2023-06-12 14:16:30.145069 minecraft-forgePY-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-06-12 14:16:05.000000 minecraft-forgePY-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 14:16:30.121425 minecraft-forgePY-1.0.1/forgepy/
--rw-rw-rw-   0        0        0       51 2023-06-12 12:54:54.000000 minecraft-forgePY-1.0.1/forgepy/__init__.py
--rw-rw-rw-   0        0        0      748 2023-06-12 12:55:07.000000 minecraft-forgePY-1.0.1/forgepy/forgepy.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:16:30.143949 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/
--rw-rw-rw-   0        0        0      844 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-12 14:16:30.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 14:16:29.000000 minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 14:16:30.146070 minecraft-forgePY-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-06-12 14:15:09.000000 minecraft-forgePY-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:55.933917 minecraft-forgePY-1.0.3/
+-rw-rw-rw-   0        0        0     1073 2023-06-12 14:32:55.932919 minecraft-forgePY-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-06-12 14:30:36.000000 minecraft-forgePY-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:55.908992 minecraft-forgePY-1.0.3/forgepy/
+-rw-rw-rw-   0        0        0       73 2023-06-12 14:31:51.000000 minecraft-forgePY-1.0.3/forgepy/__init__.py
+-rw-rw-rw-   0        0        0      748 2023-06-12 12:55:07.000000 minecraft-forgePY-1.0.3/forgepy/forgepy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:32:55.931412 minecraft-forgePY-1.0.3/minecraft_forgePY.egg-info/
+-rw-rw-rw-   0        0        0     1073 2023-06-12 14:32:55.000000 minecraft-forgePY-1.0.3/minecraft_forgePY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-12 14:32:55.000000 minecraft-forgePY-1.0.3/minecraft_forgePY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:32:55.000000 minecraft-forgePY-1.0.3/minecraft_forgePY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 14:32:55.000000 minecraft-forgePY-1.0.3/minecraft_forgePY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 14:32:55.000000 minecraft-forgePY-1.0.3/minecraft_forgePY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:32:55.933917 minecraft-forgePY-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-06-12 14:32:42.000000 minecraft-forgePY-1.0.3/setup.py
```

### Comparing `minecraft-forgePY-1.0.1/PKG-INFO` & `minecraft-forgePY-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: minecraft-forgePY
-Version: 1.0.1
+Version: 1.0.3
 Summary: Get Minecraft Forge download URLs.
 Author: matejmajny
-Keywords: python,minecraft,forge,API
+Keywords: python,minecraft,forge,API,forgepy
 Description-Content-Type: text/markdown
 
 
-# 📦 ForgePY
+# 📦 minecraft-forgepy
 A simple Python package to fetch latest and recommended download URLs of [Minecraft Forge](https://files.minecraftforge.net/net/minecraftforge/forge/) website. 
 
 ## 💾 Installation 
 ```
 pip install minecraft-forgepy 
 ```
 
 ## 🔍 How to use
 ```
 import forgepy
 
-latest = GetLatestURL("1.19.4")
-recommended = GetRecommendedURL("1.19.4")
+latest = forgepy.GetLatestURL("1.19.4")
+recommended = forgepy.GetRecommendedURL("1.19.4")
 ```
 
 ## ❗Disclaimer
-This package only supports Minecraft versions **1.5.2 and above**.
+- This package only supports Minecraft versions **1.5.2 and above**.
+- original name for this package was supposed to be forgePY, but due to PyPi not letting me upload it, PyPi name is minecraft-forgepy. **But name forgepy is still and will be used in code!**
 
 ## 🤖 Source Code
 - This project is licensed under GNU General Public License v3.0
 - [GitHub repository](https://github.com/matejmajny/forge.py)
```

### Comparing `minecraft-forgePY-1.0.1/README.md` & `minecraft-forgePY-1.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# 📦 ForgePY
+# 📦 minecraft-forgepy
 A simple Python package to fetch latest and recommended download URLs of [Minecraft Forge](https://files.minecraftforge.net/net/minecraftforge/forge/) website. 
 
 ## 💾 Installation 
 ```
 pip install minecraft-forgepy 
 ```
 
 ## 🔍 How to use
 ```
 import forgepy
 
-latest = GetLatestURL("1.19.4")
-recommended = GetRecommendedURL("1.19.4")
+latest = forgepy.GetLatestURL("1.19.4")
+recommended = forgepy.GetRecommendedURL("1.19.4")
 ```
 
 ## ❗Disclaimer
-This package only supports Minecraft versions **1.5.2 and above**.
+- This package only supports Minecraft versions **1.5.2 and above**.
+- original name for this package was supposed to be forgePY, but due to PyPi not letting me upload it, PyPi name is minecraft-forgepy. **But name forgepy is still and will be used in code!**
 
 ## 🤖 Source Code
 - This project is licensed under GNU General Public License v3.0
 - [GitHub repository](https://github.com/matejmajny/forge.py)
```

### Comparing `minecraft-forgePY-1.0.1/forgepy/forgepy.py` & `minecraft-forgePY-1.0.3/forgepy/forgepy.py`

 * *Files identical despite different names*

### Comparing `minecraft-forgePY-1.0.1/minecraft_forgePY.egg-info/PKG-INFO` & `minecraft-forgePY-1.0.3/minecraft_forgePY.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: minecraft-forgePY
-Version: 1.0.1
+Version: 1.0.3
 Summary: Get Minecraft Forge download URLs.
 Author: matejmajny
-Keywords: python,minecraft,forge,API
+Keywords: python,minecraft,forge,API,forgepy
 Description-Content-Type: text/markdown
 
 
-# 📦 ForgePY
+# 📦 minecraft-forgepy
 A simple Python package to fetch latest and recommended download URLs of [Minecraft Forge](https://files.minecraftforge.net/net/minecraftforge/forge/) website. 
 
 ## 💾 Installation 
 ```
 pip install minecraft-forgepy 
 ```
 
 ## 🔍 How to use
 ```
 import forgepy
 
-latest = GetLatestURL("1.19.4")
-recommended = GetRecommendedURL("1.19.4")
+latest = forgepy.GetLatestURL("1.19.4")
+recommended = forgepy.GetRecommendedURL("1.19.4")
 ```
 
 ## ❗Disclaimer
-This package only supports Minecraft versions **1.5.2 and above**.
+- This package only supports Minecraft versions **1.5.2 and above**.
+- original name for this package was supposed to be forgePY, but due to PyPi not letting me upload it, PyPi name is minecraft-forgepy. **But name forgepy is still and will be used in code!**
 
 ## 🤖 Source Code
 - This project is licensed under GNU General Public License v3.0
 - [GitHub repository](https://github.com/matejmajny/forge.py)
```

### Comparing `minecraft-forgePY-1.0.1/setup.py` & `minecraft-forgePY-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import codecs, os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.3'
 DESCRIPTION = 'Get Minecraft Forge download URLs.'
 LONG_DESCRIPTION = 'A package to get Forge latest and recommended download URLs.'
 
 setup(
     name="minecraft-forgePY",
     version=VERSION,
     author="matejmajny",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=["requests", "bs4"],
-    keywords=['python', "minecraft", "forge", "API"],
+    keywords=['python', "minecraft", "forge", "API", "forgepy"],
 )
```

