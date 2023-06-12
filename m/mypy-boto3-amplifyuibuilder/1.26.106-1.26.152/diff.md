# Comparing `tmp/mypy-boto3-amplifyuibuilder-1.26.106.tar.gz` & `tmp/mypy-boto3-amplifyuibuilder-1.26.152.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.26.106.tar", last modified: Tue Apr  4 19:33:30 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.26.152.tar", last modified: Mon Jun 12 19:33:28 2023, max compression
```

## Comparing `mypy-boto3-amplifyuibuilder-1.26.106.tar` & `mypy-boto3-amplifyuibuilder-1.26.152.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:33:30.525993 mypy-boto3-amplifyuibuilder-1.26.106/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-04-04 19:33:30.525993 mypy-boto3-amplifyuibuilder-1.26.106/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:33:30.521993 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39339 2023-04-04 19:32:05.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39265 2023-04-04 19:32:05.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-04 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:33:30.521993 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-04-04 19:33:30.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-04 19:33:30.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:33:30.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:33:30.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 19:33:30.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-04 19:33:30.000000 mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:33:30.525993 mypy-boto3-amplifyuibuilder-1.26.106/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-04 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.26.106/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:33:28.200150 mypy-boto3-amplifyuibuilder-1.26.152/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-06-12 19:33:28.200150 mypy-boto3-amplifyuibuilder-1.26.152/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:33:28.184150 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21995 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-12 19:32:14.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-12 19:32:14.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48039 2023-06-12 19:32:15.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47947 2023-06-12 19:32:14.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 19:32:13.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:33:28.200150 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-06-12 19:33:27.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-12 19:33:28.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:33:27.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:33:27.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 19:33:27.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 19:33:27.000000 mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:33:28.200150 mypy-boto3-amplifyuibuilder-1.26.152/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-12 19:32:12.000000 mypy-boto3-amplifyuibuilder-1.26.152/setup.py
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/LICENSE` & `mypy-boto3-amplifyuibuilder-1.26.152/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.26.152/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.26.106
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.26.106 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.152
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.26.152 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifyuibuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.26.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.26.152](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -284,76 +284,97 @@
 from boto3.session import Session
 
 from mypy_boto3_amplifyuibuilder import AmplifyUIBuilderClient
 from mypy_boto3_amplifyuibuilder.paginator import (
     ExportComponentsPaginator,
     ExportFormsPaginator,
     ExportThemesPaginator,
+    ListCodegenJobsPaginator,
     ListComponentsPaginator,
     ListFormsPaginator,
     ListThemesPaginator,
 )
 
 client: AmplifyUIBuilderClient = Session().client("amplifyuibuilder")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 export_components_paginator: ExportComponentsPaginator = client.get_paginator("export_components")
 export_forms_paginator: ExportFormsPaginator = client.get_paginator("export_forms")
 export_themes_paginator: ExportThemesPaginator = client.get_paginator("export_themes")
+list_codegen_jobs_paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
 list_forms_paginator: ListFormsPaginator = client.get_paginator("list_forms")
 list_themes_paginator: ListThemesPaginator = client.get_paginator("list_themes")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_amplifyuibuilder.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.literals import (
+    CodegenGenericDataFieldDataTypeType,
+    CodegenJobGenericDataSourceTypeType,
+    CodegenJobStatusType,
     ExportComponentsPaginatorName,
     ExportFormsPaginatorName,
     ExportThemesPaginatorName,
     FixedPositionType,
     FormActionTypeType,
     FormButtonsPositionType,
     FormDataSourceTypeType,
+    GenericDataRelationshipTypeType,
+    JSModuleType,
+    JSScriptType,
+    JSTargetType,
     LabelDecoratorType,
+    ListCodegenJobsPaginatorName,
     ListComponentsPaginatorName,
     ListFormsPaginatorName,
     ListThemesPaginatorName,
     SortDirectionType,
     StorageAccessLevelType,
     TokenProvidersType,
     AmplifyUIBuilderServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ExportComponentsPaginatorName) -> bool:
+def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     ActionParametersTypeDef,
+    CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeTypeDef,
+    CodegenJobAssetTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    CodegenJobSummaryTypeDef,
+    CodegenJobTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentBindingPropertiesValueTypeDef,
     ComponentChildTypeDef,
     ComponentConditionPropertyTypeDef,
     ComponentDataConfigurationTypeDef,
     ComponentEventTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
@@ -399,42 +420,51 @@
     FormInputBindingPropertiesValueTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
     FormInputValuePropertyTypeDef,
     FormStyleConfigTypeDef,
     FormStyleTypeDef,
     FormSummaryTypeDef,
     FormTypeDef,
+    GetCodegenJobRequestRequestTypeDef,
+    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
     GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
     GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
     GetThemeResponseTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListCodegenJobsRequestRequestTypeDef,
+    ListCodegenJobsResponseTypeDef,
     ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListComponentsResponseTypeDef,
     ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
     ListFormsResponseTypeDef,
     ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
     ListThemesResponseTypeDef,
     MutationActionSetStateParameterTypeDef,
     PaginatorConfigTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenRequestRequestTypeDef,
     RefreshTokenResponseTypeDef,
     ResponseMetadataTypeDef,
     SectionalElementTypeDef,
     SortPropertyTypeDef,
+    StartCodegenJobDataTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    StartCodegenJobResponseTypeDef,
     ThemeSummaryTypeDef,
     ThemeTypeDef,
     ThemeValueTypeDef,
     ThemeValuesTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateComponentResponseTypeDef,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/README.md` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,52 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-amplifyuibuilder
+Version: 1.26.152
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.26.152 service generated with mypy-boto3-builder 7.14.5
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-amplifyuibuilder"></a>
 
 # mypy-boto3-amplifyuibuilder
 
 [![PyPI - mypy-boto3-amplifyuibuilder](https://img.shields.io/pypi/v/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifyuibuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.26.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.26.152](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -252,76 +284,97 @@
 from boto3.session import Session
 
 from mypy_boto3_amplifyuibuilder import AmplifyUIBuilderClient
 from mypy_boto3_amplifyuibuilder.paginator import (
     ExportComponentsPaginator,
     ExportFormsPaginator,
     ExportThemesPaginator,
+    ListCodegenJobsPaginator,
     ListComponentsPaginator,
     ListFormsPaginator,
     ListThemesPaginator,
 )
 
 client: AmplifyUIBuilderClient = Session().client("amplifyuibuilder")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 export_components_paginator: ExportComponentsPaginator = client.get_paginator("export_components")
 export_forms_paginator: ExportFormsPaginator = client.get_paginator("export_forms")
 export_themes_paginator: ExportThemesPaginator = client.get_paginator("export_themes")
+list_codegen_jobs_paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
 list_forms_paginator: ListFormsPaginator = client.get_paginator("list_forms")
 list_themes_paginator: ListThemesPaginator = client.get_paginator("list_themes")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_amplifyuibuilder.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.literals import (
+    CodegenGenericDataFieldDataTypeType,
+    CodegenJobGenericDataSourceTypeType,
+    CodegenJobStatusType,
     ExportComponentsPaginatorName,
     ExportFormsPaginatorName,
     ExportThemesPaginatorName,
     FixedPositionType,
     FormActionTypeType,
     FormButtonsPositionType,
     FormDataSourceTypeType,
+    GenericDataRelationshipTypeType,
+    JSModuleType,
+    JSScriptType,
+    JSTargetType,
     LabelDecoratorType,
+    ListCodegenJobsPaginatorName,
     ListComponentsPaginatorName,
     ListFormsPaginatorName,
     ListThemesPaginatorName,
     SortDirectionType,
     StorageAccessLevelType,
     TokenProvidersType,
     AmplifyUIBuilderServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ExportComponentsPaginatorName) -> bool:
+def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     ActionParametersTypeDef,
+    CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeTypeDef,
+    CodegenJobAssetTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    CodegenJobSummaryTypeDef,
+    CodegenJobTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentBindingPropertiesValueTypeDef,
     ComponentChildTypeDef,
     ComponentConditionPropertyTypeDef,
     ComponentDataConfigurationTypeDef,
     ComponentEventTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
@@ -367,42 +420,51 @@
     FormInputBindingPropertiesValueTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
     FormInputValuePropertyTypeDef,
     FormStyleConfigTypeDef,
     FormStyleTypeDef,
     FormSummaryTypeDef,
     FormTypeDef,
+    GetCodegenJobRequestRequestTypeDef,
+    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
     GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
     GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
     GetThemeResponseTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListCodegenJobsRequestRequestTypeDef,
+    ListCodegenJobsResponseTypeDef,
     ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListComponentsResponseTypeDef,
     ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
     ListFormsResponseTypeDef,
     ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
     ListThemesResponseTypeDef,
     MutationActionSetStateParameterTypeDef,
     PaginatorConfigTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenRequestRequestTypeDef,
     RefreshTokenResponseTypeDef,
     ResponseMetadataTypeDef,
     SectionalElementTypeDef,
     SortPropertyTypeDef,
+    StartCodegenJobDataTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    StartCodegenJobResponseTypeDef,
     ThemeSummaryTypeDef,
     ThemeTypeDef,
     ThemeValueTypeDef,
     ThemeValuesTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateComponentResponseTypeDef,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/__init__.py` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -7,46 +7,49 @@
     from boto3.session import Session
     from mypy_boto3_amplifyuibuilder import (
         AmplifyUIBuilderClient,
         Client,
         ExportComponentsPaginator,
         ExportFormsPaginator,
         ExportThemesPaginator,
+        ListCodegenJobsPaginator,
         ListComponentsPaginator,
         ListFormsPaginator,
         ListThemesPaginator,
     )
 
     session = Session()
     client: AmplifyUIBuilderClient = session.client("amplifyuibuilder")
 
     export_components_paginator: ExportComponentsPaginator = client.get_paginator("export_components")
     export_forms_paginator: ExportFormsPaginator = client.get_paginator("export_forms")
     export_themes_paginator: ExportThemesPaginator = client.get_paginator("export_themes")
+    list_codegen_jobs_paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_forms_paginator: ListFormsPaginator = client.get_paginator("list_forms")
     list_themes_paginator: ListThemesPaginator = client.get_paginator("list_themes")
     ```
 """
 from .client import AmplifyUIBuilderClient
 from .paginator import (
     ExportComponentsPaginator,
     ExportFormsPaginator,
     ExportThemesPaginator,
+    ListCodegenJobsPaginator,
     ListComponentsPaginator,
     ListFormsPaginator,
     ListThemesPaginator,
 )
 
 Client = AmplifyUIBuilderClient
 
-
 __all__ = (
     "AmplifyUIBuilderClient",
     "Client",
     "ExportComponentsPaginator",
     "ExportFormsPaginator",
     "ExportThemesPaginator",
+    "ListCodegenJobsPaginator",
     "ListComponentsPaginator",
     "ListFormsPaginator",
     "ListThemesPaginator",
 )
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/__init__.pyi` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,45 +7,50 @@
     from boto3.session import Session
     from mypy_boto3_amplifyuibuilder import (
         AmplifyUIBuilderClient,
         Client,
         ExportComponentsPaginator,
         ExportFormsPaginator,
         ExportThemesPaginator,
+        ListCodegenJobsPaginator,
         ListComponentsPaginator,
         ListFormsPaginator,
         ListThemesPaginator,
     )
 
     session = Session()
     client: AmplifyUIBuilderClient = session.client("amplifyuibuilder")
 
     export_components_paginator: ExportComponentsPaginator = client.get_paginator("export_components")
     export_forms_paginator: ExportFormsPaginator = client.get_paginator("export_forms")
     export_themes_paginator: ExportThemesPaginator = client.get_paginator("export_themes")
+    list_codegen_jobs_paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_forms_paginator: ListFormsPaginator = client.get_paginator("list_forms")
     list_themes_paginator: ListThemesPaginator = client.get_paginator("list_themes")
     ```
 """
 from .client import AmplifyUIBuilderClient
 from .paginator import (
     ExportComponentsPaginator,
     ExportFormsPaginator,
     ExportThemesPaginator,
+    ListCodegenJobsPaginator,
     ListComponentsPaginator,
     ListFormsPaginator,
     ListThemesPaginator,
 )
 
 Client = AmplifyUIBuilderClient
 
+
 __all__ = (
     "AmplifyUIBuilderClient",
     "Client",
     "ExportComponentsPaginator",
     "ExportFormsPaginator",
     "ExportThemesPaginator",
+    "ListCodegenJobsPaginator",
     "ListComponentsPaginator",
     "ListFormsPaginator",
     "ListThemesPaginator",
 )
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/__main__.py` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyUIBuilder 1.26.106\nVersion:         1.26.106\nBuilder"
+        "Type annotations for boto3.AmplifyUIBuilder 1.26.152\nVersion:         1.26.152\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.106")
+    print("1.26.152")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/client.py` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ExportComponentsPaginator,
     ExportFormsPaginator,
     ExportThemesPaginator,
+    ListCodegenJobsPaginator,
     ListComponentsPaginator,
     ListFormsPaginator,
     ListThemesPaginator,
 )
 from .type_defs import (
     CreateComponentDataTypeDef,
     CreateComponentResponseTypeDef,
@@ -35,24 +36,28 @@
     CreateThemeResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
     ExchangeCodeForTokenResponseTypeDef,
     ExportComponentsResponseTypeDef,
     ExportFormsResponseTypeDef,
     ExportThemesResponseTypeDef,
+    GetCodegenJobResponseTypeDef,
     GetComponentResponseTypeDef,
     GetFormResponseTypeDef,
     GetMetadataResponseTypeDef,
     GetThemeResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListFormsResponseTypeDef,
     ListThemesResponseTypeDef,
     PutMetadataFlagBodyTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenResponseTypeDef,
+    StartCodegenJobDataTypeDef,
+    StartCodegenJobResponseTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentResponseTypeDef,
     UpdateFormDataTypeDef,
     UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
     UpdateThemeResponseTypeDef,
 )
@@ -77,14 +82,15 @@
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     ResourceConflictException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
+    ThrottlingException: Type[BotocoreClientError]
     UnauthorizedException: Type[BotocoreClientError]
 
 
 class AmplifyUIBuilderClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/)
@@ -137,15 +143,15 @@
         *,
         appId: str,
         environmentName: str,
         formToCreate: "CreateFormDataTypeDef",
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
-        Creates a new form for an Amplify app.
+        Creates a new form for an Amplify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_form)
         """
 
     def create_theme(
         self,
@@ -245,14 +251,24 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#generate_presigned_url)
         """
 
+    def get_codegen_job(
+        self, *, appId: str, environmentName: str, id: str
+    ) -> GetCodegenJobResponseTypeDef:
+        """
+        Returns an existing code generation job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_codegen_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_codegen_job)
+        """
+
     def get_component(
         self, *, appId: str, environmentName: str, id: str
     ) -> GetComponentResponseTypeDef:
         """
         Returns an existing component for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_component)
@@ -279,14 +295,25 @@
         """
         Returns an existing theme for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_theme)
         """
 
+    def list_codegen_jobs(
+        self, *, appId: str, environmentName: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListCodegenJobsResponseTypeDef:
+        """
+        Retrieves a list of code generation jobs for a specified Amplify app and backend
+        environment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_codegen_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#list_codegen_jobs)
+        """
+
     def list_components(
         self, *, appId: str, environmentName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListComponentsResponseTypeDef:
         """
         Retrieves a list of components for a specified Amplify app and backend
         environment.
 
@@ -335,14 +362,30 @@
         """
         Refreshes a previously issued access token that might have expired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#refresh_token)
         """
 
+    def start_codegen_job(
+        self,
+        *,
+        appId: str,
+        environmentName: str,
+        codegenJobToCreate: "StartCodegenJobDataTypeDef",
+        clientToken: str = ...
+    ) -> StartCodegenJobResponseTypeDef:
+        """
+        Starts a code generation job for for a specified Amplify app and backend
+        environment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#start_codegen_job)
+        """
+
     def update_component(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
         updatedComponent: "UpdateComponentDataTypeDef",
@@ -407,14 +450,23 @@
     def get_paginator(self, operation_name: Literal["export_themes"]) -> ExportThemesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_codegen_jobs"]
+    ) -> ListCodegenJobsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_components"]) -> ListComponentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/client.pyi` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import (
     ExportComponentsPaginator,
     ExportFormsPaginator,
     ExportThemesPaginator,
+    ListCodegenJobsPaginator,
     ListComponentsPaginator,
     ListFormsPaginator,
     ListThemesPaginator,
 )
 from .type_defs import (
     CreateComponentDataTypeDef,
     CreateComponentResponseTypeDef,
@@ -35,24 +36,28 @@
     CreateThemeResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
     ExchangeCodeForTokenResponseTypeDef,
     ExportComponentsResponseTypeDef,
     ExportFormsResponseTypeDef,
     ExportThemesResponseTypeDef,
+    GetCodegenJobResponseTypeDef,
     GetComponentResponseTypeDef,
     GetFormResponseTypeDef,
     GetMetadataResponseTypeDef,
     GetThemeResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListFormsResponseTypeDef,
     ListThemesResponseTypeDef,
     PutMetadataFlagBodyTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenResponseTypeDef,
+    StartCodegenJobDataTypeDef,
+    StartCodegenJobResponseTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentResponseTypeDef,
     UpdateFormDataTypeDef,
     UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
     UpdateThemeResponseTypeDef,
 )
