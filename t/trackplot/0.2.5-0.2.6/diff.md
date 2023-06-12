# Comparing `tmp/trackplot-0.2.5.tar.gz` & `tmp/trackplot-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.2.5.tar", last modified: Fri Jun  9 10:04:51 2023, max compression
+gzip compressed data, was "trackplot-0.2.6.tar", last modified: Mon Jun 12 01:54:28 2023, max compression
```

## Comparing `trackplot-0.2.5.tar` & `trackplot-0.2.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.043572 trackplot-0.2.5/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.5/LICENSE
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-09 10:04:51.043298 trackplot-0.2.5/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.5/Pipfile
--rw-r--r--   0 zhangyiming   (501) staff       (20)    95598 2023-05-30 08:48:54.000000 trackplot-0.2.5/Pipfile.lock
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6508 2023-05-30 02:06:13.000000 trackplot-0.2.5/README.md
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1136 2023-06-09 10:04:11.000000 trackplot-0.2.5/pyproject.toml
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-06-09 10:04:51.043657 trackplot-0.2.5/setup.cfg
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-06-09 10:04:11.000000 trackplot-0.2.5/setup.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.031724 trackplot-0.2.5/trackplot/
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/__init__.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.034517 trackplot-0.2.5/trackplot/anno/
--rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/anno/AxLabel.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/anno/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/anno/theme.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.037855 trackplot-0.2.5/trackplot/base/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/CoordinateMap.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.5/trackplot/base/GenomicLoci.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Protein.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8662 2023-05-06 03:18:03.000000 trackplot-0.2.5/trackplot/base/ReadDepth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.5/trackplot/base/Readder.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Stroke.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/Transcript.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/base/pyUniprot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-06-09 10:04:39.000000 trackplot-0.2.5/trackplot/cli.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.038966 trackplot-0.2.5/trackplot/conf/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/DomainSetting.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/config.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/conf/drawing.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.042996 trackplot-0.2.5/trackplot/file/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.5/trackplot/file/ATAC.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.5/trackplot/file/Bam.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/BedGraph.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Bigwig.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Depth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Fasta.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.5/trackplot/file/File.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.5/trackplot/file/Motif.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.5/trackplot/file/ReadSegments.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.5/trackplot/file/Reference.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/file/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    45357 2023-05-06 03:20:22.000000 trackplot-0.2.5/trackplot/plot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.5/trackplot/plot_func.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.5/trackplot/plot_tests.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-09 10:04:51.033720 trackplot-0.2.5/trackplot.egg-info/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/entry_points.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/not-zip-safe
--rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/requires.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-06-09 10:04:51.000000 trackplot-0.2.5/trackplot.egg-info/top_level.txt
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.437972 trackplot-0.2.6/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.6/LICENSE
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-12 01:54:28.437698 trackplot-0.2.6/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.6/Pipfile
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    95598 2023-05-30 08:48:54.000000 trackplot-0.2.6/Pipfile.lock
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6508 2023-05-30 02:06:13.000000 trackplot-0.2.6/README.md
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1136 2023-06-12 01:53:15.000000 trackplot-0.2.6/pyproject.toml
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-06-12 01:54:28.438048 trackplot-0.2.6/setup.cfg
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-06-12 01:53:15.000000 trackplot-0.2.6/setup.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.414211 trackplot-0.2.6/trackplot/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/__init__.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.428011 trackplot-0.2.6/trackplot/anno/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/anno/AxLabel.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/anno/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/anno/theme.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.432356 trackplot-0.2.6/trackplot/base/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/CoordinateMap.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.6/trackplot/base/GenomicLoci.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Protein.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8580 2023-06-12 01:40:46.000000 trackplot-0.2.6/trackplot/base/ReadDepth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.6/trackplot/base/Readder.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Stroke.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Transcript.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/pyUniprot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-06-12 01:53:38.000000 trackplot-0.2.6/trackplot/cli.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.433500 trackplot-0.2.6/trackplot/conf/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/DomainSetting.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/config.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/drawing.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.437394 trackplot-0.2.6/trackplot/file/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.6/trackplot/file/ATAC.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.6/trackplot/file/Bam.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/BedGraph.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Bigwig.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Depth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Fasta.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.6/trackplot/file/File.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.6/trackplot/file/Motif.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.6/trackplot/file/ReadSegments.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.6/trackplot/file/Reference.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    45357 2023-05-06 03:20:22.000000 trackplot-0.2.6/trackplot/plot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.6/trackplot/plot_func.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/plot_tests.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.426488 trackplot-0.2.6/trackplot.egg-info/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/entry_points.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/not-zip-safe
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/requires.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/top_level.txt
```

### Comparing `trackplot-0.2.5/LICENSE` & `trackplot-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/PKG-INFO` & `trackplot-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
```

### Comparing `trackplot-0.2.5/Pipfile.lock` & `trackplot-0.2.6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/README.md` & `trackplot-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/pyproject.toml` & `trackplot-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trackplot"
-version = "0.2.5"
+version = "0.2.6"
 description = "The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/"
 authors = ["ygidtu <ygidtu@gmail.com>"]
 license = "BSD-3"
 readme = "README.md"
 packages = [{include = "trackplot"}]
 
 [tool.poetry.dependencies]
