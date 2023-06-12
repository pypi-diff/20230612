# Comparing `tmp/picframe-2023.5.17.tar.gz` & `tmp/picframe-2023.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picframe-2023.5.17.tar", last modified: Wed May 17 08:43:42 2023, max compression
+gzip compressed data, was "picframe-2023.6.12.tar", last modified: Mon Jun 12 15:41:29 2023, max compression
```

## Comparing `picframe-2023.5.17.tar` & `picframe-2023.6.12.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 08:43:19.000000 picframe-2023.5.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-17 08:43:42.030278 picframe-2023.5.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-17 08:43:19.000000 picframe-2023.5.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-17 08:43:19.000000 picframe-2023.5.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 08:43:42.030278 picframe-2023.5.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 08:43:19.000000 picframe-2023.5.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.018278 picframe-2023.5.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/config/configuration_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe/data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   455164 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   471004 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   470472 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   455188 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/data/mat/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_bevel.png
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_drop_shadow.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_highlight.png
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/9_patch_inner_shadow.png
--rw-r--r--   0 runner    (1001) docker     (123)  2081776 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/mat/mat_texture.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   160442 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/no_pictures.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/data/shaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/shaders/blend_new.fs
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/data/shaders/blend_new.vs
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/geo_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/get_image_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/src/picframe/html/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/html/pf_functions.js
--rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/interface_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/interface_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/interface_peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/mat_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/start.py
--rw-r--r--   0 runner    (1001) docker     (123)    27228 2023-05-17 08:43:19.000000 picframe-2023.5.17/src/picframe/viewer_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.026278 picframe-2023.5.17/src/picframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 08:43:42.000000 picframe-2023.5.17/src/picframe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:43:42.030278 picframe-2023.5.17/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-17 08:43:19.000000 picframe-2023.5.17/test/test_get_image_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-17 08:43:19.000000 picframe-2023.5.17/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.540731 picframe-2023.6.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 15:41:14.000000 picframe-2023.6.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-12 15:41:29.540731 picframe-2023.6.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-12 15:41:14.000000 picframe-2023.6.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-12 15:41:14.000000 picframe-2023.6.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-12 15:41:29.540731 picframe-2023.6.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 15:41:14.000000 picframe-2023.6.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.528731 picframe-2023.6.12/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.540731 picframe-2023.6.12/src/picframe/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 15:41:29.540731 picframe-2023.6.12/src/picframe/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.536731 picframe-2023.6.12/src/picframe/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/config/configuration_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.536731 picframe-2023.6.12/src/picframe/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.536731 picframe-2023.6.12/src/picframe/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   455164 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/fonts/NotoSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   471004 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/fonts/NotoSans-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   470472 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/fonts/NotoSans-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   455188 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/fonts/NotoSans-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.536731 picframe-2023.6.12/src/picframe/data/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/mat/9_patch_bevel.png
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/mat/9_patch_drop_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/mat/9_patch_highlight.png
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/mat/9_patch_inner_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2081776 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/mat/mat_texture.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   160442 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/no_pictures.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.540731 picframe-2023.6.12/src/picframe/data/shaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/shaders/blend_new.fs
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/data/shaders/blend_new.vs
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/geo_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/get_image_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.540731 picframe-2023.6.12/src/picframe/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/html/pf_functions.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/interface_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/interface_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/interface_peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/mat_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27228 2023-06-12 15:41:14.000000 picframe-2023.6.12/src/picframe/viewer_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.536731 picframe-2023.6.12/src/picframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-12 15:41:29.000000 picframe-2023.6.12/src/picframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-12 15:41:29.000000 picframe-2023.6.12/src/picframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:41:29.000000 picframe-2023.6.12/src/picframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 15:41:29.000000 picframe-2023.6.12/src/picframe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-12 15:41:29.000000 picframe-2023.6.12/src/picframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 15:41:29.000000 picframe-2023.6.12/src/picframe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:41:29.540731 picframe-2023.6.12/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-12 15:41:14.000000 picframe-2023.6.12/test/test_get_image_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-12 15:41:14.000000 picframe-2023.6.12/versioneer.py
```

### Comparing `picframe-2023.5.17/LICENSE` & `picframe-2023.6.12/LICENSE`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/PKG-INFO` & `picframe-2023.6.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2023.5.17
+Version: 2023.6.12
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Author: Paddy Gaunt, Jeff Godfrey
 Author-email: Helge Erbe <helge@erbehome.de>
 Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
 Project-URL: Homepage, https://github.com/helgeerbe/picframe
 Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
```

