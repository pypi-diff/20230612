# Comparing `tmp/selenium_simplified-1.0.tar.gz` & `tmp/selenium_simplified-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_simplified-1.0.tar", last modified: Mon Jun 12 08:54:34 2023, max compression
+gzip compressed data, was "selenium_simplified-1.1.tar", last modified: Mon Jun 12 10:33:13 2023, max compression
```

## Comparing `selenium_simplified-1.0.tar` & `selenium_simplified-1.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 08:54:34.234916 selenium_simplified-1.0/
--rw-rw-rw-   0        0        0      565 2023-06-12 08:54:34.234916 selenium_simplified-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       98 2023-06-12 07:42:11.000000 selenium_simplified-1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-12 08:53:39.000000 selenium_simplified-1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-12 08:54:34.228898 selenium_simplified-1.0/selenium_simplified.egg-info/
--rw-rw-rw-   0        0        0      565 2023-06-12 08:54:34.000000 selenium_simplified-1.0/selenium_simplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-12 08:54:34.000000 selenium_simplified-1.0/selenium_simplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 08:54:34.000000 selenium_simplified-1.0/selenium_simplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 08:54:34.000000 selenium_simplified-1.0/selenium_simplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 08:54:34.234916 selenium_simplified-1.0/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-06-12 07:43:55.000000 selenium_simplified-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:33:13.009833 selenium_simplified-1.1/
+-rw-rw-rw-   0        0        0      664 2023-06-12 10:33:13.009833 selenium_simplified-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-12 09:03:20.000000 selenium_simplified-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:33:12.993435 selenium_simplified-1.1/SeleniumSimplified/
+-rw-rw-rw-   0        0        0     1413 2023-06-12 05:07:01.000000 selenium_simplified-1.1/SeleniumSimplified/UserActions.py
+-rw-rw-rw-   0        0        0      990 2023-06-12 05:05:49.000000 selenium_simplified-1.1/SeleniumSimplified/UserActivities.py
+-rw-rw-rw-   0        0        0       26 2023-06-12 10:30:05.000000 selenium_simplified-1.1/SeleniumSimplified/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-06-12 08:53:39.000000 selenium_simplified-1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-12 10:33:13.009833 selenium_simplified-1.1/selenium_simplified.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-06-12 10:33:12.000000 selenium_simplified-1.1/selenium_simplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-06-12 10:33:12.000000 selenium_simplified-1.1/selenium_simplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:33:12.000000 selenium_simplified-1.1/selenium_simplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-12 10:33:12.000000 selenium_simplified-1.1/selenium_simplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:33:13.009833 selenium_simplified-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      706 2023-06-12 10:32:21.000000 selenium_simplified-1.1/setup.py
```

### Comparing `selenium_simplified-1.0/PKG-INFO` & `selenium_simplified-1.1/selenium_simplified.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
-Name: selenium_simplified
-Version: 1.0
+Name: selenium-simplified
+Version: 1.1
 Summary: a better approach to do automation using selenium python on chrome browser
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # SeleniumSimplified
 a better approach to do automation using selenium python on chrome browser
+
+
+https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
```

### Comparing `selenium_simplified-1.0/selenium_simplified.egg-info/PKG-INFO` & `selenium_simplified-1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
-Name: selenium-simplified
-Version: 1.0
+Name: selenium_simplified
+Version: 1.1
 Summary: a better approach to do automation using selenium python on chrome browser
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # SeleniumSimplified
 a better approach to do automation using selenium python on chrome browser
+
+
+https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
```

### Comparing `selenium_simplified-1.0/setup.py` & `selenium_simplified-1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium_simplified",
-    version="1.0",
+    version="1.1",
     author="rajnish kumar",
     author_email="raajrajnish@gmail.com",
     description="a better approach to do automation using selenium python on chrome browser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raajrajnish/SeleniumSimplified.git",
     packages=setuptools.find_packages(),
```

