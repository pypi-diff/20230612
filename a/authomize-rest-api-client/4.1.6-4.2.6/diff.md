# Comparing `tmp/authomize-rest-api-client-4.1.6.tar.gz` & `tmp/authomize-rest-api-client-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.1.6.tar", last modified: Sun Jun  4 13:30:06 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.2.6.tar", last modified: Mon Jun 12 11:24:29 2023, max compression
```

## Comparing `authomize-rest-api-client-4.1.6.tar` & `authomize-rest-api-client-4.2.6.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.089781 authomize-rest-api-client-4.1.6/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84288 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37380 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200259 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89370 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-06-04 13:29:47.000000 authomize-rest-api-client-4.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76002 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37380 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190165 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89370 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-12 11:24:29.528043 authomize-rest-api-client-4.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-12 11:24:28.000000 authomize-rest-api-client-4.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/tests/
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/tests/test_import.py
```

### Comparing `authomize-rest-api-client-4.1.6/LICENSE.txt` & `authomize-rest-api-client-4.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/README.md` & `authomize-rest-api-client-4.2.6/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-31T12:40:10+00:00
+#   timestamp: 2023-06-12T11:05:04+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -250,19 +250,14 @@
     )
     data: Optional[NewAccountsAssociationResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewAccountsAssociationsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewAccountsAssociationRequestSchema] = Field(
         ...,
         description='New Accounts Associations',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -298,14 +293,19 @@
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
         default='Other',
         description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
+    alternativeName: Optional[str] = Field(
+        default=None,
+        description='Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n',
+        title='Alternativename',
+    )
     originType: Optional[str] = Field(
         default=None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
         default=None,
@@ -332,19 +332,14 @@
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class NewAssetsInheritanceListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewAssetInheritanceRequestSchema] = Field(
         ...,
         description='New Assets Inheritance',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -388,19 +383,14 @@
     )
     data: Optional[NewAssetsInheritanceResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewAssetsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewAssetRequestSchema] = Field(
         ..., description='New Assets', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -549,19 +539,14 @@
     )
     data: Optional[NewGroupingsAssociationResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewGroupingsAssociationsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewGroupingsAssociationRequestSchema] = Field(
         ...,
         description='New Groupings Associations',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -569,19 +554,14 @@
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewGroupingsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewGroupingRequestSchema] = Field(
         ..., description='New Groupings', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validate Only\n',
@@ -697,19 +677,14 @@
     )
     data: Optional[NewPrivilegeGrantsResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewPrivilegesGrantsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewPrivilegeGrantsRequestSchema] = Field(
         ...,
         description='New Privileges Grants',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -893,14 +868,19 @@
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
         default='Other',
         description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
+    alternativeName: Optional[str] = Field(
+        default=None,
+        description='Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n',
+        title='Alternativename',
+    )
     originType: Optional[str] = Field(
         default=None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
         default=None,
@@ -927,19 +907,14 @@
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class UpdateAssetsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[UpdateAssetRequestSchema] = Field(
         ..., description='Update Assets', max_items=10000, min_items=1, title='Data'
     )
 
 
 class UpdateGroupingsRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
@@ -1023,19 +998,14 @@
         default=None,
         description='The privilege name in the source system.',
         title='Originname',
     )
 
 
 class UpdatePrivilegesListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[UpdatePrivilegeRequestSchema] = Field(
         ..., description='Update Privileges', max_items=10000, min_items=1, title='Data'
     )
 
 
 class UserStatus(Enum):
     Staged = 'Staged'
@@ -1087,14 +1057,19 @@
         description='The name of the asset. The default is the Asset ID. **Mandatory**\n',
         title='Name',
     )
     type: Optional[AssetType] = Field(
         default='Other',
         description='The asset types that are supported by Authomize **Mandatory**\n\nPermitted values:\n\n   •\t`Application` (federation) \n   •\t`Database`\n   •\t`Drive`\n   •\t`File`\n   •\t`Folder`\n   •\t`GitRepository`\n   •\t`Integration`\n   •\t`Project`\n   •\t`Site`\n   •\t`Table`\n   •\t`Ticket`\n   •\t`VirtualMachine`\n   •\t`Other`\n\nIf the asset type does not exist use `Other`.\n',
     )
+    alternativeName: Optional[str] = Field(
+        default=None,
+        description='Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n',
+        title='Alternativename',
+    )
     originType: Optional[str] = Field(
         default=None,
         description='The asset type in the source system.\nThe default is the canonical type (if not mentioned).\n',
         title='Origintype',
     )
     createdAt: Optional[datetime] = Field(
         default=None,
@@ -1412,19 +1387,14 @@
         default=False,
         description="If `true`, it's possible to perform a privilege escalation using the permission.   \nexample: User has Read access to a secret containing credentials of another user.  This allows \nprivilege escalation.\nopposite example: User has Read metadata permission to a secret containing credentials of another user. This *Does NOT* allows \nprivilege escalation.\n\n",
         title='Escalationpathpossible',
     )
 
 
 class NewPermissionsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewPermissionRequestSchema] = Field(
         ..., description='New Permissions', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validate Only\n',
@@ -1450,19 +1420,14 @@
         default=None,
         description='The privilege name in the source system.',
         title='Originname',
     )
 
 
 class NewPrivilegesListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewPrivilegeRequestSchema] = Field(
         ..., description='New Privileges', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -1518,19 +1483,14 @@
         default=None,
         description='One or more tags on the user account.\n',
         title='Tags',
     )
 
 
 class NewUsersListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewUserRequestSchema] = Field(
         ..., description='New Users', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -1591,19 +1551,14 @@
         default=None,
         description='The privilege name in the source system.',
         title='Originname',
     )
 
 
 class RequestsBundleSchema(BaseModel):
