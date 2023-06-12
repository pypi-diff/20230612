# Comparing `tmp/FindJobsTW-1.0.0.tar.gz` & `tmp/FindJobsTW-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FindJobsTW-1.0.0.tar", last modified: Mon Jun 12 09:25:51 2023, max compression
+gzip compressed data, was "FindJobsTW-1.0.1.tar", last modified: Mon Jun 12 09:37:51 2023, max compression
```

## Comparing `FindJobsTW-1.0.0.tar` & `FindJobsTW-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:25:51.899273 FindJobsTW-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-12 09:25:51.885274 FindJobsTW-1.0.0/FindJobsTW.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 09:25:51.000000 FindJobsTW-1.0.0/FindJobsTW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      591 2023-06-12 09:25:51.898290 FindJobsTW-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 09:25:51.894290 FindJobsTW-1.0.0/findJobs/
--rw-rw-rw-   0        0        0    17529 2023-06-12 09:09:07.000000 FindJobsTW-1.0.0/findJobs/FindJobs.py
--rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.0/findJobs/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-06-12 09:15:10.000000 FindJobsTW-1.0.0/findJobs/app.py
--rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.0/findJobs/url.py
--rw-rw-rw-   0        0        0       42 2023-06-12 09:25:51.901276 FindJobsTW-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-06-12 09:25:08.000000 FindJobsTW-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.839067 FindJobsTW-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.820070 FindJobsTW-1.0.1/FindJobsTW.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 09:37:51.000000 FindJobsTW-1.0.1/FindJobsTW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-06-06 03:11:17.000000 FindJobsTW-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-06-12 09:32:38.000000 FindJobsTW-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:37:51.838070 FindJobsTW-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      125 2023-06-06 06:07:54.000000 FindJobsTW-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.831072 FindJobsTW-1.0.1/findJobs/
+-rw-rw-rw-   0        0        0    17529 2023-06-12 09:09:07.000000 FindJobsTW-1.0.1/findJobs/FindJobs.py
+-rw-rw-rw-   0        0        0      133 2023-06-12 09:19:48.000000 FindJobsTW-1.0.1/findJobs/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-06-12 09:15:10.000000 FindJobsTW-1.0.1/findJobs/app.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.834077 FindJobsTW-1.0.1/findJobs/static/
+-rw-rw-rw-   0        0        0      382 2023-06-12 08:30:14.000000 FindJobsTW-1.0.1/findJobs/static/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-12 09:37:51.836068 FindJobsTW-1.0.1/findJobs/templates/
+-rw-rw-rw-   0        0        0    28017 2023-06-12 08:41:44.000000 FindJobsTW-1.0.1/findJobs/templates/index.html
+-rw-rw-rw-   0        0        0     4908 2023-06-12 04:00:23.000000 FindJobsTW-1.0.1/findJobs/url.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:37:51.839067 FindJobsTW-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      936 2023-06-12 09:37:47.000000 FindJobsTW-1.0.1/setup.py
```

### Comparing `FindJobsTW-1.0.0/FindJobsTW.egg-info/PKG-INFO` & `FindJobsTW-1.0.1/FindJobsTW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.0/LICENSE` & `FindJobsTW-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.0/PKG-INFO` & `FindJobsTW-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FindJobsTW
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to find jobs on 104.com.tw based on specific keywords.
 Home-page: https://github.com/DannyFin/FindJobsTW
 Author: Danny Fin
 Author-email: dannyfinselect@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FindJobsTW-1.0.0/findJobs/FindJobs.py` & `FindJobsTW-1.0.1/findJobs/FindJobs.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.0/findJobs/app.py` & `FindJobsTW-1.0.1/findJobs/app.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.0/findJobs/url.py` & `FindJobsTW-1.0.1/findJobs/url.py`

 * *Files identical despite different names*

### Comparing `FindJobsTW-1.0.0/setup.py` & `FindJobsTW-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
     
 setup(
     name='FindJobsTW',    
-    version='1.0.0',      
+    version='1.0.1',      
     packages=find_packages(),    
     install_requires=requirements,
+    package_data={
+        'findJobs': ['templates/*', 'static/*']
+    },  
     author="Danny Fin",
     author_email="dannyfinselect@outlook.com",
     description="A Python package to find jobs on 104.com.tw based on specific keywords.",
     long_description=open('README.md', 'r', encoding='utf-8').read(),# 若Discription.md中有中文 須加上 encoding="utf-8"
     long_description_content_type="text/markdown",
     url="https://github.com/DannyFin/FindJobsTW",
     classifiers=[
```

