# Comparing `tmp/aorta_sirius-0.6.tar.gz` & `tmp/aorta_sirius-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aorta_sirius-0.6.tar", last modified: Sun Jun 11 10:12:00 2023, max compression
+gzip compressed data, was "aorta_sirius-0.7.tar", last modified: Sun Jun 11 22:25:39 2023, max compression
```

## Comparing `aorta_sirius-0.6.tar` & `aorta_sirius-0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.481194 aorta_sirius-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 10:12:00.481194 aorta_sirius-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 10:11:44.000000 aorta_sirius-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 10:12:00.481194 aorta_sirius-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-11 10:11:44.000000 aorta_sirius-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/aorta_sirius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 10:12:00.000000 aorta_sirius-0.6/src/aorta_sirius.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/sirius/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/sirius/application_performance_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/application_performance_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:12:00.477194 aorta_sirius-0.6/src/sirius/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-11 10:11:44.000000 aorta_sirius-0.6/src/sirius/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 22:25:39.397873 aorta_sirius-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-11 22:25:03.000000 aorta_sirius-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 22:25:39.397873 aorta_sirius-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-11 22:25:03.000000 aorta_sirius-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.393874 aorta_sirius-0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.393874 aorta_sirius-0.7/src/aorta_sirius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 22:25:39.000000 aorta_sirius-0.7/src/aorta_sirius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/src/sirius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/src/sirius/application_performance_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/application_performance_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 22:25:39.397873 aorta_sirius-0.7/src/sirius/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-11 22:25:03.000000 aorta_sirius-0.7/src/sirius/logger/__init__.py
```

### Comparing `aorta_sirius-0.6/setup.py` & `aorta_sirius-0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import List
 
 import requests
 from requests import Response
 from setuptools import setup, find_packages
 
 
 def get_package_name() -> str:
@@ -17,19 +18,22 @@
     return ".".join(version_number.split(".")[0:-1], ) + "." + str(next_subversion_number)
 
 
 def is_production_branch() -> bool:
     return "production" == os.getenv("GITHUB_REF_NAME")
 
 
+def get_required_packages() -> List[str]:
+    with open("requirements.txt", "r") as requirements_file:
+        return requirements_file.read().split("\n")
+
+
 setup(
     name=get_package_name(),
     version=get_next_version(),
     url="https://github.com/kontinuum-investments/Aorta-Sirius",
     author="Kavindu Athaudha",
     author_email="kavindu@kih.com.sg",
     packages=find_packages(where="src", include=["sirius*"]),
     package_dir={"": "src"},
-    install_requires=[
-        "rollbar"
-    ]
+    install_requires=get_required_packages()
 )
```

### Comparing `aorta_sirius-0.6/src/sirius/application_performance_monitoring/__init__.py` & `aorta_sirius-0.7/src/sirius/application_performance_monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `aorta_sirius-0.6/src/sirius/common.py` & `aorta_sirius-0.7/src/sirius/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     if value is None:
         raise ApplicationException(f"Environment variable with the key is not available: {key}")
 
     return value
 
 
 def get_environment() -> Environment:
-    environment: str = os.getenv(EnvironmentVariable.ENVIRONMENT)
+    environment: str = os.getenv(EnvironmentVariable.ENVIRONMENT.value)
     try:
         return Environment.Development if environment is None else Environment(environment)
     except ValueError:
         raise ApplicationException(f"Invalid environment variable setup: {environment}")
 
 
 def threaded(func: Callable) -> Callable:
```