-    workflow_id: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflow Id',
-    )
     delete_app_data: Optional[bool] = Field(
         default=False,
         description='The Delete Application Data API is used to delete app data by `{appId}`.',
         title='Delete App Data',
     )
     createdAt: Optional[datetime] = Field(default=None, title='Createdat')
     new_users: Optional[List[NewUserRequestSchema]] = Field(
@@ -1694,19 +1649,14 @@
 
 class TransactionPaginatedSearchSchema(BaseModel):
     data: List[BundleTransactionSchema] = Field(..., title='Data')
     pagination: Pagination
 
 
 class UpdateGroupingsListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[UpdateGroupingsRequestSchema] = Field(
         ...,
         description='List of update user requests.\n',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -1946,19 +1896,14 @@
         default=None,
         description='The Update Application Data API is used to update app data on `{appId}`.\n',
         title='App',
     )
 
 
 class NewIdentitiesListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[NewIdentityRequestSchema] = Field(
         ..., description='New Identities', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -1966,34 +1911,24 @@
 
 
 class SearchUsersListResponseSchema(BaseModel):
     data: List[UserSchema] = Field(..., description='Users', title='Data')
 
 
 class UpdateIdentitiesListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[UpdateIdentityRequestSchema] = Field(
         ...,
         description='List of update identity requests.\n',
         max_items=10000,
         min_items=1,
         title='Data',
     )
 
 
 class UpdateUserListRequestSchema(BaseModel):
-    workflowId: Optional[str] = Field(
-        default='default',
-        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
-        title='Workflowid',
-    )
     data: List[UpdateUserRequestSchema] = Field(
         ...,
         description='List of update user requests.\n',
         max_items=10000,
         min_items=1,
         title='Data',
     )
```

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.987372691733459%*

 * *Differences: {"'components'": "{'schemas': {'AssetSchema': {'properties': {'alternativeName': "*

 * *                 "OrderedDict([('title', 'Alternativename'), ('type', 'string'), ('description', "*

 * *                 "'Any alternative name for the resource, or any other representation of the "*

 * *                 "resource, if it exists.\\nThe default is `null`.\\n')])}}, "*

 * *                 "'NewAccountsAssociationsListRequestSchema': {'properties': {delete: "*

 * *                 "['workflowId']}}, 'NewAssetRequestSchema': {'prope […]*

```diff
@@ -175,14 +175,19 @@
                 ],
                 "title": "AssetInheritanceSchema",
                 "type": "object"
             },
             "AssetSchema": {
                 "description": "Asset schema",
                 "properties": {
+                    "alternativeName": {
+                        "description": "Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n",
+                        "title": "Alternativename",
+                        "type": "string"
+                    },
                     "createdAt": {
                         "description": "The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n",
                         "format": "date-time",
                         "title": "Createdat",
                         "type": "string"
                     },
                     "description": {
@@ -1131,20 +1136,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewAccountsAssociationsListRequestSchema",
                 "type": "object"
@@ -1171,14 +1170,19 @@
                 ],
                 "title": "NewAssetInheritanceRequestSchema",
                 "type": "object"
             },
             "NewAssetRequestSchema": {
                 "description": "New asset request schema",
                 "properties": {
+                    "alternativeName": {
+                        "description": "Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n",
+                        "title": "Alternativename",
+                        "type": "string"
+                    },
                     "createdAt": {
                         "description": "The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n",
                         "format": "date-time",
                         "title": "Createdat",
                         "type": "string"
                     },
                     "description": {
@@ -1265,20 +1269,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewAssetsInheritanceListRequestSchema",
                 "type": "object"
@@ -1379,20 +1377,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewAssetsListRequestSchema",
                 "type": "object"
@@ -1691,20 +1683,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewGroupingsAssociationsListRequestSchema",
                 "type": "object"
@@ -1723,20 +1709,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validate Only\n",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewGroupingsListRequestSchema",
                 "type": "object"
@@ -1755,20 +1735,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewIdentitiesListRequestSchema",
                 "type": "object"
@@ -1918,14 +1892,15 @@
                     "requestId",
                     "numberOfAcceptedEntities"
                 ],
                 "title": "NewIdentityResponseSchema",
                 "type": "object"
             },
             "NewPermissionRequestSchema": {
+                "description": "New permission request schema",
                 "properties": {
                     "assetId": {
                         "description": "The ID of the asset.\n\nWhen `null`, this is a global permission on the entire application (not just locally).",
                         "title": "Assetid",
                         "type": "string"
                     },
                     "escalationPathPossible": {
@@ -1992,20 +1967,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validate Only\n",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewPermissionsListRequestSchema",
                 "type": "object"
@@ -2283,20 +2252,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewPrivilegesGrantsListRequestSchema",
                 "type": "object"
@@ -2315,20 +2278,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewPrivilegesListRequestSchema",
                 "type": "object"
@@ -2510,20 +2467,14 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewUsersListRequestSchema",
                 "type": "object"
@@ -2827,20 +2778,14 @@
                     "new_users": {
                         "description": "The Create Users APIs sets up App users(by App ID).",
                         "items": {
                             "$ref": "#/components/schemas/NewUserRequestSchema"
                         },
                         "title": "New Users",
                         "type": "array"
-                    },
-                    "workflow_id": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflow Id",
-                        "type": "string"
                     }
                 },
                 "title": "RequestsBundleSchema",
                 "type": "object"
             },
             "RestApiConnectorListSchema": {
                 "properties": {
@@ -3183,14 +3128,19 @@
                 },
                 "title": "UpdateAppSchema",
                 "type": "object"
             },
             "UpdateAssetRequestSchema": {
                 "description": "Update asset request schema",
                 "properties": {
+                    "alternativeName": {
+                        "description": "Any alternative name for the resource, or any other representation of the resource, if it exists.\nThe default is `null`.\n",
+                        "title": "Alternativename",
+                        "type": "string"
+                    },
                     "createdAt": {
                         "description": "The date (in ISO 8601 format) that the asset was created.\nThe default is `null`.\n",
                         "format": "date-time",
                         "title": "Createdat",
                         "type": "string"
                     },
                     "description": {
@@ -3271,20 +3221,14 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateAssetRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateAssetsListRequestSchema",
                 "type": "object"
@@ -3297,20 +3241,14 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateGroupingsRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateGroupingsListRequestSchema",
                 "type": "object"
@@ -3430,20 +3368,14 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateIdentityRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateIdentitiesListRequestSchema",
                 "type": "object"
@@ -3607,20 +3539,14 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdatePrivilegeRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdatePrivilegesListRequestSchema",
                 "type": "object"
@@ -3633,20 +3559,14 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateUserRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
-                    },
-                    "workflowId": {
-                        "default": "default",
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "title": "Workflowid",
-                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateUserListRequestSchema",
                 "type": "object"
@@ -3859,15 +3779,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.1.4",
+        "version": "3.2.3",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -5665,28 +5585,16 @@
                         "required": true,
                         "schema": {
                             "title": "Appid",
                             "type": "string"
                         }
                     },
                     {
-                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                        "in": "query",
-                        "name": "workflowId",
-                        "required": false,
-                        "schema": {
-                            "default": "default",
-                            "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
-                            "title": "Workflowid",
-                            "type": "string"
-                        }
-                    },
-                    {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-05-31T12:18:31.018274+00:00",
+                        "example": "2023-06-12T11:04:31.189262+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
 authomize/rest_api_client/openapi/external_rest_api/__init__.py
 authomize/rest_api_client/openapi/external_rest_api/openapi.json
 authomize_rest_api_client.egg-info/PKG-INFO
 authomize_rest_api_client.egg-info/SOURCES.txt
 authomize_rest_api_client.egg-info/dependency_links.txt
 authomize_rest_api_client.egg-info/requires.txt
-authomize_rest_api_client.egg-info/top_level.txt
+authomize_rest_api_client.egg-info/top_level.txt
+tests/test_import.py
```

### Comparing `authomize-rest-api-client-4.1.6/setup.py` & `authomize-rest-api-client-4.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.1.6',
+        version='4.2.6',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

