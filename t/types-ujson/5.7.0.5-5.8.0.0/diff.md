# Comparing `tmp/types-ujson-5.7.0.5.tar.gz` & `tmp/types-ujson-5.8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ujson-5.7.0.5.tar", last modified: Mon May  1 18:18:31 2023, max compression
+gzip compressed data, was "types-ujson-5.8.0.0.tar", last modified: Mon Jun 12 01:37:12 2023, max compression
```

## Comparing `types-ujson-5.7.0.5.tar` & `types-ujson-5.8.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:18:31.790346 types-ujson-5.7.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-01 18:18:28.000000 types-ujson-5.7.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 18:18:28.000000 types-ujson-5.7.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 18:18:31.790346 types-ujson-5.7.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:18:31.790346 types-ujson-5.7.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-01 18:18:28.000000 types-ujson-5.7.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:18:31.790346 types-ujson-5.7.0.5/types_ujson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 18:18:31.000000 types-ujson-5.7.0.5/types_ujson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 18:18:31.000000 types-ujson-5.7.0.5/types_ujson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:18:31.000000 types-ujson-5.7.0.5/types_ujson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 18:18:31.000000 types-ujson-5.7.0.5/types_ujson.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:18:31.790346 types-ujson-5.7.0.5/ujson-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 18:18:28.000000 types-ujson-5.7.0.5/ujson-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-01 18:18:28.000000 types-ujson-5.7.0.5/ujson-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/types_ujson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/ujson-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/ujson-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/ujson-stubs/__init__.pyi
```

### Comparing `types-ujson-5.7.0.5/CHANGELOG.md` & `types-ujson-5.8.0.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 5.8.0.0 (2023-06-12)
+
+[stubsabot] Bump ujson to 5.8.* (#10302)
+
+Release: https://pypi.org/pypi/ujson/5.8.0
+Homepage: https://github.com/ultrajson/ultrajson
+Diff: https://github.com/ultrajson/ultrajson/compare/5.7.0...5.8.0
+
+Stubsabot analysis of the diff between the two releases:
+ - Total lines of Python code added: 15.
+ - Total lines of Python code deleted: 17.
+
 ## 5.7.0.5 (2023-05-01)
 
 Convert the remaining ujson uses of AnyStr (#10086)
 
 Followup from #10081
 
 ## 5.7.0.4 (2023-04-25)
```

### Comparing `types-ujson-5.7.0.5/PKG-INFO` & `types-ujson-5.8.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.7.0.5
+Version: 5.8.0.0
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d208d5a83394e9ad1d0dd5d567818c597dfaa28f`.
+This package was generated from typeshed commit `6a94c9d677db9e9f85d764cc46294fd5c5e2a4b8`.
```

### Comparing `types-ujson-5.7.0.5/setup.py` & `types-ujson-5.8.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d208d5a83394e9ad1d0dd5d567818c597dfaa28f`.
+This package was generated from typeshed commit `6a94c9d677db9e9f85d764cc46294fd5c5e2a4b8`.
 '''.lstrip()
 
 setup(name=name,
-      version="5.7.0.5",
+      version="5.8.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md",
```

### Comparing `types-ujson-5.7.0.5/types_ujson.egg-info/PKG-INFO` & `types-ujson-5.8.0.0/types_ujson.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.7.0.5
+Version: 5.8.0.0
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d208d5a83394e9ad1d0dd5d567818c597dfaa28f`.
+This package was generated from typeshed commit `6a94c9d677db9e9f85d764cc46294fd5c5e2a4b8`.
```

### Comparing `types-ujson-5.7.0.5/ujson-stubs/__init__.pyi` & `types-ujson-5.8.0.0/ujson-stubs/__init__.pyi`

 * *Files identical despite different names*

