# Comparing `tmp/whist_score-0.1.12.tar.gz` & `tmp/whist_score-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whist_score-0.1.12.tar", last modified: Mon Jun 12 19:30:14 2023, max compression
+gzip compressed data, was "whist_score-0.1.13.tar", last modified: Mon Jun 12 19:39:36 2023, max compression
```

## Comparing `whist_score-0.1.12.tar` & `whist_score-0.1.13.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:30:14.485942 whist_score-0.1.12/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    35149 2023-06-12 16:32:28.000000 whist_score-0.1.12/LICENSE
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       14 2023-06-12 19:29:48.000000 whist_score-0.1.12/MANIFEST.in
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 19:30:14.485942 whist_score-0.1.12/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-12 16:24:02.000000 whist_score-0.1.12/README.md
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:30:14.485942 whist_score-0.1.12/config/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     3269 2023-06-12 17:47:59.000000 whist_score-0.1.12/config/abondance_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1299 2023-06-12 17:44:14.000000 whist_score-0.1.12/config/game_types.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      671 2023-06-12 17:44:58.000000 whist_score-0.1.12/config/miserie_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1913 2023-06-12 17:46:13.000000 whist_score-0.1.12/config/solo_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1277 2023-06-12 17:45:32.000000 whist_score-0.1.12/config/troel_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     3869 2023-06-12 17:47:06.000000 whist_score-0.1.12/config/vragen_en_meegaan_point_system.json
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      797 2023-06-12 18:53:38.000000 whist_score-0.1.12/main.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2023-06-12 19:30:14.485942 whist_score-0.1.12/setup.cfg
--rw-rw-r--   0 erwin     (1000) erwin     (1000)     1014 2023-06-12 19:29:29.000000 whist_score-0.1.12/setup.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:30:14.485942 whist_score-0.1.12/whist_score/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:19:17.000000 whist_score-0.1.12/whist_score/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      827 2023-06-12 19:18:00.000000 whist_score-0.1.12/whist_score/constants.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:30:14.485942 whist_score-0.1.12/whist_score/models/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    17347 2023-06-12 19:12:55.000000 whist_score-0.1.12/whist_score/models/Game.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      505 2023-06-05 14:32:02.000000 whist_score-0.1.12/whist_score/models/Player.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)    10315 2023-06-12 19:19:38.000000 whist_score-0.1.12/whist_score/models/RoundTypes.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:22:20.000000 whist_score-0.1.12/whist_score/models/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      252 2023-06-12 18:46:17.000000 whist_score-0.1.12/whist_score/utils.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:30:14.485942 whist_score-0.1.12/whist_score/views/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 10:00:47.000000 whist_score-0.1.12/whist_score/views/__init__.py
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      973 2023-06-12 18:53:29.000000 whist_score-0.1.12/whist_score/views/games.py
-drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:30:14.485942 whist_score-0.1.12/whist_score.egg-info/
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 19:30:14.000000 whist_score-0.1.12/whist_score.egg-info/PKG-INFO
--rw-rw-r--   0 erwin     (1000) erwin     (1000)      700 2023-06-12 19:30:14.000000 whist_score-0.1.12/whist_score.egg-info/SOURCES.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2023-06-12 19:30:14.000000 whist_score-0.1.12/whist_score.egg-info/dependency_links.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       42 2023-06-12 19:30:14.000000 whist_score-0.1.12/whist_score.egg-info/entry_points.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       29 2023-06-12 19:30:14.000000 whist_score-0.1.12/whist_score.egg-info/requires.txt
--rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2023-06-12 19:30:14.000000 whist_score-0.1.12/whist_score.egg-info/top_level.txt
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    35149 2023-06-12 16:32:28.000000 whist_score-0.1.13/LICENSE
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       14 2023-06-12 19:29:48.000000 whist_score-0.1.13/MANIFEST.in
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 19:39:36.457894 whist_score-0.1.13/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-12 16:24:02.000000 whist_score-0.1.13/README.md
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/config/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     3269 2023-06-12 17:47:59.000000 whist_score-0.1.13/config/abondance_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1299 2023-06-12 17:44:14.000000 whist_score-0.1.13/config/game_types.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      671 2023-06-12 17:44:58.000000 whist_score-0.1.13/config/miserie_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1913 2023-06-12 17:46:13.000000 whist_score-0.1.13/config/solo_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     1277 2023-06-12 17:45:32.000000 whist_score-0.1.13/config/troel_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)     3869 2023-06-12 17:47:06.000000 whist_score-0.1.13/config/vragen_en_meegaan_point_system.json
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      797 2023-06-12 18:53:38.000000 whist_score-0.1.13/main.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       38 2023-06-12 19:39:36.457894 whist_score-0.1.13/setup.cfg
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      996 2023-06-12 19:31:35.000000 whist_score-0.1.13/setup.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:19:17.000000 whist_score-0.1.13/whist_score/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      827 2023-06-12 19:18:00.000000 whist_score-0.1.13/whist_score/constants.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score/models/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    17347 2023-06-12 19:12:55.000000 whist_score-0.1.13/whist_score/models/Game.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      505 2023-06-05 14:32:02.000000 whist_score-0.1.13/whist_score/models/Player.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)    10315 2023-06-12 19:19:38.000000 whist_score-0.1.13/whist_score/models/RoundTypes.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 09:22:20.000000 whist_score-0.1.13/whist_score/models/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      252 2023-06-12 18:46:17.000000 whist_score-0.1.13/whist_score/utils.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score/views/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        0 2023-06-05 10:00:47.000000 whist_score-0.1.13/whist_score/views/__init__.py
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      973 2023-06-12 18:53:29.000000 whist_score-0.1.13/whist_score/views/games.py
+drwxrwxr-x   0 erwin     (1000) erwin     (1000)        0 2023-06-12 19:39:36.457894 whist_score-0.1.13/whist_score.egg-info/
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      424 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/PKG-INFO
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)      700 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/SOURCES.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)        1 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/dependency_links.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       42 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/entry_points.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       29 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/requires.txt
+-rw-rw-r--   0 erwin     (1000) erwin     (1000)       12 2023-06-12 19:39:36.000000 whist_score-0.1.13/whist_score.egg-info/top_level.txt
```

### Comparing `whist_score-0.1.12/LICENSE` & `whist_score-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/config/abondance_point_system.json` & `whist_score-0.1.13/config/abondance_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/config/game_types.json` & `whist_score-0.1.13/config/game_types.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/config/miserie_point_system.json` & `whist_score-0.1.13/config/miserie_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/config/solo_point_system.json` & `whist_score-0.1.13/config/solo_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/config/troel_point_system.json` & `whist_score-0.1.13/config/troel_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/config/vragen_en_meegaan_point_system.json` & `whist_score-0.1.13/config/vragen_en_meegaan_point_system.json`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/main.py` & `whist_score-0.1.13/main.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/setup.py` & `whist_score-0.1.13/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,25 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name="whist_score",
-    version="0.1.12",
+    version="0.1.13",
     author="Erwin Mintiens",
     author_email="erwin.mintiens@protonmail.com",
     license_files=("LICENSE",),
     description="whist_score is a scorekeeper for the whist card game.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erwinmintiens/whist-score",
     packages=find_packages(),
     include_package_data=True,
-    package_data={"whist_score": ["config/*.json"]},
+    package_data={"": ["*.json"]},
     install_requires=["click>=7.1.2", "colorama>=0.4.6"],
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     entry_points="""
```

### Comparing `whist_score-0.1.12/whist_score/constants.py` & `whist_score-0.1.13/whist_score/constants.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/whist_score/models/Game.py` & `whist_score-0.1.13/whist_score/models/Game.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/whist_score/models/RoundTypes.py` & `whist_score-0.1.13/whist_score/models/RoundTypes.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/whist_score/views/games.py` & `whist_score-0.1.13/whist_score/views/games.py`

 * *Files identical despite different names*

### Comparing `whist_score-0.1.12/whist_score.egg-info/SOURCES.txt` & `whist_score-0.1.13/whist_score.egg-info/SOURCES.txt`

 * *Files identical despite different names*

