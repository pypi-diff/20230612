# Comparing `tmp/mypy-boto3-dynamodbstreams-1.26.152.tar.gz` & `tmp/mypy-boto3-dynamodbstreams-1.26.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodbstreams-1.26.152.tar", last modified: Mon Jun 12 19:33:28 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodbstreams-1.26.24.tar", last modified: Tue Dec  6 20:25:48 2022, max compression
```

## Comparing `mypy-boto3-dynamodbstreams-1.26.152.tar` & `mypy-boto3-dynamodbstreams-1.26.24.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:33:28.224150 mypy-boto3-dynamodbstreams-1.26.152/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-12 19:33:28.224150 mypy-boto3-dynamodbstreams-1.26.152/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:33:28.216150 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-12 19:32:27.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-12 19:32:27.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:33:28.216150 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-12 19:33:27.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-12 19:33:28.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:33:27.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:33:27.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 19:33:27.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 19:33:27.000000 mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:33:28.224150 mypy-boto3-dynamodbstreams-1.26.152/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-12 19:32:26.000000 mypy-boto3-dynamodbstreams-1.26.152/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:48.529962 mypy-boto3-dynamodbstreams-1.26.24/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    12801 2022-12-06 20:25:48.521961 mypy-boto3-dynamodbstreams-1.26.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11332 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:48.521961 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5831 2022-12-06 20:25:28.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5821 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8173 2022-12-06 20:25:28.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/literals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8171 2022-12-06 20:25:28.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6282 2022-12-06 20:25:28.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6275 2022-12-06 20:25:28.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:25:48.521961 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12801 2022-12-06 20:25:48.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2022-12-06 20:25:48.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 20:25:48.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 20:25:48.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-06 20:25:48.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2022-12-06 20:25:48.000000 mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-06 20:25:48.529962 mypy-boto3-dynamodbstreams-1.26.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2020 2022-12-06 20:25:27.000000 mypy-boto3-dynamodbstreams-1.26.24/setup.py
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/LICENSE` & `mypy-boto3-dynamodbstreams-1.26.24/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/PKG-INFO` & `mypy-boto3-dynamodbstreams-1.26.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodbstreams
-Version: 1.26.152
-Summary: Type annotations for boto3.DynamoDBStreams 1.26.152 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.24
+Summary: Type annotations for boto3.DynamoDBStreams 1.26.24 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-dynamodbstreams"></a>
 
 # mypy-boto3-dynamodbstreams
 
 [![PyPI - mypy-boto3-dynamodbstreams](https://img.shields.io/pypi/v/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodbstreams?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDBStreams 1.26.152](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[boto3.DynamoDBStreams 1.26.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,24 +303,24 @@
 `mypy_boto3_dynamodbstreams.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
@@ -334,42 +333,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/README.md` & `mypy-boto3-dynamodbstreams-1.26.24/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dynamodbstreams"></a>
 
 # mypy-boto3-dynamodbstreams
 
 [![PyPI - mypy-boto3-dynamodbstreams](https://img.shields.io/pypi/v/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodbstreams?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDBStreams 1.26.152](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[boto3.DynamoDBStreams 1.26.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,24 +272,24 @@
 `mypy_boto3_dynamodbstreams.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
@@ -302,42 +302,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/__main__.py` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDBStreams 1.26.152\nVersion:         1.26.152\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.DynamoDBStreams 1.26.24\nVersion:         1.26.24\nBuilder"
+        " version: 7.11.11\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.152")
+    print("1.26.24")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/client.py` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/client.pyi` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/literals.py` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "KeyTypeType",
     "OperationTypeType",
     "ShardIteratorTypeType",
     "StreamStatusType",
     "StreamViewTypeType",
     "DynamoDBStreamsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 KeyTypeType = Literal["HASH", "RANGE"]
 OperationTypeType = Literal["INSERT", "MODIFY", "REMOVE"]
 ShardIteratorTypeType = Literal[
     "AFTER_SEQUENCE_NUMBER", "AT_SEQUENCE_NUMBER", "LATEST", "TRIM_HORIZON"
 ]
 StreamStatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLING"]
 StreamViewTypeType = Literal["KEYS_ONLY", "NEW_AND_OLD_IMAGES", "NEW_IMAGE", "OLD_IMAGE"]
@@ -79,26 +77,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -184,15 +180,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -203,38 +198,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -247,15 +238,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -274,19 +264,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -324,15 +311,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -366,20 +352,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -408,15 +392,14 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/literals.pyi` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "KeyTypeType",
     "OperationTypeType",
     "ShardIteratorTypeType",
     "StreamStatusType",
     "StreamViewTypeType",
     "DynamoDBStreamsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 KeyTypeType = Literal["HASH", "RANGE"]
 OperationTypeType = Literal["INSERT", "MODIFY", "REMOVE"]
 ShardIteratorTypeType = Literal[
     "AFTER_SEQUENCE_NUMBER", "AT_SEQUENCE_NUMBER", "LATEST", "TRIM_HORIZON"
 ]
 StreamStatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLING"]
 StreamViewTypeType = Literal["KEYS_ONLY", "NEW_AND_OLD_IMAGES", "NEW_IMAGE", "OLD_IMAGE"]
@@ -77,26 +79,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -182,15 +182,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -201,38 +200,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -245,15 +240,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -272,19 +266,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -322,15 +313,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -364,20 +354,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -406,15 +394,14 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/type_defs.py` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttributeValueTypeDef",
     "DescribeStreamInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRecordsInputRequestTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IdentityTypeDef",
     "KeySchemaElementTypeDef",
     "ListStreamsInputRequestTypeDef",
     "StreamTypeDef",
     "StreamRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "RecordTypeDef",
     "ShardTypeDef",
     "GetRecordsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "DescribeStreamOutputTypeDef",
 )
@@ -85,14 +85,25 @@
 
 class DescribeStreamInputRequestTypeDef(
     _RequiredDescribeStreamInputRequestTypeDef, _OptionalDescribeStreamInputRequestTypeDef
 ):
     pass
 
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -129,22 +140,14 @@
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "PrincipalId": str,
         "Type": str,
     },
     total=False,
