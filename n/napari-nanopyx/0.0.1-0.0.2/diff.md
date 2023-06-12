# Comparing `tmp/napari-nanopyx-0.0.1.tar.gz` & `tmp/napari-nanopyx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-nanopyx-0.0.1.tar", last modified: Wed May 10 08:49:53 2023, max compression
+gzip compressed data, was "napari-nanopyx-0.0.2.tar", last modified: Mon Jun 12 13:40:10 2023, max compression
```

## Comparing `napari-nanopyx-0.0.1.tar` & `napari-nanopyx-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-05-10 08:49:53.687201 napari-nanopyx-0.0.1/
--rw-r--r--   0 abrito   (1547774166) 931978602     7653 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/LICENSE
--rw-r--r--   0 abrito   (1547774166) 931978602       96 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/MANIFEST.in
--rw-r--r--   0 abrito   (1547774166) 931978602     3273 2023-05-10 08:49:53.687274 napari-nanopyx-0.0.1/PKG-INFO
--rw-r--r--   0 abrito   (1547774166) 931978602     2573 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/README.md
--rw-r--r--   0 abrito   (1547774166) 931978602     1045 2023-05-10 08:49:38.000000 napari-nanopyx-0.0.1/pyproject.toml
--rw-r--r--   0 abrito   (1547774166) 931978602     1337 2023-05-10 08:49:53.687615 napari-nanopyx-0.0.1/setup.cfg
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-05-10 08:49:53.684284 napari-nanopyx-0.0.1/src/
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-05-10 08:49:53.686087 napari-nanopyx-0.0.1/src/napari_nanopyx/
--rw-r--r--   0 abrito   (1547774166) 931978602       41 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/src/napari_nanopyx/__init__.py
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-05-10 08:49:53.687099 napari-nanopyx-0.0.1/src/napari_nanopyx/_tests/
--rw-r--r--   0 abrito   (1547774166) 931978602        0 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/src/napari_nanopyx/_tests/__init__.py
--rw-r--r--   0 abrito   (1547774166) 931978602     3980 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/src/napari_nanopyx/channel_registration.py
--rw-r--r--   0 abrito   (1547774166) 931978602     4408 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/src/napari_nanopyx/drift_alignment.py
--rw-r--r--   0 abrito   (1547774166) 931978602     2308 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/src/napari_nanopyx/napari.yaml
--rw-r--r--   0 abrito   (1547774166) 931978602     3750 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/src/napari_nanopyx/squirrel.py
--rw-r--r--   0 abrito   (1547774166) 931978602     2421 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.1/src/napari_nanopyx/srrf.py
-drwxr-xr-x   0 abrito   (1547774166) 931978602        0 2023-05-10 08:49:53.686966 napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/
--rw-r--r--   0 abrito   (1547774166) 931978602     3273 2023-05-10 08:49:53.000000 napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/PKG-INFO
--rw-r--r--   0 abrito   (1547774166) 931978602      547 2023-05-10 08:49:53.000000 napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/SOURCES.txt
--rw-r--r--   0 abrito   (1547774166) 931978602        1 2023-05-10 08:49:53.000000 napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/dependency_links.txt
--rw-r--r--   0 abrito   (1547774166) 931978602       62 2023-05-10 08:49:53.000000 napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/entry_points.txt
--rw-r--r--   0 abrito   (1547774166) 931978602       44 2023-05-10 08:49:53.000000 napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/requires.txt
--rw-r--r--   0 abrito   (1547774166) 931978602       15 2023-05-10 08:49:53.000000 napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/top_level.txt
+drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.223234 napari-nanopyx-0.0.2/
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     7653 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/LICENSE
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       96 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/MANIFEST.in
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3273 2023-06-12 13:40:10.223316 napari-nanopyx-0.0.2/PKG-INFO
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     2573 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/README.md
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     1045 2023-06-12 13:29:33.000000 napari-nanopyx-0.0.2/pyproject.toml
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     1337 2023-06-12 13:40:10.223658 napari-nanopyx-0.0.2/setup.cfg
+drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.219364 napari-nanopyx-0.0.2/src/
+drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.221877 napari-nanopyx-0.0.2/src/napari_nanopyx/
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       41 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/__init__.py
+drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.223093 napari-nanopyx-0.0.2/src/napari_nanopyx/_tests/
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/_tests/__init__.py
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3980 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/channel_registration.py
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     4408 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/drift_alignment.py
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     2308 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/napari.yaml
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3750 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/squirrel.py
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     2421 2023-05-10 08:33:29.000000 napari-nanopyx-0.0.2/src/napari_nanopyx/srrf.py
+drwxr-xr-x   0 abrito   (1547774166) RAS\Domain Users (931978602)        0 2023-06-12 13:40:10.222929 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)     3273 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/PKG-INFO
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)      547 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/SOURCES.txt
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)        1 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/dependency_links.txt
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       62 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/entry_points.txt
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       44 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/requires.txt
+-rw-r--r--   0 abrito   (1547774166) RAS\Domain Users (931978602)       15 2023-06-12 13:40:10.000000 napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/top_level.txt
```

### Comparing `napari-nanopyx-0.0.1/LICENSE` & `napari-nanopyx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.1/PKG-INFO` & `napari-nanopyx-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-nanopyx
-Version: 0.0.1
+Version: 0.0.2
 Summary: napari plugin for NanoPyx
 Author: Bruno Saraiva
 Author-email: Ricardo Henriques <ricardo.jv.henriques@gmail.com>, Bruno Saraiva <bruno.msaraiva2@gmail.com>, Inês Cunha <inescunha200@gmail.com>, António Brito <antmsbrito95@gmail.com>
 Maintainer-email: Bruno Saraiva <bruno.msaraiva2@gmail.com>
 Keywords: napari,NanoJ,Super-Resolution Microscopy,Fluorescence,BioImage Analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napari-nanopyx-0.0.1/README.md` & `napari-nanopyx-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.1/pyproject.toml` & `napari-nanopyx-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napari-nanopyx"
