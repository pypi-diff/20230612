# Comparing `tmp/pyquet-0.1.5.tar.gz` & `tmp/pyquet-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\github\pyquet\dist\.tmp-hkftgdl7\pyquet-0.1.5.tar", last modified: Wed May 31 10:35:12 2023, max compression
+gzip compressed data, was "pyquet-0.1.6.tar", last modified: Mon Jun 12 20:39:08 2023, max compression
```

## Comparing `pyquet-0.1.5.tar` & `pyquet-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 10:35:12.000000 pyquet-0.1.5/
--rw-rw-rw-   0        0        0     1086 2023-05-30 07:37:22.000000 pyquet-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      546 2023-05-31 10:35:12.000000 pyquet-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-05-30 07:37:22.000000 pyquet-0.1.5/README.md
--rw-rw-rw-   0        0        0      104 2023-05-30 07:42:55.000000 pyquet-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      674 2023-05-31 10:35:12.000000 pyquet-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/pyquet/
--rw-rw-rw-   0        0        0        0 2023-05-30 08:16:35.000000 pyquet-0.1.5/src/pyquet/__init__.py
--rw-rw-rw-   0        0        0      628 2023-05-30 07:38:36.000000 pyquet-0.1.5/src/pyquet/common.py
--rw-rw-rw-   0        0        0     6584 2023-05-31 10:34:28.000000 pyquet-0.1.5/src/pyquet/generator.py
--rw-rw-rw-   0        0        0     2176 2023-05-30 08:18:01.000000 pyquet-0.1.5/src/pyquet/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/pyquet.egg-info/
--rw-rw-rw-   0        0        0      546 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/pyquet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/pyquet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/pyquet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/pyquet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 10:35:12.000000 pyquet-0.1.5/src/pyquet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 10:35:12.000000 pyquet-0.1.5/tests/
--rw-rw-rw-   0        0        0     2078 2023-05-30 08:17:11.000000 pyquet-0.1.5/tests/test_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.136924 pyquet-0.1.6/
+-rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      546 2023-06-12 20:39:08.136924 pyquet-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.1.6/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-11 07:58:49.000000 pyquet-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      674 2023-06-12 20:39:08.140913 pyquet-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.120416 pyquet-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.126906 pyquet-0.1.6/src/pyquet/
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.1.6/src/pyquet/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-06-12 19:39:16.000000 pyquet-0.1.6/src/pyquet/common.py
+-rw-rw-rw-   0        0        0     1867 2023-06-11 09:50:23.000000 pyquet-0.1.6/src/pyquet/editor.py
+-rw-rw-rw-   0        0        0     3088 2023-06-12 20:32:51.000000 pyquet-0.1.6/src/pyquet/editor_ui.py
+-rw-rw-rw-   0        0        0     6599 2023-06-11 09:50:23.000000 pyquet-0.1.6/src/pyquet/generator.py
+-rw-rw-rw-   0        0        0     2176 2023-05-27 09:33:39.000000 pyquet-0.1.6/src/pyquet/schemas.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.135927 pyquet-0.1.6/src/pyquet.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 20:39:08.000000 pyquet-0.1.6/src/pyquet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 20:39:08.135927 pyquet-0.1.6/tests/
+-rw-rw-rw-   0        0        0     2078 2023-05-27 09:31:42.000000 pyquet-0.1.6/tests/test_reader.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyquet-0.1.5/LICENSE` & `pyquet-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.5/PKG-INFO` & `pyquet-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.5
+Version: 0.1.6
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.5/setup.cfg` & `pyquet-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7971 7565 740d 0a76 6572 7369   = pyquet..versi
-00000020: 6f6e 203d 2030 2e31 2e35 0d0a 6175 7468  on = 0.1.5..auth
+00000020: 6f6e 203d 2030 2e31 2e36 0d0a 6175 7468  on = 0.1.6..auth
 00000030: 6f72 203d 2052 6963 6172 646f 204d 7567  or = Ricardo Mug
 00000040: 6963 610d 0a61 7574 686f 725f 656d 6169  ica..author_emai
 00000050: 6c20 3d20 726d 7567 6963 6167 4067 6d61  l = rmugicag@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5465 7874 2063 6f6d 7061  ion = Text compa
 00000080: 7261 746f 7220 5549 0d0a 6c6f 6e67 5f64  rator UI..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `pyquet-0.1.5/src/pyquet/common.py` & `pyquet-0.1.6/src/pyquet/common.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.5/src/pyquet/generator.py` & `pyquet-0.1.6/src/pyquet/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if os.path.isfile(destination_path):
             os.remove(destination_path)
         df = pd.DataFrame(data)
         table = pa.Table.from_pandas(df)
         target_schema = pa.schema(pa.schema(field_format))
         table = table.cast(target_schema)
         pq.write_to_dataset(table, destination_path, partition_cols=partitions)
-        return destination_path
+        return destination_path, target_schema
 
     def generate_alphanumeric(self, name, size=1):
         alphanumeric_list = []
         for counter in range(self.min_rows):
             if name in self.catalog:
                 value = self.catalog[name][counter % len(self.catalog[name])]
             else:
```

### Comparing `pyquet-0.1.5/src/pyquet/schemas.py` & `pyquet-0.1.6/src/pyquet/schemas.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.5/src/pyquet.egg-info/PKG-INFO` & `pyquet-0.1.6/src/pyquet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.5
+Version: 0.1.6
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.5/tests/test_reader.py` & `pyquet-0.1.6/tests/test_reader.py`

 * *Files identical despite different names*

