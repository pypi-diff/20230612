# Comparing `tmp/notionizer-0.0.5.tar.gz` & `tmp/notionizer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionizer-0.0.5.tar", last modified: Sun Jun 11 23:57:40 2023, max compression
+gzip compressed data, was "notionizer-0.0.6.tar", last modified: Mon Jun 12 00:16:08 2023, max compression
```

## Comparing `notionizer-0.0.5.tar` & `notionizer-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-06-11 23:57:40.371324 notionizer-0.0.5/PKG-INFO
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      368 2022-06-22 11:05:47.000000 notionizer-0.0.5/README.md
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/notionizer/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      732 2023-02-17 11:30:57.000000 notionizer-0.0.5/notionizer/__init__.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2153 2023-02-09 05:51:58.000000 notionizer-0.0.5/notionizer/enum.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      371 2023-05-16 10:10:19.000000 notionizer-0.0.5/notionizer/exception.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1799 2023-05-22 15:08:10.000000 notionizer-0.0.5/notionizer/functions.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3901 2023-05-22 22:50:26.000000 notionizer-0.0.5/notionizer/http_request.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4034 2023-05-15 08:29:49.000000 notionizer-0.0.5/notionizer/notion.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     9289 2023-02-15 01:34:21.000000 notionizer-0.0.5/notionizer/object_adt.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     7654 2023-05-22 10:04:46.000000 notionizer-0.0.5/notionizer/object_basic.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2380 2023-02-27 08:22:48.000000 notionizer-0.0.5/notionizer/object_block.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    17656 2023-05-22 21:42:21.000000 notionizer-0.0.5/notionizer/object_database.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     5048 2023-05-24 03:33:53.000000 notionizer-0.0.5/notionizer/object_page.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1643 2023-05-24 03:34:20.000000 notionizer-0.0.5/notionizer/object_user.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     6805 2023-05-22 23:24:23.000000 notionizer-0.0.5/notionizer/properties_basic.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4155 2023-05-22 11:31:36.000000 notionizer-0.0.5/notionizer/properties_db.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     5144 2023-05-22 23:23:28.000000 notionizer-0.0.5/notionizer/properties_page.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4530 2023-05-22 09:59:24.000000 notionizer-0.0.5/notionizer/properties_property.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    42595 2023-04-24 07:29:16.000000 notionizer-0.0.5/notionizer/query.py
--rw-r--r--   0 sungyo    (1000) sungyo    (1000)      126 2023-02-27 08:38:48.000000 notionizer-0.0.5/notionizer/settings.py
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/notionizer.egg-info/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/PKG-INFO
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      855 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/SOURCES.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        1 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/dependency_links.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        9 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/requires.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       16 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/top_level.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       38 2023-06-11 23:57:40.371324 notionizer-0.0.5/setup.cfg
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      993 2023-06-11 23:57:32.000000 notionizer-0.0.5/setup.py
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/test/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        0 2022-06-14 09:15:51.000000 notionizer-0.0.5/test/__init__.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1986 2023-02-21 05:40:06.000000 notionizer-0.0.5/test/test_block.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      639 2023-04-21 11:11:36.000000 notionizer-0.0.5/test/test_notion.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4912 2023-02-09 07:32:20.000000 notionizer-0.0.5/test/test_notion1.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      398 2023-02-21 12:44:32.000000 notionizer-0.0.5/test/test_notion_getdatabase.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2647 2023-02-21 07:46:13.000000 notionizer-0.0.5/test/test_object_database.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2596 2023-02-27 08:22:48.000000 notionizer-0.0.5/test/test_object_page.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      169 2023-02-15 02:03:42.000000 notionizer-0.0.5/test/test_objects.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    14244 2023-02-13 05:30:10.000000 notionizer-0.0.5/test/test_query.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-12 00:16:08.004386 notionizer-0.0.6/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-06-12 00:16:08.004386 notionizer-0.0.6/PKG-INFO
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      368 2022-06-22 11:05:47.000000 notionizer-0.0.6/README.md
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-12 00:16:08.004386 notionizer-0.0.6/notionizer/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      732 2023-02-17 11:30:57.000000 notionizer-0.0.6/notionizer/__init__.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2153 2023-02-09 05:51:58.000000 notionizer-0.0.6/notionizer/enum.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      371 2023-05-16 10:10:19.000000 notionizer-0.0.6/notionizer/exception.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1799 2023-05-22 15:08:10.000000 notionizer-0.0.6/notionizer/functions.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3901 2023-05-22 22:50:26.000000 notionizer-0.0.6/notionizer/http_request.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4034 2023-05-15 08:29:49.000000 notionizer-0.0.6/notionizer/notion.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     9289 2023-02-15 01:34:21.000000 notionizer-0.0.6/notionizer/object_adt.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     7654 2023-05-22 10:04:46.000000 notionizer-0.0.6/notionizer/object_basic.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2380 2023-02-27 08:22:48.000000 notionizer-0.0.6/notionizer/object_block.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    17656 2023-05-22 21:42:21.000000 notionizer-0.0.6/notionizer/object_database.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     5048 2023-05-24 03:33:53.000000 notionizer-0.0.6/notionizer/object_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1643 2023-05-24 03:34:20.000000 notionizer-0.0.6/notionizer/object_user.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     6805 2023-05-22 23:24:23.000000 notionizer-0.0.6/notionizer/properties_basic.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4155 2023-06-12 00:12:33.000000 notionizer-0.0.6/notionizer/properties_db.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     5144 2023-06-12 00:12:33.000000 notionizer-0.0.6/notionizer/properties_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4530 2023-05-22 09:59:24.000000 notionizer-0.0.6/notionizer/properties_property.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    42595 2023-04-24 07:29:16.000000 notionizer-0.0.6/notionizer/query.py
+-rw-r--r--   0 sungyo    (1000) sungyo    (1000)      126 2023-02-27 08:38:48.000000 notionizer-0.0.6/notionizer/settings.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-12 00:16:08.004386 notionizer-0.0.6/notionizer.egg-info/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-06-12 00:16:07.000000 notionizer-0.0.6/notionizer.egg-info/PKG-INFO
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      855 2023-06-12 00:16:07.000000 notionizer-0.0.6/notionizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        1 2023-06-12 00:16:07.000000 notionizer-0.0.6/notionizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        9 2023-06-12 00:16:07.000000 notionizer-0.0.6/notionizer.egg-info/requires.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       16 2023-06-12 00:16:07.000000 notionizer-0.0.6/notionizer.egg-info/top_level.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       38 2023-06-12 00:16:08.004386 notionizer-0.0.6/setup.cfg
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      994 2023-06-12 00:15:51.000000 notionizer-0.0.6/setup.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-12 00:16:08.004386 notionizer-0.0.6/test/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        0 2022-06-14 09:15:51.000000 notionizer-0.0.6/test/__init__.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1986 2023-02-21 05:40:06.000000 notionizer-0.0.6/test/test_block.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      639 2023-04-21 11:11:36.000000 notionizer-0.0.6/test/test_notion.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4912 2023-02-09 07:32:20.000000 notionizer-0.0.6/test/test_notion1.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      398 2023-02-21 12:44:32.000000 notionizer-0.0.6/test/test_notion_getdatabase.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2647 2023-02-21 07:46:13.000000 notionizer-0.0.6/test/test_object_database.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2596 2023-02-27 08:22:48.000000 notionizer-0.0.6/test/test_object_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      169 2023-02-15 02:03:42.000000 notionizer-0.0.6/test/test_objects.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    14244 2023-02-13 05:30:10.000000 notionizer-0.0.6/test/test_query.py
```

### Comparing `notionizer-0.0.5/PKG-INFO` & `notionizer-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionizer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python wrapper for Notion API
 Home-page: https://github.com/kimsg1984/notionizer
 Author: SeonGyo Kim
 Author-email: kimsg1984@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `notionizer-0.0.5/notionizer/__init__.py` & `notionizer-0.0.6/notionizer/__init__.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/enum.py` & `notionizer-0.0.6/notionizer/enum.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/functions.py` & `notionizer-0.0.6/notionizer/functions.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/http_request.py` & `notionizer-0.0.6/notionizer/http_request.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/notion.py` & `notionizer-0.0.6/notionizer/notion.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/object_adt.py` & `notionizer-0.0.6/notionizer/object_adt.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/object_basic.py` & `notionizer-0.0.6/notionizer/object_basic.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/object_block.py` & `notionizer-0.0.6/notionizer/object_block.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/object_database.py` & `notionizer-0.0.6/notionizer/object_database.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/object_page.py` & `notionizer-0.0.6/notionizer/object_page.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/object_user.py` & `notionizer-0.0.6/notionizer/object_user.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/properties_basic.py` & `notionizer-0.0.6/notionizer/properties_basic.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/properties_db.py` & `notionizer-0.0.6/notionizer/properties_db.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/properties_page.py` & `notionizer-0.0.6/notionizer/properties_page.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/properties_property.py` & `notionizer-0.0.6/notionizer/properties_property.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer/query.py` & `notionizer-0.0.6/notionizer/query.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/notionizer.egg-info/PKG-INFO` & `notionizer-0.0.6/notionizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionizer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python wrapper for Notion API
 Home-page: https://github.com/kimsg1984/notionizer
 Author: SeonGyo Kim
 Author-email: kimsg1984@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `notionizer-0.0.5/notionizer.egg-info/SOURCES.txt` & `notionizer-0.0.6/notionizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/setup.py` & `notionizer-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 reqs = parse_requirements("requirements.txt", session=False)
 install_requires = [str(ir.requirement) for ir in reqs]
 
 setuptools.setup(
     name="notionizer",
-    version="0.0.5",
+    version="0.0.6 ",
     author="SeonGyo Kim",
     author_email="kimsg1984@gmail.com",
     description="Python wrapper for Notion API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimsg1984/notionizer",
     install_requires=install_requires,
```

### Comparing `notionizer-0.0.5/test/test_block.py` & `notionizer-0.0.6/test/test_block.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/test/test_notion.py` & `notionizer-0.0.6/test/test_notion.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/test/test_notion1.py` & `notionizer-0.0.6/test/test_notion1.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/test/test_object_database.py` & `notionizer-0.0.6/test/test_object_database.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/test/test_object_page.py` & `notionizer-0.0.6/test/test_object_page.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.5/test/test_query.py` & `notionizer-0.0.6/test/test_query.py`

 * *Files identical despite different names*

