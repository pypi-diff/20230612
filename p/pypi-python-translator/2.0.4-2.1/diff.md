# Comparing `tmp/pypi_python_translator-2.0.4.tar.gz` & `tmp/pypi_python_translator-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-2.0.4.tar", last modified: Sun Jun 11 22:10:59 2023, max compression
+gzip compressed data, was "pypi_python_translator-2.1.tar", last modified: Mon Jun 12 12:18:37 2023, max compression
```

## Comparing `pypi_python_translator-2.0.4.tar` & `pypi_python_translator-2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 22:10:59.677245 pypi_python_translator-2.0.4/
--rw-rw-rw-   0        0        0     4131 2023-06-11 22:10:59.676238 pypi_python_translator-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3690 2023-06-11 22:10:40.000000 pypi_python_translator-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 22:10:59.670242 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     4131 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 22:10:59.000000 pypi_python_translator-2.0.4/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 22:10:59.678239 pypi_python_translator-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-06-11 22:10:46.000000 pypi_python_translator-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 22:10:59.675238 pypi_python_translator-2.0.4/translator/
--rw-rw-rw-   0        0        0     3744 2023-06-11 16:22:57.000000 pypi_python_translator-2.0.4/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.0.4/translator/languageExamples.py
--rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.0.4/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.0.4/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:18:37.667239 pypi_python_translator-2.1/
+-rw-rw-rw-   0        0        0     4779 2023-06-12 12:18:37.666244 pypi_python_translator-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2023-06-12 12:18:19.000000 pypi_python_translator-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 12:18:37.658181 pypi_python_translator-2.1/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     4779 2023-06-12 12:18:37.000000 pypi_python_translator-2.1/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-12 12:18:37.000000 pypi_python_translator-2.1/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 12:18:37.000000 pypi_python_translator-2.1/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 12:18:37.000000 pypi_python_translator-2.1/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:18:37.667239 pypi_python_translator-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-06-12 12:18:22.000000 pypi_python_translator-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 12:18:37.664238 pypi_python_translator-2.1/translator/
+-rw-rw-rw-   0        0        0     3744 2023-06-11 16:22:57.000000 pypi_python_translator-2.1/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.1/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.1/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.1/translator/services.py
```

### Comparing `pypi_python_translator-2.0.4/PKG-INFO` & `pypi_python_translator-2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pypi_python_translator
-Version: 2.0.4
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
 
@@ -67,48 +54,59 @@
 
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
-## **Examples**
-`Example Usage (1):`
+# **Examples**
+Example usages for this package.
+---
+---
+## `Example Usage (1):`
 
 Using `init()` function to start program.
 ```python
 from translator import *
 init("<language code>") #for ex -> init("en")
 ```
-`Example Usage (2):`<br>
+This code start program for "1" times, and won't repeat himself.<br>
+
+---
+## `Example Usage (2):`<br>
 Using `TRnslte()` function:
 
 ```python
 from translator import *
 
 your_message = "Hello world"
 
 translated_message = TRnslte(your_message,"<language code>")
 
 print(translated_message)
 
 ```
-`Example Usage (3):`<br>
+---
+## `Example Usage (3):`<br>
 Using this program for full file translating;<br>
 I have to warn you: in this example `with` function only supports utf-8 characters. if you want to use any other encoding you can change it by editing `encoding=""` part.
 
 ```python
 from translator import *
 
 filecontent = []
-with open("<your_file_name>.txt", "r",encoding="utf-8") as file:
+with open("<your_file>.txt", "r",encoding="utf-8") as file: #read the file for translation.
+    #The .txt extension is not mandatory, it can be any extension. The important thing is that you specify the encoding of the file correctly.
     for line in file:
         line = line.strip()  # Remove spaces and empty lines  
         if line:  # If line has characters
             filecontent.append(line)
 
-with open("<output_file>.txt","w",encoding="utf-8") as file:
-    for line in filecontent:
-        translated_line = TRnslte(line,"<language_code>")
-        file.write(translated_line + "\n")
+with open("<output_file>.txt","w",encoding="utf-8") as file: #output file writing, it has to be same encoding with reading file
+    for line in filecontent: #Every line in our list;
+        translated_line = TRnslte(line,"<language_code>") #translate line to the "your language code"
+        file.write(translated_line + "\n") #write the translated line to the file.
 ```