```

### Comparing `trackplot-0.2.5/setup.py` & `trackplot-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from configparser import ConfigParser
 from setuptools import setup, find_packages
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def locate_packages():
     __dir__ = os.path.dirname(os.path.abspath(__file__))
     pipfile = os.path.join(__dir__, "Pipfile")
```

### Comparing `trackplot-0.2.5/trackplot/anno/theme.py` & `trackplot-0.2.6/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/CoordinateMap.py` & `trackplot-0.2.6/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/GenomicLoci.py` & `trackplot-0.2.6/trackplot/base/GenomicLoci.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/Junction.py` & `trackplot-0.2.6/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/Protein.py` & `trackplot-0.2.6/trackplot/base/Protein.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/ReadDepth.py` & `trackplot-0.2.6/trackplot/base/ReadDepth.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,21 @@
         self.site_plus = site_plus
         self.site_minus = site_minus * -1 if site_minus is not None else site_minus
 
         self._number_of_merged_ = 1
 
     @property
     def plus(self) -> Optional[np.array]:
-        if not self._transformed_or_normalized_ and self._plus_ is not None and self._number_of_merged_ > 0:
+        if self._plus_ is not None and self._number_of_merged_ > 0:
             return self._plus_ / self._number_of_merged_
         return self._plus_
 
     @property
     def minus(self) -> Optional[np.array]:
-        if not self._transformed_or_normalized_ and self._minus_ is not None and self._number_of_merged_ > 0:
+        if self._minus_ is not None and self._number_of_merged_ > 0:
             return self._minus_ / self._number_of_merged_
         return self._minus_
 
     @property
     def wiggle(self) -> np.array:
         if (self._plus_ is None or not self._plus_.any()) and self._minus_ is not None:
             return self.minus
```

### Comparing `trackplot-0.2.5/trackplot/base/Readder.py` & `trackplot-0.2.6/trackplot/base/Readder.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/Stroke.py` & `trackplot-0.2.6/trackplot/base/Stroke.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/Transcript.py` & `trackplot-0.2.6/trackplot/base/Transcript.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/base/pyUniprot.py` & `trackplot-0.2.6/trackplot/base/pyUniprot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/cli.py` & `trackplot-0.2.6/trackplot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from loguru import logger
 
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.conf.config import CLUSTERING_METHOD, COLORS, COLORMAP, DISTANCE_METRIC, IMAGE_TYPE, NORMALIZATION
 from trackplot.file.ATAC import ATAC
 from trackplot.plot import Plot
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def decode_region(region: str):
     regions = region.split(":")
```

### Comparing `trackplot-0.2.5/trackplot/conf/DomainSetting.py` & `trackplot-0.2.6/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/conf/config.py` & `trackplot-0.2.6/trackplot/conf/config.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/conf/drawing.py` & `trackplot-0.2.6/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/ATAC.py` & `trackplot-0.2.6/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/Bam.py` & `trackplot-0.2.6/trackplot/file/Bam.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/BedGraph.py` & `trackplot-0.2.6/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/Bigwig.py` & `trackplot-0.2.6/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/Depth.py` & `trackplot-0.2.6/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/Fasta.py` & `trackplot-0.2.6/trackplot/file/Fasta.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/File.py` & `trackplot-0.2.6/trackplot/file/File.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.2.6/trackplot/file/HiCMatrixTrack.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/Junction.py` & `trackplot-0.2.6/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/Motif.py` & `trackplot-0.2.6/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/ReadSegments.py` & `trackplot-0.2.6/trackplot/file/ReadSegments.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/file/Reference.py` & `trackplot-0.2.6/trackplot/file/Reference.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/plot.py` & `trackplot-0.2.6/trackplot/plot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/plot_func.py` & `trackplot-0.2.6/trackplot/plot_func.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot/plot_tests.py` & `trackplot-0.2.6/trackplot/plot_tests.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.5/trackplot.egg-info/PKG-INFO` & `trackplot-0.2.6/trackplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
```

### Comparing `trackplot-0.2.5/trackplot.egg-info/SOURCES.txt` & `trackplot-0.2.6/trackplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

