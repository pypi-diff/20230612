# Comparing `tmp/models-files-manager-1.0.1.tar.gz` & `tmp/models-files-manager-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "models-files-manager-1.0.1.tar", last modified: Sun Apr 30 20:17:38 2023, max compression
+gzip compressed data, was "models-files-manager-1.0.2.tar", last modified: Mon Jun 12 19:57:36 2023, max compression
```

## Comparing `models-files-manager-1.0.1.tar` & `models-files-manager-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-04-30 20:17:38.190002 models-files-manager-1.0.1/
--rw-r--r--   0 ramnathaniel   (501) staff       (20)     1070 2023-04-30 19:46:03.000000 models-files-manager-1.0.1/LICENSE
--rw-r--r--   0 ramnathaniel   (501) staff       (20)     3741 2023-04-30 20:17:38.189846 models-files-manager-1.0.1/PKG-INFO
--rw-r--r--   0 ramnathaniel   (501) staff       (20)     1859 2023-04-30 19:46:03.000000 models-files-manager-1.0.1/README.md
-drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-04-30 20:17:38.188663 models-files-manager-1.0.1/models_files_manager/
--rw-r--r--   0 ramnathaniel   (501) staff       (20)       76 2023-04-30 19:46:03.000000 models-files-manager-1.0.1/models_files_manager/__init__.py
--rw-r--r--   0 ramnathaniel   (501) staff       (20)     4174 2023-04-30 19:46:03.000000 models-files-manager-1.0.1/models_files_manager/models_files_manager.py
-drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-04-30 20:17:38.189507 models-files-manager-1.0.1/models_files_manager.egg-info/
--rw-r--r--   0 ramnathaniel   (501) staff       (20)     3741 2023-04-30 20:17:38.000000 models-files-manager-1.0.1/models_files_manager.egg-info/PKG-INFO
--rw-r--r--   0 ramnathaniel   (501) staff       (20)      350 2023-04-30 20:17:38.000000 models-files-manager-1.0.1/models_files_manager.egg-info/SOURCES.txt
--rw-r--r--   0 ramnathaniel   (501) staff       (20)        1 2023-04-30 20:17:38.000000 models-files-manager-1.0.1/models_files_manager.egg-info/dependency_links.txt
--rw-r--r--   0 ramnathaniel   (501) staff       (20)       63 2023-04-30 20:17:38.000000 models-files-manager-1.0.1/models_files_manager.egg-info/requires.txt
--rw-r--r--   0 ramnathaniel   (501) staff       (20)       21 2023-04-30 20:17:38.000000 models-files-manager-1.0.1/models_files_manager.egg-info/top_level.txt
--rw-r--r--   0 ramnathaniel   (501) staff       (20)      900 2023-04-30 20:17:21.000000 models-files-manager-1.0.1/pyproject.toml
--rw-r--r--   0 ramnathaniel   (501) staff       (20)       38 2023-04-30 20:17:38.190048 models-files-manager-1.0.1/setup.cfg
-drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-04-30 20:17:38.189644 models-files-manager-1.0.1/test/
--rw-r--r--   0 ramnathaniel   (501) staff       (20)     3556 2023-04-30 19:46:03.000000 models-files-manager-1.0.1/test/test_manager.py
+drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-06-12 19:57:36.073527 models-files-manager-1.0.2/
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)     1070 2023-04-30 19:46:03.000000 models-files-manager-1.0.2/LICENSE
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)     3741 2023-06-12 19:57:36.073278 models-files-manager-1.0.2/PKG-INFO
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)     1859 2023-04-30 19:46:03.000000 models-files-manager-1.0.2/README.md
+drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-06-12 19:57:36.071747 models-files-manager-1.0.2/models_files_manager/
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)       76 2023-06-12 19:32:08.000000 models-files-manager-1.0.2/models_files_manager/__init__.py
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)     4174 2023-06-12 19:28:55.000000 models-files-manager-1.0.2/models_files_manager/models_files_manager.py
+drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-06-12 19:57:36.072440 models-files-manager-1.0.2/models_files_manager.egg-info/
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)     3741 2023-06-12 19:57:36.000000 models-files-manager-1.0.2/models_files_manager.egg-info/PKG-INFO
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)      350 2023-06-12 19:57:36.000000 models-files-manager-1.0.2/models_files_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)        1 2023-06-12 19:57:36.000000 models-files-manager-1.0.2/models_files_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)       63 2023-06-12 19:57:36.000000 models-files-manager-1.0.2/models_files_manager.egg-info/requires.txt
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)       21 2023-06-12 19:57:36.000000 models-files-manager-1.0.2/models_files_manager.egg-info/top_level.txt
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)      900 2023-06-12 19:32:41.000000 models-files-manager-1.0.2/pyproject.toml
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)       38 2023-06-12 19:57:36.073608 models-files-manager-1.0.2/setup.cfg
+drwxr-xr-x   0 ramnathaniel   (501) staff       (20)        0 2023-06-12 19:57:36.072597 models-files-manager-1.0.2/test/
+-rw-r--r--   0 ramnathaniel   (501) staff       (20)     3839 2023-06-12 19:31:49.000000 models-files-manager-1.0.2/test/test_manager.py
```

### Comparing `models-files-manager-1.0.1/LICENSE` & `models-files-manager-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `models-files-manager-1.0.1/PKG-INFO` & `models-files-manager-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: models-files-manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: Manage saved models files, encode fields into filenames
 Author-email: Ram Nathaniel <ram.nathaniel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ram Nathaniel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `models-files-manager-1.0.1/README.md` & `models-files-manager-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `models-files-manager-1.0.1/models_files_manager/models_files_manager.py` & `models-files-manager-1.0.2/models_files_manager/models_files_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,18 +70,18 @@
 
         path_parts = path.split('/')
         filename = path_parts[-1][: -len(self._ext)-1]
         parts = filename.split('_')
 
         parts = [self.path_decode(p) for p in parts]
 
-        if len(parts) != len(self._fields):
-            raise Exception(f'Path {path} does not have the same number of fields as {self._fields}')
+        if len(parts) < len(self._fields):
+            raise Exception(f'Path {path} does not have all fields (expecting {self._fields})')
 
-        return {self._fields[i]: parts[i] for i in range(len(parts))}
+        return {self._fields[i]: parts[i] for i in range(len(self._fields))}
 
     def get_file_name(self, fields: dict) -> str:
         """
         Generate a file name from the fields
 
         Args:
             fields (dict): _description_
```

