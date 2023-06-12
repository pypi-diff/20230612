# Comparing `tmp/robotframework_openapidriver-4.0.0.tar.gz` & `tmp/robotframework_openapidriver-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapidriver-4.0.0.tar", max compression
+gzip compressed data, was "robotframework_openapidriver-4.1.0.tar", max compression
```

## Comparing `robotframework_openapidriver-4.0.0.tar` & `robotframework_openapidriver-4.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     4763 2023-05-22 14:37:21.907738 robotframework_openapidriver-4.0.0/docs/README.md
--rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-4.0.0/LICENSE
--rw-r--r--   0        0        0     2966 2023-05-22 13:30:25.858447 robotframework_openapidriver-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1103 2022-01-11 08:27:46.400406 robotframework_openapidriver-4.0.0/src/OpenApiDriver/__init__.py
--rw-r--r--   0        0        0    32663 2023-05-22 14:15:42.315705 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_executors.py
--rw-r--r--   0        0        0     4573 2023-05-22 14:23:32.088745 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_reader.py
--rw-r--r--   0        0        0    23429 2023-05-22 14:37:21.799096 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.libspec
--rw-r--r--   0        0        0    14035 2023-05-22 14:25:04.781026 robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.py
--rw-r--r--   0        0        0     5640 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.0.0/setup.py
--rw-r--r--   0        0        0     5794 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4817 2023-06-12 08:01:12.404483 robotframework_openapidriver-4.1.0/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-10-01 09:02:52.229239 robotframework_openapidriver-4.1.0/LICENSE
+-rw-r--r--   0        0        0     2966 2023-06-09 13:44:41.052342 robotframework_openapidriver-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1103 2022-01-11 08:27:46.400406 robotframework_openapidriver-4.1.0/src/OpenApiDriver/__init__.py
+-rw-r--r--   0        0        0    32993 2023-06-12 07:31:09.890507 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_executors.py
+-rw-r--r--   0        0        0     4573 2023-05-22 14:48:18.048301 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_reader.py
+-rw-r--r--   0        0        0    25265 2023-06-12 08:01:12.327460 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.libspec
+-rw-r--r--   0        0        0    15519 2023-06-12 08:01:08.206636 robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:27:05.636214 robotframework_openapidriver-4.1.0/src/OpenApiDriver/py.typed
+-rw-r--r--   0        0        0     5694 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.1.0/setup.py
+-rw-r--r--   0        0        0     5848 1970-01-01 00:00:00.000000 robotframework_openapidriver-4.1.0/PKG-INFO
```

### Comparing `robotframework_openapidriver-4.0.0/docs/README.md` & `robotframework_openapidriver-4.1.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,31 +51,31 @@
 
 This can be done using the command line interface of a package that is installed as
 a prerequisite for OpenApiDriver.
 Both a local openapi.json or openapi.yaml file or one hosted by the API server
 can be checked using the `prance validate <reference_to_file>` shell command:
 
 ```shell
-prance validate http://localhost:8000/openapi.json
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
 Processing "http://localhost:8000/openapi.json"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 
-prance validate /tests/files/petstore_openapi.yaml
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
 Processing "/tests/files/petstore_openapi.yaml"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 ```
 
 You'll have to change the url or file reference to the location of the openapi
 document for your API.
 
 > Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the API to not use recursion is recommended.
-At present OpenApiLibCore has limited support for parsing OpenAPI documents with
+and changing the OAS to not use recursion is recommended.
+OpenApiDriver has limited support for parsing OpenAPI documents with
 recursion in them. See the `recursion_limit` and `recursion_default` parameters.
 
 If the openapi document passes this validation, the next step is trying to do a test
 run with a minimal test suite.
 The example below can be used, with `source` and `origin` altered to fit your situation.
 
 ``` robotframework
```

### Comparing `robotframework_openapidriver-4.0.0/LICENSE` & `robotframework_openapidriver-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.0.0/pyproject.toml` & `robotframework_openapidriver-4.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapidriver"
-version = "4.0.0"
+version = "4.1.0"
 description = "A library for contract-testing OpenAPI / Swagger APIs."
 license = "Apache-2.0"
 authors = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 maintainers = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 readme =  "./docs/README.md"
 homepage = "https://github.com/MarketSquare/robotframework-openapidriver"
 classifiers = [
@@ -20,15 +20,15 @@
     { include = "OpenApiDriver", from = "src" },
 ]
 include = ["*.libspec"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 robotframework-datadriver = ">=1.6.1"
-robotframework-openapi-libcore = "^1.8.5"
+robotframework-openapi-libcore = "^1.9.0"
 
 [tool.poetry.group.dev.dependencies]
 fastapi = ">=0.95.0"
 uvicorn = ">=0.22.0"
 invoke = ">=2.0.0"
 coverage = {version=">=7.2.5", extras = ["toml"]}
 robotframework-stacktrace = ">=0.4.1"
```

### Comparing `robotframework_openapidriver-4.0.0/src/OpenApiDriver/__init__.py` & `robotframework_openapidriver-4.1.0/src/OpenApiDriver/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_executors.py` & `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from openapi_core.contrib.requests import (
     RequestsOpenAPIRequest,
     RequestsOpenAPIResponse,
 )
 from openapi_core.templating.paths.exceptions import ServerNotFound
-from openapi_core.unmarshalling.schemas.exceptions import InvalidSchemaValue
+from openapi_core.validation.schemas.exceptions import InvalidSchemaValue
 from OpenApiLibCore import OpenApiLibCore, RequestData, RequestValues, resolve_schema
 from requests import Response
 from requests.auth import AuthBase
+from requests.cookies import RequestsCookieJar as CookieJar
 from robot.api import SkipExecution
 from robot.api.deco import keyword, library
 from robot.libraries.BuiltIn import BuiltIn
 
 run_keyword = BuiltIn().run_keyword
 
 
@@ -41,45 +42,51 @@
     """Main class providing the keywords and core logic to perform endpoint validations."""
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         source: str,
         origin: str = "",
         base_path: str = "",
+        response_validation: ValidationLevel = ValidationLevel.WARN,
+        disable_server_validation: bool = True,
         mappings_path: Union[str, Path] = "",
+        invalid_property_default_response: int = 422,
+        default_id_property_name: str = "id",
+        faker_locale: Optional[Union[str, List[str]]] = None,
+        require_body_for_invalid_url: bool = False,
+        recursion_limit: int = 1,
+        recursion_default: Any = {},
         username: str = "",
         password: str = "",
         security_token: str = "",
         auth: Optional[AuthBase] = None,
         cert: Optional[Union[str, Tuple[str, str]]] = None,
+        verify_tls: Optional[Union[bool, str]] = True,
         extra_headers: Optional[Dict[str, str]] = None,
-        response_validation: ValidationLevel = ValidationLevel.WARN,
-        disable_server_validation: bool = True,
-        require_body_for_invalid_url: bool = False,
-        invalid_property_default_response: int = 422,
-        recursion_limit: int = 1,
-        recursion_default: Any = {},
-        faker_locale: Optional[Union[str, List[str]]] = None,
-        default_id_property_name: str = "id",
+        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
+        proxies: Optional[Dict[str, str]] = None,
     ) -> None:
         super().__init__(
             source=source,
             origin=origin,
             base_path=base_path,
             mappings_path=mappings_path,
+            default_id_property_name=default_id_property_name,
+            faker_locale=faker_locale,
+            recursion_limit=recursion_limit,
+            recursion_default=recursion_default,
             username=username,
             password=password,
             security_token=security_token,
             auth=auth,
             cert=cert,
+            verify_tls=verify_tls,
             extra_headers=extra_headers,
-            recursion_limit=recursion_limit,
-            recursion_default=recursion_default,
-            faker_locale=faker_locale,
-            default_id_property_name=default_id_property_name,
+            cookies=cookies,
+            proxies=proxies,
         )
         self.response_validation = response_validation
         self.disable_server_validation = disable_server_validation
         self.require_body_for_invalid_url = require_body_for_invalid_url
         self.invalid_property_default_response = invalid_property_default_response
 
     @keyword