@@ -74,14 +79,15 @@
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     ResourceConflictException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
+    ThrottlingException: Type[BotocoreClientError]
     UnauthorizedException: Type[BotocoreClientError]
 
 class AmplifyUIBuilderClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/)
     """
@@ -129,15 +135,15 @@
         *,
         appId: str,
         environmentName: str,
         formToCreate: "CreateFormDataTypeDef",
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
-        Creates a new form for an Amplify app.
+        Creates a new form for an Amplify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_form)
         """
     def create_theme(
         self,
         *,
@@ -227,14 +233,23 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#generate_presigned_url)
         """
+    def get_codegen_job(
+        self, *, appId: str, environmentName: str, id: str
+    ) -> GetCodegenJobResponseTypeDef:
+        """
+        Returns an existing code generation job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_codegen_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_codegen_job)
+        """
     def get_component(
         self, *, appId: str, environmentName: str, id: str
     ) -> GetComponentResponseTypeDef:
         """
         Returns an existing component for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_component)
@@ -257,14 +272,24 @@
     def get_theme(self, *, appId: str, environmentName: str, id: str) -> GetThemeResponseTypeDef:
         """
         Returns an existing theme for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_theme)
         """
+    def list_codegen_jobs(
+        self, *, appId: str, environmentName: str, nextToken: str = ..., maxResults: int = ...
+    ) -> ListCodegenJobsResponseTypeDef:
+        """
+        Retrieves a list of code generation jobs for a specified Amplify app and backend
+        environment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.list_codegen_jobs)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#list_codegen_jobs)
+        """
     def list_components(
         self, *, appId: str, environmentName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListComponentsResponseTypeDef:
         """
         Retrieves a list of components for a specified Amplify app and backend
         environment.
 
@@ -308,14 +333,29 @@
     ) -> RefreshTokenResponseTypeDef:
         """
         Refreshes a previously issued access token that might have expired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#refresh_token)
         """
+    def start_codegen_job(
+        self,
+        *,
+        appId: str,
+        environmentName: str,
+        codegenJobToCreate: "StartCodegenJobDataTypeDef",
+        clientToken: str = ...
+    ) -> StartCodegenJobResponseTypeDef:
+        """
+        Starts a code generation job for for a specified Amplify app and backend
+        environment.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#start_codegen_job)
+        """
     def update_component(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
         updatedComponent: "UpdateComponentDataTypeDef",
@@ -374,14 +414,22 @@
     @overload
     def get_paginator(self, operation_name: Literal["export_themes"]) -> ExportThemesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_paginator)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_codegen_jobs"]
+    ) -> ListCodegenJobsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_components"]) -> ListComponentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#get_paginator)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_forms"]) -> ListFormsPaginator:
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/literals.py` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/literals.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,58 +2,92 @@
 Type annotations for amplifyuibuilder service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifyuibuilder.literals import ExportComponentsPaginatorName
+    from mypy_boto3_amplifyuibuilder.literals import CodegenGenericDataFieldDataTypeType
 
-    data: ExportComponentsPaginatorName = "export_components"
+    data: CodegenGenericDataFieldDataTypeType = "AWSDate"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
+    "CodegenGenericDataFieldDataTypeType",
+    "CodegenJobGenericDataSourceTypeType",
+    "CodegenJobStatusType",
     "ExportComponentsPaginatorName",
     "ExportFormsPaginatorName",
     "ExportThemesPaginatorName",
     "FixedPositionType",
     "FormActionTypeType",
     "FormButtonsPositionType",
     "FormDataSourceTypeType",
+    "GenericDataRelationshipTypeType",
+    "JSModuleType",
+    "JSScriptType",
+    "JSTargetType",
     "LabelDecoratorType",
+    "ListCodegenJobsPaginatorName",
     "ListComponentsPaginatorName",
     "ListFormsPaginatorName",
     "ListThemesPaginatorName",
     "SortDirectionType",
     "StorageAccessLevelType",
     "TokenProvidersType",
     "AmplifyUIBuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
+CodegenGenericDataFieldDataTypeType = Literal[
+    "AWSDate",
+    "AWSDateTime",
+    "AWSEmail",
+    "AWSIPAddress",
+    "AWSJSON",
+    "AWSPhone",
+    "AWSTime",
+    "AWSTimestamp",
+    "AWSURL",
+    "Boolean",
+    "Enum",
+    "Float",
+    "ID",
+    "Int",
+    "Model",
+    "NonModel",
+    "String",
+]
+CodegenJobGenericDataSourceTypeType = Literal["DataStore"]
+CodegenJobStatusType = Literal["failed", "in_progress", "succeeded"]
 ExportComponentsPaginatorName = Literal["export_components"]
 ExportFormsPaginatorName = Literal["export_forms"]
 ExportThemesPaginatorName = Literal["export_themes"]
 FixedPositionType = Literal["first"]
 FormActionTypeType = Literal["create", "update"]
 FormButtonsPositionType = Literal["bottom", "top", "top_and_bottom"]
 FormDataSourceTypeType = Literal["Custom", "DataStore"]
+GenericDataRelationshipTypeType = Literal["BELONGS_TO", "HAS_MANY", "HAS_ONE"]
+JSModuleType = Literal["es2020", "esnext"]
+JSScriptType = Literal["js", "jsx", "tsx"]
+JSTargetType = Literal["es2015", "es2020"]
 LabelDecoratorType = Literal["none", "optional", "required"]
+ListCodegenJobsPaginatorName = Literal["list_codegen_jobs"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListFormsPaginatorName = Literal["list_forms"]
 ListThemesPaginatorName = Literal["list_themes"]
 SortDirectionType = Literal["ASC", "DESC"]
 StorageAccessLevelType = Literal["private", "protected", "public"]
 TokenProvidersType = Literal["figma"]
 AmplifyUIBuilderServiceName = Literal["amplifyuibuilder"]
@@ -264,14 +298,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -290,16 +325,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -414,27 +452,29 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "export_components",
     "export_forms",
     "export_themes",
+    "list_codegen_jobs",
     "list_components",
     "list_forms",
     "list_themes",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/literals.pyi` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/literals.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -2,56 +2,90 @@
 Type annotations for amplifyuibuilder service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifyuibuilder.literals import ExportComponentsPaginatorName
+    from mypy_boto3_amplifyuibuilder.literals import CodegenGenericDataFieldDataTypeType
 
-    data: ExportComponentsPaginatorName = "export_components"
+    data: CodegenGenericDataFieldDataTypeType = "AWSDate"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "CodegenGenericDataFieldDataTypeType",
+    "CodegenJobGenericDataSourceTypeType",
+    "CodegenJobStatusType",
     "ExportComponentsPaginatorName",
     "ExportFormsPaginatorName",
     "ExportThemesPaginatorName",
     "FixedPositionType",
     "FormActionTypeType",
     "FormButtonsPositionType",
     "FormDataSourceTypeType",
+    "GenericDataRelationshipTypeType",
+    "JSModuleType",
+    "JSScriptType",
+    "JSTargetType",
     "LabelDecoratorType",
+    "ListCodegenJobsPaginatorName",
     "ListComponentsPaginatorName",
     "ListFormsPaginatorName",
     "ListThemesPaginatorName",
     "SortDirectionType",
     "StorageAccessLevelType",
     "TokenProvidersType",
     "AmplifyUIBuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+CodegenGenericDataFieldDataTypeType = Literal[
+    "AWSDate",
+    "AWSDateTime",
+    "AWSEmail",
+    "AWSIPAddress",
+    "AWSJSON",
+    "AWSPhone",
+    "AWSTime",
+    "AWSTimestamp",
+    "AWSURL",
+    "Boolean",
+    "Enum",
+    "Float",
+    "ID",
+    "Int",
+    "Model",
+    "NonModel",
+    "String",
+]
+CodegenJobGenericDataSourceTypeType = Literal["DataStore"]
+CodegenJobStatusType = Literal["failed", "in_progress", "succeeded"]
 ExportComponentsPaginatorName = Literal["export_components"]
 ExportFormsPaginatorName = Literal["export_forms"]
 ExportThemesPaginatorName = Literal["export_themes"]
 FixedPositionType = Literal["first"]
 FormActionTypeType = Literal["create", "update"]
 FormButtonsPositionType = Literal["bottom", "top", "top_and_bottom"]
 FormDataSourceTypeType = Literal["Custom", "DataStore"]
+GenericDataRelationshipTypeType = Literal["BELONGS_TO", "HAS_MANY", "HAS_ONE"]
+JSModuleType = Literal["es2020", "esnext"]
+JSScriptType = Literal["js", "jsx", "tsx"]
+JSTargetType = Literal["es2015", "es2020"]
 LabelDecoratorType = Literal["none", "optional", "required"]
+ListCodegenJobsPaginatorName = Literal["list_codegen_jobs"]
 ListComponentsPaginatorName = Literal["list_components"]
 ListFormsPaginatorName = Literal["list_forms"]
 ListThemesPaginatorName = Literal["list_themes"]
 SortDirectionType = Literal["ASC", "DESC"]
 StorageAccessLevelType = Literal["private", "protected", "public"]
 TokenProvidersType = Literal["figma"]
 AmplifyUIBuilderServiceName = Literal["amplifyuibuilder"]
@@ -262,14 +296,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -288,16 +323,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -412,27 +450,29 @@
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
     "export_components",
     "export_forms",
     "export_themes",
+    "list_codegen_jobs",
     "list_components",
     "list_forms",
     "list_themes",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
+    "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/paginator.py` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,108 +9,120 @@
     from boto3.session import Session
 
     from mypy_boto3_amplifyuibuilder.client import AmplifyUIBuilderClient
     from mypy_boto3_amplifyuibuilder.paginator import (
         ExportComponentsPaginator,
         ExportFormsPaginator,
         ExportThemesPaginator,
+        ListCodegenJobsPaginator,
         ListComponentsPaginator,
         ListFormsPaginator,
         ListThemesPaginator,
     )
 
     session = Session()
     client: AmplifyUIBuilderClient = session.client("amplifyuibuilder")
 
     export_components_paginator: ExportComponentsPaginator = client.get_paginator("export_components")
     export_forms_paginator: ExportFormsPaginator = client.get_paginator("export_forms")
     export_themes_paginator: ExportThemesPaginator = client.get_paginator("export_themes")
+    list_codegen_jobs_paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_forms_paginator: ListFormsPaginator = client.get_paginator("list_forms")
     list_themes_paginator: ListThemesPaginator = client.get_paginator("list_themes")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ExportComponentsResponseTypeDef,
     ExportFormsResponseTypeDef,
     ExportThemesResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListFormsResponseTypeDef,
     ListThemesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ExportComponentsPaginator",
     "ExportFormsPaginator",
     "ExportThemesPaginator",
+    "ListCodegenJobsPaginator",
     "ListComponentsPaginator",
     "ListFormsPaginator",
     "ListThemesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ExportComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ExportComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
         """
 
-
 class ExportFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ExportFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
         """
 
-
 class ExportThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ExportThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
         """
 
+class ListCodegenJobsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
+    """
+
+    def paginate(
+        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListCodegenJobsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
+        """
 
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
     """
 
@@ -118,30 +130,28 @@
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
         """
 
-
 class ListFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
         """
 
-
 class ListThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listthemespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/paginator.pyi` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,131 +9,158 @@
     from boto3.session import Session
 
     from mypy_boto3_amplifyuibuilder.client import AmplifyUIBuilderClient
     from mypy_boto3_amplifyuibuilder.paginator import (
         ExportComponentsPaginator,
         ExportFormsPaginator,
         ExportThemesPaginator,
+        ListCodegenJobsPaginator,
         ListComponentsPaginator,
         ListFormsPaginator,
         ListThemesPaginator,
     )
 
     session = Session()
     client: AmplifyUIBuilderClient = session.client("amplifyuibuilder")
 
     export_components_paginator: ExportComponentsPaginator = client.get_paginator("export_components")
     export_forms_paginator: ExportFormsPaginator = client.get_paginator("export_forms")
     export_themes_paginator: ExportThemesPaginator = client.get_paginator("export_themes")
+    list_codegen_jobs_paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")
     list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
     list_forms_paginator: ListFormsPaginator = client.get_paginator("list_forms")
     list_themes_paginator: ListThemesPaginator = client.get_paginator("list_themes")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ExportComponentsResponseTypeDef,
     ExportFormsResponseTypeDef,
     ExportThemesResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListFormsResponseTypeDef,
     ListThemesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "ExportComponentsPaginator",
     "ExportFormsPaginator",
     "ExportThemesPaginator",
+    "ListCodegenJobsPaginator",
     "ListComponentsPaginator",
     "ListFormsPaginator",
     "ListThemesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ExportComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ExportComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
         """
 
+
 class ExportFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ExportFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
         """
 
+
 class ExportThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ExportThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
         """
 
+
+class ListCodegenJobsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
+    """
+
+    def paginate(
+        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListCodegenJobsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
+        """
+
+
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
         """
 
+
 class ListFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
     """
 
     def paginate(
         self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
         """
 
+
 class ListThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listthemespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/type_defs.py` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,17 +12,23 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
+    CodegenGenericDataFieldDataTypeType,
+    CodegenJobStatusType,
     FormActionTypeType,
     FormButtonsPositionType,
     FormDataSourceTypeType,
+    GenericDataRelationshipTypeType,
+    JSModuleType,
+    JSScriptType,
+    JSTargetType,
     LabelDecoratorType,
     SortDirectionType,
     StorageAccessLevelType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -32,14 +38,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActionParametersTypeDef",
+    "CodegenFeatureFlagsTypeDef",
+    "CodegenGenericDataEnumTypeDef",
+    "CodegenGenericDataFieldTypeDef",
+    "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelTypeDef",
+    "CodegenGenericDataRelationshipTypeTypeDef",
+    "CodegenJobAssetTypeDef",
+    "CodegenJobGenericDataSchemaTypeDef",
+    "CodegenJobRenderConfigTypeDef",
+    "CodegenJobSummaryTypeDef",
+    "CodegenJobTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
     "ComponentChildTypeDef",
     "ComponentConditionPropertyTypeDef",
     "ComponentDataConfigurationTypeDef",
     "ComponentEventTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
@@ -85,42 +102,51 @@
     "FormInputBindingPropertiesValueTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
     "FormInputValuePropertyTypeDef",
     "FormStyleConfigTypeDef",
     "FormStyleTypeDef",
     "FormSummaryTypeDef",
     "FormTypeDef",
+    "GetCodegenJobRequestRequestTypeDef",
+    "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetComponentResponseTypeDef",
     "GetFormRequestRequestTypeDef",
     "GetFormResponseTypeDef",
     "GetMetadataRequestRequestTypeDef",
     "GetMetadataResponseTypeDef",
     "GetThemeRequestRequestTypeDef",
     "GetThemeResponseTypeDef",
+    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    "ListCodegenJobsRequestRequestTypeDef",
+    "ListCodegenJobsResponseTypeDef",
     "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListComponentsResponseTypeDef",
     "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
     "ListFormsResponseTypeDef",
     "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
     "ListThemesResponseTypeDef",
     "MutationActionSetStateParameterTypeDef",
     "PaginatorConfigTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "RefreshTokenResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SectionalElementTypeDef",
     "SortPropertyTypeDef",
+    "StartCodegenJobDataTypeDef",
+    "StartCodegenJobRequestRequestTypeDef",
+    "StartCodegenJobResponseTypeDef",
     "ThemeSummaryTypeDef",
     "ThemeTypeDef",
     "ThemeValueTypeDef",
     "ThemeValuesTypeDef",
     "UpdateComponentDataTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateComponentResponseTypeDef",
@@ -146,14 +172,193 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": "MutationActionSetStateParameterTypeDef",
     },
     total=False,
 )
 
+CodegenFeatureFlagsTypeDef = TypedDict(
+    "CodegenFeatureFlagsTypeDef",
+    {
+        "isRelationshipSupported": bool,
+        "isNonModelSupported": bool,
+    },
+    total=False,
+)
+
+CodegenGenericDataEnumTypeDef = TypedDict(
+    "CodegenGenericDataEnumTypeDef",
+    {
+        "values": List[str],
+    },
+)
+
+_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldTypeDef",
+    {
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
+    },
+)
+_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldTypeDef",
+    {
+        "relationship": "CodegenGenericDataRelationshipTypeTypeDef",
+    },
+    total=False,
+)
+
+
+class CodegenGenericDataFieldTypeDef(
+    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
+):
+    pass
+
+
+_RequiredCodegenGenericDataModelTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
+        "primaryKeys": List[str],
+    },
+)
+_OptionalCodegenGenericDataModelTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelTypeDef",
+    {
+        "isJoinTable": bool,
+    },
+    total=False,
+)
+
+
+class CodegenGenericDataModelTypeDef(
+    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
+):
+    pass
+
+
+CodegenGenericDataNonModelTypeDef = TypedDict(
+    "CodegenGenericDataNonModelTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
+    },
+)
+
+_RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
+    {
+        "type": GenericDataRelationshipTypeType,
+        "relatedModelName": str,
+    },
+)
+_OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
+    {
+        "relatedModelFields": List[str],
+        "canUnlinkAssociatedModel": bool,
+        "relatedJoinFieldName": str,
+        "relatedJoinTableName": str,
+        "belongsToFieldOnRelatedModel": str,
+        "associatedFields": List[str],
+        "isHasManyIndex": bool,
+    },
+    total=False,
+)
+
+
+class CodegenGenericDataRelationshipTypeTypeDef(
+    _RequiredCodegenGenericDataRelationshipTypeTypeDef,
+    _OptionalCodegenGenericDataRelationshipTypeTypeDef,
+):
+    pass
+
+
+CodegenJobAssetTypeDef = TypedDict(
+    "CodegenJobAssetTypeDef",
+    {
+        "downloadUrl": str,
+    },
+    total=False,
+)
+
+CodegenJobGenericDataSchemaTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, "CodegenGenericDataModelTypeDef"],
+        "enums": Dict[str, "CodegenGenericDataEnumTypeDef"],
+        "nonModels": Dict[str, "CodegenGenericDataNonModelTypeDef"],
+    },
+)
+
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
+    {
+        "react": "ReactStartCodegenJobDataTypeDef",
+    },
+    total=False,
+)
+
+_RequiredCodegenJobSummaryTypeDef = TypedDict(
+    "_RequiredCodegenJobSummaryTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
+_OptionalCodegenJobSummaryTypeDef = TypedDict(
+    "_OptionalCodegenJobSummaryTypeDef",
+    {
+        "createdAt": datetime,
+        "modifiedAt": datetime,
+    },
+    total=False,
+)
+
+
+class CodegenJobSummaryTypeDef(
+    _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
+):
+    pass
+
+
+_RequiredCodegenJobTypeDef = TypedDict(
+    "_RequiredCodegenJobTypeDef",
+    {
+        "id": str,
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalCodegenJobTypeDef = TypedDict(
+    "_OptionalCodegenJobTypeDef",
+    {
+        "renderConfig": "CodegenJobRenderConfigTypeDef",
+        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
+        "autoGenerateForms": bool,
+        "features": "CodegenFeatureFlagsTypeDef",
+        "status": CodegenJobStatusType,
+        "statusMessage": str,
+        "asset": "CodegenJobAssetTypeDef",
+        "tags": Dict[str, str],
+        "createdAt": datetime,
+        "modifiedAt": datetime,
+    },
+    total=False,
+)
+
+
+class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
+    pass
+
+
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -997,14 +1202,31 @@
 )
 
 
 class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
     pass
 
 
+GetCodegenJobRequestRequestTypeDef = TypedDict(
+    "GetCodegenJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
+
+GetCodegenJobResponseTypeDef = TypedDict(
+    "GetCodegenJobResponseTypeDef",
+    {
+        "job": "CodegenJobTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetComponentRequestRequestTypeDef = TypedDict(
     "GetComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
@@ -1064,14 +1286,69 @@
     "GetThemeResponseTypeDef",
     {
         "theme": "ThemeTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
+    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListCodegenJobsRequestRequestTypeDef(
+    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
+):
+    pass
+
+
+ListCodegenJobsResponseTypeDef = TypedDict(
+    "ListCodegenJobsResponseTypeDef",
+    {
+        "entities": List["CodegenJobSummaryTypeDef"],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
     "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
@@ -1278,14 +1555,26 @@
         "appId": str,
         "environmentName": str,
         "featureName": str,
         "body": "PutMetadataFlagBodyTypeDef",
     },
 )
 
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+    },
+    total=False,
+)
+
 _RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
     "_RequiredRefreshTokenRequestBodyTypeDef",
     {
         "token": str,
     },
 )
 _OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
@@ -1358,14 +1647,69 @@
     "SortPropertyTypeDef",
     {
         "field": str,
         "direction": SortDirectionType,
     },
 )
 
+_RequiredStartCodegenJobDataTypeDef = TypedDict(
+    "_RequiredStartCodegenJobDataTypeDef",
+    {
+        "renderConfig": "CodegenJobRenderConfigTypeDef",
+    },
+)
+_OptionalStartCodegenJobDataTypeDef = TypedDict(
+    "_OptionalStartCodegenJobDataTypeDef",
+    {
+        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
+        "autoGenerateForms": bool,
+        "features": "CodegenFeatureFlagsTypeDef",
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class StartCodegenJobDataTypeDef(
+    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
+):
+    pass
+
+
+_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCodegenJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "codegenJobToCreate": "StartCodegenJobDataTypeDef",
+    },
+)
+_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCodegenJobRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class StartCodegenJobRequestRequestTypeDef(
+    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
+):
+    pass
+
+
+StartCodegenJobResponseTypeDef = TypedDict(
+    "StartCodegenJobResponseTypeDef",
+    {
+        "entity": "CodegenJobTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ThemeSummaryTypeDef = TypedDict(
     "ThemeSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder/type_defs.pyi` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,23 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
+    CodegenGenericDataFieldDataTypeType,
+    CodegenJobStatusType,
     FormActionTypeType,
     FormButtonsPositionType,
     FormDataSourceTypeType,
+    GenericDataRelationshipTypeType,
+    JSModuleType,
+    JSScriptType,
+    JSTargetType,
     LabelDecoratorType,
     SortDirectionType,
     StorageAccessLevelType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -31,14 +37,25 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionParametersTypeDef",
+    "CodegenFeatureFlagsTypeDef",
+    "CodegenGenericDataEnumTypeDef",
+    "CodegenGenericDataFieldTypeDef",
+    "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelTypeDef",
+    "CodegenGenericDataRelationshipTypeTypeDef",
+    "CodegenJobAssetTypeDef",
+    "CodegenJobGenericDataSchemaTypeDef",
+    "CodegenJobRenderConfigTypeDef",
+    "CodegenJobSummaryTypeDef",
+    "CodegenJobTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
     "ComponentChildTypeDef",
     "ComponentConditionPropertyTypeDef",
     "ComponentDataConfigurationTypeDef",
     "ComponentEventTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
@@ -84,42 +101,51 @@
     "FormInputBindingPropertiesValueTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
     "FormInputValuePropertyTypeDef",
     "FormStyleConfigTypeDef",
     "FormStyleTypeDef",
     "FormSummaryTypeDef",
     "FormTypeDef",
+    "GetCodegenJobRequestRequestTypeDef",
+    "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetComponentResponseTypeDef",
     "GetFormRequestRequestTypeDef",
     "GetFormResponseTypeDef",
     "GetMetadataRequestRequestTypeDef",
     "GetMetadataResponseTypeDef",
     "GetThemeRequestRequestTypeDef",
     "GetThemeResponseTypeDef",
+    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    "ListCodegenJobsRequestRequestTypeDef",
+    "ListCodegenJobsResponseTypeDef",
     "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListComponentsResponseTypeDef",
     "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
     "ListFormsResponseTypeDef",
     "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
     "ListThemesResponseTypeDef",
     "MutationActionSetStateParameterTypeDef",
     "PaginatorConfigTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "RefreshTokenResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SectionalElementTypeDef",
     "SortPropertyTypeDef",
+    "StartCodegenJobDataTypeDef",
+    "StartCodegenJobRequestRequestTypeDef",
+    "StartCodegenJobResponseTypeDef",
     "ThemeSummaryTypeDef",
     "ThemeTypeDef",
     "ThemeValueTypeDef",
     "ThemeValuesTypeDef",
     "UpdateComponentDataTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateComponentResponseTypeDef",
@@ -145,14 +171,183 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": "MutationActionSetStateParameterTypeDef",
     },
     total=False,
 )
 
+CodegenFeatureFlagsTypeDef = TypedDict(
+    "CodegenFeatureFlagsTypeDef",
+    {
+        "isRelationshipSupported": bool,
+        "isNonModelSupported": bool,
+    },
+    total=False,
+)
+
+CodegenGenericDataEnumTypeDef = TypedDict(
+    "CodegenGenericDataEnumTypeDef",
+    {
+        "values": List[str],
+    },
+)
+
+_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldTypeDef",
+    {
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
+    },
+)
+_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldTypeDef",
+    {
+        "relationship": "CodegenGenericDataRelationshipTypeTypeDef",
+    },
+    total=False,
+)
+
+class CodegenGenericDataFieldTypeDef(
+    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
+):
+    pass
+
+_RequiredCodegenGenericDataModelTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
+        "primaryKeys": List[str],
+    },
+)
+_OptionalCodegenGenericDataModelTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelTypeDef",
+    {
+        "isJoinTable": bool,
+    },
+    total=False,
+)
+
+class CodegenGenericDataModelTypeDef(
+    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
+):
+    pass
+
+CodegenGenericDataNonModelTypeDef = TypedDict(
+    "CodegenGenericDataNonModelTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
+    },
+)
+
+_RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
+    {
+        "type": GenericDataRelationshipTypeType,
+        "relatedModelName": str,
+    },
+)
+_OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
+    {
+        "relatedModelFields": List[str],
+        "canUnlinkAssociatedModel": bool,
+        "relatedJoinFieldName": str,
+        "relatedJoinTableName": str,
+        "belongsToFieldOnRelatedModel": str,
+        "associatedFields": List[str],
+        "isHasManyIndex": bool,
+    },
+    total=False,
+)
+
+class CodegenGenericDataRelationshipTypeTypeDef(
+    _RequiredCodegenGenericDataRelationshipTypeTypeDef,
+    _OptionalCodegenGenericDataRelationshipTypeTypeDef,
+):
+    pass
+
+CodegenJobAssetTypeDef = TypedDict(
+    "CodegenJobAssetTypeDef",
+    {
+        "downloadUrl": str,
+    },
+    total=False,
+)
+
+CodegenJobGenericDataSchemaTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, "CodegenGenericDataModelTypeDef"],
+        "enums": Dict[str, "CodegenGenericDataEnumTypeDef"],
+        "nonModels": Dict[str, "CodegenGenericDataNonModelTypeDef"],
+    },
+)
+
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
+    {
+        "react": "ReactStartCodegenJobDataTypeDef",
+    },
+    total=False,
+)
+
+_RequiredCodegenJobSummaryTypeDef = TypedDict(
+    "_RequiredCodegenJobSummaryTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
+_OptionalCodegenJobSummaryTypeDef = TypedDict(
+    "_OptionalCodegenJobSummaryTypeDef",
+    {
+        "createdAt": datetime,
+        "modifiedAt": datetime,
+    },
+    total=False,
+)
+
+class CodegenJobSummaryTypeDef(
+    _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
+):
+    pass
+
+_RequiredCodegenJobTypeDef = TypedDict(
+    "_RequiredCodegenJobTypeDef",
+    {
+        "id": str,
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalCodegenJobTypeDef = TypedDict(
+    "_OptionalCodegenJobTypeDef",
+    {
+        "renderConfig": "CodegenJobRenderConfigTypeDef",
+        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
+        "autoGenerateForms": bool,
+        "features": "CodegenFeatureFlagsTypeDef",
+        "status": CodegenJobStatusType,
+        "statusMessage": str,
+        "asset": "CodegenJobAssetTypeDef",
+        "tags": Dict[str, str],
+        "createdAt": datetime,
+        "modifiedAt": datetime,
+    },
+    total=False,
+)
+
+class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
+    pass
+
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -952,14 +1147,31 @@
     },
     total=False,
 )
 
 class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
     pass
 
+GetCodegenJobRequestRequestTypeDef = TypedDict(
+    "GetCodegenJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
+
+GetCodegenJobResponseTypeDef = TypedDict(
+    "GetCodegenJobResponseTypeDef",
+    {
+        "job": "CodegenJobTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetComponentRequestRequestTypeDef = TypedDict(
     "GetComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
@@ -1019,14 +1231,65 @@
     "GetThemeResponseTypeDef",
     {
         "theme": "ThemeTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
+    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListCodegenJobsRequestRequestTypeDef(
+    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
+):
+    pass
+
+ListCodegenJobsResponseTypeDef = TypedDict(
+    "ListCodegenJobsResponseTypeDef",
+    {
+        "entities": List["CodegenJobSummaryTypeDef"],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
     "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
@@ -1221,14 +1484,26 @@
         "appId": str,
         "environmentName": str,
         "featureName": str,
         "body": "PutMetadataFlagBodyTypeDef",
     },
 )
 
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+    },
+    total=False,
+)
+
 _RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
     "_RequiredRefreshTokenRequestBodyTypeDef",
     {
         "token": str,
     },
 )
 _OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
@@ -1297,14 +1572,65 @@
     "SortPropertyTypeDef",
     {
         "field": str,
         "direction": SortDirectionType,
     },
 )
 
+_RequiredStartCodegenJobDataTypeDef = TypedDict(
+    "_RequiredStartCodegenJobDataTypeDef",
+    {
+        "renderConfig": "CodegenJobRenderConfigTypeDef",
+    },
+)
+_OptionalStartCodegenJobDataTypeDef = TypedDict(
+    "_OptionalStartCodegenJobDataTypeDef",
+    {
+        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
+        "autoGenerateForms": bool,
+        "features": "CodegenFeatureFlagsTypeDef",
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartCodegenJobDataTypeDef(
+    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
+):
+    pass
+
+_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCodegenJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "codegenJobToCreate": "StartCodegenJobDataTypeDef",
+    },
+)
+_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCodegenJobRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class StartCodegenJobRequestRequestTypeDef(
+    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
+):
+    pass
+
+StartCodegenJobResponseTypeDef = TypedDict(
+    "StartCodegenJobResponseTypeDef",
+    {
+        "entity": "CodegenJobTypeDef",
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ThemeSummaryTypeDef = TypedDict(
     "ThemeSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.26.152/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,20 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-amplifyuibuilder
-Version: 1.26.106
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.26.106 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-amplifyuibuilder"></a>
 
 # mypy-boto3-amplifyuibuilder
 
 [![PyPI - mypy-boto3-amplifyuibuilder](https://img.shields.io/pypi/v/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifyuibuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.26.106](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.26.152](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -284,76 +252,97 @@
 from boto3.session import Session
 
 from mypy_boto3_amplifyuibuilder import AmplifyUIBuilderClient
 from mypy_boto3_amplifyuibuilder.paginator import (
     ExportComponentsPaginator,
     ExportFormsPaginator,
     ExportThemesPaginator,
+    ListCodegenJobsPaginator,
     ListComponentsPaginator,
     ListFormsPaginator,
     ListThemesPaginator,
 )
 
 client: AmplifyUIBuilderClient = Session().client("amplifyuibuilder")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 export_components_paginator: ExportComponentsPaginator = client.get_paginator("export_components")
 export_forms_paginator: ExportFormsPaginator = client.get_paginator("export_forms")
 export_themes_paginator: ExportThemesPaginator = client.get_paginator("export_themes")
+list_codegen_jobs_paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")
 list_components_paginator: ListComponentsPaginator = client.get_paginator("list_components")
 list_forms_paginator: ListFormsPaginator = client.get_paginator("list_forms")
 list_themes_paginator: ListThemesPaginator = client.get_paginator("list_themes")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_amplifyuibuilder.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.literals import (
+    CodegenGenericDataFieldDataTypeType,
+    CodegenJobGenericDataSourceTypeType,
+    CodegenJobStatusType,
     ExportComponentsPaginatorName,
     ExportFormsPaginatorName,
     ExportThemesPaginatorName,
     FixedPositionType,
     FormActionTypeType,
     FormButtonsPositionType,
     FormDataSourceTypeType,
+    GenericDataRelationshipTypeType,
+    JSModuleType,
+    JSScriptType,
+    JSTargetType,
     LabelDecoratorType,
+    ListCodegenJobsPaginatorName,
     ListComponentsPaginatorName,
     ListFormsPaginatorName,
     ListThemesPaginatorName,
     SortDirectionType,
     StorageAccessLevelType,
     TokenProvidersType,
     AmplifyUIBuilderServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     RegionName,
 )
 
 
-def check_value(value: ExportComponentsPaginatorName) -> bool:
+def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     ActionParametersTypeDef,
+    CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeTypeDef,
+    CodegenJobAssetTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    CodegenJobSummaryTypeDef,
+    CodegenJobTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentBindingPropertiesValueTypeDef,
     ComponentChildTypeDef,
     ComponentConditionPropertyTypeDef,
     ComponentDataConfigurationTypeDef,
     ComponentEventTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
@@ -399,42 +388,51 @@
     FormInputBindingPropertiesValueTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
     FormInputValuePropertyTypeDef,
     FormStyleConfigTypeDef,
     FormStyleTypeDef,
     FormSummaryTypeDef,
     FormTypeDef,
+    GetCodegenJobRequestRequestTypeDef,
+    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
     GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
     GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
     GetThemeResponseTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListCodegenJobsRequestRequestTypeDef,
+    ListCodegenJobsResponseTypeDef,
     ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListComponentsResponseTypeDef,
     ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
     ListFormsResponseTypeDef,
     ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
     ListThemesResponseTypeDef,
     MutationActionSetStateParameterTypeDef,
     PaginatorConfigTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenRequestRequestTypeDef,
     RefreshTokenResponseTypeDef,
     ResponseMetadataTypeDef,
     SectionalElementTypeDef,
     SortPropertyTypeDef,
+    StartCodegenJobDataTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    StartCodegenJobResponseTypeDef,
     ThemeSummaryTypeDef,
     ThemeTypeDef,
     ThemeValueTypeDef,
     ThemeValuesTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateComponentResponseTypeDef,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt` & `mypy-boto3-amplifyuibuilder-1.26.152/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.26.106/setup.py` & `mypy-boto3-amplifyuibuilder-1.26.152/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifyuibuilder",
-    version="1.26.106",
+    version="1.26.152",
     packages=["mypy_boto3_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyUIBuilder 1.26.106 service generated with"
+        "Type annotations for boto3.AmplifyUIBuilder 1.26.152 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