@@ -188,40 +191,37 @@
         "SequenceNumber": str,
         "SizeBytes": int,
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 SequenceNumberRangeTypeDef = TypedDict(
     "SequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
         "EndingSequenceNumber": str,
     },
     total=False,
 )
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "Streams": List[StreamTypeDef],
         "LastEvaluatedStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "eventID": str,
@@ -246,15 +246,15 @@
 )
 
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamDescriptionTypeDef = TypedDict(
     "StreamDescriptionTypeDef",
     {
         "StreamArn": str,
@@ -270,10 +270,10 @@
     total=False,
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams/type_defs.pyi` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttributeValueTypeDef",
     "DescribeStreamInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRecordsInputRequestTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IdentityTypeDef",
     "KeySchemaElementTypeDef",
     "ListStreamsInputRequestTypeDef",
     "StreamTypeDef",
     "StreamRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "RecordTypeDef",
     "ShardTypeDef",
     "GetRecordsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "DescribeStreamOutputTypeDef",
 )
@@ -82,14 +82,25 @@
 )
 
 class DescribeStreamInputRequestTypeDef(
     _RequiredDescribeStreamInputRequestTypeDef, _OptionalDescribeStreamInputRequestTypeDef
 ):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -122,22 +133,14 @@
 )
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "PrincipalId": str,
         "Type": str,
     },
     total=False,
@@ -181,40 +184,37 @@
         "SequenceNumber": str,
         "SizeBytes": int,
         "StreamViewType": StreamViewTypeType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 SequenceNumberRangeTypeDef = TypedDict(
     "SequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
         "EndingSequenceNumber": str,
     },
     total=False,
 )
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "Streams": List[StreamTypeDef],
         "LastEvaluatedStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "eventID": str,
@@ -239,15 +239,15 @@
 )
 
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamDescriptionTypeDef = TypedDict(
     "StreamDescriptionTypeDef",
     {
         "StreamArn": str,
@@ -263,10 +263,10 @@
     total=False,
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodbstreams
-Version: 1.26.152
-Summary: Type annotations for boto3.DynamoDBStreams 1.26.152 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.24
+Summary: Type annotations for boto3.DynamoDBStreams 1.26.24 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-dynamodbstreams"></a>
 
 # mypy-boto3-dynamodbstreams
 
 [![PyPI - mypy-boto3-dynamodbstreams](https://img.shields.io/pypi/v/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodbstreams?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDBStreams 1.26.152](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[boto3.DynamoDBStreams 1.26.24](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,24 +303,24 @@
 `mypy_boto3_dynamodbstreams.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
@@ -334,42 +333,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt` & `mypy-boto3-dynamodbstreams-1.26.24/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.26.152/setup.py` & `mypy-boto3-dynamodbstreams-1.26.24/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 """
 Setup script for mypy-boto3-dynamodbstreams.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-dynamodbstreams",
-    version="1.26.152",
+    version="1.26.24",
     packages=["mypy_boto3_dynamodbstreams"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDBStreams 1.26.152 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.DynamoDBStreams 1.26.24 service generated with"
+        " mypy-boto3-builder 7.11.11"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 dynamodbstreams type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_dynamodbstreams": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_dynamodbstreams": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