```

### Comparing `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapi_reader.py` & `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapi_reader.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.libspec`

 * *Files 2% similar despite different names*

#### Comparing `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.libspec` & `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.libspec`

```diff
@@ -1,19 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-05-22T14:37:22+00:00" specversion="4" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="316">
-  <version>4.0.0</version>
+<keywordspec name="OpenApiDriver" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-06-12T08:01:12+00:00" specversion="4" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapidriver.py" lineno="351">
+  <version>4.1.0</version>
   <doc>&lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapidriver&quot;&gt;library page&lt;/a&gt; for an introduction and examples.&lt;/p&gt;</doc>
   <tags/>
   <inits>
-    <init name="__init__" lineno="142">
-      <arguments repr="source: str, included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, origin: str = , base_path: str = , mappings_path: str | Path = , username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, extra_headers: Dict[str, str] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, require_body_for_invalid_url: bool = False, invalid_property_default_response: int = 422, recursion_limit: int = 1, recursion_default: Any = {}, faker_locale: str | List[str] | None = None, default_id_property_name: str = id">
+    <init name="__init__" lineno="143">
+      <arguments repr="source: str, origin: str = , base_path: str = , included_paths: Iterable[str] | None = None, ignored_paths: Iterable[str] | None = None, ignored_responses: Iterable[int] | None = None, ignored_testcases: Iterable[Tuple[str, str, int]] | None = None, response_validation: ValidationLevel = WARN, disable_server_validation: bool = True, mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, require_body_for_invalid_url: bool = False, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
           <type typedoc="string">str</type>
         </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
+          <name>origin</name>
+          <type typedoc="string">str</type>
+          <default/>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="base_path: str = ">
+          <name>base_path</name>
+          <type typedoc="string">str</type>
+          <default/>
+        </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="included_paths: Iterable[str] | None = None">
           <name>included_paths</name>
           <type>Iterable[str]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_paths: Iterable[str] | None = None">
@@ -30,30 +40,62 @@
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="ignored_testcases: Iterable[Tuple[str, str, int]] | None = None">
           <name>ignored_testcases</name>
           <type>Iterable[Tuple[str, str, int]]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
-          <name>origin</name>
-          <type typedoc="string">str</type>
-          <default/>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="response_validation: ValidationLevel = WARN">
+          <name>response_validation</name>
+          <type typedoc="ValidationLevel">ValidationLevel</type>
+          <default>WARN</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="base_path: str = ">
-          <name>base_path</name>
-          <type typedoc="string">str</type>
-          <default/>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="disable_server_validation: bool = True">
+          <name>disable_server_validation</name>
+          <type typedoc="boolean">bool</type>
+          <default>True</default>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="mappings_path: str | Path = ">
           <name>mappings_path</name>
           <type typedoc="string">str</type>
           <type typedoc="Path">Path</type>
           <default/>
         </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="invalid_property_default_response: int = 422">
+          <name>invalid_property_default_response</name>
+          <type typedoc="integer">int</type>
+          <default>422</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="default_id_property_name: str = id">
+          <name>default_id_property_name</name>
+          <type typedoc="string">str</type>
+          <default>id</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="faker_locale: str | List[str] | None = None">
+          <name>faker_locale</name>
+          <type typedoc="string">str</type>
+          <type typedoc="list">List[str]</type>
+          <type typedoc="None">None</type>
+          <default>None</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="require_body_for_invalid_url: bool = False">
+          <name>require_body_for_invalid_url</name>
+          <type typedoc="boolean">bool</type>
+          <default>False</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_limit: int = 1">
+          <name>recursion_limit</name>
+          <type typedoc="integer">int</type>
+          <default>1</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_default: Any = {}">
+          <name>recursion_default</name>
+          <type>Any</type>
+          <default>{}</default>
+        </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="username: str = ">
           <name>username</name>
           <type typedoc="string">str</type>
           <default/>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="password: str = ">
           <name>password</name>
@@ -74,119 +116,109 @@
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="cert: str | Tuple[str, str] | None = None">
           <name>cert</name>
           <type typedoc="string">str</type>
           <type typedoc="tuple">Tuple[str, str]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="verify_tls: bool | str | None = True">
+          <name>verify_tls</name>
+          <type typedoc="boolean">bool</type>
+          <type typedoc="string">str</type>
+          <type typedoc="None">None</type>
+          <default>True</default>
+        </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="extra_headers: Dict[str, str] | None = None">
           <name>extra_headers</name>
           <type typedoc="dictionary">Dict[str, str]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="response_validation: ValidationLevel = WARN">
