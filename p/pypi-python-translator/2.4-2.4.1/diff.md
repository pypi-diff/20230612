# Comparing `tmp/pypi_python_translator-2.4.tar.gz` & `tmp/pypi_python_translator-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi_python_translator-2.4.tar", last modified: Mon Jun 12 18:07:54 2023, max compression
+gzip compressed data, was "pypi_python_translator-2.4.1.tar", last modified: Mon Jun 12 18:10:18 2023, max compression
```

## Comparing `pypi_python_translator-2.4.tar` & `pypi_python_translator-2.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:07:54.709084 pypi_python_translator-2.4/
--rw-rw-rw-   0        0        0     5412 2023-06-12 18:07:54.708068 pypi_python_translator-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4971 2023-06-12 18:04:29.000000 pypi_python_translator-2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:07:54.696756 pypi_python_translator-2.4/pypi_python_translator.egg-info/
--rw-rw-rw-   0        0        0     5412 2023-06-12 18:07:54.000000 pypi_python_translator-2.4/pypi_python_translator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-06-12 18:07:54.000000 pypi_python_translator-2.4/pypi_python_translator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:07:54.000000 pypi_python_translator-2.4/pypi_python_translator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 18:07:54.000000 pypi_python_translator-2.4/pypi_python_translator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 18:07:54.709084 pypi_python_translator-2.4/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-06-12 18:07:50.000000 pypi_python_translator-2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:07:54.705546 pypi_python_translator-2.4/translator/
--rw-rw-rw-   0        0        0      700 2023-06-12 18:06:45.000000 pypi_python_translator-2.4/translator/ExampleUsages.py
--rw-rw-rw-   0        0        0     4448 2023-06-12 18:06:59.000000 pypi_python_translator-2.4/translator/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.4/translator/languageExamples.py
--rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.4/translator/messages.py
--rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.4/translator/services.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:10:18.373813 pypi_python_translator-2.4.1/
+-rw-rw-rw-   0        0        0     5414 2023-06-12 18:10:18.372793 pypi_python_translator-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4971 2023-06-12 18:04:29.000000 pypi_python_translator-2.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:10:18.362743 pypi_python_translator-2.4.1/pypi_python_translator.egg-info/
+-rw-rw-rw-   0        0        0     5414 2023-06-12 18:10:18.000000 pypi_python_translator-2.4.1/pypi_python_translator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-12 18:10:18.000000 pypi_python_translator-2.4.1/pypi_python_translator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:10:18.000000 pypi_python_translator-2.4.1/pypi_python_translator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 18:10:18.000000 pypi_python_translator-2.4.1/pypi_python_translator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 18:10:18.374810 pypi_python_translator-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-12 18:10:09.000000 pypi_python_translator-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:10:18.371267 pypi_python_translator-2.4.1/translator/
+-rw-rw-rw-   0        0        0      700 2023-06-12 18:06:45.000000 pypi_python_translator-2.4.1/translator/ExampleUsages.py
+-rw-rw-rw-   0        0        0     4469 2023-06-12 18:10:05.000000 pypi_python_translator-2.4.1/translator/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-11 15:35:03.000000 pypi_python_translator-2.4.1/translator/languageExamples.py
+-rw-rw-rw-   0        0        0      543 2023-06-11 16:17:04.000000 pypi_python_translator-2.4.1/translator/messages.py
+-rw-rw-rw-   0        0        0     5895 2023-06-11 15:30:09.000000 pypi_python_translator-2.4.1/translator/services.py
```

### Comparing `pypi_python_translator-2.4/PKG-INFO` & `pypi_python_translator-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi_python_translator
-Version: 2.4
+Version: 2.4.1
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-2.4/README.md` & `pypi_python_translator-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.4/pypi_python_translator.egg-info/PKG-INFO` & `pypi_python_translator-2.4.1/pypi_python_translator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-python-translator
-Version: 2.4
+Version: 2.4.1
 Summary: A Python package for translation
 Home-page: https://github.com/SForces/pypi_python_translator
 Author: SForces
 Author-email: osmntn08@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypi_python_translator-2.4/setup.py` & `pypi_python_translator-2.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypi_python_translator",
-    version="2.4",
+    version="2.4.1",
     author="SForces",
     author_email="osmntn08@gmail.com",
     description="A Python package for translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SForces/pypi_python_translator",
     packages=["translator"],
```

### Comparing `pypi_python_translator-2.4/translator/ExampleUsages.py` & `pypi_python_translator-2.4.1/translator/ExampleUsages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.4/translator/__init__.py` & `pypi_python_translator-2.4.1/translator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     Writing Usages
     ~~~
     This code will write the given example with the value of "num" as file "example_num.py".
     """
     if num == 1:
         with open("example_1.py","w") as f:
             for line in example_1:
-                f.write(line)
+                f.write(line + "\n")
     elif num == 2:
         with open("example_2.py","w") as f:
             for line in example_2:
-                f.write(line)
+                f.write(line + "\n")
     elif num == 3:
         with open("example_3.py","w") as f:
             for line in example_3:
-                f.write(line)
+                f.write(line + "\n")
     else:
         raise ValueError(f"Example Usage Number must be 1 or 2 or 3, not '{num}'")
 def TRnslte(text:str,languages:str) -> str:
     """
     What is that ?
     ~~~
     This is self translate.
```

### Comparing `pypi_python_translator-2.4/translator/messages.py` & `pypi_python_translator-2.4.1/translator/messages.py`

 * *Files identical despite different names*

### Comparing `pypi_python_translator-2.4/translator/services.py` & `pypi_python_translator-2.4.1/translator/services.py`

 * *Files identical despite different names*

