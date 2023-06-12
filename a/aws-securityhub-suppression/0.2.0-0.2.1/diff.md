# Comparing `tmp/aws_securityhub_suppression-0.2.0.tar.gz` & `tmp/aws_securityhub_suppression-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_securityhub_suppression-0.2.0.tar", max compression
+gzip compressed data, was "aws_securityhub_suppression-0.2.1.tar", max compression
```

## Comparing `aws_securityhub_suppression-0.2.0.tar` & `aws_securityhub_suppression-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      820 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/README.md
--rw-r--r--   0        0        0     1236 2023-06-12 17:39:10.784961 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/__init__.py
--rw-r--r--   0        0        0     1058 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/account.py
--rw-r--r--   0        0        0      515 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/__init__.py
--rw-r--r--   0        0        0      970 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/prepare.py
--rw-r--r--   0        0        0     1583 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/update.py
--rw-r--r--   0        0        0      793 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/context.py
--rw-r--r--   0        0        0      744 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/handler.py
--rw-r--r--   0        0        0     1133 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/documentation_generator.py
--rw-r--r--   0        0        0     1024 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/finding.py
--rw-r--r--   0        0        0     1307 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppress_findings.py
--rw-r--r--   0        0        0      865 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppression.py
--rw-r--r--   0        0        0      672 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload.py
--rw-r--r--   0        0        0     1695 2023-06-12 17:39:09.832973 aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload_generator.py
--rw-r--r--   0        0        0     1197 2023-06-12 17:39:10.788961 aws_securityhub_suppression-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      820 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/README.md
+-rw-r--r--   0        0        0     1236 2023-06-12 18:12:10.871699 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/__init__.py
+-rw-r--r--   0        0        0     1058 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/account.py
+-rw-r--r--   0        0        0      515 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/__init__.py
+-rw-r--r--   0        0        0      970 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/prepare.py
+-rw-r--r--   0        0        0     1583 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/update.py
+-rw-r--r--   0        0        0      793 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/context.py
+-rw-r--r--   0        0        0      744 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/handler.py
+-rw-r--r--   0        0        0     1133 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/documentation_generator.py
+-rw-r--r--   0        0        0     1024 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/finding.py
+-rw-r--r--   0        0        0     1307 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppress_findings.py
+-rw-r--r--   0        0        0      865 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppression.py
+-rw-r--r--   0        0        0      672 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload.py
+-rw-r--r--   0        0        0     1695 2023-06-12 18:12:09.999688 aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload_generator.py
+-rw-r--r--   0        0        0     1197 2023-06-12 18:12:10.871699 aws_securityhub_suppression-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.2.1/PKG-INFO
```

### Comparing `aws_securityhub_suppression-0.2.0/README.md` & `aws_securityhub_suppression-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/__init__.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import yaml
 from aws_securityhub_suppression.account import Account
 from aws_securityhub_suppression.workload import Workload
 from aws_securityhub_suppression.suppression import Suppression
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 def load_workloads(workload_path: str) -> List[Workload]:
     workloads = glob.glob(os.path.join(workload_path, "**/info.yaml"), recursive=True)
 
     def load_workload(file: str) -> Optional[Workload]:
         return load_workload_by_file(file)
```

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/account.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/account.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/__init__.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/prepare.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/commands/update.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/context.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/context.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/cli/handler.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/documentation_generator.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/finding.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/finding.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     def __init__(self, finding_arn: str) -> None:
         parts = finding_arn.split(":")
         self.__finding_arn = finding_arn
         self.__service = parts[2]
         self.__region = parts[3]
         self.__account_id = parts[4]
         self.__finding_id = parts[-1].split("/")[-1]
-        self.__generator_id = "/".join(finding_arn.split("/")[1:-1])
+        self.__generator_id = "/".join(finding_arn.split("/")[1:-2])
 
     @property
     def arn(self) -> str:
         return self.__finding_arn
 
     @property
     def id(self) -> str:
```

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppress_findings.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppress_findings.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/suppression.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/suppression.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/aws_securityhub_suppression/workload_generator.py` & `aws_securityhub_suppression-0.2.1/aws_securityhub_suppression/workload_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.2.0/pyproject.toml` & `aws_securityhub_suppression-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-securityhub-suppression"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_securityhub_suppression"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_securityhub_suppression-0.2.0/PKG-INFO` & `aws_securityhub_suppression-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-securityhub-suppression
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

