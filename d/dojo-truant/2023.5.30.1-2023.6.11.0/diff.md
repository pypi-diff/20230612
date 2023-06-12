# Comparing `tmp/dojo_truant-2023.5.30.1.tar.gz` & `tmp/dojo_truant-2023.6.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.5.30.1.tar", last modified: Tue May 30 18:02:09 2023, max compression
+gzip compressed data, was "dojo_truant-2023.6.11.0.tar", last modified: Mon Jun 12 04:05:34 2023, max compression
```

## Comparing `dojo_truant-2023.5.30.1.tar` & `dojo_truant-2023.6.11.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:02:09.000949 dojo_truant-2023.5.30.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 18:02:09.000949 dojo_truant-2023.5.30.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:02:09.000949 dojo_truant-2023.5.30.1/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/development_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/stub_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:02:09.000949 dojo_truant-2023.5.30.1/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 18:02:08.000000 dojo_truant-2023.5.30.1/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 18:02:08.000000 dojo_truant-2023.5.30.1/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:02:08.000000 dojo_truant-2023.5.30.1/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 18:02:08.000000 dojo_truant-2023.5.30.1/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 18:02:08.000000 dojo_truant-2023.5.30.1/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-30 18:01:53.000000 dojo_truant-2023.5.30.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:02:09.000949 dojo_truant-2023.5.30.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:05:34.446391 dojo_truant-2023.6.11.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 04:05:34.446391 dojo_truant-2023.6.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:05:34.442391 dojo_truant-2023.6.11.0/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:05:34.446391 dojo_truant-2023.6.11.0/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 04:05:34.000000 dojo_truant-2023.6.11.0/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 04:05:34.000000 dojo_truant-2023.6.11.0/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:05:34.000000 dojo_truant-2023.6.11.0/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 04:05:34.000000 dojo_truant-2023.6.11.0/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 04:05:34.000000 dojo_truant-2023.6.11.0/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-12 04:05:15.000000 dojo_truant-2023.6.11.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:05:34.446391 dojo_truant-2023.6.11.0/setup.cfg
```

### Comparing `dojo_truant-2023.5.30.1/LICENSE.txt` & `dojo_truant-2023.6.11.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/PKG-INFO` & `dojo_truant-2023.6.11.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.5.30.1
+Version: 2023.6.11.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.5.30.1/dojo/__init__.py` & `dojo_truant-2023.6.11.0/dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/api.py` & `dojo_truant-2023.6.11.0/dojo/api.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/development_environment.py` & `dojo_truant-2023.6.11.0/dojo/development_environment.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/dojo_group.py` & `dojo_truant-2023.6.11.0/dojo/dojo_group.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/engagement.py` & `dojo_truant-2023.6.11.0/dojo/engagement.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/finding.py` & `dojo_truant-2023.6.11.0/dojo/finding.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,18 +37,18 @@
                  "required": False,
                  "regex": "\d{4}-\d{2}-\d{2}"},
         "sla_start_date": {"type": str,
                            "required": False,
                            "regex": "\d{4}-\d{2}-\d{2}"},
         "cwe": {"type": int,
                 "required": False},
-        "cvss3": {"type": str,
+        "cvssv3": {"type": str,
                   "required": False,
                   "cvss": 3},
-        "cvss3_score": {"type": float,
+        "cvssv3_score": {"type": float,
                         "required": False},
         "severity": {"type": str,
                      "required": True,
                      "enum": ("Critical", "High", "Medium", "Low", "Informtional")},
         "description": {"type": str,
                         "required": True},
         "mitigation": {"type": str,
```

### Comparing `dojo_truant-2023.5.30.1/dojo/product.py` & `dojo_truant-2023.6.11.0/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/product_type.py` & `dojo_truant-2023.6.11.0/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/stub_finding.py` & `dojo_truant-2023.6.11.0/dojo/stub_finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/test.py` & `dojo_truant-2023.6.11.0/dojo/test.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/test_type.py` & `dojo_truant-2023.6.11.0/dojo/test_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo/write_chain.py` & `dojo_truant-2023.6.11.0/dojo/write_chain.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.5.30.1/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.6.11.0/dojo_truant.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.5.30.1
+Version: 2023.6.11.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.5.30.1/pyproject.toml` & `dojo_truant-2023.6.11.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.05.30.1"
+version = "2023.6.11.0"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["defectDojo"]
```

