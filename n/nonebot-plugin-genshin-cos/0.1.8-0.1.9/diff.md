# Comparing `tmp/nonebot_plugin_genshin_cos-0.1.8.tar.gz` & `tmp/nonebot_plugin_genshin_cos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_genshin_cos-0.1.8.tar` & `nonebot_plugin_genshin_cos-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.8/LICENSE
--rw-r--r--   0        0        0     8905 2023-06-05 05:33:05.302878 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/__init__.py
--rw-r--r--   0        0        0      269 2023-06-05 05:24:06.712318 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/config.py
--rw-r--r--   0        0        0   459180 2023-06-05 05:24:06.718316 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
--rw-r--r--   0        0        0    11068 2023-06-05 05:24:06.719317 nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/utils.py
--rw-r--r--   0        0        0      661 2023-06-05 05:38:03.920857 nonebot_plugin_genshin_cos-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3636 2023-06-05 05:24:06.711314 nonebot_plugin_genshin_cos-0.1.8/README.md
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.9/LICENSE
+-rw-r--r--   0        0        0     9064 2023-06-12 11:50:54.865621 nonebot_plugin_genshin_cos-0.1.9/nonebot_plugin_genshin_cos/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-05 05:24:06.712318 nonebot_plugin_genshin_cos-0.1.9/nonebot_plugin_genshin_cos/config.py
+-rw-r--r--   0        0        0   459180 2023-06-05 05:24:06.718316 nonebot_plugin_genshin_cos-0.1.9/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
+-rw-r--r--   0        0        0    11068 2023-06-05 05:24:06.719317 nonebot_plugin_genshin_cos-0.1.9/nonebot_plugin_genshin_cos/utils.py
+-rw-r--r--   0        0        0      661 2023-06-12 11:52:40.997032 nonebot_plugin_genshin_cos-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3636 2023-06-05 05:24:06.711314 nonebot_plugin_genshin_cos-0.1.9/README.md
+-rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_genshin_cos-0.1.8/LICENSE` & `nonebot_plugin_genshin_cos-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/__init__.py` & `nonebot_plugin_genshin_cos-0.1.9/nonebot_plugin_genshin_cos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 import re
 from datetime import datetime, timedelta
 
 __plugin_meta__ = PluginMetadata(
     name="米游社cos",
     description="获取原神coser图片",
     config=Config,
-    usage="原神cos",
+    usage="原神cos,CosPlus,下载cos",
+    type = "application",
+    homepage = "https://github.com/Cvandia/nonebot_plugin_genshin_cos",
+    supported_adapters={"~onebot.v11"},
     extra={
         "unique_name": "genshin_cos",
         "example": "保存cos:保存cos图片至本地文件",
         "author": "divandia <106718176+Cvandia@users.noreply.github.com>",
-        "version": "0.1.7",
+        "version": "0.1.9",
     },
 )
 logo = """<g>
   /$$$$$$                                /$$       /$$                  /$$$$$$                     
  /$$__  $$                              | $$      |__/                 /$$__  $$                    
 | $$  \__/  /$$$$$$  /$$$$$$$   /$$$$$$$| $$$$$$$  /$$ /$$$$$$$       | $$  \__/  /$$$$$$   /$$$$$$$
 | $$ /$$$$ /$$__  $$| $$__  $$ /$$_____/| $$__  $$| $$| $$__  $$      | $$       /$$__  $$ /$$_____/
```

### Comparing `nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF` & `nonebot_plugin_genshin_cos-0.1.9/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.8/nonebot_plugin_genshin_cos/utils.py` & `nonebot_plugin_genshin_cos-0.1.9/nonebot_plugin_genshin_cos/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.8/pyproject.toml` & `nonebot_plugin_genshin_cos-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-genshin-cos"
-version = "0.1.8"
+version = "0.1.9"
 description = "米游社原神cos图获取"
 authors = ["Cvandia <106718176+Cvandia@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_genshin_cos"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_genshin_cos-0.1.8/README.md` & `nonebot_plugin_genshin_cos-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.8/PKG-INFO` & `nonebot_plugin_genshin_cos-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshin-cos
-Version: 0.1.8
+Version: 0.1.9
 Summary: 米游社原神cos图获取
 License: MIT
 Author: Cvandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.9 Summary:
 ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: Cvandia Author-email:
 106718176+Cvandia@users.noreply.github.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-
```

