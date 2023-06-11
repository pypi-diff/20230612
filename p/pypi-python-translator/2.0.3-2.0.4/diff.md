# Comparing `tmp/pypi_python_translator-2.0.3.tar.gz` & `tmp/pypi_python_translator-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-2.0.3.tar", last modified: Sun Jun 11 22:05:46 2023, max compression
+gzip compressed data, was "pypi_python_translator-2.0.4.tar", last modified: Sun Jun 11 22:10:59 2023, max compression
```

## Comparing `pypi_python_translator-2.0.3.tar` & `pypi_python_translator-2.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 22:05:46.579628 pypi_python_translator-2.0.3/
--rw-rw-rw-   0        0        0     4028 2023-06-11 22:05:46.579628 pypi_python_translator-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3587 2023-06-11 22:05:23.000000 pypi_python_translator-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 22:05:46.573632 pypi_python_translator-2.0.3/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     4028 2023-06-11 22:05:46.000000 pypi_python_translator-2.0.3/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-11 22:05:46.000000 pypi_python_translator-2.0.3/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 22:05:46.000000 pypi_python_translator-2.0.3/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 22:05:46.000000 pypi_python_translator-2.0.3/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 22:05:46.580633 pypi_python_translator-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-06-11 22:05:43.000000 pypi_python_translator-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 22:05:46.578626 pypi_python_translator-2.0.3/translator/
--rw-rw-rw-   0        0        0     3744 2023-06-11 16:22:57.000000 pypi_python_translator-2.0.3/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.0.3/translator/languageExamples.py
--rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.0.3/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.0.3/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:10:59.677245 pypi_python_translator-2.0.4/
+-rw-rw-rw-   0        0        0     4131 2023-06-11 22:10:59.676238 pypi_python_translator-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3690 2023-06-11 22:10:40.000000 pypi_python_translator-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 22:10:59.670242 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     4131 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 22:10:59.678239 pypi_python_translator-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-11 22:10:46.000000 pypi_python_translator-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:10:59.675238 pypi_python_translator-2.0.4/translator/
+-rw-rw-rw-   0        0        0     3744 2023-06-11 16:22:57.000000 pypi_python_translator-2.0.4/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.0.4/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.0.4/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.0.4/translator/services.py
```

### Comparing `pypi_python_translator-2.0.3/PKG-INFO` & `pypi_python_translator-2.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pypi_python_translator
-Version: 2.0.3
-Summary: A Python package for translation
-Home-page: https://github.com/SForces/pypi_python_translator
-Author: SForces
-Author-email: osmntn08@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # **PYPI PYTHON TRANSLATOR**
 This is a translation application that allows you to translate text from one language to another using the Google Translate service. The program provides a user-friendly interface that automatically translates itself into the selected language.
 
 ---
 
 ## **Getting Started**
 
@@ -90,25 +77,25 @@
 translated_message = TRnslte(your_message,"<language code>")
 
 print(translated_message)
 
 ```
 `Example Usage (3):`<br>
 Using this program for full file translating;<br>
-I have to warn you: `with` function only supports utf-8 characters.
+I have to warn you: in this example `with` function only supports utf-8 characters. if you want to use any other encoding you can change it by editing `encoding=""` part.
 
 ```python
 from translator import *
 
 filecontent = []
-with open("<your_file_name>.txt", "r",encdoing="utf-8") as file:
+with open("<your_file_name>.txt", "r",encoding="utf-8") as file:
     for line in file:
         line = line.strip()  # Remove spaces and empty lines  
         if line:  # If line has characters
             filecontent.append(line)
 
-with open("<output_file>.txt","w",encdoing="utf-8") as file:
+with open("<output_file>.txt","w",encoding="utf-8") as file:
     for line in filecontent:
         translated_line = TRnslte(line,"<language_code>")
         file.write(translated_line + "\n")
 ```
 ---
```

### Comparing `pypi_python_translator-2.0.3/README.md` & `pypi_python_translator-2.0.4/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pypi-python-translator
+Version: 2.0.4
+Summary: A Python package for translation
+Home-page: https://github.com/SForces/pypi_python_translator
+Author: SForces
+Author-email: osmntn08@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # **PYPI PYTHON TRANSLATOR**
 This is a translation application that allows you to translate text from one language to another using the Google Translate service. The program provides a user-friendly interface that automatically translates itself into the selected language.
 
 ---
 
 ## **Getting Started**
 
@@ -77,25 +90,25 @@
 translated_message = TRnslte(your_message,"<language code>")
 
 print(translated_message)
 
 ```
 `Example Usage (3):`<br>
 Using this program for full file translating;<br>
-I have to warn you: `with` function only supports utf-8 characters.
+I have to warn you: in this example `with` function only supports utf-8 characters. if you want to use any other encoding you can change it by editing `encoding=""` part.
 
 ```python
 from translator import *
 
 filecontent = []
-with open("<your_file_name>.txt", "r",encdoing="utf-8") as file:
+with open("<your_file_name>.txt", "r",encoding="utf-8") as file:
     for line in file:
         line = line.strip()  # Remove spaces and empty lines  
         if line:  # If line has characters
             filecontent.append(line)
 
-with open("<output_file>.txt","w",encdoing="utf-8") as file:
+with open("<output_file>.txt","w",encoding="utf-8") as file:
     for line in filecontent:
         translated_line = TRnslte(line,"<language_code>")
         file.write(translated_line + "\n")
 ```
 ---
```

### Comparing `pypi_python_translator-2.0.3/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-2.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pypi-python-translator
-Version: 2.0.3
+Name: pypi_python_translator
+Version: 2.0.4
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -90,25 +90,25 @@
 translated_message = TRnslte(your_message,"<language code>")
 
 print(translated_message)
 
 ```
 `Example Usage (3):`<br>
 Using this program for full file translating;<br>
-I have to warn you: `with` function only supports utf-8 characters.
+I have to warn you: in this example `with` function only supports utf-8 characters. if you want to use any other encoding you can change it by editing `encoding=""` part.
 
 ```python
 from translator import *
 
 filecontent = []
-with open("<your_file_name>.txt", "r",encdoing="utf-8") as file:
+with open("<your_file_name>.txt", "r",encoding="utf-8") as file:
     for line in file:
         line = line.strip()  # Remove spaces and empty lines  
         if line:  # If line has characters
             filecontent.append(line)
 
-with open("<output_file>.txt","w",encdoing="utf-8") as file:
+with open("<output_file>.txt","w",encoding="utf-8") as file:
     for line in filecontent:
         translated_line = TRnslte(line,"<language_code>")
         file.write(translated_line + "\n")
 ```
 ---
```

### Comparing `pypi_python_translator-2.0.3/setup.py` & `pypi_python_translator-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="2.0.3",
+    version="2.0.4",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-2.0.3/translator/__init__.py` & `pypi_python_translator-2.0.4/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.0.3/translator/messages.py` & `pypi_python_translator-2.0.4/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.0.3/translator/services.py` & `pypi_python_translator-2.0.4/translator/services.py`

 * *Files identical despite different names*

