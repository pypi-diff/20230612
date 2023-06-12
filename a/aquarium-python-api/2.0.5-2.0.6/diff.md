# Comparing `tmp/aquarium-python-api-2.0.5.tar.gz` & `tmp/aquarium-python-api-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-2.0.5.tar", last modified: Wed Jun  7 07:24:04 2023, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.0.6.tar", last modified: Mon Jun 12 16:10:51 2023, max compression
```

## Comparing `aquarium-python-api-2.0.5.tar` & `aquarium-python-api-2.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-07 07:24:04.374192 aquarium-python-api-2.0.5/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.5/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-07 07:24:04.374571 aquarium-python-api-2.0.5/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.5/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-07 07:24:04.345426 aquarium-python-api-2.0.5/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.5/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)    12505 2023-06-05 10:02:50.000000 aquarium-python-api-2.0.5/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.5/aquarium/auth.py
--rw-r--r--   0 yann       (501) staff       (20)     3541 2023-06-06 16:57:13.000000 aquarium-python-api-2.0.5/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.5/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.5/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.5/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    27588 2023-06-06 16:56:50.000000 aquarium-python-api-2.0.5/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-07 07:24:04.367453 aquarium-python-api-2.0.5/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.5/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.5/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     5068 2023-06-05 10:10:16.000000 aquarium-python-api-2.0.5/aquarium/items/organisation.py
--rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.5/aquarium/items/playlist.py
--rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.5/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.5/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.5/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.5/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     4345 2023-06-05 10:38:49.000000 aquarium-python-api-2.0.5/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.0.5/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.5/aquarium/tools.py
--rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.5/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-07 07:24:04.373467 aquarium-python-api-2.0.5/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-07 07:24:03.000000 aquarium-python-api-2.0.5/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-07 07:24:03.000000 aquarium-python-api-2.0.5/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-07 07:24:03.000000 aquarium-python-api-2.0.5/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-07 07:24:03.000000 aquarium-python-api-2.0.5/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-07 07:24:03.000000 aquarium-python-api-2.0.5/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-07 07:24:04.375763 aquarium-python-api-2.0.5/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.5/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.116188 aquarium-python-api-2.0.6/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.6/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-12 16:10:51.116544 aquarium-python-api-2.0.6/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.6/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.089125 aquarium-python-api-2.0.6/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.0.6/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    12505 2023-06-05 10:02:50.000000 aquarium-python-api-2.0.6/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.0.6/aquarium/auth.py
+-rw-r--r--   0 yann       (501) staff       (20)     3541 2023-06-06 16:57:13.000000 aquarium-python-api-2.0.6/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.6/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.6/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.6/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    27598 2023-06-12 15:25:14.000000 aquarium-python-api-2.0.6/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.110702 aquarium-python-api-2.0.6/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.6/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.6/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     5068 2023-06-05 10:10:16.000000 aquarium-python-api-2.0.6/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.6/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.6/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.6/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.6/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.6/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     4345 2023-06-05 10:38:49.000000 aquarium-python-api-2.0.6/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.0.6/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.6/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.6/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-12 16:10:51.115712 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      703 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-12 16:10:49.000000 aquarium-python-api-2.0.6/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-12 16:10:51.118658 aquarium-python-api-2.0.6/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.6/setup.py
```

### Comparing `aquarium-python-api-2.0.5/LICENSE.md` & `aquarium-python-api-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/PKG-INFO` & `aquarium-python-api-2.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.5
+Version: 2.0.6
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.5/README.md` & `aquarium-python-api-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/__init__.py` & `aquarium-python-api-2.0.6/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/aquarium.py` & `aquarium-python-api-2.0.6/aquarium/aquarium.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/edge.py` & `aquarium-python-api-2.0.6/aquarium/edge.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/element.py` & `aquarium-python-api-2.0.6/aquarium/element.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/entity.py` & `aquarium-python-api-2.0.6/aquarium/entity.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/exceptions.py` & `aquarium-python-api-2.0.6/aquarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/item.py` & `aquarium-python-api-2.0.6/aquarium/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,15 +570,15 @@
         Move item to the trash
 
         :returns:   Trashed item
         :rtype:     dictionary
         """
         logger.debug('Trash item %s', self._key)
         result = self.do_request(
-            'POST', 'items/{itemKey}/trash'.format(
+            'DELETE', 'items/{itemKey}/trash'.format(
                 itemKey=self._key
             ))
         result = self.parent.element(result)
         return result
 
     def restore(self):
         """
@@ -603,15 +603,15 @@
             The item will be completely deleted. You can use :func:`~aquarium.item.Item.trash` instead
 
         :returns:   Deleted item object from API
         :rtype:     dictionary
         """
         logger.debug('Delete item %s', self._key)
         result = self.do_request(
-            'DELETE', 'items/'+self._key)
+            'DELETE', 'trashed_items/'+self._key)
         return result
 
     def upload_file(self, path='', data = {}, message = None):
         """
         Upload a file on the item
 
         .. warning::
```

### Comparing `aquarium-python-api-2.0.5/aquarium/items/asset.py` & `aquarium-python-api-2.0.6/aquarium/items/asset.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/items/organisation.py` & `aquarium-python-api-2.0.6/aquarium/items/organisation.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/items/playlist.py` & `aquarium-python-api-2.0.6/aquarium/items/playlist.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/items/project.py` & `aquarium-python-api-2.0.6/aquarium/items/project.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/items/task.py` & `aquarium-python-api-2.0.6/aquarium/items/task.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/items/template.py` & `aquarium-python-api-2.0.6/aquarium/items/template.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/items/user.py` & `aquarium-python-api-2.0.6/aquarium/items/user.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/items/usergroup.py` & `aquarium-python-api-2.0.6/aquarium/items/usergroup.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/tools.py` & `aquarium-python-api-2.0.6/aquarium/tools.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium/utils.py` & `aquarium-python-api-2.0.6/aquarium/utils.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.0.6/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.5
+Version: 2.0.6
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.5/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.0.6/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.5/setup.cfg` & `aquarium-python-api-2.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.fatfish.app/dev/python/index.html
 project_urls = 
 	Documentation = https://docs.fatfish.app/dev/python/index.html
 	Source = https://github.com/fatfish-lab/aquarium-python-api
 	Aquarium = https://fatfi.sh/aquarium
-version = 2.0.5
+version = 2.0.6
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
```