-          <name>response_validation</name>
-          <type typedoc="ValidationLevel">ValidationLevel</type>
-          <default>WARN</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="disable_server_validation: bool = True">
-          <name>disable_server_validation</name>
-          <type typedoc="boolean">bool</type>
-          <default>True</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="require_body_for_invalid_url: bool = False">
-          <name>require_body_for_invalid_url</name>
-          <type typedoc="boolean">bool</type>
-          <default>False</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="invalid_property_default_response: int = 422">
-          <name>invalid_property_default_response</name>
-          <type typedoc="integer">int</type>
-          <default>422</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_limit: int = 1">
-          <name>recursion_limit</name>
-          <type typedoc="integer">int</type>
-          <default>1</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="recursion_default: Any = {}">
-          <name>recursion_default</name>
-          <type>Any</type>
-          <default>{}</default>
-        </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="faker_locale: str | List[str] | None = None">
-          <name>faker_locale</name>
-          <type typedoc="string">str</type>
-          <type typedoc="list">List[str]</type>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="cookies: Dict[str, str] | RequestsCookieJar | None = None">
+          <name>cookies</name>
+          <type typedoc="dictionary">Dict[str, str]</type>
+          <type typedoc="dictionary">RequestsCookieJar</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="default_id_property_name: str = id">
-          <name>default_id_property_name</name>
-          <type typedoc="string">str</type>
-          <default>id</default>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="proxies: Dict[str, str] | None = None">
+          <name>proxies</name>
+          <type typedoc="dictionary">Dict[str, str]</type>
+          <type typedoc="None">None</type>
+          <default>None</default>
         </arg>
       </arguments>
-      <doc>&lt;h4&gt;source&lt;/h4&gt;
+      <doc>&lt;h3&gt;Base parameters&lt;/h3&gt;
+&lt;h4&gt;source&lt;/h4&gt;
 &lt;p&gt;An absolute path to an openapi.json or openapi.yaml file or an url to such a file.&lt;/p&gt;
+&lt;h4&gt;origin&lt;/h4&gt;
+&lt;p&gt;The server (and port) of the target server. E.g. &lt;code&gt;https://localhost:8000&lt;/code&gt;&lt;/p&gt;
+&lt;h4&gt;base_path&lt;/h4&gt;
+&lt;p&gt;The routing between &lt;code&gt;origin&lt;/code&gt; and the endpoints as found in the &lt;code&gt;paths&lt;/code&gt; section in the openapi document. E.g. &lt;code&gt;/petshop/v2&lt;/code&gt;.&lt;/p&gt;
+&lt;h3&gt;Test case generation and execution&lt;/h3&gt;
 &lt;h4&gt;included_paths&lt;/h4&gt;
 &lt;p&gt;A list of paths that will be included when generating the test cases. The &lt;code&gt;*&lt;/code&gt; character can be used at the end of a partial path to include all paths starting with the partial path (wildcard include).&lt;/p&gt;
 &lt;h4&gt;ignored_paths&lt;/h4&gt;
 &lt;p&gt;A list of paths that will be ignored when generating the test cases. The &lt;code&gt;*&lt;/code&gt; character can be used at the end of a partial path to ignore all paths starting with the partial path (wildcard ignore).&lt;/p&gt;
 &lt;h4&gt;ignored_responses&lt;/h4&gt;
 &lt;p&gt;A list of responses that will be ignored when generating the test cases.&lt;/p&gt;
 &lt;h4&gt;ignored_testcases&lt;/h4&gt;
 &lt;p&gt;A list of specific test cases that, if it would be generated, will be ignored. Specific test cases to ignore must be specified as a &lt;code&gt;Tuple&lt;/code&gt; or &lt;code&gt;List&lt;/code&gt; of &lt;code&gt;path&lt;/code&gt;, &lt;code&gt;method&lt;/code&gt; and &lt;code&gt;response&lt;/code&gt;.&lt;/p&gt;
-&lt;h4&gt;origin&lt;/h4&gt;
-&lt;p&gt;The server (and port) of the target server. E.g. &lt;code&gt;https://localhost:8000&lt;/code&gt;&lt;/p&gt;
-&lt;h4&gt;base_path&lt;/h4&gt;
-&lt;p&gt;The routing between &lt;code&gt;origin&lt;/code&gt; and the paths as found in the &lt;code&gt;paths&lt;/code&gt; in the openapi document. E.g. &lt;code&gt;/petshop/v2&lt;/code&gt;.&lt;/p&gt;
-&lt;h4&gt;mappings_path&lt;/h4&gt;
-&lt;p&gt;See &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;here&lt;/a&gt;.&lt;/p&gt;
-&lt;h4&gt;username&lt;/h4&gt;
-&lt;p&gt;The username to be used for Basic Authentication.&lt;/p&gt;
-&lt;h4&gt;password&lt;/h4&gt;
-&lt;p&gt;The password to be used for Basic Authentication.&lt;/p&gt;
-&lt;h4&gt;security_token&lt;/h4&gt;
-&lt;p&gt;The token to be used for token based security using the &lt;code&gt;Authorization&lt;/code&gt; header.&lt;/p&gt;
-&lt;h4&gt;auth&lt;/h4&gt;
-&lt;p&gt;A &lt;a href=&quot;https://requests.readthedocs.io/en/latest/api/#authentication&quot;&gt;requests AuthBase instance&lt;/a&gt; to be used for authentication instead of the &lt;code&gt;username&lt;/code&gt; and &lt;code&gt;password&lt;/code&gt;.&lt;/p&gt;
-&lt;h4&gt;cert&lt;/h4&gt;
-&lt;p&gt;The SSL certificate to use with all requests. If string: the path to ssl client cert file (.pem). If tuple, ('cert', 'key') pair.&lt;/p&gt;
-&lt;h4&gt;extra_headers&lt;/h4&gt;
-&lt;p&gt;A dictionary with extra / custom headers that will be send with every request. This parameter can be used to send headers that are not documented in the openapi document.&lt;/p&gt;
 &lt;h4&gt;response_validation&lt;/h4&gt;
 &lt;p&gt;By default, a &lt;code&gt;WARN&lt;/code&gt; is logged when the Response received after a Request does not comply with the schema as defined in the openapi document for the given operation. The following values are supported:&lt;/p&gt;
 &lt;ul&gt;
 &lt;li&gt;&lt;code&gt;DISABLED&lt;/code&gt;: All Response validation errors will be ignored&lt;/li&gt;
 &lt;li&gt;&lt;code&gt;INFO&lt;/code&gt;: Any Response validation erros will be logged at &lt;code&gt;INFO&lt;/code&gt; level&lt;/li&gt;
 &lt;li&gt;&lt;code&gt;WARN&lt;/code&gt;: Any Response validation erros will be logged at &lt;code&gt;WARN&lt;/code&gt; level&lt;/li&gt;
 &lt;li&gt;&lt;code&gt;STRICT&lt;/code&gt;: The Test Case will fail on any Response validation errors&lt;/li&gt;
 &lt;/ul&gt;
 &lt;h4&gt;disable_server_validation&lt;/h4&gt;
 &lt;p&gt;If enabled by setting this parameter to &lt;code&gt;True&lt;/code&gt;, the Response validation will also include possible errors for Requests made to a server address that is not defined in the list of servers in the openapi document. This generally means that if there is a mismatch, every Test Case will raise this error. Note that &lt;code&gt;localhost&lt;/code&gt; and &lt;code&gt;127.0.0.1&lt;/code&gt; are not considered the same by Response validation.&lt;/p&gt;
