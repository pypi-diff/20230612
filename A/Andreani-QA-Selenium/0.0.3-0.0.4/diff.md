# Comparing `tmp/Andreani_QA_Selenium-0.0.3.tar.gz` & `tmp/Andreani_QA_Selenium-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Selenium-0.0.3.tar", last modified: Fri Jun  9 20:41:02 2023, max compression
+gzip compressed data, was "Andreani_QA_Selenium-0.0.4.tar", last modified: Mon Jun 12 13:43:17 2023, max compression
```

## Comparing `Andreani_QA_Selenium-0.0.3.tar` & `Andreani_QA_Selenium-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:41:02.211073 Andreani_QA_Selenium-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-09 20:41:02.178445 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium/
--rw-rw-rw-   0        0        0    96639 2023-06-08 13:48:30.000000 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium/Selenium.py
--rw-rw-rw-   0        0        0       33 2023-02-13 17:35:28.000000 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:41:02.204443 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium.egg-info/
--rw-rw-rw-   0        0        0      310 2023-06-09 20:41:02.000000 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-09 20:41:02.000000 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:41:02.000000 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-06-09 20:41:02.000000 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-09 20:41:02.000000 Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      310 2023-06-09 20:41:02.208831 Andreani_QA_Selenium-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 20:41:02.211073 Andreani_QA_Selenium-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-06-09 20:40:51.000000 Andreani_QA_Selenium-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:43:17.676567 Andreani_QA_Selenium-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-12 13:43:17.660856 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/
+-rw-rw-rw-   0        0        0    96650 2023-06-09 20:57:03.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/Selenium.py
+-rw-rw-rw-   0        0        0       33 2023-02-13 17:35:28.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:43:17.673429 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      310 2023-06-12 13:43:17.675526 Andreani_QA_Selenium-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 13:43:17.676567 Andreani_QA_Selenium-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2023-06-09 20:57:03.000000 Andreani_QA_Selenium-0.0.4/setup.py
```

### Comparing `Andreani_QA_Selenium-0.0.3/Andreani_QA_Selenium/Selenium.py` & `Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/Selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import IEDriverManager
 from Andreani_QA_parameters.Parameters import Parameters
 from Andreani_QA_Functions.Functions import Functions
 
 if platform.system() == "Windows":
     from win32com.client import Dispatch
-    from functions.Debugger import Debugger
+    from Andreani_QA_Debugger.Debugger import Debugger
 
 
 class Selenium(Functions, Parameters):
     windows = {}
     driver = None
     value_to_find = None
     get_locator_type = None
```

### Comparing `Andreani_QA_Selenium-0.0.3/setup.py` & `Andreani_QA_Selenium-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 PACKAGE_NAME = 'Andreani_QA_Selenium'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'SeleniumFramework para ejecución de casos automatizados'  # Descripción corta
```

