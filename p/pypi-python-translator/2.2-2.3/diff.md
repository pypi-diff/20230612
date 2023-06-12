# Comparing `tmp/pypi_python_translator-2.2.tar.gz` & `tmp/pypi_python_translator-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-2.2.tar", last modified: Mon Jun 12 18:02:02 2023, max compression
+gzip compressed data, was "pypi_python_translator-2.3.tar", last modified: Mon Jun 12 18:04:44 2023, max compression
```

## Comparing `pypi_python_translator-2.2.tar` & `pypi_python_translator-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:02:02.881022 pypi_python_translator-2.2/
--rw-rw-rw-   0        0        0     5237 2023-06-12 18:02:02.880024 pypi_python_translator-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4796 2023-06-12 17:59:27.000000 pypi_python_translator-2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:02:02.870002 pypi_python_translator-2.2/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     5237 2023-06-12 18:02:02.000000 pypi_python_translator-2.2/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-06-12 18:02:02.000000 pypi_python_translator-2.2/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:02:02.000000 pypi_python_translator-2.2/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 18:02:02.000000 pypi_python_translator-2.2/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 18:02:02.882032 pypi_python_translator-2.2/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-06-12 18:01:52.000000 pypi_python_translator-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:02:02.878008 pypi_python_translator-2.2/translator/
--rw-rw-rw-   0        0        0      740 2023-06-12 17:53:35.000000 pypi_python_translator-2.2/translator/ExampleUsages.py
--rw-rw-rw-   0        0        0     4469 2023-06-12 18:00:33.000000 pypi_python_translator-2.2/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.2/translator/languageExamples.py
--rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.2/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.2/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:04:44.769446 pypi_python_translator-2.3/
+-rw-rw-rw-   0        0        0     5412 2023-06-12 18:04:44.768431 pypi_python_translator-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4971 2023-06-12 18:04:29.000000 pypi_python_translator-2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:04:44.758916 pypi_python_translator-2.3/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     5412 2023-06-12 18:04:44.000000 pypi_python_translator-2.3/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-12 18:04:44.000000 pypi_python_translator-2.3/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:04:44.000000 pypi_python_translator-2.3/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 18:04:44.000000 pypi_python_translator-2.3/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:04:44.769446 pypi_python_translator-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-06-12 18:04:32.000000 pypi_python_translator-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:04:44.765931 pypi_python_translator-2.3/translator/
+-rw-rw-rw-   0        0        0      740 2023-06-12 17:53:35.000000 pypi_python_translator-2.3/translator/ExampleUsages.py
+-rw-rw-rw-   0        0        0     4469 2023-06-12 18:00:33.000000 pypi_python_translator-2.3/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.3/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.3/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.3/translator/services.py
```

### Comparing `pypi_python_translator-2.2/PKG-INFO` & `pypi_python_translator-2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi_python_translator
-Version: 2.2
+Version: 2.3
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,15 +72,21 @@
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
 # **Examples**
-Example usages for this package.
+Example usages for this package. you can also write those examples by using code: 
+
+```python
+from translator import *
+writeusage(example_number) #for ex -> writeusage(1) writes the first example.
+```
+
 ---
 ---
 ## `Example Usage (1): Using init() function to start program.`
 In this example we are going to use init() function to start main program in given `<language code>`, no need to much talk this is the easiest.
 ```python
 from translator import *
 init("<language code>") #For ex -> init("en") start code in english GUI.
```

### Comparing `pypi_python_translator-2.2/README.md` & `pypi_python_translator-2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,21 @@
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
 # **Examples**
-Example usages for this package.
+Example usages for this package. you can also write those examples by using code: 
+
+```python
+from translator import *
+writeusage(example_number) #for ex -> writeusage(1) writes the first example.
+```
+
 ---
 ---
 ## `Example Usage (1): Using init() function to start program.`
 In this example we are going to use init() function to start main program in given `<language code>`, no need to much talk this is the easiest.
 ```python
 from translator import *
 init("<language code>") #For ex -> init("en") start code in english GUI.
```

### Comparing `pypi_python_translator-2.2/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-2.3/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-python-translator
-Version: 2.2
+Version: 2.3
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,15 +72,21 @@
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
 # **Examples**
-Example usages for this package.
+Example usages for this package. you can also write those examples by using code: 
+
+```python
+from translator import *
+writeusage(example_number) #for ex -> writeusage(1) writes the first example.
+```
+
 ---
 ---
 ## `Example Usage (1): Using init() function to start program.`
 In this example we are going to use init() function to start main program in given `<language code>`, no need to much talk this is the easiest.
 ```python
 from translator import *
 init("<language code>") #For ex -> init("en") start code in english GUI.
```

### Comparing `pypi_python_translator-2.2/setup.py` & `pypi_python_translator-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="2.2",
+    version="2.3",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-2.2/translator/ExampleUsages.py` & `pypi_python_translator-2.3/translator/ExampleUsages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.2/translator/__init__.py` & `pypi_python_translator-2.3/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.2/translator/messages.py` & `pypi_python_translator-2.3/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.2/translator/services.py` & `pypi_python_translator-2.3/translator/services.py`

 * *Files identical despite different names*

