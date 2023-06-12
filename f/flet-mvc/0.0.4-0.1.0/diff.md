# Comparing `tmp/flet-mvc-0.0.4.tar.gz` & `tmp/flet-mvc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-mvc-0.0.4.tar", last modified: Thu Jan 12 08:41:25 2023, max compression
+gzip compressed data, was "flet-mvc-0.1.0.tar", last modified: Mon Jun 12 05:19:44 2023, max compression
```

## Comparing `flet-mvc-0.0.4.tar` & `flet-mvc-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Charlie    (501) staff       (20)        0 2023-01-12 08:41:25.820862 flet-mvc-0.0.4/
--rw-r--r--   0 Charlie    (501) staff       (20)     1083 2023-01-10 05:17:53.000000 flet-mvc-0.0.4/LICENSE
--rw-r--r--   0 Charlie    (501) staff       (20)    13377 2023-01-12 08:41:25.820548 flet-mvc-0.0.4/PKG-INFO
--rw-r--r--   0 Charlie    (501) staff       (20)    12670 2023-01-12 08:33:22.000000 flet-mvc-0.0.4/README.md
-drwxr-xr-x   0 Charlie    (501) staff       (20)        0 2023-01-12 08:41:25.818897 flet-mvc-0.0.4/flet_mvc/
--rw-r--r--   0 Charlie    (501) staff       (20)      125 2023-01-10 08:32:38.000000 flet-mvc-0.0.4/flet_mvc/__init__.py
--rw-r--r--   0 Charlie    (501) staff       (20)      112 2023-01-10 08:43:26.000000 flet-mvc-0.0.4/flet_mvc/alert.py
--rw-r--r--   0 Charlie    (501) staff       (20)     2728 2023-01-10 08:43:53.000000 flet-mvc-0.0.4/flet_mvc/controller.py
--rw-r--r--   0 Charlie    (501) staff       (20)     3281 2023-01-10 01:46:18.000000 flet-mvc-0.0.4/flet_mvc/model.py
--rw-r--r--   0 Charlie    (501) staff       (20)      268 2023-01-09 20:09:31.000000 flet-mvc-0.0.4/flet_mvc/view.py
-drwxr-xr-x   0 Charlie    (501) staff       (20)        0 2023-01-12 08:41:25.820156 flet-mvc-0.0.4/flet_mvc.egg-info/
--rw-r--r--   0 Charlie    (501) staff       (20)    13377 2023-01-12 08:41:25.000000 flet-mvc-0.0.4/flet_mvc.egg-info/PKG-INFO
--rw-r--r--   0 Charlie    (501) staff       (20)      282 2023-01-12 08:41:25.000000 flet-mvc-0.0.4/flet_mvc.egg-info/SOURCES.txt
--rw-r--r--   0 Charlie    (501) staff       (20)        1 2023-01-12 08:41:25.000000 flet-mvc-0.0.4/flet_mvc.egg-info/dependency_links.txt
--rw-r--r--   0 Charlie    (501) staff       (20)        5 2023-01-12 08:41:25.000000 flet-mvc-0.0.4/flet_mvc.egg-info/requires.txt
--rw-r--r--   0 Charlie    (501) staff       (20)        9 2023-01-12 08:41:25.000000 flet-mvc-0.0.4/flet_mvc.egg-info/top_level.txt
--rw-r--r--   0 Charlie    (501) staff       (20)       38 2023-01-12 08:41:25.820996 flet-mvc-0.0.4/setup.cfg
--rw-r--r--   0 Charlie    (501) staff       (20)     1055 2023-01-12 08:41:16.000000 flet-mvc-0.0.4/setup.py
+drwxr-xr-x   0 Charlie    (501) staff       (20)        0 2023-06-12 05:19:44.595978 flet-mvc-0.1.0/
+-rw-r--r--   0 Charlie    (501) staff       (20)     1083 2023-01-10 05:17:53.000000 flet-mvc-0.1.0/LICENSE
+-rw-r--r--   0 Charlie    (501) staff       (20)    32785 2023-06-12 05:19:44.595822 flet-mvc-0.1.0/PKG-INFO
+-rw-r--r--   0 Charlie    (501) staff       (20)    32115 2023-06-12 05:07:43.000000 flet-mvc-0.1.0/README.md
+drwxr-xr-x   0 Charlie    (501) staff       (20)        0 2023-06-12 05:19:44.594813 flet-mvc-0.1.0/flet_mvc/
+-rw-r--r--   0 Charlie    (501) staff       (20)      125 2023-02-06 07:36:29.000000 flet-mvc-0.1.0/flet_mvc/__init__.py
+-rw-r--r--   0 Charlie    (501) staff       (20)      113 2023-06-11 21:34:25.000000 flet-mvc-0.1.0/flet_mvc/alert.py
+-rw-r--r--   0 Charlie    (501) staff       (20)     2685 2023-06-11 21:34:29.000000 flet-mvc-0.1.0/flet_mvc/controller.py
+-rw-r--r--   0 Charlie    (501) staff       (20)    11458 2023-06-12 02:35:05.000000 flet-mvc-0.1.0/flet_mvc/model.py
+-rw-r--r--   0 Charlie    (501) staff       (20)      559 2023-06-11 21:34:35.000000 flet-mvc-0.1.0/flet_mvc/view.py
+drwxr-xr-x   0 Charlie    (501) staff       (20)        0 2023-06-12 05:19:44.595561 flet-mvc-0.1.0/flet_mvc.egg-info/
+-rw-r--r--   0 Charlie    (501) staff       (20)    32785 2023-06-12 05:19:44.000000 flet-mvc-0.1.0/flet_mvc.egg-info/PKG-INFO
+-rw-r--r--   0 Charlie    (501) staff       (20)      282 2023-06-12 05:19:44.000000 flet-mvc-0.1.0/flet_mvc.egg-info/SOURCES.txt
+-rw-r--r--   0 Charlie    (501) staff       (20)        1 2023-06-12 05:19:44.000000 flet-mvc-0.1.0/flet_mvc.egg-info/dependency_links.txt
+-rw-r--r--   0 Charlie    (501) staff       (20)        5 2023-06-12 05:19:44.000000 flet-mvc-0.1.0/flet_mvc.egg-info/requires.txt
+-rw-r--r--   0 Charlie    (501) staff       (20)        9 2023-06-12 05:19:44.000000 flet-mvc-0.1.0/flet_mvc.egg-info/top_level.txt
+-rw-r--r--   0 Charlie    (501) staff       (20)       38 2023-06-12 05:19:44.596018 flet-mvc-0.1.0/setup.cfg
+-rw-r--r--   0 Charlie    (501) staff       (20)     1055 2023-06-05 06:01:02.000000 flet-mvc-0.1.0/setup.py
```

### Comparing `flet-mvc-0.0.4/LICENSE` & `flet-mvc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-mvc-0.0.4/flet_mvc/controller.py` & `flet-mvc-0.1.0/flet_mvc/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 """
 Flet Base Controller Class
 """
 
