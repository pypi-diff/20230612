# Comparing `tmp/muheqa-0.0.2.tar.gz` & `tmp/muheqa-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muheqa-0.0.2.tar", last modified: Sat Jun 10 18:19:44 2023, max compression
+gzip compressed data, was "muheqa-0.0.3.tar", last modified: Mon Jun 12 08:14:43 2023, max compression
```

## Comparing `muheqa-0.0.2.tar` & `muheqa-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.319593 muheqa-0.0.2/
--rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.2/LICENSE
--rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-10 18:19:44.319458 muheqa-0.0.2/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      543 2023-06-10 18:08:18.000000 muheqa-0.0.2/README.md
--rw-r--r--   0 cbadenes   (501) staff       (20)      945 2023-06-10 18:18:49.000000 muheqa-0.0.2/pyproject.toml
--rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-10 18:19:44.319635 muheqa-0.0.2/setup.cfg
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.313505 muheqa-0.0.2/src/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.314005 muheqa-0.0.2/src/muheqa/
--rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.2/src/muheqa/__init__.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.315178 muheqa-0.0.2/src/muheqa/answer/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.315454 muheqa-0.0.2/src/muheqa/answer/analysis/
--rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.2/src/muheqa/answer/analysis/classifier.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.2/src/muheqa/answer/composer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.315735 muheqa-0.0.2/src/muheqa/answer/generation/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.2/src/muheqa/answer/generation/model.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.2/src/muheqa/connection.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      145 2023-06-10 17:08:51.000000 muheqa-0.0.2/src/muheqa/connector.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.316016 muheqa-0.0.2/src/muheqa/evidence/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.316313 muheqa-0.0.2/src/muheqa/evidence/candidates/
--rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.2/src/muheqa/evidence/candidates/ranking.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.2/src/muheqa/evidence/discoverer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.316596 muheqa-0.0.2/src/muheqa/evidence/documents/
--rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.2/src/muheqa/evidence/documents/splitter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.316891 muheqa-0.0.2/src/muheqa/evidence/responses/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1364 2023-06-09 14:48:51.000000 muheqa-0.0.2/src/muheqa/evidence/responses/retriever.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.2/src/muheqa/logformatter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.317167 muheqa-0.0.2/src/muheqa/summary/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.317889 muheqa-0.0.2/src/muheqa/summary/keywords/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.2/src/muheqa/summary/keywords/concept.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.2/src/muheqa/summary/keywords/discovery.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.2/src/muheqa/summary/keywords/entity.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.318866 muheqa-0.0.2/src/muheqa/summary/resources/
--rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.2/src/muheqa/summary/resources/d4c.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     6296 2023-06-09 14:46:22.000000 muheqa-0.0.2/src/muheqa/summary/resources/dbpedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-09 14:59:33.000000 muheqa-0.0.2/src/muheqa/summary/resources/graph.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-09 14:47:38.000000 muheqa-0.0.2/src/muheqa/summary/resources/wikipedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.2/src/muheqa/summary/summarizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.319106 muheqa-0.0.2/src/muheqa/summary/texts/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.2/src/muheqa/summary/texts/verbalizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-10 18:19:44.314924 muheqa-0.0.2/src/muheqa.egg-info/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-10 18:19:44.000000 muheqa-0.0.2/src/muheqa.egg-info/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      930 2023-06-10 18:19:44.000000 muheqa-0.0.2/src/muheqa.egg-info/SOURCES.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-10 18:19:44.000000 muheqa-0.0.2/src/muheqa.egg-info/dependency_links.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-10 18:19:44.000000 muheqa-0.0.2/src/muheqa.egg-info/requires.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       14 2023-06-10 18:19:44.000000 muheqa-0.0.2/src/muheqa.egg-info/top_level.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)      207 2023-06-10 17:08:16.000000 muheqa-0.0.2/src/sample.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.591401 muheqa-0.0.3/
+-rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.3/LICENSE
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 08:14:43.591268 muheqa-0.0.3/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      543 2023-06-10 18:08:18.000000 muheqa-0.0.3/README.md
+-rw-r--r--   0 cbadenes   (501) staff       (20)      945 2023-06-12 08:13:58.000000 muheqa-0.0.3/pyproject.toml
+-rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-12 08:14:43.591442 muheqa-0.0.3/setup.cfg
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.584734 muheqa-0.0.3/src/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.585769 muheqa-0.0.3/src/muheqa/
+-rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.3/src/muheqa/__init__.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.586986 muheqa-0.0.3/src/muheqa/answer/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.587232 muheqa-0.0.3/src/muheqa/answer/analysis/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.3/src/muheqa/answer/analysis/classifier.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.3/src/muheqa/answer/composer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.587458 muheqa-0.0.3/src/muheqa/answer/generation/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.3/src/muheqa/answer/generation/model.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.3/src/muheqa/connection.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      146 2023-06-12 08:13:34.000000 muheqa-0.0.3/src/muheqa/connector.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.587709 muheqa-0.0.3/src/muheqa/evidence/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.587953 muheqa-0.0.3/src/muheqa/evidence/candidates/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.3/src/muheqa/evidence/candidates/ranking.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.3/src/muheqa/evidence/discoverer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.588251 muheqa-0.0.3/src/muheqa/evidence/documents/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.3/src/muheqa/evidence/documents/splitter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.588516 muheqa-0.0.3/src/muheqa/evidence/responses/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1364 2023-06-09 14:48:51.000000 muheqa-0.0.3/src/muheqa/evidence/responses/retriever.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.3/src/muheqa/logformatter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.588766 muheqa-0.0.3/src/muheqa/summary/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.589522 muheqa-0.0.3/src/muheqa/summary/keywords/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.3/src/muheqa/summary/keywords/concept.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.3/src/muheqa/summary/keywords/discovery.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.3/src/muheqa/summary/keywords/entity.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.590675 muheqa-0.0.3/src/muheqa/summary/resources/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.3/src/muheqa/summary/resources/d4c.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     6296 2023-06-09 14:46:22.000000 muheqa-0.0.3/src/muheqa/summary/resources/dbpedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-09 14:59:33.000000 muheqa-0.0.3/src/muheqa/summary/resources/graph.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-09 14:47:38.000000 muheqa-0.0.3/src/muheqa/summary/resources/wikipedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.3/src/muheqa/summary/summarizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.590934 muheqa-0.0.3/src/muheqa/summary/texts/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.3/src/muheqa/summary/texts/verbalizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 08:14:43.586820 muheqa-0.0.3/src/muheqa.egg-info/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 08:14:43.000000 muheqa-0.0.3/src/muheqa.egg-info/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      930 2023-06-12 08:14:43.000000 muheqa-0.0.3/src/muheqa.egg-info/SOURCES.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-12 08:14:43.000000 muheqa-0.0.3/src/muheqa.egg-info/dependency_links.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-12 08:14:43.000000 muheqa-0.0.3/src/muheqa.egg-info/requires.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       14 2023-06-12 08:14:43.000000 muheqa-0.0.3/src/muheqa.egg-info/top_level.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)      207 2023-06-10 17:08:16.000000 muheqa-0.0.3/src/sample.py
```

### Comparing `muheqa-0.0.2/LICENSE` & `muheqa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/PKG-INFO` & `muheqa-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `muheqa-0.0.2/README.md` & `muheqa-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/pyproject.toml` & `muheqa-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "sentence-transformers",
     "sparqlwrapper"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "muheqa"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Carlos Badenes-Olmedo", email="carlos.badenes@upm.es" },
 ]
 description = "Multiple and Heterogeneous Question-Answering"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `muheqa-0.0.2/src/muheqa/answer/analysis/classifier.py` & `muheqa-0.0.3/src/muheqa/answer/analysis/classifier.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/answer/composer.py` & `muheqa-0.0.3/src/muheqa/answer/composer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/answer/generation/model.py` & `muheqa-0.0.3/src/muheqa/answer/generation/model.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/connection.py` & `muheqa-0.0.3/src/muheqa/connection.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/evidence/candidates/ranking.py` & `muheqa-0.0.3/src/muheqa/evidence/candidates/ranking.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/evidence/discoverer.py` & `muheqa-0.0.3/src/muheqa/evidence/discoverer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/evidence/documents/splitter.py` & `muheqa-0.0.3/src/muheqa/evidence/documents/splitter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/evidence/responses/retriever.py` & `muheqa-0.0.3/src/muheqa/evidence/responses/retriever.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/logformatter.py` & `muheqa-0.0.3/src/muheqa/logformatter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/keywords/concept.py` & `muheqa-0.0.3/src/muheqa/summary/keywords/concept.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/keywords/discovery.py` & `muheqa-0.0.3/src/muheqa/summary/keywords/discovery.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/keywords/entity.py` & `muheqa-0.0.3/src/muheqa/summary/keywords/entity.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/resources/d4c.py` & `muheqa-0.0.3/src/muheqa/summary/resources/d4c.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/resources/dbpedia.py` & `muheqa-0.0.3/src/muheqa/summary/resources/dbpedia.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/resources/graph.py` & `muheqa-0.0.3/src/muheqa/summary/resources/graph.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/resources/wikipedia.py` & `muheqa-0.0.3/src/muheqa/summary/resources/wikipedia.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/summarizer.py` & `muheqa-0.0.3/src/muheqa/summary/summarizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa/summary/texts/verbalizer.py` & `muheqa-0.0.3/src/muheqa/summary/texts/verbalizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.2/src/muheqa.egg-info/PKG-INFO` & `muheqa-0.0.3/src/muheqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `muheqa-0.0.2/src/muheqa.egg-info/SOURCES.txt` & `muheqa-0.0.3/src/muheqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