-&lt;h4&gt;require_body_for_invalid_url&lt;/h4&gt;
-&lt;p&gt;When a request is made against an invalid url, this usually is because of a &quot;404&quot; request; a request for a resource that does not exist. Depending on API implementation, when a request with a missing or invalid request body is made on a non-existent resource, either a 404 or a 422 or 400 Response is normally returned. If the API being tested processes the request body before checking if the requested resource exists, set this parameter to True.&lt;/p&gt;
+&lt;h3&gt;API-specific configurations&lt;/h3&gt;
+&lt;h4&gt;mappings_path&lt;/h4&gt;
+&lt;p&gt;See &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;this page&lt;/a&gt; for an in-depth explanation.&lt;/p&gt;
 &lt;h4&gt;invalid_property_default_response&lt;/h4&gt;
 &lt;p&gt;The default response code for requests with a JSON body that does not comply with the schema. Example: a value outside the specified range or a string value for a property defined as integer in the schema.&lt;/p&gt;
+&lt;h4&gt;default_id_property_name&lt;/h4&gt;
+&lt;p&gt;The default name for the property that identifies a resource (i.e. a unique entity) within the API. The default value for this property name is &lt;code&gt;id&lt;/code&gt;. If the target API uses a different name for all the resources within the API, you can configure it globally using this property.&lt;/p&gt;
+&lt;p&gt;If different property names are used for the unique identifier for different types of resources, an &lt;code&gt;ID_MAPPING&lt;/code&gt; can be implemented using the &lt;code&gt;mappings_path&lt;/code&gt;.&lt;/p&gt;
+&lt;h4&gt;faker_locale&lt;/h4&gt;
+&lt;p&gt;A locale string or list of locale strings to pass to the Faker library to be used in generation of string data for supported format types.&lt;/p&gt;
+&lt;h4&gt;require_body_for_invalid_url&lt;/h4&gt;
+&lt;p&gt;When a request is made against an invalid url, this usually is because of a &quot;404&quot; request; a request for a resource that does not exist. Depending on API implementation, when a request with a missing or invalid request body is made on a non-existent resource, either a 404 or a 422 or 400 Response is normally returned. If the API being tested processes the request body before checking if the requested resource exists, set this parameter to True.&lt;/p&gt;
+&lt;h3&gt;Parsing parameters&lt;/h3&gt;
 &lt;h4&gt;recursion_limit&lt;/h4&gt;
 &lt;p&gt;The recursion depth to which to fully parse recursive references before the &lt;span class=&quot;name&quot;&gt;recursion_default&lt;/span&gt; is used to end the recursion.&lt;/p&gt;
 &lt;h4&gt;recursion_default&lt;/h4&gt;
