# Comparing `tmp/muheqa-0.0.8.tar.gz` & `tmp/muheqa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muheqa-0.0.8.tar", last modified: Mon Jun 12 17:19:00 2023, max compression
+gzip compressed data, was "muheqa-0.0.9.tar", last modified: Mon Jun 12 18:11:28 2023, max compression
```

## Comparing `muheqa-0.0.8.tar` & `muheqa-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.845975 muheqa-0.0.8/
--rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.8/LICENSE
--rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 17:19:00.845791 muheqa-0.0.8/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      543 2023-06-10 18:08:18.000000 muheqa-0.0.8/README.md
--rw-r--r--   0 cbadenes   (501) staff       (20)      945 2023-06-12 17:18:05.000000 muheqa-0.0.8/pyproject.toml
--rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-12 17:19:00.846049 muheqa-0.0.8/setup.cfg
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.837526 muheqa-0.0.8/src/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.838600 muheqa-0.0.8/src/muheqa/
--rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.8/src/muheqa/__init__.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.839872 muheqa-0.0.8/src/muheqa/answer/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.840124 muheqa-0.0.8/src/muheqa/answer/analysis/
--rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.8/src/muheqa/answer/analysis/classifier.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.8/src/muheqa/answer/composer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.840348 muheqa-0.0.8/src/muheqa/answer/generation/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.8/src/muheqa/answer/generation/model.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.8/src/muheqa/connection.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      146 2023-06-12 08:13:34.000000 muheqa-0.0.8/src/muheqa/connector.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.840781 muheqa-0.0.8/src/muheqa/evidence/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.841147 muheqa-0.0.8/src/muheqa/evidence/candidates/
--rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.8/src/muheqa/evidence/candidates/ranking.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.8/src/muheqa/evidence/discoverer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.841440 muheqa-0.0.8/src/muheqa/evidence/documents/
--rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.8/src/muheqa/evidence/documents/splitter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.841698 muheqa-0.0.8/src/muheqa/evidence/responses/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1395 2023-06-12 10:17:15.000000 muheqa-0.0.8/src/muheqa/evidence/responses/retriever.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.8/src/muheqa/logformatter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.841953 muheqa-0.0.8/src/muheqa/summary/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.843072 muheqa-0.0.8/src/muheqa/summary/keywords/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.8/src/muheqa/summary/keywords/concept.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.8/src/muheqa/summary/keywords/discovery.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.8/src/muheqa/summary/keywords/entity.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.844424 muheqa-0.0.8/src/muheqa/summary/resources/
--rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.8/src/muheqa/summary/resources/d4c.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     6299 2023-06-12 17:17:49.000000 muheqa-0.0.8/src/muheqa/summary/resources/dbpedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-12 17:17:59.000000 muheqa-0.0.8/src/muheqa/summary/resources/graph.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-12 16:10:14.000000 muheqa-0.0.8/src/muheqa/summary/resources/wikipedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.8/src/muheqa/summary/summarizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.845260 muheqa-0.0.8/src/muheqa/summary/texts/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.8/src/muheqa/summary/texts/verbalizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 17:19:00.839737 muheqa-0.0.8/src/muheqa.egg-info/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 17:19:00.000000 muheqa-0.0.8/src/muheqa.egg-info/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      930 2023-06-12 17:19:00.000000 muheqa-0.0.8/src/muheqa.egg-info/SOURCES.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-12 17:19:00.000000 muheqa-0.0.8/src/muheqa.egg-info/dependency_links.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-12 17:19:00.000000 muheqa-0.0.8/src/muheqa.egg-info/requires.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       14 2023-06-12 17:19:00.000000 muheqa-0.0.8/src/muheqa.egg-info/top_level.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)      194 2023-06-12 10:17:46.000000 muheqa-0.0.8/src/sample.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.830895 muheqa-0.0.9/
+-rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.9/LICENSE
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 18:11:28.830675 muheqa-0.0.9/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      543 2023-06-10 18:08:18.000000 muheqa-0.0.9/README.md
+-rw-r--r--   0 cbadenes   (501) staff       (20)      945 2023-06-12 18:10:10.000000 muheqa-0.0.9/pyproject.toml
+-rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-12 18:11:28.830960 muheqa-0.0.9/setup.cfg
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.826161 muheqa-0.0.9/src/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.826671 muheqa-0.0.9/src/muheqa/
+-rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.9/src/muheqa/__init__.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.827550 muheqa-0.0.9/src/muheqa/answer/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.827662 muheqa-0.0.9/src/muheqa/answer/analysis/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.9/src/muheqa/answer/analysis/classifier.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.9/src/muheqa/answer/composer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.827769 muheqa-0.0.9/src/muheqa/answer/generation/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.9/src/muheqa/answer/generation/model.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.9/src/muheqa/connection.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      146 2023-06-12 08:13:34.000000 muheqa-0.0.9/src/muheqa/connector.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.827873 muheqa-0.0.9/src/muheqa/evidence/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.828009 muheqa-0.0.9/src/muheqa/evidence/candidates/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.9/src/muheqa/evidence/candidates/ranking.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.9/src/muheqa/evidence/discoverer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.828124 muheqa-0.0.9/src/muheqa/evidence/documents/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.9/src/muheqa/evidence/documents/splitter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.828237 muheqa-0.0.9/src/muheqa/evidence/responses/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1395 2023-06-12 10:17:15.000000 muheqa-0.0.9/src/muheqa/evidence/responses/retriever.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.9/src/muheqa/logformatter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.828342 muheqa-0.0.9/src/muheqa/summary/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.828749 muheqa-0.0.9/src/muheqa/summary/keywords/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.9/src/muheqa/summary/keywords/concept.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.9/src/muheqa/summary/keywords/discovery.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.9/src/muheqa/summary/keywords/entity.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.830169 muheqa-0.0.9/src/muheqa/summary/resources/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.9/src/muheqa/summary/resources/d4c.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     6309 2023-06-12 18:10:53.000000 muheqa-0.0.9/src/muheqa/summary/resources/dbpedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-12 17:17:59.000000 muheqa-0.0.9/src/muheqa/summary/resources/graph.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-12 16:10:14.000000 muheqa-0.0.9/src/muheqa/summary/resources/wikipedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.9/src/muheqa/summary/summarizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.830358 muheqa-0.0.9/src/muheqa/summary/texts/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.9/src/muheqa/summary/texts/verbalizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 18:11:28.827378 muheqa-0.0.9/src/muheqa.egg-info/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 18:11:28.000000 muheqa-0.0.9/src/muheqa.egg-info/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      954 2023-06-12 18:11:28.000000 muheqa-0.0.9/src/muheqa.egg-info/SOURCES.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-12 18:11:28.000000 muheqa-0.0.9/src/muheqa.egg-info/dependency_links.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-12 18:11:28.000000 muheqa-0.0.9/src/muheqa.egg-info/requires.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       31 2023-06-12 18:11:28.000000 muheqa-0.0.9/src/muheqa.egg-info/top_level.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1484 2023-06-12 18:04:36.000000 muheqa-0.0.9/src/process_evidence.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      194 2023-06-12 10:17:46.000000 muheqa-0.0.9/src/sample.py
```

### Comparing `muheqa-0.0.8/LICENSE` & `muheqa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/PKG-INFO` & `muheqa-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `muheqa-0.0.8/README.md` & `muheqa-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/pyproject.toml` & `muheqa-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "sentence-transformers",
     "sparqlwrapper"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "muheqa"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Carlos Badenes-Olmedo", email="carlos.badenes@upm.es" },
 ]
 description = "Multiple and Heterogeneous Question-Answering"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `muheqa-0.0.8/src/muheqa/answer/analysis/classifier.py` & `muheqa-0.0.9/src/muheqa/answer/analysis/classifier.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/answer/composer.py` & `muheqa-0.0.9/src/muheqa/answer/composer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/answer/generation/model.py` & `muheqa-0.0.9/src/muheqa/answer/generation/model.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/connection.py` & `muheqa-0.0.9/src/muheqa/connection.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/evidence/candidates/ranking.py` & `muheqa-0.0.9/src/muheqa/evidence/candidates/ranking.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/evidence/discoverer.py` & `muheqa-0.0.9/src/muheqa/evidence/discoverer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/evidence/documents/splitter.py` & `muheqa-0.0.9/src/muheqa/evidence/documents/splitter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/evidence/responses/retriever.py` & `muheqa-0.0.9/src/muheqa/evidence/responses/retriever.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/logformatter.py` & `muheqa-0.0.9/src/muheqa/logformatter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/keywords/concept.py` & `muheqa-0.0.9/src/muheqa/summary/keywords/concept.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/keywords/discovery.py` & `muheqa-0.0.9/src/muheqa/summary/keywords/discovery.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/keywords/entity.py` & `muheqa-0.0.9/src/muheqa/summary/keywords/entity.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/resources/d4c.py` & `muheqa-0.0.9/src/muheqa/summary/resources/d4c.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/resources/dbpedia.py` & `muheqa-0.0.9/src/muheqa/summary/resources/dbpedia.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self):
         self.logger = logging.getLogger('muheqa')
         self.logger.debug("initializing DBpedia retriever...")
         self.sparql = SPARQLWrapper(
             "https://dbpedia.org/sparql/", agent='Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/50.0.2661.102 Safari/537.36')
         self.sparql.setReturnFormat(JSON)
         self.sparql.setTimeout(timeout=60)