### Comparing `picframe-2023.5.17/README.md` & `picframe-2023.6.12/README.md`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/pyproject.toml` & `picframe-2023.6.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/config/configuration_example.yaml` & `picframe-2023.6.12/src/picframe/config/configuration_example.yaml`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/controller.py` & `picframe-2023.6.12/src/picframe/controller.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/fonts/LICENSE.txt` & `picframe-2023.6.12/src/picframe/data/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Bold.ttf` & `picframe-2023.6.12/src/picframe/data/fonts/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/fonts/NotoSans-BoldItalic.ttf` & `picframe-2023.6.12/src/picframe/data/fonts/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Italic.ttf` & `picframe-2023.6.12/src/picframe/data/fonts/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/fonts/NotoSans-Regular.ttf` & `picframe-2023.6.12/src/picframe/data/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/mat/9_patch_drop_shadow.png` & `picframe-2023.6.12/src/picframe/data/mat/9_patch_drop_shadow.png`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/mat/mat_texture.jpg` & `picframe-2023.6.12/src/picframe/data/mat/mat_texture.jpg`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/no_pictures.jpg` & `picframe-2023.6.12/src/picframe/data/no_pictures.jpg`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/data/shaders/blend_new.fs` & `picframe-2023.6.12/src/picframe/data/shaders/blend_new.fs`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/geo_reverse.py` & `picframe-2023.6.12/src/picframe/geo_reverse.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/get_image_meta.py` & `picframe-2023.6.12/src/picframe/get_image_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 from PIL import Image
 from PIL.ExifTags import TAGS, GPSTAGS
-from pi_heif import register_heif_opener
 from fractions import Fraction
 
+try:
+    from pi_heif import register_heif_opener
 
-register_heif_opener()
+    register_heif_opener()
+except ImportError:
+    register_heif_opener = None
 
 
 class GetImageMeta:
 
     def __init__(self, filename):
         self.__logger = logging.getLogger("get_image_meta.GetImageMeta")
         self.__tags = {}
```

### Comparing `picframe-2023.5.17/src/picframe/html/index.html` & `picframe-2023.6.12/src/picframe/html/index.html`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/html/pf_functions.js` & `picframe-2023.6.12/src/picframe/html/pf_functions.js`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/image_cache.py` & `picframe-2023.6.12/src/picframe/image_cache.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/interface_http.py` & `picframe-2023.6.12/src/picframe/interface_http.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,33 @@
 try:
     from http.server import BaseHTTPRequestHandler, HTTPServer  # py3
     import urllib.parse as urlparse
 except ImportError:
     from BaseHTTPServer import BaseHTTPRequestHandler, HTTPServer  # py2
     import urlparse
 
-EXTENSIONS = [".jpg", ".jpeg", ".png", ".heif", ".heic"]
+try:
+    from pi_heif import register_heif_opener
+except ImportError:
+    register_heif_opener = None
+
+EXTENSIONS = [".jpg", ".jpeg", ".png"]
+if register_heif_opener is not None:
+    EXTENSIONS += [".heif", ".heic"]
 
 
 def heif_to_jpg(fname):
     try:
         from PIL import Image
-        from pi_heif import register_heif_opener
+        try:
+            from pi_heif import register_heif_opener
+            register_heif_opener()
+        except ImportError:
+            register_heif_opener = None
 
-        register_heif_opener()
         image = Image.open(fname)
         if image.mode not in ("RGB", "RGBA"):
             image = image.convert("RGB")
         image.save("/dev/shm/temp.jpg")  # default 75% quality
         return "/dev/shm/temp.jpg"
     except Exception:
         logger = logging.getLogger("interface_http.heif_to_jpg")
```

### Comparing `picframe-2023.5.17/src/picframe/interface_mqtt.py` & `picframe-2023.6.12/src/picframe/interface_mqtt.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/interface_peripherals.py` & `picframe-2023.6.12/src/picframe/interface_peripherals.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/mat_image.py` & `picframe-2023.6.12/src/picframe/mat_image.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/model.py` & `picframe-2023.6.12/src/picframe/model.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/start.py` & `picframe-2023.6.12/src/picframe/start.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe/viewer_display.py` & `picframe-2023.6.12/src/picframe/viewer_display.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/src/picframe.egg-info/PKG-INFO` & `picframe-2023.6.12/src/picframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2023.5.17
+Version: 2023.6.12
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Author: Paddy Gaunt, Jeff Godfrey
 Author-email: Helge Erbe <helge@erbehome.de>
 Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
 Project-URL: Homepage, https://github.com/helgeerbe/picframe
 Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
```

### Comparing `picframe-2023.5.17/src/picframe.egg-info/SOURCES.txt` & `picframe-2023.6.12/src/picframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/test/test_get_image_meta.py` & `picframe-2023.6.12/test/test_get_image_meta.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.5.17/versioneer.py` & `picframe-2023.6.12/versioneer.py`

 * *Files identical despite different names*