-&lt;p&gt;The value that is used instead of the referenced schema when the &lt;span class=&quot;name&quot;&gt;recursion_limit&lt;/span&gt; has been reached. The default &lt;span class=&quot;name&quot;&gt;{}&lt;/span&gt; represents an empty object in JSON. Depending on schema definitions, this may cause schema validation errors. If this is the case, &lt;a href=&quot;#type-None&quot; class=&quot;name&quot;&gt;None&lt;/a&gt; (&lt;span class=&quot;name&quot;&gt;${NONE}&lt;/span&gt; in Robot Framework) can be tried as an alternative.&lt;/p&gt;
-&lt;h4&gt;faker_locale&lt;/h4&gt;
-&lt;p&gt;A locale string or list of locale strings to pass to Faker to be used in generation of string data for supported format types.&lt;/p&gt;
-&lt;h4&gt;default_id_property_name&lt;/h4&gt;
-&lt;p&gt;The default name for the property that identifies a resource (i.e. a unique entiry) within the API. The default value for this property name is &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt;. If the target API uses a different name for all the resources within the API, you can configure it globally using this property.&lt;/p&gt;
-&lt;p&gt;If different property names are used for the unique identifier for different types of resources, an &lt;span class=&quot;name&quot;&gt;ID_MAPPING&lt;/span&gt; can be implemented in the &lt;span class=&quot;name&quot;&gt;mappings_path&lt;/span&gt;.&lt;/p&gt;</doc>
-      <shortdoc>=== source === An absolute path to an openapi.json or openapi.yaml file or an url to such a file.</shortdoc>
+&lt;p&gt;The value that is used instead of the referenced schema when the &lt;span class=&quot;name&quot;&gt;recursion_limit&lt;/span&gt; has been reached. The default &lt;span class=&quot;name&quot;&gt;{}&lt;/span&gt; represents an empty object in JSON. Depending on schema definitions, this may cause schema validation errors. If this is the case, 'None' (&lt;code&gt;${NONE}&lt;/code&gt; in Robot Framework) or an empty list can be tried as an alternative.&lt;/p&gt;
+&lt;h3&gt;Security-related parameters&lt;/h3&gt;
+&lt;p&gt;&lt;i&gt;Note: these parameters are equivalent to those in the &lt;code&gt;requests&lt;/code&gt; library.&lt;/i&gt;&lt;/p&gt;
+&lt;h4&gt;username&lt;/h4&gt;
+&lt;p&gt;The username to be used for Basic Authentication.&lt;/p&gt;
+&lt;h4&gt;password&lt;/h4&gt;
+&lt;p&gt;The password to be used for Basic Authentication.&lt;/p&gt;
+&lt;h4&gt;security_token&lt;/h4&gt;
+&lt;p&gt;The token to be used for token based security using the &lt;code&gt;Authorization&lt;/code&gt; header.&lt;/p&gt;
+&lt;h4&gt;auth&lt;/h4&gt;
+&lt;p&gt;A &lt;a href=&quot;https://requests.readthedocs.io/en/latest/api/#authentication&quot;&gt;requests &lt;code&gt;AuthBase&lt;/code&gt; instance&lt;/a&gt; to be used for authentication instead of the &lt;code&gt;username&lt;/code&gt; and &lt;code&gt;password&lt;/code&gt;.&lt;/p&gt;
+&lt;h4&gt;cert&lt;/h4&gt;
+&lt;p&gt;The SSL certificate to use with all requests. If string: the path to ssl client cert file (.pem). If tuple: the ('cert', 'key') pair.&lt;/p&gt;
+&lt;h4&gt;verify_tls&lt;/h4&gt;
+&lt;p&gt;Whether or not to verify the TLS / SSL certificate of the server. If boolean: whether or not to verify the server TLS certificate. If string: path to a CA bundle to use for verification.&lt;/p&gt;
+&lt;h4&gt;extra_headers&lt;/h4&gt;
+&lt;p&gt;A dictionary with extra / custom headers that will be send with every request. This parameter can be used to send headers that are not documented in the openapi document or to provide an API-key.&lt;/p&gt;
+&lt;h4&gt;cookies&lt;/h4&gt;
+&lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
+&lt;h4&gt;proxies&lt;/h4&gt;
+&lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
+      <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Test Endpoint" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="148">
+    <kw name="Test Endpoint" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="155">
       <arguments repr="path: str, method: str, status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -198,15 +230,15 @@
         </arg>
       </arguments>
       <doc>&lt;p&gt;Validate that performing the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; results in a &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; response.&lt;/p&gt;
 &lt;p&gt;This is the main keyword to be used in the &lt;span class=&quot;name&quot;&gt;Test Template&lt;/span&gt; keyword when using the OpenApiDriver.&lt;/p&gt;
 &lt;p&gt;The keyword calls other keywords to generate the neccesary data to perform the desired operation and validate the response against the openapi document.&lt;/p&gt;</doc>
       <shortdoc>Validate that performing the `method` operation on `path` results in a `status_code` response.</shortdoc>
     </kw>
-    <kw name="Test Invalid Url" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="106">
+    <kw name="Test Invalid Url" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="113">
       <arguments repr="path: str, method: str, expected_status_code: int = 404">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -220,15 +252,15 @@
       </arguments>
       <doc>&lt;p&gt;Perform a request for the provided 'path' and 'method' where the url for the &lt;a href=&quot;#type-Path&quot; class=&quot;name&quot;&gt;path&lt;/a&gt; is invalidated.&lt;/p&gt;
 &lt;p&gt;This keyword will be &lt;span class=&quot;name&quot;&gt;SKIPPED&lt;/span&gt; if the path contains no parts that can be invalidated.&lt;/p&gt;
 &lt;p&gt;The optional &lt;span class=&quot;name&quot;&gt;expected_status_code&lt;/span&gt; parameter (default: 404) can be set to the expected status code for APIs that do not return a 404 on invalid urls.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: Depending on API design, the url may be validated before or after validation of headers, query parameters and / or (json) body. By default, no parameters are send with the request. The &lt;span class=&quot;name&quot;&gt;require_body_for_invalid_url&lt;/span&gt; parameter can be set to &lt;span class=&quot;name&quot;&gt;True&lt;/span&gt; if needed.&lt;/p&gt;</doc>
       <shortdoc>Perform a request for the provided 'path' and 'method' where the url for the `path` is invalidated.</shortdoc>
     </kw>
-    <kw name="Test Unauthorized" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="86">
+    <kw name="Test Unauthorized" source="C:\GitHub\robotframework-openapidriver\src\OpenApiDriver\openapi_executors.py" lineno="93">
       <arguments repr="path: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="path: str">
           <name>path</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
```

### Comparing `robotframework_openapidriver-4.0.0/src/OpenApiDriver/openapidriver.py` & `robotframework_openapidriver-4.1.0/src/OpenApiDriver/openapidriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,31 +49,31 @@
 
 This can be done using the command line interface of a package that is installed as
 a prerequisite for OpenApiDriver.
 Both a local openapi.json or openapi.yaml file or one hosted by the API server
 can be checked using the `prance validate <reference_to_file>` shell command:
 
 ```shell
-prance validate http://localhost:8000/openapi.json
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
 Processing "http://localhost:8000/openapi.json"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 
-prance validate /tests/files/petstore_openapi.yaml
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
 Processing "/tests/files/petstore_openapi.yaml"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 ```
 
 You'll have to change the url or file reference to the location of the openapi
 document for your API.
 
 > Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the API to not use recursion is recommended.