### Comparing `models-files-manager-1.0.1/models_files_manager.egg-info/PKG-INFO` & `models-files-manager-1.0.2/models_files_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: models-files-manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: Manage saved models files, encode fields into filenames
 Author-email: Ram Nathaniel <ram.nathaniel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ram Nathaniel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `models-files-manager-1.0.1/pyproject.toml` & `models-files-manager-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "models-files-manager"
-version = "1.0.1"
+version = "1.0.2"
 description = "Manage saved models files, encode fields into filenames"
 readme = "README.md"
 authors = [{ name = "Ram Nathaniel", email = "ram.nathaniel@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `models-files-manager-1.0.1/test/test_manager.py` & `models-files-manager-1.0.2/test/test_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,22 @@
     fields = manager.get_fields_values('root_folder/value1_value2.ext')
 
     assert fields is not None
     assert len(fields) == 2
     assert fields['field1'] == 'value1'
     assert fields['field2'] == 'value2'
 
+    # test with more fields in name than manager - take first 2
+    fields = manager.get_fields_values('root_folder/value1_value2_value3.ext')
+
+    assert fields is not None
+    assert len(fields) == 2
+    assert fields['field1'] == 'value1'
+    assert fields['field2'] == 'value2'
+
 def test_get_file_name():
     manager = ModelsFilesManager('root_folder', ['field1', 'field2'], 'ext')
     file_name = manager.get_file_name({'field1': 'value1', 'field2': 'value2'})
 
     assert file_name is not None
     assert file_name == 'value1_value2.ext'
```

