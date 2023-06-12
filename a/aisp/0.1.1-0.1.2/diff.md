# Comparing `tmp/aisp-0.1.1.tar.gz` & `tmp/aisp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisp-0.1.1.tar", last modified: Thu Jun  8 16:10:38 2023, max compression
+gzip compressed data, was "aisp-0.1.2.tar", last modified: Mon Jun 12 17:37:41 2023, max compression
```

## Comparing `aisp-0.1.1.tar` & `aisp-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.136405 aisp-0.1.1/
--rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     8016 2023-06-08 16:10:38.133383 aisp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6852 2023-06-08 15:06:17.000000 aisp-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.100382 aisp-0.1.1/aisp/
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.129382 aisp-0.1.1/aisp/NSA/
--rw-rw-rw-   0        0        0      116 2023-05-28 13:47:18.000000 aisp-0.1.1/aisp/NSA/__init__.py
--rw-rw-rw-   0        0        0    48346 2023-06-08 15:27:54.000000 aisp-0.1.1/aisp/NSA/_negativeSelection.py
--rw-rw-rw-   0        0        0     8040 2023-06-08 15:52:49.000000 aisp-0.1.1/aisp/_base.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.119385 aisp-0.1.1/aisp.egg-info/
--rw-rw-rw-   0        0        0     8016 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1349 2023-06-08 15:56:51.000000 aisp-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 16:10:38.137386 aisp-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 17:37:41.698555 aisp-0.1.2/
+-rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8135 2023-06-12 17:37:41.696553 aisp-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6854 2023-06-08 16:13:42.000000 aisp-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 17:37:41.694552 aisp-0.1.2/aisp.egg-info/
+-rw-rw-rw-   0        0        0     8135 2023-06-12 17:37:41.000000 aisp-0.1.2/aisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-12 17:37:41.000000 aisp-0.1.2/aisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 17:37:41.000000 aisp-0.1.2/aisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-12 17:37:41.000000 aisp-0.1.2/aisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 17:37:41.000000 aisp-0.1.2/aisp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1349 2023-06-12 17:24:25.000000 aisp-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 17:37:41.698555 aisp-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-06-12 17:23:50.000000 aisp-0.1.2/setup.py
```

### Comparing `aisp-0.1.1/LICENSE` & `aisp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aisp-0.1.1/PKG-INFO` & `aisp-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package with techniques of artificial immune systems.
+Home-page: https://github.com/AIS-Package/aisp
+Author: João Paulo da Silva Barros
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
+Maintainer: Alison Zille Lopes
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
 Project-URL: Tracker, https://github.com/AIS-Package/aisp/issues
 Keywords: Artificial Immune Systems,classification,Natural computing,machine learning,artificial intelligence