-At present OpenApiLibCore has limited support for parsing OpenAPI documents with
+and changing the OAS to not use recursion is recommended.
+OpenApiDriver has limited support for parsing OpenAPI documents with
 recursion in them. See the `recursion_limit` and `recursion_default` parameters.
 
 If the openapi document passes this validation, the next step is trying to do a test
 run with a minimal test suite.
 The example below can be used, with `source` and `origin` altered to fit your situation.
 
 ``` robotframework
@@ -122,14 +122,15 @@
 
 """
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 from DataDriver import DataDriver
 from requests.auth import AuthBase
+from requests.cookies import RequestsCookieJar as CookieJar
 from robot.api.deco import library
 
 from OpenApiDriver.openapi_executors import OpenApiExecutors, ValidationLevel
 from OpenApiDriver.openapi_reader import OpenApiReader
 
 
 @library(scope="TEST SUITE", doc_format="ROBOT")
@@ -138,171 +139,205 @@
     Visit the [https://github.com/MarketSquare/robotframework-openapidriver | library page]
     for an introduction and examples.
     """
 
     def __init__(  # pylint: disable=too-many-arguments, too-many-locals, dangerous-default-value
         self,
         source: str,
+        origin: str = "",
+        base_path: str = "",
         included_paths: Optional[Iterable[str]] = None,
         ignored_paths: Optional[Iterable[str]] = None,
         ignored_responses: Optional[Iterable[int]] = None,
         ignored_testcases: Optional[Iterable[Tuple[str, str, int]]] = None,
-        origin: str = "",
-        base_path: str = "",
+        response_validation: ValidationLevel = ValidationLevel.WARN,
+        disable_server_validation: bool = True,
         mappings_path: Union[str, Path] = "",
+        invalid_property_default_response: int = 422,
+        default_id_property_name: str = "id",
+        faker_locale: Optional[Union[str, List[str]]] = None,
+        require_body_for_invalid_url: bool = False,
+        recursion_limit: int = 1,
+        recursion_default: Any = {},
         username: str = "",
         password: str = "",
         security_token: str = "",
         auth: Optional[AuthBase] = None,
         cert: Optional[Union[str, Tuple[str, str]]] = None,
+        verify_tls: Optional[Union[bool, str]] = True,
         extra_headers: Optional[Dict[str, str]] = None,
-        response_validation: ValidationLevel = ValidationLevel.WARN,
-        disable_server_validation: bool = True,
-        require_body_for_invalid_url: bool = False,
-        invalid_property_default_response: int = 422,
-        recursion_limit: int = 1,
-        recursion_default: Any = {},
-        faker_locale: Optional[Union[str, List[str]]] = None,
-        default_id_property_name: str = "id",
+        cookies: Optional[Union[Dict[str, str], CookieJar]] = None,
+        proxies: Optional[Dict[str, str]] = None,
     ):
         """
-        === source ===
-        An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
+         == Base parameters ==
 
-        === included_paths ===
-        A list of paths that will be included when generating the test cases.
-        The ``*`` character can be used at the end of a partial path to include all paths
-        starting with the partial path (wildcard include).
-
-        === ignored_paths ===
-        A list of paths that will be ignored when generating the test cases.
-        The ``*`` character can be used at the end of a partial path to ignore all paths
-        starting with the partial path (wildcard ignore).
-
-        === ignored_responses ===
-        A list of responses that will be ignored when generating the test cases.
-
-        === ignored_testcases ===
-        A list of specific test cases that, if it would be generated, will be ignored.
-        Specific test cases to ignore must be specified as a ``Tuple`` or ``List``
-        of ``path``, ``method`` and ``response``.
+         === source ===
+         An absolute path to an openapi.json or openapi.yaml file or an url to such a file.
 
-        === origin ===
-        The server (and port) of the target server. E.g. ``https://localhost:8000``
+         === origin ===
+         The server (and port) of the target server. E.g. ``https://localhost:8000``
 
         === base_path ===
-        The routing between ``origin`` and the paths as found in the ``paths`` in the
-        openapi document. E.g. ``/petshop/v2``.
+         The routing between ``origin`` and the endpoints as found in the ``paths``
+         section in the openapi document.
+         E.g. ``/petshop/v2``.
+
+         == Test case generation and execution ==
+
+         === included_paths ===
+         A list of paths that will be included when generating the test cases.
+         The ``*`` character can be used at the end of a partial path to include all paths
+         starting with the partial path (wildcard include).
+
+         === ignored_paths ===
+         A list of paths that will be ignored when generating the test cases.
+         The ``*`` character can be used at the end of a partial path to ignore all paths
+         starting with the partial path (wildcard ignore).
+
+         === ignored_responses ===
+         A list of responses that will be ignored when generating the test cases.
+
+         === ignored_testcases ===
+         A list of specific test cases that, if it would be generated, will be ignored.
+         Specific test cases to ignore must be specified as a ``Tuple`` or ``List``
+         of ``path``, ``method`` and ``response``.
+
+         === response_validation ===
+         By default, a ``WARN`` is logged when the Response received after a Request does not
+         comply with the schema as defined in the openapi document for the given operation. The
+         following values are supported:
+
+         - ``DISABLED``: All Response validation errors will be ignored
+         - ``INFO``: Any Response validation erros will be logged at ``INFO`` level
+         - ``WARN``: Any Response validation erros will be logged at ``WARN`` level
+         - ``STRICT``: The Test Case will fail on any Response validation errors
+
+         === disable_server_validation ===
+         If enabled by setting this parameter to ``True``, the Response validation will also
+         include possible errors for Requests made to a server address that is not defined in
+         the list of servers in the openapi document. This generally means that if there is a
+         mismatch, every Test Case will raise this error. Note that ``localhost`` and
+         ``127.0.0.1`` are not considered the same by Response validation.
+
+         == API-specific configurations ==
+
+         === mappings_path ===
+         See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | this page]
+         for an in-depth explanation.
+
+         === invalid_property_default_response ===
+         The default response code for requests with a JSON body that does not comply
+         with the schema.
+         Example: a value outside the specified range or a string value
+         for a property defined as integer in the schema.
+
+         === default_id_property_name ===
+         The default name for the property that identifies a resource (i.e. a unique
+         entity) within the API.
+         The default value for this property name is ``id``.
+         If the target API uses a different name for all the resources within the API,
+         you can configure it globally using this property.
+
+         If different property names are used for the unique identifier for different
+         types of resources, an ``ID_MAPPING`` can be implemented using the ``mappings_path``.
+
+         === faker_locale ===
+         A locale string or list of locale strings to pass to the Faker library to be
+         used in generation of string data for supported format types.
+
+         === require_body_for_invalid_url ===
+         When a request is made against an invalid url, this usually is because of a "404" request;
+         a request for a resource that does not exist. Depending on API implementation, when a
+         request with a missing or invalid request body is made on a non-existent resource,
+         either a 404 or a 422 or 400 Response is normally returned. If the API being tested
+         processes the request body before checking if the requested resource exists, set
+         this parameter to True.
+
+         == Parsing parameters ==
+
+         === recursion_limit ===
+         The recursion depth to which to fully parse recursive references before the
+         `recursion_default` is used to end the recursion.
+
+         === recursion_default ===
+         The value that is used instead of the referenced schema when the
+         `recursion_limit` has been reached.
+         The default `{}` represents an empty object in JSON.
+         Depending on schema definitions, this may cause schema validation errors.
+         If this is the case, 'None' (``${NONE}`` in Robot Framework) or an empty list
+         can be tried as an alternative.
+
+         == Security-related parameters ==
+         _Note: these parameters are equivalent to those in the ``requests`` library._
+
+         === username ===
+         The username to be used for Basic Authentication.
+
+         === password ===
+         The password to be used for Basic Authentication.
+
+         === security_token ===
+         The token to be used for token based security using the ``Authorization`` header.
+
+         === auth ===
+         A [https://requests.readthedocs.io/en/latest/api/#authentication | requests ``AuthBase`` instance]
+         to be used for authentication instead of the ``username`` and ``password``.
+
+         === cert ===
+         The SSL certificate to use with all requests.
+         If string: the path to ssl client cert file (.pem).
+         If tuple: the ('cert', 'key') pair.
+
+         === verify_tls ===
+         Whether or not to verify the TLS / SSL certificate of the server.
+         If boolean: whether or not to verify the server TLS certificate.
+         If string: path to a CA bundle to use for verification.
+
+         === extra_headers ===
+         A dictionary with extra / custom headers that will be send with every request.
+         This parameter can be used to send headers that are not documented in the
+         openapi document or to provide an API-key.
+
+         === cookies ===
+         A dictionary or [https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar | CookieJar object]
+         to send with all requests.
 
-        === mappings_path ===
-        See [https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html | here].
-
-        === username ===
-        The username to be used for Basic Authentication.
-
-        === password ===
-        The password to be used for Basic Authentication.
-
-        === security_token ===
-        The token to be used for token based security using the ``Authorization`` header.
-
-        === auth ===
-        A [https://requests.readthedocs.io/en/latest/api/#authentication | requests AuthBase instance]
-        to be used for authentication instead of the ``username`` and ``password``.
-
-        === cert ===
-        The SSL certificate to use with all requests.
-        If string: the path to ssl client cert file (.pem). If tuple, ('cert', 'key') pair.
-
-        === extra_headers ===
-        A dictionary with extra / custom headers that will be send with every request.
-        This parameter can be used to send headers that are not documented in the
-        openapi document.
-
-        === response_validation ===
-        By default, a ``WARN`` is logged when the Response received after a Request does not
-        comply with the schema as defined in the openapi document for the given operation. The
-        following values are supported:
-
-        - ``DISABLED``: All Response validation errors will be ignored
-        - ``INFO``: Any Response validation erros will be logged at ``INFO`` level
-        - ``WARN``: Any Response validation erros will be logged at ``WARN`` level
-        - ``STRICT``: The Test Case will fail on any Response validation errors
-
-        === disable_server_validation ===
-        If enabled by setting this parameter to ``True``, the Response validation will also
-        include possible errors for Requests made to a server address that is not defined in
-        the list of servers in the openapi document. This generally means that if there is a
-        mismatch, every Test Case will raise this error. Note that ``localhost`` and
-        ``127.0.0.1`` are not considered the same by Response validation.
-
-        === require_body_for_invalid_url ===
-        When a request is made against an invalid url, this usually is because of a "404" request;
-        a request for a resource that does not exist. Depending on API implementation, when a
-        request with a missing or invalid request body is made on a non-existent resource,
-        either a 404 or a 422 or 400 Response is normally returned. If the API being tested
-        processes the request body before checking if the requested resource exists, set
-        this parameter to True.
-
-        === invalid_property_default_response ===
-        The default response code for requests with a JSON body that does not comply with
-        the schema. Example: a value outside the specified range or a string value for a
-        property defined as integer in the schema.
-
-        === recursion_limit ===
-        The recursion depth to which to fully parse recursive references before the
-        `recursion_default` is used to end the recursion.
-
-        === recursion_default ===
-        The value that is used instead of the referenced schema when the
-        `recursion_limit` has been reached. The default `{}` represents an empty
-        object in JSON. Depending on schema definitions, this may cause schema
-        validation errors. If this is the case, `None` (`${NONE}` in Robot Framework)
-        can be tried as an alternative.
-
-        === faker_locale ===
-        A locale string or list of locale strings to pass to Faker to be used in
-        generation of string data for supported format types.
-
-        === default_id_property_name ===
-        The default name for the property that identifies a resource (i.e. a unique
-        entiry) within the API.
-        The default value for this property name is `id`.
-        If the target API uses a different name for all the resources within the API,
-        you can configure it globally using this property.
-
-        If different property names are used for the unique identifier for different
-        types of resources, an `ID_MAPPING` can be implemented in the `mappings_path`.
+         === proxies ===
+         A dictionary of 'protocol': 'proxy url' to use for all requests.
         """
         included_paths = included_paths if included_paths else ()
         ignored_paths = ignored_paths if ignored_paths else ()
         ignored_responses = ignored_responses if ignored_responses else ()
         ignored_testcases = ignored_testcases if ignored_testcases else ()
 
         mappings_path = Path(mappings_path).as_posix()
         OpenApiExecutors.__init__(
             self,
             source=source,
             origin=origin,
             base_path=base_path,
+            response_validation=response_validation,
+            disable_server_validation=disable_server_validation,
             mappings_path=mappings_path,
+            invalid_property_default_response=invalid_property_default_response,
+            default_id_property_name=default_id_property_name,
+            faker_locale=faker_locale,
+            require_body_for_invalid_url=require_body_for_invalid_url,
+            recursion_limit=recursion_limit,
+            recursion_default=recursion_default,
             username=username,
             password=password,
             security_token=security_token,
             auth=auth,
             cert=cert,
+            verify_tls=verify_tls,
             extra_headers=extra_headers,
-            response_validation=response_validation,
-            disable_server_validation=disable_server_validation,
-            require_body_for_invalid_url=require_body_for_invalid_url,
-            invalid_property_default_response=invalid_property_default_response,
-            recursion_limit=recursion_limit,
-            recursion_default=recursion_default,
-            faker_locale=faker_locale,
-            default_id_property_name=default_id_property_name,
+            cookies=cookies,
+            proxies=proxies,
         )
 
         paths = self.openapi_spec["paths"]
         DataDriver.__init__(
             self,
             reader_class=OpenApiReader,
             paths=paths,
```

