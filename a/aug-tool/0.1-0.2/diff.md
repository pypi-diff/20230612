# Comparing `tmp/aug_tool-0.1.tar.gz` & `tmp/aug_tool-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug_tool-0.1.tar", last modified: Mon Jun 12 18:14:52 2023, max compression
+gzip compressed data, was "aug_tool-0.2.tar", last modified: Mon Jun 12 18:26:57 2023, max compression
```

## Comparing `aug_tool-0.1.tar` & `aug_tool-0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.888255 aug_tool-0.1/
--rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug_tool-0.1/LICENCE
--rw-rw-rw-   0        0        0       19 2023-06-12 18:12:54.000000 aug_tool-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10113 2023-06-12 18:14:52.889251 aug_tool-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug_tool-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.841410 aug_tool-0.1/icons/
--rw-rw-rw-   0        0        0   126732 2023-06-10 15:04:41.000000 aug_tool-0.1/icons/example2Img.png
--rw-rw-rw-   0        0        0   131854 2023-06-10 15:04:14.000000 aug_tool-0.1/icons/example3.png
--rw-rw-rw-   0        0        0    70097 2023-06-10 15:03:42.000000 aug_tool-0.1/icons/example4.png
--rw-rw-rw-   0        0        0    89216 2023-06-10 15:03:21.000000 aug_tool-0.1/icons/exampleImg.png
--rw-rw-rw-   0        0        0    19425 2023-06-04 13:53:14.000000 aug_tool-0.1/icons/logo.png
--rw-rw-rw-   0        0        0    18151 2023-06-04 13:39:07.000000 aug_tool-0.1/icons/logo2.png
--rw-rw-rw-   0        0        0      108 2023-06-12 18:12:54.000000 aug_tool-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      775 2023-06-12 18:14:52.891245 aug_tool-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.821478 aug_tool-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.845397 aug_tool-0.1/src/aug_tool/
--rw-rw-rw-   0        0        0        0 2023-06-11 19:50:49.000000 aug_tool-0.1/src/aug_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.865332 aug_tool-0.1/src/aug_tool/dataAugmentor/
--rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/annAug.py
--rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/dataAug.py
--rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/imgAug.py
--rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/txtAug.py
--rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/xmlAug.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.876295 aug_tool-0.1/src/aug_tool/dataOpener/
--rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug_tool-0.1/src/aug_tool/dataOpener/__init__.py
--rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug_tool-0.1/src/aug_tool/dataOpener/annOp.py
--rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug_tool-0.1/src/aug_tool/dataOpener/dataOp.py
--rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug_tool-0.1/src/aug_tool/dataOpener/imgOp.py
--rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug_tool-0.1/src/aug_tool/dataOpener/txtOp.py
--rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug_tool-0.1/src/aug_tool/dataOpener/xmlOp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.887257 aug_tool-0.1/src/aug_tool/dataSaver/
--rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug_tool-0.1/src/aug_tool/dataSaver/__init__.py
--rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug_tool-0.1/src/aug_tool/dataSaver/annSav.py
--rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug_tool-0.1/src/aug_tool/dataSaver/dataSav.py
--rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug_tool-0.1/src/aug_tool/dataSaver/imgSav.py
--rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug_tool-0.1/src/aug_tool/dataSaver/txtSav.py
--rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug_tool-0.1/src/aug_tool/dataSaver/xmlSav.py
--rw-rw-rw-   0        0        0     7134 2023-06-11 19:27:26.000000 aug_tool-0.1/src/aug_tool/factory.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.854372 aug_tool-0.1/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0    10113 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1022 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.938805 aug_tool-0.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug_tool-0.2/LICENCE
+-rw-rw-rw-   0        0        0       19 2023-06-12 18:12:54.000000 aug_tool-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    10113 2023-06-12 18:26:57.938805 aug_tool-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug_tool-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.897996 aug_tool-0.2/icons/
+-rw-rw-rw-   0        0        0   126732 2023-06-10 15:04:41.000000 aug_tool-0.2/icons/example2Img.png
+-rw-rw-rw-   0        0        0   131854 2023-06-10 15:04:14.000000 aug_tool-0.2/icons/example3.png
+-rw-rw-rw-   0        0        0    70097 2023-06-10 15:03:42.000000 aug_tool-0.2/icons/example4.png
+-rw-rw-rw-   0        0        0    89216 2023-06-10 15:03:21.000000 aug_tool-0.2/icons/exampleImg.png
+-rw-rw-rw-   0        0        0    19425 2023-06-04 13:53:14.000000 aug_tool-0.2/icons/logo.png
+-rw-rw-rw-   0        0        0    18151 2023-06-04 13:39:07.000000 aug_tool-0.2/icons/logo2.png
+-rw-rw-rw-   0        0        0      108 2023-06-12 18:12:54.000000 aug_tool-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      775 2023-06-12 18:26:57.940797 aug_tool-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.867709 aug_tool-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.900995 aug_tool-0.2/src/aug_tool/
+-rw-rw-rw-   0        0        0      119 2023-06-11 18:59:24.000000 aug_tool-0.2/src/aug_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.917873 aug_tool-0.2/src/aug_tool/dataAugmentor/
+-rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug_tool-0.2/src/aug_tool/dataAugmentor/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug_tool-0.2/src/aug_tool/dataAugmentor/annAug.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug_tool-0.2/src/aug_tool/dataAugmentor/dataAug.py
+-rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug_tool-0.2/src/aug_tool/dataAugmentor/imgAug.py
+-rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug_tool-0.2/src/aug_tool/dataAugmentor/txtAug.py
+-rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug_tool-0.2/src/aug_tool/dataAugmentor/xmlAug.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.927835 aug_tool-0.2/src/aug_tool/dataOpener/
+-rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug_tool-0.2/src/aug_tool/dataOpener/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug_tool-0.2/src/aug_tool/dataOpener/annOp.py
+-rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug_tool-0.2/src/aug_tool/dataOpener/dataOp.py
+-rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug_tool-0.2/src/aug_tool/dataOpener/imgOp.py
+-rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug_tool-0.2/src/aug_tool/dataOpener/txtOp.py
+-rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug_tool-0.2/src/aug_tool/dataOpener/xmlOp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.936805 aug_tool-0.2/src/aug_tool/dataSaver/
+-rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug_tool-0.2/src/aug_tool/dataSaver/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug_tool-0.2/src/aug_tool/dataSaver/annSav.py
+-rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug_tool-0.2/src/aug_tool/dataSaver/dataSav.py
+-rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug_tool-0.2/src/aug_tool/dataSaver/imgSav.py
+-rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug_tool-0.2/src/aug_tool/dataSaver/txtSav.py
+-rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug_tool-0.2/src/aug_tool/dataSaver/xmlSav.py
+-rw-rw-rw-   0        0        0     7134 2023-06-11 19:27:26.000000 aug_tool-0.2/src/aug_tool/factory.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:26:57.908903 aug_tool-0.2/src/aug_tool.egg-info/
+-rw-rw-rw-   0        0        0    10113 2023-06-12 18:26:57.000000 aug_tool-0.2/src/aug_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1022 2023-06-12 18:26:57.000000 aug_tool-0.2/src/aug_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:26:57.000000 aug_tool-0.2/src/aug_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-12 18:26:57.000000 aug_tool-0.2/src/aug_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 18:26:57.000000 aug_tool-0.2/src/aug_tool.egg-info/top_level.txt
```

### Comparing `aug_tool-0.1/LICENCE` & `aug_tool-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/PKG-INFO` & `aug_tool-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug_tool
-Version: 0.1
+Version: 0.2
 Summary: A package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aug_tool-0.1/README.md` & `aug_tool-0.2/README.md`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/icons/example2Img.png` & `aug_tool-0.2/icons/example2Img.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/icons/example3.png` & `aug_tool-0.2/icons/example3.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/icons/example4.png` & `aug_tool-0.2/icons/example4.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/icons/exampleImg.png` & `aug_tool-0.2/icons/exampleImg.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/icons/logo.png` & `aug_tool-0.2/icons/logo.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/icons/logo2.png` & `aug_tool-0.2/icons/logo2.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/setup.cfg` & `aug_tool-0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7567 5f74 6f6f 6c0d 0a76 6572   = aug_tool..ver
-00000020: 7369 6f6e 203d 2030 2e31 0d0a 6175 7468  sion = 0.1..auth
+00000020: 7369 6f6e 203d 2030 2e32 0d0a 6175 7468  sion = 0.2..auth
 00000030: 6f72 203d 2048 616b 616e 2041 6b74 61c5  or = Hakan Akta.
 00000040: 9f0d 0a61 7574 686f 725f 656d 6169 6c20  ...author_email 
 00000050: 3d20 6861 6b61 6e61 6b74 6173 3435 3431  = hakanaktas4541
 00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000070: 7269 7074 696f 6e20 3d20 4120 7061 636b  ription = A pack
 00000080: 6167 6520 746f 2069 6e63 7265 6173 6520  age to increase 
 00000090: 796f 7572 2064 6174 6120 666f 7220 796f  your data for yo
```

### Comparing `aug_tool-0.1/src/aug_tool/dataAugmentor/imgAug.py` & `aug_tool-0.2/src/aug_tool/dataAugmentor/imgAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/dataAugmentor/txtAug.py` & `aug_tool-0.2/src/aug_tool/dataAugmentor/txtAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/dataAugmentor/xmlAug.py` & `aug_tool-0.2/src/aug_tool/dataAugmentor/xmlAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/dataOpener/dataOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/dataOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/dataOpener/imgOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/imgOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/dataOpener/txtOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/txtOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/dataOpener/xmlOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/xmlOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/dataSaver/xmlSav.py` & `aug_tool-0.2/src/aug_tool/dataSaver/xmlSav.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool/factory.py` & `aug_tool-0.2/src/aug_tool/factory.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1/src/aug_tool.egg-info/PKG-INFO` & `aug_tool-0.2/src/aug_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.1
+Version: 0.2
 Summary: A package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aug_tool-0.1/src/aug_tool.egg-info/SOURCES.txt` & `aug_tool-0.2/src/aug_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