-        self.graph 		= kg_graph.Graph()
+        self.graph 	= kg_graph.Graph()
 
     def get_property_value(self, filter):
         query = """
 			PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#> 
 			PREFIX dbr: <http://dbpedia.org/resource/> 
 			select distinct ?object ?label {
 			{ FILTER }
@@ -102,15 +102,15 @@
         try:
             r = requests.get(request, headers=headers)
         except:
             self.logger.error("An error getting data from DBpedia lookup service: ")
             return []
         if (len(r.json()['docs']) == 0):
             lemma = self.graph.lemmatize(label)	
-			self.logger.debug("retry search by lemma:" + str(lemma))
+            self.logger.debug("search retried by lemma:" + str(lemma))
             r = requests.get(query_path.replace("QUERY_TEXT", lemma))
             size = len(label.split(" "))
             index = 1
             while(('search' in r.json()) and (len(r.json()['search']) == 0) and (index < size)):
                 query_label = " ".join(label.split(" ")[index:])
                 index += 1
                 r = requests.get(query_path.replace("QUERY_TEXT", query_label))
```

### Comparing `muheqa-0.0.8/src/muheqa/summary/resources/graph.py` & `muheqa-0.0.9/src/muheqa/summary/resources/graph.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/resources/wikipedia.py` & `muheqa-0.0.9/src/muheqa/summary/resources/wikipedia.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/summarizer.py` & `muheqa-0.0.9/src/muheqa/summary/summarizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa/summary/texts/verbalizer.py` & `muheqa-0.0.9/src/muheqa/summary/texts/verbalizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.8/src/muheqa.egg-info/PKG-INFO` & `muheqa-0.0.9/src/muheqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `muheqa-0.0.8/src/muheqa.egg-info/SOURCES.txt` & `muheqa-0.0.9/src/muheqa.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+src/process_evidence.py
 src/sample.py
 src/muheqa/__init__.py
 src/muheqa/connection.py
 src/muheqa/connector.py
 src/muheqa/logformatter.py
 src/muheqa.egg-info/PKG-INFO
 src/muheqa.egg-info/SOURCES.txt
```