+# LICENSE
+[SForces/PyPi_Python_Translator is licensed under the
+GNU General Public License v2.0](https://github.com/SForces/PyPi_Python_Translator/blob/main/LICENSE)
 ---
```

### Comparing `pypi_python_translator-2.0.4/README.md` & `pypi_python_translator-2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pypi_python_translator
+Version: 2.1
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
 
@@ -54,48 +67,59 @@
 
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
-## **Examples**
-`Example Usage (1):`
+# **Examples**
+Example usages for this package.
+---
+---
+## `Example Usage (1):`
 
 Using `init()` function to start program.
 ```python
 from translator import *
 init("<language code>") #for ex -> init("en")
 ```
-`Example Usage (2):`<br>
+This code start program for "1" times, and won't repeat himself.<br>
+
+---
+## `Example Usage (2):`<br>
 Using `TRnslte()` function:
 
 ```python
 from translator import *
 
 your_message = "Hello world"
 
 translated_message = TRnslte(your_message,"<language code>")
 
 print(translated_message)
 
 ```
-`Example Usage (3):`<br>
+---
+## `Example Usage (3):`<br>
 Using this program for full file translating;<br>
 I have to warn you: in this example `with` function only supports utf-8 characters. if you want to use any other encoding you can change it by editing `encoding=""` part.
 
 ```python
 from translator import *
 
 filecontent = []
-with open("<your_file_name>.txt", "r",encoding="utf-8") as file:
+with open("<your_file>.txt", "r",encoding="utf-8") as file: #read the file for translation.
+    #The .txt extension is not mandatory, it can be any extension. The important thing is that you specify the encoding of the file correctly.
     for line in file:
         line = line.strip()  # Remove spaces and empty lines  
         if line:  # If line has characters
             filecontent.append(line)
 
-with open("<output_file>.txt","w",encoding="utf-8") as file:
-    for line in filecontent:
-        translated_line = TRnslte(line,"<language_code>")
-        file.write(translated_line + "\n")
+with open("<output_file>.txt","w",encoding="utf-8") as file: #output file writing, it has to be same encoding with reading file
+    for line in filecontent: #Every line in our list;
+        translated_line = TRnslte(line,"<language_code>") #translate line to the "your language code"
+        file.write(translated_line + "\n") #write the translated line to the file.
 ```
+# LICENSE
+[SForces/PyPi_Python_Translator is licensed under the
+GNU General Public License v2.0](https://github.com/SForces/PyPi_Python_Translator/blob/main/LICENSE)
 ---
```

### Comparing `pypi_python_translator-2.0.4/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-2.1/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-python-translator
-Version: 2.0.4
+Version: 2.1
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -67,48 +67,59 @@
 
 ## **Usage**
 
 After setting up the necessary files and libraries, you can use the `init("language-code")` function to start the translation application. The program will guide you through the translation process, displaying the input and output languages, the translated text, and the translation accuracy.
 
 Please make sure to enter valid languages and follow the instructions provided by the program.
 
-## **Examples**
-`Example Usage (1):`
+# **Examples**
+Example usages for this package.
+---
+---
+## `Example Usage (1):`
 
 Using `init()` function to start program.
 ```python
 from translator import *
 init("<language code>") #for ex -> init("en")
 ```
-`Example Usage (2):`<br>
+This code start program for "1" times, and won't repeat himself.<br>
+
+---
+## `Example Usage (2):`<br>
 Using `TRnslte()` function:
 
 ```python
 from translator import *
 
 your_message = "Hello world"
 
 translated_message = TRnslte(your_message,"<language code>")
 
 print(translated_message)
 
 ```
-`Example Usage (3):`<br>
+---
+## `Example Usage (3):`<br>
 Using this program for full file translating;<br>
 I have to warn you: in this example `with` function only supports utf-8 characters. if you want to use any other encoding you can change it by editing `encoding=""` part.
 
 ```python
 from translator import *
 
 filecontent = []
-with open("<your_file_name>.txt", "r",encoding="utf-8") as file:
+with open("<your_file>.txt", "r",encoding="utf-8") as file: #read the file for translation.
+    #The .txt extension is not mandatory, it can be any extension. The important thing is that you specify the encoding of the file correctly.
     for line in file:
         line = line.strip()  # Remove spaces and empty lines  
         if line:  # If line has characters
             filecontent.append(line)
 
-with open("<output_file>.txt","w",encoding="utf-8") as file:
-    for line in filecontent:
-        translated_line = TRnslte(line,"<language_code>")
-        file.write(translated_line + "\n")
+with open("<output_file>.txt","w",encoding="utf-8") as file: #output file writing, it has to be same encoding with reading file
+    for line in filecontent: #Every line in our list;
+        translated_line = TRnslte(line,"<language_code>") #translate line to the "your language code"
+        file.write(translated_line + "\n") #write the translated line to the file.
 ```
+# LICENSE
+[SForces/PyPi_Python_Translator is licensed under the
+GNU General Public License v2.0](https://github.com/SForces/PyPi_Python_Translator/blob/main/LICENSE)
 ---
```

### Comparing `pypi_python_translator-2.0.4/setup.py` & `pypi_python_translator-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="2.0.4",
+    version="2.1",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-2.0.4/translator/__init__.py` & `pypi_python_translator-2.1/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.0.4/translator/messages.py` & `pypi_python_translator-2.1/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.0.4/translator/services.py` & `pypi_python_translator-2.1/translator/services.py`

 * *Files identical despite different names*

