# Comparing `tmp/agsi-1.5.tar.gz` & `tmp/agsi-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.5.tar", last modified: Thu May 25 07:01:02 2023, max compression
+gzip compressed data, was "agsi-1.6.tar", last modified: Mon Jun 12 08:09:23 2023, max compression
```

## Comparing `agsi-1.5.tar` & `agsi-1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 07:01:02.884931 agsi-1.5/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       71 2023-05-24 10:23:11.000000 agsi-1.5/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-25 07:01:02.884931 agsi-1.5/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     2077 2023-05-17 09:13:44.000000 agsi-1.5/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 07:01:02.884931 agsi-1.5/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-17 09:19:23.000000 agsi-1.5/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 07:01:02.884931 agsi-1.5/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    15406 2023-05-25 07:00:38.000000 agsi-1.5/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-17 09:16:41.000000 agsi-1.5/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-17 09:13:44.000000 agsi-1.5/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)   931124 2023-05-19 09:52:59.000000 agsi-1.5/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-17 09:13:44.000000 agsi-1.5/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-17 09:13:44.000000 agsi-1.5/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-05-25 07:01:02.884931 agsi-1.5/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-05-25 07:01:02.000000 agsi-1.5/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-05-25 07:01:02.000000 agsi-1.5/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-05-25 07:01:02.000000 agsi-1.5/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-05-25 07:01:02.000000 agsi-1.5/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-05-25 07:01:02.000000 agsi-1.5/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-05-25 07:01:02.884931 agsi-1.5/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-05-25 07:00:59.000000 agsi-1.5/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:09:23.225407 agsi-1.6/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-1.6/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 08:09:23.225407 agsi-1.6/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-1.6/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:09:23.225407 agsi-1.6/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-1.6/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:09:23.225407 agsi-1.6/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15499 2023-06-12 08:02:59.000000 agsi-1.6/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-1.6/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-25 15:09:48.000000 agsi-1.6/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075103 2023-06-12 08:02:57.000000 agsi-1.6/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-1.6/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-1.6/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:09:23.225407 agsi-1.6/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 08:09:23.000000 agsi-1.6/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-12 08:09:23.000000 agsi-1.6/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-12 08:09:23.000000 agsi-1.6/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-12 08:09:23.000000 agsi-1.6/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-12 08:09:23.000000 agsi-1.6/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-12 08:09:23.225407 agsi-1.6/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-12 08:09:15.000000 agsi-1.6/setup.py
```

### Comparing `agsi-1.5/agsi/data/FarmData.py` & `agsi-1.6/agsi/data/FarmData.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,14 +345,18 @@
         return clipped_chip
   
   def get_chips(self,chip_size=200,valid_threshold=0.1,modality_type="drone",resolution=75,timestamp=None):
      
       block_image=self.get_modality(modality_type=modality_type,timestamp=timestamp)
       return Chip(block_image,chip_size,valid_threshold)
   
+  def get_times(self):
+     times = self.info['data_path'].keys()
+     return list(times)
+  
   
 class Chip(FarmData):
   def __init__(self,block_chip,size=200,valid_threshold=0.1):
 
     """
         Represents a chip or tile extracted from a block.
```

### Comparing `agsi-1.5/agsi/data/utils.py` & `agsi-1.6/agsi/data/utils.py`

 * *Files identical despite different names*

