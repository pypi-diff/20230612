# Comparing `tmp/aug_tool-0.1.2.tar.gz` & `tmp/aug_tool-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aug_tool-0.1.2.tar", last modified: Mon Jun 12 18:35:32 2023, max compression
+gzip compressed data, was "aug_tool-0.2.tar", last modified: Mon Jun 12 18:26:57 2023, max compression
```

## Comparing `aug_tool-0.1.2.tar` & `aug_tool-0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.623249 aug_tool-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-05-13 18:17:23.000000 aug_tool-0.1.2/LICENCE
--rw-rw-rw-   0        0        0       19 2023-06-12 18:12:54.000000 aug_tool-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    10115 2023-06-12 18:35:32.624240 aug_tool-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9564 2023-06-10 15:10:39.000000 aug_tool-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.569951 aug_tool-0.1.2/icons/
--rw-rw-rw-   0        0        0   126732 2023-06-10 15:04:41.000000 aug_tool-0.1.2/icons/example2Img.png
--rw-rw-rw-   0        0        0   131854 2023-06-10 15:04:14.000000 aug_tool-0.1.2/icons/example3.png
--rw-rw-rw-   0        0        0    70097 2023-06-10 15:03:42.000000 aug_tool-0.1.2/icons/example4.png
--rw-rw-rw-   0        0        0    89216 2023-06-10 15:03:21.000000 aug_tool-0.1.2/icons/exampleImg.png
--rw-rw-rw-   0        0        0    19425 2023-06-04 13:53:14.000000 aug_tool-0.1.2/icons/logo.png
--rw-rw-rw-   0        0        0    18151 2023-06-04 13:39:07.000000 aug_tool-0.1.2/icons/logo2.png
--rw-rw-rw-   0        0        0      108 2023-06-12 18:12:54.000000 aug_tool-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      777 2023-06-12 18:35:32.625241 aug_tool-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.534753 aug_tool-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.581924 aug_tool-0.1.2/src/aug_tool/
--rw-rw-rw-   0        0        0      117 2023-06-12 18:35:09.000000 aug_tool-0.1.2/src/aug_tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.600841 aug_tool-0.1.2/src/aug_tool/dataAugmentor/
--rw-rw-rw-   0        0        0      117 2023-05-14 16:08:12.000000 aug_tool-0.1.2/src/aug_tool/dataAugmentor/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-17 20:04:01.000000 aug_tool-0.1.2/src/aug_tool/dataAugmentor/annAug.py
--rw-rw-rw-   0        0        0      443 2023-06-11 10:38:27.000000 aug_tool-0.1.2/src/aug_tool/dataAugmentor/dataAug.py
--rw-rw-rw-   0        0        0     2146 2023-06-11 10:59:25.000000 aug_tool-0.1.2/src/aug_tool/dataAugmentor/imgAug.py
--rw-rw-rw-   0        0        0     1043 2023-06-11 08:53:47.000000 aug_tool-0.1.2/src/aug_tool/dataAugmentor/txtAug.py
--rw-rw-rw-   0        0        0     2708 2023-06-11 10:59:24.000000 aug_tool-0.1.2/src/aug_tool/dataAugmentor/xmlAug.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.609811 aug_tool-0.1.2/src/aug_tool/dataOpener/
--rw-rw-rw-   0        0        0      165 2023-05-14 16:11:15.000000 aug_tool-0.1.2/src/aug_tool/dataOpener/__init__.py
--rw-rw-rw-   0        0        0      503 2023-05-14 16:11:11.000000 aug_tool-0.1.2/src/aug_tool/dataOpener/annOp.py
--rw-rw-rw-   0        0        0      524 2023-05-15 18:16:39.000000 aug_tool-0.1.2/src/aug_tool/dataOpener/dataOp.py
--rw-rw-rw-   0        0        0     1010 2023-05-16 20:08:15.000000 aug_tool-0.1.2/src/aug_tool/dataOpener/imgOp.py
--rw-rw-rw-   0        0        0     1422 2023-05-17 19:37:14.000000 aug_tool-0.1.2/src/aug_tool/dataOpener/txtOp.py
--rw-rw-rw-   0        0        0     1586 2023-06-09 18:46:29.000000 aug_tool-0.1.2/src/aug_tool/dataOpener/xmlOp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.622245 aug_tool-0.1.2/src/aug_tool/dataSaver/
--rw-rw-rw-   0        0        0      142 2023-05-14 16:12:52.000000 aug_tool-0.1.2/src/aug_tool/dataSaver/__init__.py
--rw-rw-rw-   0        0        0      310 2023-05-15 19:34:14.000000 aug_tool-0.1.2/src/aug_tool/dataSaver/annSav.py
--rw-rw-rw-   0        0        0      490 2023-05-15 19:34:17.000000 aug_tool-0.1.2/src/aug_tool/dataSaver/dataSav.py
--rw-rw-rw-   0        0        0      402 2023-05-16 18:30:28.000000 aug_tool-0.1.2/src/aug_tool/dataSaver/imgSav.py
--rw-rw-rw-   0        0        0      502 2023-05-17 19:32:38.000000 aug_tool-0.1.2/src/aug_tool/dataSaver/txtSav.py
--rw-rw-rw-   0        0        0      541 2023-06-11 10:59:24.000000 aug_tool-0.1.2/src/aug_tool/dataSaver/xmlSav.py
--rw-rw-rw-   0        0        0     7134 2023-06-11 19:27:26.000000 aug_tool-0.1.2/src/aug_tool/factory.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:35:32.590875 aug_tool-0.1.2/src/aug_tool.egg-info/
--rw-rw-rw-   0        0        0    10115 2023-06-12 18:35:32.000000 aug_tool-0.1.2/src/aug_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1022 2023-06-12 18:35:32.000000 aug_tool-0.1.2/src/aug_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:35:32.000000 aug_tool-0.1.2/src/aug_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-12 18:35:32.000000 aug_tool-0.1.2/src/aug_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 18:35:32.000000 aug_tool-0.1.2/src/aug_tool.egg-info/top_level.txt
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