### Comparing `robotframework_openapidriver-4.0.0/setup.py` & `robotframework_openapidriver-4.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 ['OpenApiDriver']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['robotframework-datadriver>=1.6.1',
- 'robotframework-openapi-libcore>=1.8.5,<2.0.0']
+ 'robotframework-openapi-libcore>=1.9.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'robotframework-openapidriver',
-    'version': '4.0.0',
+    'version': '4.1.0',
     'description': 'A library for contract-testing OpenAPI / Swagger APIs.',
-    'long_description': '---\n---\n\n# OpenApiDriver for Robot Framework®\n\nOpenApiDriver is an extension of the Robot Framework® DataDriver library that allows\nfor generation and execution of test cases based on the information in an OpenAPI\ndocument (also known as Swagger document).\nThis document explains how to use the OpenApiDriver library.\n\nFor more information about Robot Framework®, see http://robotframework.org.\n\nFor more information about the DataDriver library, see\nhttps://github.com/Snooz82/robotframework-datadriver.\n\n---\n\n> Note: OpenApiDriver is still under development so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapidriver`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiDriver module implements a reader class that generates a test case for\neach path, method and response (i.e. every response for each endpoint) that is defined\nin an OpenAPI document, typically an openapi.json or openapi.yaml file.\n\n> Note: OpenApiDriver is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use OpenApiDriver to run automatic validations on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiDriver.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the API to not use recursion is recommended.\nAt present OpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source` and `origin` altered to fit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiDriver\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\nTest Template      Validate Using Test Endpoint Keyword\n\n*** Test Cases ***\nTest Endpoint for ${method} on ${path} where ${status_code} is expected\n\n*** Keywords ***\nValidate Using Test Endpoint Keyword\n    [Arguments]    ${path}    ${method}    ${status_code}\n    Test Endpoint\n    ...    path=${path}    method=${method}    status_code=${status_code}\n\n```\n\nRunning the above suite for the first time is likely to result in some\nerrors / failed tests.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiDriver library parameters that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).\n\nThe OpenApiDriver also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-path authorization levels (only simple 401 / 403 validation).\n\n',
+    'long_description': '---\n---\n\n# OpenApiDriver for Robot Framework®\n\nOpenApiDriver is an extension of the Robot Framework® DataDriver library that allows\nfor generation and execution of test cases based on the information in an OpenAPI\ndocument (also known as Swagger document).\nThis document explains how to use the OpenApiDriver library.\n\nFor more information about Robot Framework®, see http://robotframework.org.\n\nFor more information about the DataDriver library, see\nhttps://github.com/Snooz82/robotframework-datadriver.\n\n---\n\n> Note: OpenApiDriver is still under development so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapidriver`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiDriver module implements a reader class that generates a test case for\neach path, method and response (i.e. every response for each endpoint) that is defined\nin an OpenAPI document, typically an openapi.json or openapi.yaml file.\n\n> Note: OpenApiDriver is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use OpenApiDriver to run automatic validations on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiDriver.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the OAS to not use recursion is recommended.\nOpenApiDriver has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source` and `origin` altered to fit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiDriver\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\nTest Template      Validate Using Test Endpoint Keyword\n\n*** Test Cases ***\nTest Endpoint for ${method} on ${path} where ${status_code} is expected\n\n*** Keywords ***\nValidate Using Test Endpoint Keyword\n    [Arguments]    ${path}    ${method}    ${status_code}\n    Test Endpoint\n    ...    path=${path}    method=${method}    status_code=${status_code}\n\n```\n\nRunning the above suite for the first time is likely to result in some\nerrors / failed tests.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiDriver library parameters that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapidriver/openapidriver.html).\n\nThe OpenApiDriver also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-path authorization levels (only simple 401 / 403 validation).\n\n',
     'author': 'Robin Mackaij',
     'author_email': 'r.a.mackaij@gmail.com',
     'maintainer': 'Robin Mackaij',
     'maintainer_email': 'r.a.mackaij@gmail.com',
     'url': 'https://github.com/MarketSquare/robotframework-openapidriver',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `robotframework_openapidriver-4.0.0/PKG-INFO` & `robotframework_openapidriver-4.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapidriver
-Version: 4.0.0
+Version: 4.1.0
 Summary: A library for contract-testing OpenAPI / Swagger APIs.
 Home-page: https://github.com/MarketSquare/robotframework-openapidriver
 License: Apache-2.0
 Author: Robin Mackaij
 Author-email: r.a.mackaij@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Requires-Dist: robotframework-datadriver (>=1.6.1)
-Requires-Dist: robotframework-openapi-libcore (>=1.8.5,<2.0.0)
+Requires-Dist: robotframework-openapi-libcore (>=1.9.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ---
 ---
 
 # OpenApiDriver for Robot Framework®
 
@@ -78,31 +78,31 @@
 
 This can be done using the command line interface of a package that is installed as
 a prerequisite for OpenApiDriver.
 Both a local openapi.json or openapi.yaml file or one hosted by the API server
 can be checked using the `prance validate <reference_to_file>` shell command:
 
 ```shell
-prance validate http://localhost:8000/openapi.json
+prance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json
 Processing "http://localhost:8000/openapi.json"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 
-prance validate /tests/files/petstore_openapi.yaml
+prance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml
 Processing "/tests/files/petstore_openapi.yaml"...
  -> Resolving external references.
 Validates OK as OpenAPI 3.0.2!
 ```
 
 You'll have to change the url or file reference to the location of the openapi
 document for your API.
 
 > Note: Although recursion is technically allowed under the OAS, tool support is limited
-and changing the API to not use recursion is recommended.
-At present OpenApiLibCore has limited support for parsing OpenAPI documents with
+and changing the OAS to not use recursion is recommended.
+OpenApiDriver has limited support for parsing OpenAPI documents with
 recursion in them. See the `recursion_limit` and `recursion_default` parameters.
 
 If the openapi document passes this validation, the next step is trying to do a test
 run with a minimal test suite.
 The example below can be used, with `source` and `origin` altered to fit your situation.
 
 ``` robotframework
```

