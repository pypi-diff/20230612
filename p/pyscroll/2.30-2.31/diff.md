# Comparing `tmp/pyscroll-2.30.tar.gz` & `tmp/pyscroll-2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscroll-2.30.tar", last modified: Fri Apr  8 21:44:48 2022, max compression
+gzip compressed data, was "pyscroll-2.31.tar", last modified: Mon Jun 12 21:31:35 2023, max compression
```

## Comparing `pyscroll-2.30.tar` & `pyscroll-2.31.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 ltheden   (1000) ltheden   (1000)        0 2022-04-08 21:44:48.011279 pyscroll-2.30/
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      886 2022-04-08 21:44:48.011279 pyscroll-2.30/PKG-INFO
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     8083 2022-04-04 21:28:10.000000 pyscroll-2.30/README.md
-drwxrwxr-x   0 ltheden   (1000) ltheden   (1000)        0 2022-04-08 21:44:48.011279 pyscroll-2.30/pyscroll/
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      302 2022-04-08 21:40:10.000000 pyscroll-2.30/pyscroll/__init__.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     1767 2021-11-19 11:42:49.000000 pyscroll-2.30/pyscroll/animation.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      777 2021-12-10 22:34:35.000000 pyscroll-2.30/pyscroll/common.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)    14906 2022-04-08 21:42:09.000000 pyscroll-2.30/pyscroll/data.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     2127 2021-11-19 11:45:37.000000 pyscroll-2.30/pyscroll/group.py
--rw-r--r--   0 ltheden   (1000) ltheden   (1000)     4587 2021-11-10 15:41:45.000000 pyscroll-2.30/pyscroll/isometric.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)    22662 2021-12-10 20:34:19.000000 pyscroll-2.30/pyscroll/orthographic.py
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     4443 2021-11-19 11:42:49.000000 pyscroll-2.30/pyscroll/quadtree.py
-drwxrwxr-x   0 ltheden   (1000) ltheden   (1000)        0 2022-04-08 21:44:48.011279 pyscroll-2.30/pyscroll.egg-info/
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      886 2022-04-08 21:44:47.000000 pyscroll-2.30/pyscroll.egg-info/PKG-INFO
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)      352 2022-04-08 21:44:47.000000 pyscroll-2.30/pyscroll.egg-info/SOURCES.txt
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)        1 2022-04-08 21:44:47.000000 pyscroll-2.30/pyscroll.egg-info/dependency_links.txt
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)        7 2022-04-08 21:44:47.000000 pyscroll-2.30/pyscroll.egg-info/requires.txt
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)        9 2022-04-08 21:44:47.000000 pyscroll-2.30/pyscroll.egg-info/top_level.txt
--rw-r--r--   0 ltheden   (1000) ltheden   (1000)       79 2022-04-08 21:44:48.012279 pyscroll-2.30/setup.cfg
--rw-rw-r--   0 ltheden   (1000) ltheden   (1000)     1235 2022-04-08 21:40:10.000000 pyscroll-2.30/setup.py
+drwxr-xr-x   0 ltheden   (1000) ltheden   (1000)        0 2023-06-12 21:31:35.943925 pyscroll-2.31/
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      867 2023-06-12 21:31:35.943925 pyscroll-2.31/PKG-INFO
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     8083 2023-06-12 20:17:50.000000 pyscroll-2.31/README.md
+drwxr-xr-x   0 ltheden   (1000) ltheden   (1000)        0 2023-06-12 21:31:35.943925 pyscroll-2.31/pyscroll/
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      302 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/__init__.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     1767 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/animation.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      777 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/common.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)    14906 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/data.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     2157 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/group.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     4587 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/isometric.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)    22662 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/orthographic.py
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     4443 2023-06-12 20:17:50.000000 pyscroll-2.31/pyscroll/quadtree.py
+drwxr-xr-x   0 ltheden   (1000) ltheden   (1000)        0 2023-06-12 21:31:35.943925 pyscroll-2.31/pyscroll.egg-info/
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      867 2023-06-12 21:31:35.000000 pyscroll-2.31/pyscroll.egg-info/PKG-INFO
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)      321 2023-06-12 21:31:35.000000 pyscroll-2.31/pyscroll.egg-info/SOURCES.txt
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)        1 2023-06-12 21:31:35.000000 pyscroll-2.31/pyscroll.egg-info/dependency_links.txt
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)        9 2023-06-12 21:31:35.000000 pyscroll-2.31/pyscroll.egg-info/top_level.txt
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)       79 2023-06-12 21:31:35.943925 pyscroll-2.31/setup.cfg
+-rw-r--r--   0 ltheden   (1000) ltheden   (1000)     1202 2023-06-12 21:30:50.000000 pyscroll-2.31/setup.py
```

### Comparing `pyscroll-2.30/PKG-INFO` & `pyscroll-2.31/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: pyscroll
-Version: 2.30
+Version: 2.31
 Summary: Fast scrolling maps library for pygame
 Home-page: https://github.com/bitcraft/pyscroll
 Author: bitcraft
 Author-email: leif.theden@gmail.com
 License: LGPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries :: pygame
 
 see readme.md