-version = "0.0.1"
+version = "0.0.2"
 description = "napari plugin for NanoPyx"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 keywords = [
     "napari",
     "NanoJ",
```

### Comparing `napari-nanopyx-0.0.1/setup.cfg` & `napari-nanopyx-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-nanopyx
-version = 0.0.1
+version = 0.0.2
 description = napari plugin of Nanoscopy Python library (NanoPyx, the successor to NanoJ) - focused on light microscopy and super-resolution imaging
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Bruno Saraiva
 author_email = bruno.msaraiva2@gmail.com
 license = LGPL-3.0-only
 license_files = LICENSE
```

### Comparing `napari-nanopyx-0.0.1/src/napari_nanopyx/channel_registration.py` & `napari-nanopyx-0.0.2/src/napari_nanopyx/channel_registration.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.1/src/napari_nanopyx/drift_alignment.py` & `napari-nanopyx-0.0.2/src/napari_nanopyx/drift_alignment.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.1/src/napari_nanopyx/napari.yaml` & `napari-nanopyx-0.0.2/src/napari_nanopyx/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.1/src/napari_nanopyx/squirrel.py` & `napari-nanopyx-0.0.2/src/napari_nanopyx/squirrel.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.1/src/napari_nanopyx/srrf.py` & `napari-nanopyx-0.0.2/src/napari_nanopyx/srrf.py`

 * *Files identical despite different names*

### Comparing `napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/PKG-INFO` & `napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-nanopyx
-Version: 0.0.1
+Version: 0.0.2
 Summary: napari plugin for NanoPyx
 Author: Bruno Saraiva
 Author-email: Ricardo Henriques <ricardo.jv.henriques@gmail.com>, Bruno Saraiva <bruno.msaraiva2@gmail.com>, Inês Cunha <inescunha200@gmail.com>, António Brito <antmsbrito95@gmail.com>
 Maintainer-email: Bruno Saraiva <bruno.msaraiva2@gmail.com>
 Keywords: napari,NanoJ,Super-Resolution Microscopy,Fluorescence,BioImage Analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napari-nanopyx-0.0.1/src/napari_nanopyx.egg-info/SOURCES.txt` & `napari-nanopyx-0.0.2/src/napari_nanopyx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

