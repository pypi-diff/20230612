# Comparing `tmp/aug_tool-0.0.7.tar.gz` & `tmp/aug_tool-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug_tool-0.0.7.tar", last modified: Sun Jun 11 19:47:53 2023, max compression
+gzip compressed data, was "aug_tool-0.1.tar", last modified: Mon Jun 12 18:14:52 2023, max compression
```

## Comparing `aug_tool-0.0.7.tar` & `aug_tool-0.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.431842 aug_tool-0.0.7/
--rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug_tool-0.0.7/LICENCE
--rw-rw-rw-   0        0        0       19 2023-06-11 18:43:10.000000 aug_tool-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    10121 2023-06-11 19:47:53.432834 aug_tool-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug_tool-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.389980 aug_tool-0.0.7/icons/
--rw-rw-rw-   0        0        0   126732 2023-06-10 15:04:41.000000 aug_tool-0.0.7/icons/example2Img.png
--rw-rw-rw-   0        0        0   131854 2023-06-10 15:04:14.000000 aug_tool-0.0.7/icons/example3.png
--rw-rw-rw-   0        0        0    70097 2023-06-10 15:03:42.000000 aug_tool-0.0.7/icons/example4.png
--rw-rw-rw-   0        0        0    89216 2023-06-10 15:03:21.000000 aug_tool-0.0.7/icons/exampleImg.png
--rw-rw-rw-   0        0        0    19425 2023-06-04 13:53:14.000000 aug_tool-0.0.7/icons/logo.png
--rw-rw-rw-   0        0        0    18151 2023-06-04 13:39:07.000000 aug_tool-0.0.7/icons/logo2.png
--rw-rw-rw-   0        0        0      108 2023-06-11 19:23:07.000000 aug_tool-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      753 2023-06-11 19:47:53.433831 aug_tool-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.371044 aug_tool-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.393968 aug_tool-0.0.7/src/aug-tool/
--rw-rw-rw-   0        0        0        0 2023-05-12 19:34:11.000000 aug_tool-0.0.7/src/aug-tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.403935 aug_tool-0.0.7/src/aug-tool/dataAugmentor/
--rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug_tool-0.0.7/src/aug-tool/dataAugmentor/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug_tool-0.0.7/src/aug-tool/dataAugmentor/annAug.py
--rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug_tool-0.0.7/src/aug-tool/dataAugmentor/dataAug.py
--rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug_tool-0.0.7/src/aug-tool/dataAugmentor/imgAug.py
--rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug_tool-0.0.7/src/aug-tool/dataAugmentor/txtAug.py
--rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug_tool-0.0.7/src/aug-tool/dataAugmentor/xmlAug.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.413897 aug_tool-0.0.7/src/aug-tool/dataOpener/
--rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug_tool-0.0.7/src/aug-tool/dataOpener/__init__.py
--rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug_tool-0.0.7/src/aug-tool/dataOpener/annOp.py
--rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug_tool-0.0.7/src/aug-tool/dataOpener/dataOp.py
--rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug_tool-0.0.7/src/aug-tool/dataOpener/imgOp.py
--rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug_tool-0.0.7/src/aug-tool/dataOpener/txtOp.py
--rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug_tool-0.0.7/src/aug-tool/dataOpener/xmlOp.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.422874 aug_tool-0.0.7/src/aug-tool/dataSaver/
--rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug_tool-0.0.7/src/aug-tool/dataSaver/__init__.py
--rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug_tool-0.0.7/src/aug-tool/dataSaver/annSav.py
--rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug_tool-0.0.7/src/aug-tool/dataSaver/dataSav.py
--rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug_tool-0.0.7/src/aug-tool/dataSaver/imgSav.py
--rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug_tool-0.0.7/src/aug-tool/dataSaver/txtSav.py
--rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug_tool-0.0.7/src/aug-tool/dataSaver/xmlSav.py
--rw-rw-rw-   0        0        0      699 2023-06-10 09:47:20.000000 aug_tool-0.0.7/src/aug-tool/deneme.py
--rw-rw-rw-   0        0        0     7134 2023-06-11 19:27:26.000000 aug_tool-0.0.7/src/aug-tool/factory.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:47:53.430841 aug_tool-0.0.7/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0    10121 2023-06-11 19:47:53.000000 aug_tool-0.0.7/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-06-11 19:47:53.000000 aug_tool-0.0.7/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 19:47:53.000000 aug_tool-0.0.7/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-11 19:47:53.000000 aug_tool-0.0.7/src/aug_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 19:47:53.000000 aug_tool-0.0.7/src/aug_tool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.888255 aug_tool-0.1/
+-rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug_tool-0.1/LICENCE
+-rw-rw-rw-   0        0        0       19 2023-06-12 18:12:54.000000 aug_tool-0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10113 2023-06-12 18:14:52.889251 aug_tool-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug_tool-0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.841410 aug_tool-0.1/icons/
+-rw-rw-rw-   0        0        0   126732 2023-06-10 15:04:41.000000 aug_tool-0.1/icons/example2Img.png
+-rw-rw-rw-   0        0        0   131854 2023-06-10 15:04:14.000000 aug_tool-0.1/icons/example3.png
+-rw-rw-rw-   0        0        0    70097 2023-06-10 15:03:42.000000 aug_tool-0.1/icons/example4.png
+-rw-rw-rw-   0        0        0    89216 2023-06-10 15:03:21.000000 aug_tool-0.1/icons/exampleImg.png
+-rw-rw-rw-   0        0        0    19425 2023-06-04 13:53:14.000000 aug_tool-0.1/icons/logo.png
+-rw-rw-rw-   0        0        0    18151 2023-06-04 13:39:07.000000 aug_tool-0.1/icons/logo2.png
+-rw-rw-rw-   0        0        0      108 2023-06-12 18:12:54.000000 aug_tool-0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      775 2023-06-12 18:14:52.891245 aug_tool-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.821478 aug_tool-0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.845397 aug_tool-0.1/src/aug_tool/
+-rw-rw-rw-   0        0        0        0 2023-06-11 19:50:49.000000 aug_tool-0.1/src/aug_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.865332 aug_tool-0.1/src/aug_tool/dataAugmentor/
+-rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/annAug.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/dataAug.py
+-rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/imgAug.py
+-rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/txtAug.py
+-rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug_tool-0.1/src/aug_tool/dataAugmentor/xmlAug.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.876295 aug_tool-0.1/src/aug_tool/dataOpener/
+-rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug_tool-0.1/src/aug_tool/dataOpener/__init__.py
+-rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug_tool-0.1/src/aug_tool/dataOpener/annOp.py
+-rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug_tool-0.1/src/aug_tool/dataOpener/dataOp.py
+-rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug_tool-0.1/src/aug_tool/dataOpener/imgOp.py
+-rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug_tool-0.1/src/aug_tool/dataOpener/txtOp.py
+-rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug_tool-0.1/src/aug_tool/dataOpener/xmlOp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.887257 aug_tool-0.1/src/aug_tool/dataSaver/
+-rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug_tool-0.1/src/aug_tool/dataSaver/__init__.py
+-rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug_tool-0.1/src/aug_tool/dataSaver/annSav.py
+-rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug_tool-0.1/src/aug_tool/dataSaver/dataSav.py
+-rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug_tool-0.1/src/aug_tool/dataSaver/imgSav.py
+-rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug_tool-0.1/src/aug_tool/dataSaver/txtSav.py
+-rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug_tool-0.1/src/aug_tool/dataSaver/xmlSav.py
+-rw-rw-rw-   0        0        0     7134 2023-06-11 19:27:26.000000 aug_tool-0.1/src/aug_tool/factory.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:14:52.854372 aug_tool-0.1/src/aug_tool.egg-info/
+-rw-rw-rw-   0        0        0    10113 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1022 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 18:14:52.000000 aug_tool-0.1/src/aug_tool.egg-info/top_level.txt
```

### Comparing `aug_tool-0.0.7/LICENCE` & `aug_tool-0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/PKG-INFO` & `aug_tool-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aug_tool
-Version: 0.0.7
-Summary: A small package to increase your data for your machine learning project
+Version: 0.1
+Summary: A package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aug_tool-0.0.7/README.md` & `aug_tool-0.1/README.md`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/icons/example2Img.png` & `aug_tool-0.1/icons/example2Img.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/icons/example3.png` & `aug_tool-0.1/icons/example3.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/icons/example4.png` & `aug_tool-0.1/icons/example4.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/icons/exampleImg.png` & `aug_tool-0.1/icons/exampleImg.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/icons/logo.png` & `aug_tool-0.1/icons/logo.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/icons/logo2.png` & `aug_tool-0.1/icons/logo2.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/setup.cfg` & `aug_tool-0.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7567 5f74 6f6f 6c0d 0a76 6572   = aug_tool..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6175  sion = 0.0.7..au
-00000030: 7468 6f72 203d 2048 616b 616e 2041 6b74  thor = Hakan Akt
-00000040: 61c5 9f0d 0a61 7574 686f 725f 656d 6169  a....author_emai
-00000050: 6c20 3d20 6861 6b61 6e61 6b74 6173 3435  l = hakanaktas45
-00000060: 3431 4067 6d61 696c 2e63 6f6d 0d0a 6465  41@gmail.com..de
-00000070: 7363 7269 7074 696f 6e20 3d20 4120 736d  scription = A sm
-00000080: 616c 6c20 7061 636b 6167 6520 746f 2069  all package to i
-00000090: 6e63 7265 6173 6520 796f 7572 2064 6174  ncrease your dat
-000000a0: 6120 666f 7220 796f 7572 206d 6163 6869  a for your machi
-000000b0: 6e65 206c 6561 726e 696e 6720 7072 6f6a  ne learning proj
-000000c0: 6563 740d 0a6c 6f6e 675f 6465 7363 7269  ect..long_descri
-000000d0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-000000e0: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
-000000f0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000100: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
-00000110: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
-00000120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000130: 2f68 616b 616e 616b 7461 7331 2f61 7567  /hakanaktas1/aug
-00000140: 2d74 6f6f 6c0d 0a70 726f 6a65 6374 5f75  -tool..project_u
-00000150: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000160: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000170: 6974 6875 622e 636f 6d2f 6861 6b61 6e61  ithub.com/hakana
-00000180: 6b74 6173 312f 6175 672d 746f 6f6c 0d0a  ktas1/aug-tool..
-00000190: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001a0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001c0: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
-000001d0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-000001e0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-000001f0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000200: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000210: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000220: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000230: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
-00000240: 7320 3d20 6669 6e64 3a0d 0a69 6e73 7461  s = find:..insta
-00000250: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000260: 0950 696c 6c6f 773e 3d38 2e32 0d0a 0962  .Pillow>=8.2...b
-00000270: 7334 3e3d 302e 302e 310d 0a09 7479 7069  s4>=0.0.1...typi
-00000280: 6e67 0d0a 7079 7468 6f6e 5f72 6571 7569  ng..python_requi
-00000290: 7265 7320 3d20 3e3d 332e 360d 0a0d 0a5b  res = >=3.6....[
-000002a0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-000002b0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000002c0: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-000002d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000002e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000002f0: 0a                                       .
+00000020: 7369 6f6e 203d 2030 2e31 0d0a 6175 7468  sion = 0.1..auth
+00000030: 6f72 203d 2048 616b 616e 2041 6b74 61c5  or = Hakan Akta.
+00000040: 9f0d 0a61 7574 686f 725f 656d 6169 6c20  ...author_email 
+00000050: 3d20 6861 6b61 6e61 6b74 6173 3435 3431  = hakanaktas4541
+00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
+00000070: 7269 7074 696f 6e20 3d20 4120 7061 636b  ription = A pack
+00000080: 6167 6520 746f 2069 6e63 7265 6173 6520  age to increase 
+00000090: 796f 7572 2064 6174 6120 666f 7220 796f  your data for yo
+000000a0: 7572 206d 6163 6869 6e65 206c 6561 726e  ur machine learn
+000000b0: 696e 6720 7072 6f6a 6563 740d 0a6c 6f6e  ing project..lon
+000000c0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+000000d0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
+000000e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000f0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+00000100: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+00000110: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+00000120: 7468 7562 2e63 6f6d 2f68 616b 616e 616b  thub.com/hakanak
+00000130: 7461 7331 2f61 7567 2d74 6f6f 6c0d 0a70  tas1/aug-tool..p
+00000140: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000150: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000160: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000170: 6d2f 6861 6b61 6e61 6b74 6173 312f 6175  m/hakanaktas1/au
+00000180: 672d 746f 6f6c 0d0a 636c 6173 7369 6669  g-tool..classifi
+00000190: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
+000001c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000001e0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+000001f0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000200: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
+00000210: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+00000220: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
+00000230: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000240: 3a0d 0a69 6e73 7461 6c6c 5f72 6571 7569  :..install_requi
+00000250: 7265 7320 3d20 0d0a 0950 696c 6c6f 773e  res = ...Pillow>
+00000260: 3d38 2e32 0d0a 0962 7334 3e3d 302e 302e  =8.2...bs4>=0.0.
+00000270: 310d 0a09 6265 6175 7469 6675 6c73 6f75  1...beautifulsou
+00000280: 7034 3e3d 342e 3132 2e32 0d0a 096c 786d  p4>=4.12.2...lxm
+00000290: 6c3e 3d34 2e39 2e32 0d0a 7079 7468 6f6e  l>=4.9.2..python
+000002a0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+000002b0: 360d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  6....[options.pa
+000002c0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+000002d0: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
+000002e0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000002f0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000300: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `aug_tool-0.0.7/src/aug-tool/dataAugmentor/imgAug.py` & `aug_tool-0.1/src/aug_tool/dataAugmentor/imgAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/dataAugmentor/txtAug.py` & `aug_tool-0.1/src/aug_tool/dataAugmentor/txtAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/dataAugmentor/xmlAug.py` & `aug_tool-0.1/src/aug_tool/dataAugmentor/xmlAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/dataOpener/dataOp.py` & `aug_tool-0.1/src/aug_tool/dataOpener/dataOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/dataOpener/imgOp.py` & `aug_tool-0.1/src/aug_tool/dataOpener/imgOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/dataOpener/txtOp.py` & `aug_tool-0.1/src/aug_tool/dataOpener/txtOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/dataOpener/xmlOp.py` & `aug_tool-0.1/src/aug_tool/dataOpener/xmlOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/dataSaver/xmlSav.py` & `aug_tool-0.1/src/aug_tool/dataSaver/xmlSav.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug-tool/factory.py` & `aug_tool-0.1/src/aug_tool/factory.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.0.7/src/aug_tool.egg-info/PKG-INFO` & `aug_tool-0.1/src/aug_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.0.7
-Summary: A small package to increase your data for your machine learning project
+Version: 0.1
+Summary: A package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aug_tool-0.0.7/src/aug_tool.egg-info/SOURCES.txt` & `aug_tool-0.1/src/aug_tool.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 setup.cfg
 icons/example2Img.png
 icons/example3.png
 icons/example4.png
 icons/exampleImg.png
 icons/logo.png
 icons/logo2.png