-
```

### Comparing `pyscroll-2.30/README.md` & `pyscroll-2.31/README.md`

 * *Files identical despite different names*

### Comparing `pyscroll-2.30/pyscroll/animation.py` & `pyscroll-2.31/pyscroll/animation.py`

 * *Files identical despite different names*

### Comparing `pyscroll-2.30/pyscroll/common.py` & `pyscroll-2.31/pyscroll/common.py`

 * *Files identical despite different names*

### Comparing `pyscroll-2.30/pyscroll/data.py` & `pyscroll-2.31/pyscroll/data.py`

 * *Files identical despite different names*

### Comparing `pyscroll-2.30/pyscroll/group.py` & `pyscroll-2.31/pyscroll/group.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,23 +55,24 @@
 
         Args:
             surface: Surface to draw to
 
         """
         ox, oy = self._map_layer.get_center_offset()
         draw_area = surface.get_rect()
+        view_rect = self.view
 
         new_surfaces = list()
         spritedict = self.spritedict
         gl = self.get_layer_of_sprite
         new_surfaces_append = new_surfaces.append
 
         for spr in self.sprites():
             new_rect = spr.rect.move(ox, oy)
-            if new_rect.colliderect(draw_area):
+            if spr.rect.colliderect(view_rect):
                 try:
                     new_surfaces_append((spr.image, new_rect, gl(spr), spr.blendmode))
                 except AttributeError:
                     # should only fail when no blendmode available
                     new_surfaces_append((spr.image, new_rect, gl(spr)))
                 spritedict[spr] = new_rect
```

### Comparing `pyscroll-2.30/pyscroll/isometric.py` & `pyscroll-2.31/pyscroll/isometric.py`

 * *Files identical despite different names*

### Comparing `pyscroll-2.30/pyscroll/orthographic.py` & `pyscroll-2.31/pyscroll/orthographic.py`

 * *Files identical despite different names*

### Comparing `pyscroll-2.30/pyscroll/quadtree.py` & `pyscroll-2.31/pyscroll/quadtree.py`

 * *Files identical despite different names*

### Comparing `pyscroll-2.30/pyscroll.egg-info/PKG-INFO` & `pyscroll-2.31/pyscroll.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: pyscroll
-Version: 2.30
+Version: 2.31
 Summary: Fast scrolling maps library for pygame
 Home-page: https://github.com/bitcraft/pyscroll
 Author: bitcraft
 Author-email: leif.theden@gmail.com
 License: LGPLv3
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Software Development :: Libraries :: pygame
 
 see readme.md
-
```

### Comparing `pyscroll-2.30/setup.py` & `pyscroll-2.31/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 # pip install wheel twine
 # python3 setup.py sdist bdist_wheel
 # python3 -m twine upload --repository pypi dist/*
 from setuptools import setup
 
 setup(
     name="pyscroll",
-    version="2.30",
+    version="2.31",
     description="Fast scrolling maps library for pygame",
     author="bitcraft",
     author_email="leif.theden@gmail.com",
     url="https://github.com/bitcraft/pyscroll",
     packages=["pyscroll"],
-    install_requires=["pygame"],
     license="LGPLv3",
     long_description="see readme.md",
     package_data={"pyscroll": ["license.txt", "readme.md"]},
     classifiers=[
         "Intended Audience :: Developers",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
```

