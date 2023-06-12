# Comparing `tmp/tfprimate-0.1.3.tar.gz` & `tmp/tfprimate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfprimate-0.1.3.tar", max compression
+gzip compressed data, was "tfprimate-0.1.4.tar", max compression
```

## Comparing `tfprimate-0.1.3.tar` & `tfprimate-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2023-03-31 09:36:02.867810 tfprimate-0.1.3/LICENSE
--rw-r--r--   0        0        0      269 2023-06-08 10:42:26.695566 tfprimate-0.1.3/README.md
--rw-r--r--   0        0        0      424 2023-06-08 10:46:00.701122 tfprimate-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-31 09:42:11.630126 tfprimate-0.1.3/src/tfprimate/__init__.py
--rw-r--r--   0        0        0     2026 2023-06-08 10:22:12.894932 tfprimate-0.1.3/src/tfprimate/alignment.py
--rw-r--r--   0        0        0      372 2023-03-31 11:03:55.902524 tfprimate-0.1.3/src/tfprimate/phyloTree.py
--rw-r--r--   0        0        0     2520 2023-05-25 09:35:19.392084 tfprimate-0.1.3/src/tfprimate/primate_rnaseq.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 tfprimate-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-31 09:36:02.867810 tfprimate-0.1.4/LICENSE
+-rw-r--r--   0        0        0      269 2023-06-08 10:42:26.695566 tfprimate-0.1.4/README.md
+-rw-r--r--   0        0        0      470 2023-06-12 13:03:23.993699 tfprimate-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-31 09:42:11.630126 tfprimate-0.1.4/src/tfprimate/__init__.py
+-rw-r--r--   0        0        0     2026 2023-06-08 10:22:12.894932 tfprimate-0.1.4/src/tfprimate/alignment.py
+-rw-r--r--   0        0        0      653 2023-06-08 14:54:11.471941 tfprimate-0.1.4/src/tfprimate/getInfo.py
+-rw-r--r--   0        0        0      372 2023-03-31 11:03:55.902524 tfprimate-0.1.4/src/tfprimate/phyloTree.py
+-rw-r--r--   0        0        0     2520 2023-05-25 09:35:19.392084 tfprimate-0.1.4/src/tfprimate/primate_rnaseq.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 tfprimate-0.1.4/PKG-INFO
```

### Comparing `tfprimate-0.1.3/src/tfprimate/alignment.py` & `tfprimate-0.1.4/src/tfprimate/alignment.py`

 * *Files identical despite different names*

### Comparing `tfprimate-0.1.3/src/tfprimate/primate_rnaseq.py` & `tfprimate-0.1.4/src/tfprimate/primate_rnaseq.py`

 * *Files identical despite different names*

### Comparing `tfprimate-0.1.3/PKG-INFO` & `tfprimate-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfprimate
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for primate transcription factors database
 License: MIT
 Author: Yao-Chung Chen, Ekin Deniz Aksu, Melanie Sarfert, Katja Nowick
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