+from typing import Type
 import flet as ft
 from .alert import ERROR, WARNING, SUCCESS, ADVICE, INFO
+from .model import FletModel
 
-class FletController():
-    def __init__(self, page: ft.Page, model):
+
+class FletController:
+    def __init__(self, page: ft.Page, model: Type[FletModel]):
         self.page = page
         self.model = model
-        
+
     def update(self):
-        """ Updates the page by using self.update() instead of self.page.update() """
+        """Updates the page by using self.update() instead of self.page.update()"""
         self.page.update()
 
-        
-    def alert(self, msg="" , alert_type=ERROR):
-        """ Show Alert """
+    def alert(self, msg="", alert_type=ERROR):
+        """Show Alert"""
         if alert_type == ERROR:
             self.page.snack_bar = ft.SnackBar(
                 content=ft.Row(
                     controls=[
                         ft.Icon(ft.icons.ERROR_OUTLINE, color=ft.colors.WHITE),
                         ft.Text(msg),
                     ],
                 ),
                 bgcolor=ft.colors.ERROR,
             )
             self.page.snack_bar.open = True
             self.update()
-            
+
         elif alert_type == SUCCESS:
             self.page.snack_bar = ft.SnackBar(
                 content=ft.Row(
                     controls=[
                         ft.Icon(ft.icons.CHECK_CIRCLE, color=ft.colors.WHITE),
                         ft.Text(msg),
                     ],
                 ),
                 action="OK",
                 action_color=ft.colors.BLACK,
                 bgcolor=ft.colors.GREEN_300,
             )
             self.page.snack_bar.open = True
             self.update()
-            
+
         elif alert_type == ADVICE:
             self.page.snack_bar = ft.SnackBar(
-                    content=ft.Text(msg),
-                    action="Understood",
-                    action_color=ft.colors.BLUE_200
-                )
+                content=ft.Text(msg),
+                action="Understood",
+                action_color=ft.colors.BLUE_200,
+            )
             self.page.snack_bar.open = True
             self.update()
-            
+
         elif alert_type == INFO:
             self.page.snack_bar = ft.SnackBar(
-                    content=ft.Row(
-                        controls=[
-                            ft.Icon(ft.icons.INFO_OUTLINED, color=ft.colors.WHITE),
-                            ft.Text(msg),
-                        ],
-                    ),
-                    bgcolor=ft.colors.BLUE_200
+                content=ft.Row(
+                    controls=[
+                        ft.Icon(ft.icons.INFO_OUTLINED, color=ft.colors.WHITE),
+                        ft.Text(msg),
+                    ],
+                ),
+                bgcolor=ft.colors.BLUE_200,
             )
             self.page.snack_bar.open = True
             self.update()
-            
+
         elif alert_type == WARNING:
             self.page.snack_bar = ft.SnackBar(
                 content=ft.Row(
                     controls=[
                         ft.Icon(ft.icons.WARNING_AMBER_ROUNDED, color=ft.colors.WHITE),
                         ft.Text(msg),
                     ],
```

### Comparing `flet-mvc-0.0.4/setup.py` & `flet-mvc-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.4'
+VERSION = '0.1.0'
 DESCRIPTION = 'This package will allow the developer to use an mvc structure in a Flet project.'
 
 # Setting up
 setup(
     name="flet-mvc",
     version=VERSION,
     author="o0Adrian (C. Adrián Monroy)",
```

