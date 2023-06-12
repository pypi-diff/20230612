# Comparing `tmp/maadstml-3.30.tar.gz` & `tmp/maadstml-3.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.30.tar", last modified: Sun Jun 11 18:47:33 2023, max compression
+gzip compressed data, was "maadstml-3.31.tar", last modified: Sun Jun 11 18:50:11 2023, max compression
```

## Comparing `maadstml-3.30.tar` & `maadstml-3.31.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 18:47:33.637813 maadstml-3.30/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.30/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.30/MANIFEST.in
--rw-rw-rw-   0        0        0   172671 2023-06-11 18:47:33.632964 maadstml-3.30/PKG-INFO
--rw-rw-rw-   0        0        0   172074 2023-06-11 18:43:51.000000 maadstml-3.30/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 18:47:33.610923 maadstml-3.30/maadstml/
--rw-rw-rw-   0        0        0     2158 2023-06-11 18:45:29.000000 maadstml-3.30/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.30/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    78954 2023-06-11 18:44:43.000000 maadstml-3.30/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.30/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-11 18:47:33.632964 maadstml-3.30/maadstml.egg-info/
--rw-rw-rw-   0        0        0   172671 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 18:47:33.000000 maadstml-3.30/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      178 2023-06-11 18:47:05.000000 maadstml-3.30/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 18:47:33.637813 maadstml-3.30/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-11 18:46:06.000000 maadstml-3.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:50:11.022524 maadstml-3.31/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.31/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.31/MANIFEST.in
+-rw-rw-rw-   0        0        0   172671 2023-06-11 18:50:11.013882 maadstml-3.31/PKG-INFO
+-rw-rw-rw-   0        0        0   172074 2023-06-11 18:43:51.000000 maadstml-3.31/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 18:50:10.999761 maadstml-3.31/maadstml/
+-rw-rw-rw-   0        0        0     2158 2023-06-11 18:45:29.000000 maadstml-3.31/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.31/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    78954 2023-06-11 18:44:43.000000 maadstml-3.31/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.31/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-11 18:50:11.013882 maadstml-3.31/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   172671 2023-06-11 18:50:10.000000 maadstml-3.31/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-11 18:50:10.000000 maadstml-3.31/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 18:50:10.000000 maadstml-3.31/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-06-11 18:50:10.000000 maadstml-3.31/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-11 18:50:10.000000 maadstml-3.31/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      167 2023-06-11 18:49:50.000000 maadstml-3.31/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 18:50:11.022524 maadstml-3.31/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-11 18:50:00.000000 maadstml-3.31/setup.py
```

### Comparing `maadstml-3.30/LICENSE.txt` & `maadstml-3.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.30/PKG-INFO` & `maadstml-3.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.30
+Version: 3.31
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.30/README.md` & `maadstml-3.31/README.md`

 * *Files identical despite different names*

### Comparing `maadstml-3.30/maadstml/__init__.py` & `maadstml-3.31/maadstml/__init__.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.30/maadstml/readpdf.py` & `maadstml-3.31/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.30/maadstml/sendfiles.py` & `maadstml-3.31/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.30/maadstml/tmltextsummary.py` & `maadstml-3.31/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.30/maadstml.egg-info/PKG-INFO` & `maadstml-3.31/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.30
+Version: 3.31
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.30/setup.py` & `maadstml-3.31/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.30',
+    version='3.31',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

