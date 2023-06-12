# Comparing `tmp/vembrane-1.0.1.tar.gz` & `tmp/vembrane-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vembrane-1.0.1.tar", max compression
+gzip compressed data, was "vembrane-1.0.2.tar", max compression
```

## Comparing `vembrane-1.0.1.tar` & `vembrane-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-04-27 11:19:50.898834 vembrane-1.0.1/LICENSE
--rw-r--r--   0        0        0    19775 2023-04-27 11:19:50.898834 vembrane-1.0.1/README.md
--rw-r--r--   0        0        0     1101 2023-04-27 11:19:50.898834 vembrane-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      325 2023-04-27 11:19:50.906834 vembrane-1.0.1/vembrane/__init__.py
--rw-r--r--   0        0        0    28683 2023-04-27 11:19:50.906834 vembrane-1.0.1/vembrane/ann_types.py
--rw-r--r--   0        0        0      876 2023-04-27 11:19:50.906834 vembrane-1.0.1/vembrane/cli.py
--rw-r--r--   0        0        0     4166 2023-04-27 11:19:50.906834 vembrane-1.0.1/vembrane/common.py
--rw-r--r--   0        0        0     4667 2023-04-27 11:19:50.906834 vembrane-1.0.1/vembrane/errors.py
--rw-r--r--   0        0        0     5259 2023-04-27 11:19:50.906834 vembrane-1.0.1/vembrane/globals.py
--rw-r--r--   0        0        0        0 2023-04-27 11:19:50.910834 vembrane-1.0.1/vembrane/modules/__init__.py
--rw-r--r--   0        0        0     5880 2023-04-27 11:19:50.910834 vembrane-1.0.1/vembrane/modules/annotate.py
--rw-r--r--   0        0        0    13278 2023-04-27 11:19:50.910834 vembrane-1.0.1/vembrane/modules/filter.py
--rw-r--r--   0        0        0    10785 2023-04-27 11:19:50.910834 vembrane-1.0.1/vembrane/modules/table.py
--rw-r--r--   0        0        0     6935 2023-04-27 11:19:50.910834 vembrane-1.0.1/vembrane/modules/tag.py
--rw-r--r--   0        0        0    13621 2023-04-27 11:19:50.910834 vembrane-1.0.1/vembrane/representations.py
--rw-r--r--   0        0        0    20540 1970-01-01 00:00:00.000000 vembrane-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-12 16:11:32.003118 vembrane-1.0.2/LICENSE
+-rw-r--r--   0        0        0    19775 2023-06-12 16:11:32.003118 vembrane-1.0.2/README.md
+-rw-r--r--   0        0        0     1101 2023-06-12 16:11:32.007118 vembrane-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/__init__.py
+-rw-r--r--   0        0        0    28683 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/ann_types.py
+-rw-r--r--   0        0        0      876 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/cli.py
+-rw-r--r--   0        0        0     4166 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/common.py
+-rw-r--r--   0        0        0     4667 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/errors.py
+-rw-r--r--   0        0        0     5259 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/globals.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/__init__.py
+-rw-r--r--   0        0        0     5880 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/annotate.py
+-rw-r--r--   0        0        0    13278 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/filter.py
+-rw-r--r--   0        0        0    11108 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/table.py
+-rw-r--r--   0        0        0     6935 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/tag.py
+-rw-r--r--   0        0        0    13621 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/representations.py
+-rw-r--r--   0        0        0    20540 1970-01-01 00:00:00.000000 vembrane-1.0.2/PKG-INFO
```

### Comparing `vembrane-1.0.1/LICENSE` & `vembrane-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/README.md` & `vembrane-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/pyproject.toml` & `vembrane-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vembrane"
-version = "1.0.1"
+version = "1.0.2"
 description = "Filter VCF/BCF files with Python expressions."
 authors = ["Till Hartmann", "Christopher Schröder", "Johannes Köster", "Jan Forster", "Marcel Bargull", "Felix Mölder", "Elias Kuthe", "David Lähnemann"]
 readme = "README.md"
 homepage = "https://github.com/vembrane/vembrane"
 repository = "https://github.com/vembrane/vembrane"
 
 [tool.poetry.scripts]
```

### Comparing `vembrane-1.0.1/vembrane/ann_types.py` & `vembrane-1.0.2/vembrane/ann_types.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/cli.py` & `vembrane-1.0.2/vembrane/cli.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/common.py` & `vembrane-1.0.2/vembrane/common.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/errors.py` & `vembrane-1.0.2/vembrane/errors.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/globals.py` & `vembrane-1.0.2/vembrane/globals.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/modules/annotate.py` & `vembrane-1.0.2/vembrane/modules/annotate.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/modules/filter.py` & `vembrane-1.0.2/vembrane/modules/filter.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/modules/table.py` & `vembrane-1.0.2/vembrane/modules/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,22 @@
         if env.expression_annotations():
             # if the expression contains a reference to the ANN field
             # get all annotations from the record.info field
             # (or supply an empty ANN value if the record has no ANN field)
             try:
                 annotations = record.info[ann_key]
             except KeyError:
-                annotations = [""]
+                num_ann_entries = len(env._annotation._ann_conv.keys())
+                empty = "|" * num_ann_entries
+                print(
+                    f"No ANN field found in record {idx}, "
+                    f"replacing with NAs (i.e. 'ANN={empty}')",
+                    file=sys.stderr,
+                )
+                annotations = [empty]
             for annotation in annotations:
                 if long:
                     yield from env.table(annotation)
                 else:
                     yield env.table(annotation)
         else:
             if long:
```

### Comparing `vembrane-1.0.1/vembrane/modules/tag.py` & `vembrane-1.0.2/vembrane/modules/tag.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/vembrane/representations.py` & `vembrane-1.0.2/vembrane/representations.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.1/PKG-INFO` & `vembrane-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vembrane
-Version: 1.0.1
+Version: 1.0.2
 Summary: Filter VCF/BCF files with Python expressions.
 Home-page: https://github.com/vembrane/vembrane
 Author: Till Hartmann
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