@@ -65,15 +68,15 @@
 > 3. [Examples.](#examples)
 
 ---
 <section id='introduction'>
 
 #### Introduction
 
-The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (GPLv3).
+The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (LGPLv3).
 
 The package started in **2022** as a research package at the Federal Institute of Northern Minas Gerais - Salinas campus (**IFNMG - Salinas**).
 
 
 Artificial Immune Systems (AIS) are inspired by the vertebrate immune system, creating metaphors that apply the ability to detect and catalog pathogens, among other features of this system.
 
 ##### Algorithms implemented:
@@ -175,15 +178,15 @@
 > 3. [Exemplos.](#exemplos)
 
 ---
 <section id='introdução'>
 
 #### Introdução
 
-O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (GPLv3).
+O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (LGPLv3).
 
 O pacote teve início no ano de **2022** como um pacote de pesquisa no instituto federal do norte de minas gerais - campus salinas (**IFNMG - Salinas**).
 
 Os sistemas imunológicos artificiais (SIA) inspiram-se no sistema imunológico dos vertebrados, criando metáforas que aplicam a capacidade de reconhecer e catalogar os patógenos, entre outras características desse sistema.
 
 ##### Algoritmos implementados:
```

### Comparing `aisp-0.1.1/README.md` & `aisp-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 > 3. [Examples.](#examples)
 
 ---
 <section id='introduction'>
 
 #### Introduction
 
-The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (GPLv3).
+The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (LGPLv3).
 
 The package started in **2022** as a research package at the Federal Institute of Northern Minas Gerais - Salinas campus (**IFNMG - Salinas**).
 
 
 Artificial Immune Systems (AIS) are inspired by the vertebrate immune system, creating metaphors that apply the ability to detect and catalog pathogens, among other features of this system.
 
 ##### Algorithms implemented:
@@ -151,15 +151,15 @@
 > 3. [Exemplos.](#exemplos)
 
 ---
 <section id='introdução'>
 
 #### Introdução
 
-O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (GPLv3).
+O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (LGPLv3).
 
 O pacote teve início no ano de **2022** como um pacote de pesquisa no instituto federal do norte de minas gerais - campus salinas (**IFNMG - Salinas**).
 
 Os sistemas imunológicos artificiais (SIA) inspiram-se no sistema imunológico dos vertebrados, criando metáforas que aplicam a capacidade de reconhecer e catalogar os patógenos, entre outras características desse sistema.
 
 ##### Algoritmos implementados:
```

### Comparing `aisp-0.1.1/aisp.egg-info/PKG-INFO` & `aisp-0.1.2/aisp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Package with techniques of artificial immune systems.
+Home-page: https://github.com/AIS-Package/aisp
+Author: João Paulo da Silva Barros
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
+Maintainer: Alison Zille Lopes
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
 Project-URL: Tracker, https://github.com/AIS-Package/aisp/issues
 Keywords: Artificial Immune Systems,classification,Natural computing,machine learning,artificial intelligence
@@ -65,15 +68,15 @@
 > 3. [Examples.](#examples)
 
 ---
 <section id='introduction'>
 
 #### Introduction
 
-The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (GPLv3).
+The **AISP** is a python package that implements artificial immune systems techniques, distributed under the GNU Lesser General Public License v3.0 (LGPLv3).
 
 The package started in **2022** as a research package at the Federal Institute of Northern Minas Gerais - Salinas campus (**IFNMG - Salinas**).
 
 
 Artificial Immune Systems (AIS) are inspired by the vertebrate immune system, creating metaphors that apply the ability to detect and catalog pathogens, among other features of this system.
 
 ##### Algorithms implemented:
@@ -175,15 +178,15 @@
 > 3. [Exemplos.](#exemplos)
 
 ---
 <section id='introdução'>
 
 #### Introdução
 
-O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (GPLv3).
+O **AISP** é um pacote python que implementa as técnicas dos sistemas imunológicos artificiais, distribuído sob a licença GNU Lesser General Public License v3.0 (LGPLv3).
 
 O pacote teve início no ano de **2022** como um pacote de pesquisa no instituto federal do norte de minas gerais - campus salinas (**IFNMG - Salinas**).
 
 Os sistemas imunológicos artificiais (SIA) inspiram-se no sistema imunológico dos vertebrados, criando metáforas que aplicam a capacidade de reconhecer e catalogar os patógenos, entre outras características desse sistema.
 
 ##### Algoritmos implementados:
```

### Comparing `aisp-0.1.1/pyproject.toml` & `aisp-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aisp"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="João Paulo da Silva Barros", email="jpsilvabarr@gmail.com" },
 ]
 
 maintainers = [
   { name="Alison Zille Lopes",  email="alisonzille@gmail.com"},
 ]
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
     "numpy>=1.22.4",
     "scipy>=1.8.1",
-    "tqdm==4.64.1",
+    "tqdm>=4.64.1",
 ]
 
 keywords = ["Artificial Immune Systems", "classification", "Natural computing", "machine learning", "artificial intelligence"]
 
 [project.urls]
 Homepage = "https://ais-package.github.io/"
 Documentation = "https://ais-package.github.io/docs/intro"
```

