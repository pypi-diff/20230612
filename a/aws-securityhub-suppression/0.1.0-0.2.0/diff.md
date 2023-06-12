# Comparing `tmp/aws_securityhub_suppression-0.1.0.tar.gz` & `tmp/aws_securityhub_suppression-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_securityhub_suppression-0.1.0.tar", max compression
+gzip compressed data, was "aws_securityhub_suppression-0.2.0.tar", max compression
```

## Comparing `aws_securityhub_suppression-0.1.0.tar` & `aws_securityhub_suppression-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       92 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/README.md
--rw-r--r--   0        0        0     1236 2023-06-12 09:20:35.959868 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/__init__.py
--rw-r--r--   0        0        0     1058 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/account.py
--rw-r--r--   0        0        0      515 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/commands/__init__.py
--rw-r--r--   0        0        0      970 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/commands/prepare.py
--rw-r--r--   0        0        0     1583 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/commands/update.py
--rw-r--r--   0        0        0      793 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/context.py
--rw-r--r--   0        0        0      744 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/handler.py
--rw-r--r--   0        0        0     1133 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/documentation_generator.py
--rw-r--r--   0        0        0     1630 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/suppress_findings.py
--rw-r--r--   0        0        0      768 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/suppression.py
--rw-r--r--   0        0        0      672 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/workload.py
--rw-r--r--   0        0        0     1695 2023-06-12 09:20:35.251853 aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/workload_generator.py
--rw-r--r--   0        0        0     1197 2023-06-12 09:20:35.959868 aws_securityhub_suppression-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      820 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/README.md
+-rw-r--r--   0        0        0     1236 2023-06-12 17:39:10.784961 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/__init__.py
+-rw-r--r--   0        0        0     1058 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/account.py
+-rw-r--r--   0        0        0      515 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/__init__.py
+-rw-r--r--   0        0        0      970 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/prepare.py
+-rw-r--r--   0        0        0     1583 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/update.py
+-rw-r--r--   0        0        0      793 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/context.py
+-rw-r--r--   0        0        0      744 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/handler.py
+-rw-r--r--   0        0        0     1133 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/documentation_generator.py
+-rw-r--r--   0        0        0     1024 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/finding.py
+-rw-r--r--   0        0        0     1307 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppress_findings.py
+-rw-r--r--   0        0        0      865 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppression.py
+-rw-r--r--   0        0        0      672 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload.py
+-rw-r--r--   0        0        0     1695 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload_generator.py
+-rw-r--r--   0        0        0     1197 2023-06-12 17:39:10.788961 aws_securityhub_suppression-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.2.0/PKG-INFO
```

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/__init__.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import yaml
 from aws_securityhub_suppression.account import Account
 from aws_securityhub_suppression.workload import Workload
 from aws_securityhub_suppression.suppression import Suppression
 
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 
 def load_workloads(workload_path: str) -> List[Workload]:
     workloads = glob.glob(os.path.join(workload_path, "**/info.yaml"), recursive=True)
 
     def load_workload(file: str) -> Optional[Workload]:
         return load_workload_by_file(file)
```

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/account.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/account.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/__init__.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/commands/prepare.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/commands/update.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/context.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/context.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/cli/handler.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/documentation_generator.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/suppress_findings.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppress_findings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 from typing import List
 
 from aws_securityhub_suppression import Workload
+from aws_securityhub_suppression.finding import Finding
 from aws_securityhub_suppression.suppression import Suppression
 
 
 class SuppressFindings:
     def __init__(self, client, workload: Workload) -> None:
         self.__client = client
         self.__workload = workload
 
     def execute(self):
         for account in self.__workload.accounts:
             suppress_findings = account.scheduled_for_suppression()
             self.__handle_suppressions(suppress_findings)
 
     def __handle_suppressions(self, suppressions: List[Suppression]) -> None:
-        def parse_arn(arn: str) -> dict:
-            parts = arn.split(":")
+        def convert_to_finding_identifier(finding: Finding) -> dict:
             return {
-                "Partition": parts[1],
-                "Service": parts[2],
-                "Region": parts[3],
-                "AccountId": parts[4],
-                "Type": parts[5],
-            }
-
-        def convert_to_finding_identifier(finding_id: str) -> dict:
-            arn = parse_arn(finding_id)
-            return {
-                "Id": finding_id,
-                "ProductArn": f"arn:aws:securityhub:{arn['Region']}::product/aws/securityhub",
+                "Id": finding.arn,
+                "ProductArn": finding.product_arn,
             }
 
         for suppression in suppressions:
             finding_identifiers = list(
                 map(convert_to_finding_identifier, suppression.findings)
             )
```

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/suppression.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppression.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
-from typing import Optional, List
+from typing import Optional, List, Any
+
+from aws_securityhub_suppression.finding import Finding
 
 
 class Suppression:
-    def __init__(self, name: str, reason: str, findings: List[str]) -> None:
+    def __init__(self, name: str, reason: str, findings: List[Finding]) -> None:
         self.__name = name
         self.__reason = reason
         self.__findings = findings
 
     @property
     def name(self) -> str:
         return self.__name
 
     @property
     def reason(self) -> str:
         return self.__reason
 
     @property
-    def findings(self) -> List[str]:
+    def findings(self) -> List[Finding]:
         return self.__findings
 
     @staticmethod
     def from_dict(data: dict) -> Optional[Suppression]:
         # TODO: Schema validation
         if "Name" not in data:
             return None
 
-        return Suppression(
-            name=data["Name"], reason=data["Reason"], findings=data["Findings"]
-        )
+        findings = list(map(Finding, data["Findings"]))
+
+        return Suppression(name=data["Name"], reason=data["Reason"], findings=findings)
```

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/workload.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/aws_securityhub_suppression/workload_generator.py` & `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.1.0/pyproject.toml` & `aws_securityhub_suppression-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-securityhub-suppression"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_securityhub_suppression"}]
 
 [tool.poetry.group.dev.dependencies]
```

