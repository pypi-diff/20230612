# Comparing `tmp/dwiqc-0.4.2-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.4.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 24427 bytes, number of entries: 22
+Zip file size: 24434 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-Jun-08 18:05 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 14:28 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-12 14:37 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jun-08 18:05 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 23-Jun-12 14:27 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-Jun-08 18:05 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5989 b- defN 23-Jun-08 18:05 dwiqc/cli/process.py
--rw-r--r--  2.0 unx     3731 b- defN 23-Jun-08 18:05 dwiqc/cli/tandem.py
+-rw-r--r--  2.0 unx     3775 b- defN 23-Jun-12 14:37 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Jun-08 18:05 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jun-08 18:05 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jun-08 18:05 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jun-08 18:05 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    10168 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4415 b- defN 23-Jun-08 18:05 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6146 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jun-08 18:05 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13083 b- defN 23-Jun-08 18:05 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5781 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      428 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-12 14:29 dwiqc-0.4.2.dist-info/RECORD
-22 files, 67948 bytes uncompressed, 21675 bytes compressed:  68.1%
+-rwxr-xr-x  2.0 unx     5781 b- defN 23-Jun-12 14:39 dwiqc-0.4.3.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jun-12 14:39 dwiqc-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      428 b- defN 23-Jun-12 14:39 dwiqc-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 14:39 dwiqc-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-12 14:39 dwiqc-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1718 b- defN 23-Jun-12 14:39 dwiqc-0.4.3.dist-info/RECORD
+22 files, 67992 bytes uncompressed, 21682 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.4.2.data/scripts/dwiQC.py
+Filename: dwiqc-0.4.3.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.4.2.dist-info/LICENSE
+Filename: dwiqc-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.4.2.dist-info/METADATA
+Filename: dwiqc-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.4.2.dist-info/WHEEL
+Filename: dwiqc-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.4.2.dist-info/top_level.txt
+Filename: dwiqc-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.4.2.dist-info/RECORD
+Filename: dwiqc-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/tandem.py

```diff
@@ -8,14 +8,16 @@
 import argparse as ap
 import subprocess as sp
 import collections as col
 from xnattagger import Tagger
 from bids import BIDSLayout
 import dwiqc.cli.get as get
 import dwiqc.cli.process as process
+import collections as col
+import yaxil.bids
 
 
 logger = logging.getLogger(__name__)
 
 def do(args):
     if args.insecure:
         logger.warning('disabling ssl certificate verification')
```

## Comparing `dwiqc-0.4.2.data/scripts/dwiQC.py` & `dwiqc-0.4.3.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.4.2.dist-info/LICENSE` & `dwiqc-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

