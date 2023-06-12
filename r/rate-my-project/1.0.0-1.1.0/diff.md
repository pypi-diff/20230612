# Comparing `tmp/rate_my_project-1.0.0.tar.gz` & `tmp/rate_my_project-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rate_my_project-1.0.0.tar", last modified: Mon Mar  6 16:26:11 2023, max compression
+gzip compressed data, was "rate_my_project-1.1.0.tar", last modified: Mon Jun 12 15:44:19 2023, max compression
```

## Comparing `rate_my_project-1.0.0.tar` & `rate_my_project-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-06 16:26:11.703303 rate_my_project-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.695304 rate_my_project-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/src/rate_my_project/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/src/rate_my_project/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/connectors/confluenceclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/connectors/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/connectors/jiraclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/src/rate_my_project/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/metrics/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/src/rate_my_project/metrics/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/metrics/templates/report.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/src/rate_my_project/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/src/rate_my_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-03-06 16:26:11.000000 rate_my_project-1.0.0/src/rate_my_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-06 16:26:11.000000 rate_my_project-1.0.0/src/rate_my_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:26:11.000000 rate_my_project-1.0.0/src/rate_my_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-06 16:26:11.000000 rate_my_project-1.0.0/src/rate_my_project.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:26:11.000000 rate_my_project-1.0.0/src/rate_my_project.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-06 16:26:11.000000 rate_my_project-1.0.0/src/rate_my_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-06 16:26:11.000000 rate_my_project-1.0.0/src/rate_my_project.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:26:11.699303 rate_my_project-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/tests/test_confluenceclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/tests/test_httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-06 16:26:01.000000 rate_my_project-1.0.0/tests/test_jiraclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.272078 rate_my_project-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.272078 rate_my_project-1.1.0/src/rate_my_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/src/rate_my_project/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/connectors/confluenceclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/connectors/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/connectors/jiraclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/src/rate_my_project/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/metrics/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/src/rate_my_project/metrics/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/metrics/templates/report.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/src/rate_my_project/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/src/rate_my_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-12 15:44:19.000000 rate_my_project-1.1.0/src/rate_my_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-12 15:44:19.000000 rate_my_project-1.1.0/src/rate_my_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:44:19.000000 rate_my_project-1.1.0/src/rate_my_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 15:44:19.000000 rate_my_project-1.1.0/src/rate_my_project.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:44:19.000000 rate_my_project-1.1.0/src/rate_my_project.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 15:44:19.000000 rate_my_project-1.1.0/src/rate_my_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 15:44:19.000000 rate_my_project-1.1.0/src/rate_my_project.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:44:19.276078 rate_my_project-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/tests/test_confluenceclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/tests/test_httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-12 15:44:10.000000 rate_my_project-1.1.0/tests/test_jiraclient.py
```

### Comparing `rate_my_project-1.0.0/CONTRIBUTING.md` & `rate_my_project-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/LICENSE` & `rate_my_project-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/PKG-INFO` & `rate_my_project-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: rate_my_project
-Version: 1.0.0
-Summary: Swiss knife tool for analyzing project efficiency
-Home-page: https://github.com/cledouarec/rate-my-project
-Author: Christophe Le Douarec
-Author-email: ledouarec@gmail.com
-License: Apache License 2.0
-Keywords: team efficiency data visualization analysis
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Rate my project
 
 [![Lint](https://github.com/cledouarec/rate-my-project/actions/workflows/lint.yaml/badge.svg)](https://github.com/cledouarec/rate-my-project/actions/workflows/lint.yaml)
 [![Unit tests](https://github.com/cledouarec/rate-my-project/actions/workflows/test.yaml/badge.svg)](https://github.com/cledouarec/rate-my-project/actions/workflows/test.yaml)
 
 **Table of Contents**
 - [Rate my project](#rate-my-project)
@@ -196,15 +178,15 @@
 }
 ```
 
 | Attribute  | Required | Description                                      |
 |------------|:--------:|--------------------------------------------------|
 | server     |    ✅     | Main configuration node for server.              |
 | jira       |    ✅     | Jira server URL to retrieve tickets information. |
-| confluence |    ✅     | Confluence server URL to publish the report      |
+| confluence |    ✅     | Confluence server URL to publish the report.     |
 
 ### Fields configuration
 
 The `fields` node will configure the field name to use since it could be custom
 fields.
 
 **_In Yaml :_**
@@ -219,57 +201,111 @@
   "fields": {
     "sprint": "customfield_10001",
     "story_points": "customfield_10002"
   }
 }
 ```
 
-| Attribute    | Required | Description                                                    |
-|--------------|:--------:|----------------------------------------------------------------|
-| fields       |    ✅     | Main configuration node for fields.                            |
-| sprint       |    ✅     | Field to store the current sprint                              |
-| story_points |    ✅     | Field to store the estimation in story points of a development |
+| Attribute    | Required | Description                                                     |
+|--------------|:--------:|-----------------------------------------------------------------|
+| fields       |    ✅     | Main configuration node for fields.                             |
+| sprint       |    ✅     | Field to store the current sprint.                              |
+| story_points |    ✅     | Field to store the estimation in story points of a development. |
 
 ### Project configuration
 
 The `projects` node will provide the configuration for each project.
 
 **_In Yaml :_**
 ```yaml
 projects:
   <project name>:
     jql: "project = TEST"
     report:
       space: "SPACE"
       parent_page: "My Parent Page"
+    workflow:
+      - name: "Backlog"
+        status:
+          - "Backlog"
+      - name: "In progress"
+        status:
+          - "In progress"
+          - "In review"
+      - name: "Done"
+        status:
+          - "Closed"
 ```
 **_In Json :_**
 ```json
 {
   "projects": {
     "<project name>": {
       "jql": "project = TEST",
       "report": {
         "space": "SPACE",
         "parent_page": "My Parent Page"
-      }
+      },
+      "workflow": [
+        {
+          "name": "Backlog",
+          "status": [
+            "Backlog"
+          ]
+        },
+        {
+          "name": "In progress",
+          "status": [
+            "In progress",
+            "In review"
+          ]
+        },
+        {
+          "name": "Done",
+          "status": [
+            "Closed"
+          ]
+        }
+      ]
     }
   }
 }
 ```
 
-| Attribute        | Required | Description                                                                                                                           |
-|------------------|:--------:|---------------------------------------------------------------------------------------------------------------------------------------|
-| projects         |    ✅     | Main configuration node for all projects.                                                                                             |
-| \<project name\> |    ✅     | Must be replaced by the name of the project.<br/>This name will be used as a title of the report.                                     |
-| jql              |    ✅     | [JQL](https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14) query to retrieve the list of tickets |
-| report           |    ✅     | Configuration node for all attributes related to report generation                                                                    |
-| space            |    ✅     | Confluence destination space.<br/>                                                                                                    |
-| parent_page      |    ✅     | Confluence parent page of the report page.                                                                                            |
-| template         |    ❌     | Path to Jinja2 template used to produce the report page.                                                                              |
+| Attribute        | Required | Description                                                                                                                            |
+|------------------|:--------:|----------------------------------------------------------------------------------------------------------------------------------------|
+| projects         |    ✅     | Main configuration node for all projects.                                                                                              |
+| \<project name\> |    ✅     | Must be replaced by the name of the project.<br/>This name will be used as a title of the report.                                      |
+| jql              |    ✅     | [JQL](https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14) query to retrieve the list of tickets. |
+| report           |    ✅     | Configuration node for all attributes related to report generation.                                                                    |
+| space            |    ✅     | Confluence destination space.                                                                                                          |
+| parent_page      |    ✅     | Confluence parent page of the report page.                                                                                             |
+| workflow         |    ✅     | Configuration node for defining workflow.                                                                                              |
+
+#### Report configuration
+
+Specific configuration to publish the report on Confluence.
+
+| Attribute   | Required | Description                                              |
+|-------------|:--------:|----------------------------------------------------------|
+| space       |    ✅     | Confluence destination space.                            |
+| parent_page |    ✅     | Confluence parent page of the report page.               |
+| template    |    ❌     | Path to Jinja2 template used to produce the report page. |
+
+#### Workflow configuration
+
+The workflow defines a list of states. Each state permits to map several Jira
+state to a "Virtual" state to simplify the metrics charts. 
+
+| Attribute | Required | Description                                                                                                   |
+|-----------|:--------:|---------------------------------------------------------------------------------------------------------------|
+| name      |    ✅     | Confluence destination space.                                                                                 |
+| status    |    ✅     | Confluence parent page of the report page.                                                                    |
+| start     |    ❌     | Boolean value to define the current state is considered as the start of the work in order to compute metrics. |
+| stop      |    ❌     | Boolean value to define the current state is considered as the stop of the work in order to compute metrics.  |
 
 ## Contribution
 
 Unless you explicitly state otherwise, any contribution intentionally submitted
 for inclusion in the work by you, shall be as defined in the Apache-2.0 license
 without any additional terms or conditions.
```

### Comparing `rate_my_project-1.0.0/README.md` & `rate_my_project-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: rate_my_project
+Version: 1.1.0
+Summary: Swiss knife tool for analyzing project efficiency
+Home-page: https://github.com/cledouarec/rate-my-project
+Author: Christophe Le Douarec
+Author-email: ledouarec@gmail.com
+License: Apache License 2.0
+Keywords: team efficiency data visualization analysis
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Rate my project
 
 [![Lint](https://github.com/cledouarec/rate-my-project/actions/workflows/lint.yaml/badge.svg)](https://github.com/cledouarec/rate-my-project/actions/workflows/lint.yaml)
 [![Unit tests](https://github.com/cledouarec/rate-my-project/actions/workflows/test.yaml/badge.svg)](https://github.com/cledouarec/rate-my-project/actions/workflows/test.yaml)
 
 **Table of Contents**
 - [Rate my project](#rate-my-project)
@@ -178,15 +196,15 @@
 }
 ```
 
 | Attribute  | Required | Description                                      |
 |------------|:--------:|--------------------------------------------------|
 | server     |    ✅     | Main configuration node for server.              |
 | jira       |    ✅     | Jira server URL to retrieve tickets information. |
-| confluence |    ✅     | Confluence server URL to publish the report      |
+| confluence |    ✅     | Confluence server URL to publish the report.     |
 
 ### Fields configuration
 
 The `fields` node will configure the field name to use since it could be custom
 fields.
 
 **_In Yaml :_**
@@ -201,57 +219,111 @@
   "fields": {
     "sprint": "customfield_10001",
     "story_points": "customfield_10002"
   }
 }
 ```
 
-| Attribute    | Required | Description                                                    |
-|--------------|:--------:|----------------------------------------------------------------|
-| fields       |    ✅     | Main configuration node for fields.                            |
-| sprint       |    ✅     | Field to store the current sprint                              |
-| story_points |    ✅     | Field to store the estimation in story points of a development |
+| Attribute    | Required | Description                                                     |
+|--------------|:--------:|-----------------------------------------------------------------|
+| fields       |    ✅     | Main configuration node for fields.                             |
+| sprint       |    ✅     | Field to store the current sprint.                              |
+| story_points |    ✅     | Field to store the estimation in story points of a development. |
 
 ### Project configuration
 
 The `projects` node will provide the configuration for each project.
 
 **_In Yaml :_**
 ```yaml
 projects:
   <project name>:
     jql: "project = TEST"
     report:
       space: "SPACE"
       parent_page: "My Parent Page"
+    workflow:
+      - name: "Backlog"
+        status:
+          - "Backlog"
+      - name: "In progress"
+        status:
+          - "In progress"
+          - "In review"
+      - name: "Done"
+        status:
+          - "Closed"
 ```
 **_In Json :_**
 ```json
 {
   "projects": {
     "<project name>": {
       "jql": "project = TEST",
       "report": {
         "space": "SPACE",
         "parent_page": "My Parent Page"
-      }
+      },
+      "workflow": [
+        {
+          "name": "Backlog",
+          "status": [
+            "Backlog"
+          ]
+        },
+        {
+          "name": "In progress",
+          "status": [
+            "In progress",
+            "In review"
+          ]
+        },
+        {
+          "name": "Done",
+          "status": [
+            "Closed"
+          ]
+        }
+      ]
     }
   }
 }
 ```
 
-| Attribute        | Required | Description                                                                                                                           |
-|------------------|:--------:|---------------------------------------------------------------------------------------------------------------------------------------|
-| projects         |    ✅     | Main configuration node for all projects.                                                                                             |
-| \<project name\> |    ✅     | Must be replaced by the name of the project.<br/>This name will be used as a title of the report.                                     |
-| jql              |    ✅     | [JQL](https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14) query to retrieve the list of tickets |
-| report           |    ✅     | Configuration node for all attributes related to report generation                                                                    |
-| space            |    ✅     | Confluence destination space.<br/>                                                                                                    |
-| parent_page      |    ✅     | Confluence parent page of the report page.                                                                                            |
-| template         |    ❌     | Path to Jinja2 template used to produce the report page.                                                                              |
+| Attribute        | Required | Description                                                                                                                            |
+|------------------|:--------:|----------------------------------------------------------------------------------------------------------------------------------------|
+| projects         |    ✅     | Main configuration node for all projects.                                                                                              |
+| \<project name\> |    ✅     | Must be replaced by the name of the project.<br/>This name will be used as a title of the report.                                      |
+| jql              |    ✅     | [JQL](https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14) query to retrieve the list of tickets. |
+| report           |    ✅     | Configuration node for all attributes related to report generation.                                                                    |
+| space            |    ✅     | Confluence destination space.                                                                                                          |
+| parent_page      |    ✅     | Confluence parent page of the report page.                                                                                             |
+| workflow         |    ✅     | Configuration node for defining workflow.                                                                                              |
+
+#### Report configuration
+
+Specific configuration to publish the report on Confluence.
+
+| Attribute   | Required | Description                                              |
+|-------------|:--------:|----------------------------------------------------------|
+| space       |    ✅     | Confluence destination space.                            |
+| parent_page |    ✅     | Confluence parent page of the report page.               |
+| template    |    ❌     | Path to Jinja2 template used to produce the report page. |
+
+#### Workflow configuration
+
+The workflow defines a list of states. Each state permits to map several Jira
+state to a "Virtual" state to simplify the metrics charts. 
+
+| Attribute | Required | Description                                                                                                   |
+|-----------|:--------:|---------------------------------------------------------------------------------------------------------------|
+| name      |    ✅     | Confluence destination space.                                                                                 |
+| status    |    ✅     | Confluence parent page of the report page.                                                                    |
+| start     |    ❌     | Boolean value to define the current state is considered as the start of the work in order to compute metrics. |
+| stop      |    ❌     | Boolean value to define the current state is considered as the stop of the work in order to compute metrics.  |
 
 ## Contribution
 
 Unless you explicitly state otherwise, any contribution intentionally submitted
 for inclusion in the work by you, shall be as defined in the Apache-2.0 license
 without any additional terms or conditions.
```

### Comparing `rate_my_project-1.0.0/pyproject.toml` & `rate_my_project-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.0"
+version = "1.1.0"
 version_files = [
     "src/rate_my_project/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 style = [
     ["qmark", "fg:#ff9d00 bold"],
     ["question", "bold"],
```

### Comparing `rate_my_project-1.0.0/setup.cfg` & `rate_my_project-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/src/rate_my_project/cli.py` & `rate_my_project-1.1.0/src/rate_my_project/cli.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/src/rate_my_project/config.py` & `rate_my_project-1.1.0/src/rate_my_project/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
     #: Project name
     name: str
     #: Query to retrieve tickets
     jql: str
     #: Report configuration.
     report: Report
-    # Workflow configuration.
+    #: Workflow configuration.
     workflow: List[WorkflowState]
 
     class Config:
         """
         Specific configuration.
         """
```

### Comparing `rate_my_project-1.0.0/src/rate_my_project/connectors/confluenceclient.py` & `rate_my_project-1.1.0/src/rate_my_project/connectors/confluenceclient.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/src/rate_my_project/connectors/httpclient.py` & `rate_my_project-1.1.0/src/rate_my_project/connectors/httpclient.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/src/rate_my_project/connectors/jiraclient.py` & `rate_my_project-1.1.0/src/rate_my_project/connectors/jiraclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,14 +91,34 @@
 
             if query["startAt"] + query["maxResults"] >= response["total"]:
                 break
             query["startAt"] += query["maxResults"]
 
         return responses
 
+    async def ticket(
+        self, key: str, fields: Optional[Union[List[str], str]] = None
+    ) -> dict:
+        """
+        Get ticket information from a given `key`.
+
+        :param key: Key of the ticket.
+        :param fields: list of fields, for example: ['priority', 'summary']
+        :return: Ticket information.
+        """
+        if fields is None:
+            fields = "*all"
+
+        query = {
+            "fields": fields,
+        }
+        return await self._http_client.get(
+            f"issue/{key}", self.STANDARD_HEADERS, query
+        )
+
     async def validate_jql(self, jql: str):
         """
         Validate `jql` request.
 
         :param jql: JQL request to validate.
         """
         query = {"queries": [jql]}
@@ -156,14 +176,43 @@
         tasks = []
         for ticket in tickets:
             task = asyncio.create_task(self.changelogs(ticket["key"]))
             tasks.append(task)
 
         return await asyncio.gather(*tasks)
 
+    async def parents_from_tickets(self, tickets: list) -> list:
+        """
+        Get parents information from a list of `tickets`.
+
+        :param tickets: List of tickets.
+        :return: List of parents information.
+        """
+        tasks = []
+        for ticket in tickets:
+            if ticket["fields"].get("parent"):
+                task = asyncio.create_task(
+                    self.ticket(ticket["fields"]["parent"]["key"])
+                )
+                tasks.append(task)
+
+        return await asyncio.gather(*tasks)
+
+    async def versions(self, key: str) -> list:
+        """
+        Get all versions of a given project ordered by ranking.
+
+        :param key: Key of the project.
+        :return: Versions list.
+        """
+        query = {"startAt": 0, "maxResults": 100, "orderBy": "-sequence"}
+        return await self._get_paginated(
+            f"project/{key}/version", self.STANDARD_HEADERS, query, "values"
+        )
+
     async def fields_information(self):
         """
         Get all fields information like id and associated display name.
 
         :return: List of fields information.
         """
         return await self._http_client.get("field", self.STANDARD_HEADERS)
```

### Comparing `rate_my_project-1.0.0/src/rate_my_project/dashboard.py` & `rate_my_project-1.1.0/src/rate_my_project/dashboard.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/src/rate_my_project/metrics/metric.py` & `rate_my_project-1.1.0/src/rate_my_project/metrics/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 @dataclass
 class MetricData:
     """
     This class is used to store all the tickets information used to produce
     metrics and analysis.
     """
 
+    #: Raw data in case of advanced or custom processing needed
+    raw: tuple
+
     #: Basics information like title, reporter, type, nb sprint, etc
     info: pd.DataFrame
 
     #: Information which change during time like status, assignee, etc
     changes: pd.DataFrame
 
     #: Workflow of the project
@@ -39,53 +42,67 @@
     @classmethod
     def from_tickets_and_changelogs(
         cls,
         fields: dict,
         workflow: list,
         tickets: list,
         tickets_changelogs: list,
+        tickets_parents: list,
     ) -> MetricData:
         """
         Create data for metric from `tickets` and `changelogs` information.
 
         :param fields: Dictionary of fields to retrieve.
+        :param workflow: List of state in the workflow.
         :param tickets: List of tickets information.
         :param tickets_changelogs: List of changelogs associated to tickets.
-        :param workflow: List of state in the workflow.
+        :param tickets_parents: List of parent tickets associated to tickets.
         :return: Data for metric.
         """
         logger.debug("Create data for metric from tickets and changelogs")
 
+        raw = (fields, workflow, tickets, tickets_changelogs, tickets_parents)
+
         tickets_info = []
         tickets_changes = []
         status_backlog = cls._map_status_from_workflow("Backlog", workflow)
 
         for ticket, changelogs in zip(tickets, tickets_changelogs):
             key = ticket["key"]
             sprints = ticket["fields"].get(fields["sprint"])
             if not sprints:
                 sprints = []
 
+            fix_versions = []
+            for fix_version in ticket["fields"]["fixVersions"]:
+                fix_versions.append(fix_version["name"])
+
+            parent = None
+            if ticket["fields"].get("parent"):
+                parent = ticket["fields"]["parent"]["key"]
+
             tickets_info.append(
                 {
                     "key": key,
+                    "type": ticket["fields"]["issuetype"]["name"],
                     "summary": ticket["fields"]["summary"],
                     "reporter": ticket["fields"]["reporter"]["displayName"],
                     "story point": ticket["fields"].get(
                         fields["story_points"]
                     ),
                     "sprints": len(sprints),
+                    "versions": fix_versions,
+                    "parent": parent,
                 }
             )
             assignee = "Unassigned"
             status = status_backlog
             tickets_changes.append(
                 {
                     "key": key,
-                    "type": ticket["fields"]["issuetype"]["name"],
                     "date": isoparse(ticket["fields"]["created"]),
                     "assignee": assignee,
                     "status": status,
                 }
             )
 
             for changelog in changelogs:
@@ -104,15 +121,14 @@
                         )
                     else:
                         continue
 
                     tickets_changes.append(
                         {
                             "key": key,
-                            "type": ticket["fields"]["issuetype"]["name"],
                             "date": isoparse(changelog["created"]),
                             "assignee": assignee,
                             "status": status,
                         }
                     )
 
         tickets_info_df = pd.DataFrame.from_records(tickets_info, index="key")
@@ -124,15 +140,15 @@
             categories=[state["name"] for state in workflow], ordered=True
         )
         tickets_changes_df["status"] = tickets_changes_df["status"].astype(
             status_order
         )
 
         logger.debug("Data for metric created")
-        return cls(tickets_info_df, tickets_changes_df, workflow)
+        return cls(raw, tickets_info_df, tickets_changes_df, workflow)
 
     @staticmethod
     def _map_status_from_workflow(status: str, workflow: list) -> str:
         """
         Search the `status` associated in the `workflow` and map to the state
         name. If the `status` is not associated to a state, it returns the
         given `status` in input.
@@ -210,17 +226,27 @@
         """
         Helper function to set a graph in a common layout.
 
         :param title: Title of the graph.
         :param figure: Graph.
         :return: Dash widgets.
         """
+        figure.update_traces(
+            hoverinfo="label+percent", textinfo="value+percent"
+        )
         return dbc.Col(
             dbc.Card(
                 [
                     dbc.CardHeader(title),
-                    dbc.CardBody(dcc.Graph(figure=figure)),
+                    dbc.CardBody(
+                        dcc.Graph(
+                            figure=figure,
+                            config={
+                                "displaylogo": False,
+                            },
+                        )
+                    ),
                 ]
             ),
             md=12,
             lg=6,
         )
```

### Comparing `rate_my_project-1.0.0/src/rate_my_project/metrics/status.py` & `rate_my_project-1.1.0/src/rate_my_project/metrics/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         Compute the number of tickets in a status for each issue type.
 
         :param data: Metric input data.
         :return: Dictionary with a graph for each issue type name.
         """
         result = {}
 
-        groups = data.changes.groupby("type")
+        groups = data.changes.merge(data.info, on="key").groupby("type")
 
         for issue_type, group in groups:
             df_per_type = group[["key", "status"]].drop_duplicates(
                 subset="key", keep="last"
             )
             status_per_type = (
                 df_per_type["status"]
```

### Comparing `rate_my_project-1.0.0/src/rate_my_project/report.py` & `rate_my_project-1.1.0/src/rate_my_project/report.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/src/rate_my_project/utils.py` & `rate_my_project-1.1.0/src/rate_my_project/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     """
     Fetch tickets and associated changelogs information from `JQL` query.
 
     TODO The fields list will be fetched to retrieve custom fields if needed.
 
     :param jira_client: Jira client to retrieve tickets information.
     :param jql: JQL query.
-    :return: Tickets and changelogs.
+    :return: Tickets, changelogs and parents tickets.
     """
     async with jira_client as jira_session:
         tickets = await jira_session.tickets_from_jql(jql)
         changelogs = await jira_session.changelogs_from_tickets(tickets)
+        parents = await jira_session.parents_from_tickets(tickets)
         # fields = await jira_session.fields_information()
-        return tickets, changelogs
+        return tickets, changelogs, parents
```

### Comparing `rate_my_project-1.0.0/src/rate_my_project.egg-info/PKG-INFO` & `rate_my_project-1.1.0/src/rate_my_project.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rate-my-project
-Version: 1.0.0
+Version: 1.1.0
 Summary: Swiss knife tool for analyzing project efficiency
 Home-page: https://github.com/cledouarec/rate-my-project
 Author: Christophe Le Douarec
 Author-email: ledouarec@gmail.com
 License: Apache License 2.0
 Keywords: team efficiency data visualization analysis
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -196,15 +196,15 @@
 }
 ```
 
 | Attribute  | Required | Description                                      |
 |------------|:--------:|--------------------------------------------------|
 | server     |    ✅     | Main configuration node for server.              |
 | jira       |    ✅     | Jira server URL to retrieve tickets information. |
-| confluence |    ✅     | Confluence server URL to publish the report      |
+| confluence |    ✅     | Confluence server URL to publish the report.     |
 
 ### Fields configuration
 
 The `fields` node will configure the field name to use since it could be custom
 fields.
 
 **_In Yaml :_**
@@ -219,57 +219,111 @@
   "fields": {
     "sprint": "customfield_10001",
     "story_points": "customfield_10002"
   }
 }
 ```
 
-| Attribute    | Required | Description                                                    |
-|--------------|:--------:|----------------------------------------------------------------|
-| fields       |    ✅     | Main configuration node for fields.                            |
-| sprint       |    ✅     | Field to store the current sprint                              |
-| story_points |    ✅     | Field to store the estimation in story points of a development |
+| Attribute    | Required | Description                                                     |
+|--------------|:--------:|-----------------------------------------------------------------|
+| fields       |    ✅     | Main configuration node for fields.                             |
+| sprint       |    ✅     | Field to store the current sprint.                              |
+| story_points |    ✅     | Field to store the estimation in story points of a development. |
 
 ### Project configuration
 
 The `projects` node will provide the configuration for each project.
 
 **_In Yaml :_**
 ```yaml
 projects:
   <project name>:
     jql: "project = TEST"
     report:
       space: "SPACE"
       parent_page: "My Parent Page"
+    workflow:
+      - name: "Backlog"
+        status:
+          - "Backlog"
+      - name: "In progress"
+        status:
+          - "In progress"
+          - "In review"
+      - name: "Done"
+        status:
+          - "Closed"
 ```
 **_In Json :_**
 ```json
 {
   "projects": {
     "<project name>": {
       "jql": "project = TEST",
       "report": {
         "space": "SPACE",
         "parent_page": "My Parent Page"
-      }
+      },
+      "workflow": [
+        {
+          "name": "Backlog",
+          "status": [
+            "Backlog"
+          ]
+        },
+        {
+          "name": "In progress",
+          "status": [
+            "In progress",
+            "In review"
+          ]
+        },
+        {
+          "name": "Done",
+          "status": [
+            "Closed"
+          ]
+        }
+      ]
     }
   }
 }
 ```
 
-| Attribute        | Required | Description                                                                                                                           |
-|------------------|:--------:|---------------------------------------------------------------------------------------------------------------------------------------|
-| projects         |    ✅     | Main configuration node for all projects.                                                                                             |
-| \<project name\> |    ✅     | Must be replaced by the name of the project.<br/>This name will be used as a title of the report.                                     |
-| jql              |    ✅     | [JQL](https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14) query to retrieve the list of tickets |
-| report           |    ✅     | Configuration node for all attributes related to report generation                                                                    |
-| space            |    ✅     | Confluence destination space.<br/>                                                                                                    |
-| parent_page      |    ✅     | Confluence parent page of the report page.                                                                                            |
-| template         |    ❌     | Path to Jinja2 template used to produce the report page.                                                                              |
+| Attribute        | Required | Description                                                                                                                            |
+|------------------|:--------:|----------------------------------------------------------------------------------------------------------------------------------------|
+| projects         |    ✅     | Main configuration node for all projects.                                                                                              |
+| \<project name\> |    ✅     | Must be replaced by the name of the project.<br/>This name will be used as a title of the report.                                      |
+| jql              |    ✅     | [JQL](https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14) query to retrieve the list of tickets. |
+| report           |    ✅     | Configuration node for all attributes related to report generation.                                                                    |
+| space            |    ✅     | Confluence destination space.                                                                                                          |
+| parent_page      |    ✅     | Confluence parent page of the report page.                                                                                             |
+| workflow         |    ✅     | Configuration node for defining workflow.                                                                                              |
+
+#### Report configuration
+
+Specific configuration to publish the report on Confluence.
+
+| Attribute   | Required | Description                                              |
+|-------------|:--------:|----------------------------------------------------------|
+| space       |    ✅     | Confluence destination space.                            |
+| parent_page |    ✅     | Confluence parent page of the report page.               |
+| template    |    ❌     | Path to Jinja2 template used to produce the report page. |
+
+#### Workflow configuration
+
+The workflow defines a list of states. Each state permits to map several Jira
+state to a "Virtual" state to simplify the metrics charts. 
+
+| Attribute | Required | Description                                                                                                   |
+|-----------|:--------:|---------------------------------------------------------------------------------------------------------------|
+| name      |    ✅     | Confluence destination space.                                                                                 |
+| status    |    ✅     | Confluence parent page of the report page.                                                                    |
+| start     |    ❌     | Boolean value to define the current state is considered as the start of the work in order to compute metrics. |
+| stop      |    ❌     | Boolean value to define the current state is considered as the stop of the work in order to compute metrics.  |
 
 ## Contribution
 
 Unless you explicitly state otherwise, any contribution intentionally submitted
 for inclusion in the work by you, shall be as defined in the Apache-2.0 license
 without any additional terms or conditions.
```

### Comparing `rate_my_project-1.0.0/src/rate_my_project.egg-info/SOURCES.txt` & `rate_my_project-1.1.0/src/rate_my_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/tests/test_config.py` & `rate_my_project-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/tests/test_confluenceclient.py` & `rate_my_project-1.1.0/tests/test_confluenceclient.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/tests/test_httpclient.py` & `rate_my_project-1.1.0/tests/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `rate_my_project-1.0.0/tests/test_jiraclient.py` & `rate_my_project-1.1.0/tests/test_jiraclient.py`

 * *Files identical despite different names*