### Comparing `aug_tool-0.1.2/LICENCE` & `aug_tool-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/PKG-INFO` & `aug_tool-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug_tool
-Version: 0.1.2
+Version: 0.2
 Summary: A package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aug_tool-0.1.2/README.md` & `aug_tool-0.2/README.md`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/icons/example2Img.png` & `aug_tool-0.2/icons/example2Img.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/icons/example3.png` & `aug_tool-0.2/icons/example3.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/icons/example4.png` & `aug_tool-0.2/icons/example4.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/icons/exampleImg.png` & `aug_tool-0.2/icons/exampleImg.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/icons/logo.png` & `aug_tool-0.2/icons/logo.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/icons/logo2.png` & `aug_tool-0.2/icons/logo2.png`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/setup.cfg` & `aug_tool-0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7567 5f74 6f6f 6c0d 0a76 6572   = aug_tool..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e32 0d0a 6175  sion = 0.1.2..au
-00000030: 7468 6f72 203d 2048 616b 616e 2041 6b74  thor = Hakan Akt
-00000040: 61c5 9f0d 0a61 7574 686f 725f 656d 6169  a....author_emai
-00000050: 6c20 3d20 6861 6b61 6e61 6b74 6173 3435  l = hakanaktas45
-00000060: 3431 4067 6d61 696c 2e63 6f6d 0d0a 6465  41@gmail.com..de
-00000070: 7363 7269 7074 696f 6e20 3d20 4120 7061  scription = A pa
-00000080: 636b 6167 6520 746f 2069 6e63 7265 6173  ckage to increas
-00000090: 6520 796f 7572 2064 6174 6120 666f 7220  e your data for 
-000000a0: 796f 7572 206d 6163 6869 6e65 206c 6561  your machine lea
-000000b0: 726e 696e 6720 7072 6f6a 6563 740d 0a6c  rning project..l
-000000c0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000d0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000e0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000f0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000100: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000110: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000120: 6769 7468 7562 2e63 6f6d 2f68 616b 616e  github.com/hakan
-00000130: 616b 7461 7331 2f61 7567 2d74 6f6f 6c0d  aktas1/aug-tool.
-00000140: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000150: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
-00000160: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000170: 636f 6d2f 6861 6b61 6e61 6b74 6173 312f  com/hakanaktas1/
-00000180: 6175 672d 746f 6f6c 0d0a 636c 6173 7369  aug-tool..classi
-00000190: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
-000001a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-000001c0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-000001d0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-000001e0: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-000001f0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000200: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
-00000210: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000220: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
-00000230: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
-00000240: 6e64 3a0d 0a69 6e73 7461 6c6c 5f72 6571  nd:..install_req
-00000250: 7569 7265 7320 3d20 0d0a 0950 696c 6c6f  uires = ...Pillo
-00000260: 773e 3d38 2e32 0d0a 0962 7334 3e3d 302e  w>=8.2...bs4>=0.
-00000270: 302e 310d 0a09 6265 6175 7469 6675 6c73  0.1...beautifuls
-00000280: 6f75 7034 3e3d 342e 3132 2e32 0d0a 096c  oup4>=4.12.2...l
-00000290: 786d 6c3e 3d34 2e39 2e32 0d0a 7079 7468  xml>=4.9.2..pyth
-000002a0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-000002b0: 332e 360d 0a0d 0a5b 6f70 7469 6f6e 732e  3.6....[options.
-000002c0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-000002d0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-000002e0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000002f0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000300: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000020: 7369 6f6e 203d 2030 2e32 0d0a 6175 7468  sion = 0.2..auth
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

### Comparing `aug_tool-0.1.2/src/aug_tool/dataAugmentor/imgAug.py` & `aug_tool-0.2/src/aug_tool/dataAugmentor/imgAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/dataAugmentor/txtAug.py` & `aug_tool-0.2/src/aug_tool/dataAugmentor/txtAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/dataAugmentor/xmlAug.py` & `aug_tool-0.2/src/aug_tool/dataAugmentor/xmlAug.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/dataOpener/dataOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/dataOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/dataOpener/imgOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/imgOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/dataOpener/txtOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/txtOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/dataOpener/xmlOp.py` & `aug_tool-0.2/src/aug_tool/dataOpener/xmlOp.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/dataSaver/xmlSav.py` & `aug_tool-0.2/src/aug_tool/dataSaver/xmlSav.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool/factory.py` & `aug_tool-0.2/src/aug_tool/factory.py`

 * *Files identical despite different names*

### Comparing `aug_tool-0.1.2/src/aug_tool.egg-info/PKG-INFO` & `aug_tool-0.2/src/aug_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aug-tool
-Version: 0.1.2
+Version: 0.2
 Summary: A package to increase your data for your machine learning project
 Home-page: https://github.com/hakanaktas1/aug-tool
 Author: Hakan Aktaş
 Author-email: hakanaktas4541@gmail.com
 Project-URL: Bug Tracker, https://github.com/hakanaktas1/aug-tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aug_tool-0.1.2/src/aug_tool.egg-info/SOURCES.txt` & `aug_tool-0.2/src/aug_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