-src/aug-tool/__init__.py
-src/aug-tool/deneme.py
-src/aug-tool/factory.py
-src/aug-tool/dataAugmentor/__init__.py
-src/aug-tool/dataAugmentor/annAug.py
-src/aug-tool/dataAugmentor/dataAug.py
-src/aug-tool/dataAugmentor/imgAug.py
-src/aug-tool/dataAugmentor/txtAug.py
-src/aug-tool/dataAugmentor/xmlAug.py
-src/aug-tool/dataOpener/__init__.py
-src/aug-tool/dataOpener/annOp.py
-src/aug-tool/dataOpener/dataOp.py
-src/aug-tool/dataOpener/imgOp.py
-src/aug-tool/dataOpener/txtOp.py
-src/aug-tool/dataOpener/xmlOp.py
-src/aug-tool/dataSaver/__init__.py
-src/aug-tool/dataSaver/annSav.py
-src/aug-tool/dataSaver/dataSav.py
-src/aug-tool/dataSaver/imgSav.py
-src/aug-tool/dataSaver/txtSav.py
-src/aug-tool/dataSaver/xmlSav.py
+src/aug_tool/__init__.py
+src/aug_tool/factory.py
 src/aug_tool.egg-info/PKG-INFO
 src/aug_tool.egg-info/SOURCES.txt
 src/aug_tool.egg-info/dependency_links.txt
 src/aug_tool.egg-info/requires.txt
-src/aug_tool.egg-info/top_level.txt
+src/aug_tool.egg-info/top_level.txt
+src/aug_tool/dataAugmentor/__init__.py
+src/aug_tool/dataAugmentor/annAug.py
+src/aug_tool/dataAugmentor/dataAug.py
+src/aug_tool/dataAugmentor/imgAug.py
+src/aug_tool/dataAugmentor/txtAug.py
+src/aug_tool/dataAugmentor/xmlAug.py
+src/aug_tool/dataOpener/__init__.py
+src/aug_tool/dataOpener/annOp.py
+src/aug_tool/dataOpener/dataOp.py
+src/aug_tool/dataOpener/imgOp.py
+src/aug_tool/dataOpener/txtOp.py
+src/aug_tool/dataOpener/xmlOp.py
+src/aug_tool/dataSaver/__init__.py
+src/aug_tool/dataSaver/annSav.py
+src/aug_tool/dataSaver/dataSav.py
+src/aug_tool/dataSaver/imgSav.py
+src/aug_tool/dataSaver/txtSav.py
+src/aug_tool/dataSaver/xmlSav.py
```

