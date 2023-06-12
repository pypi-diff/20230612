# Comparing `tmp/muheqa-0.0.6.tar.gz` & `tmp/muheqa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muheqa-0.0.6.tar", last modified: Mon Jun 12 10:20:48 2023, max compression
+gzip compressed data, was "muheqa-0.0.7.tar", last modified: Mon Jun 12 16:10:42 2023, max compression
```

## Comparing `muheqa-0.0.6.tar` & `muheqa-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.850795 muheqa-0.0.6/
--rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.6/LICENSE
--rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 10:20:48.850653 muheqa-0.0.6/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      543 2023-06-10 18:08:18.000000 muheqa-0.0.6/README.md
--rw-r--r--   0 cbadenes   (501) staff       (20)      945 2023-06-12 10:19:44.000000 muheqa-0.0.6/pyproject.toml
--rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-12 10:20:48.850839 muheqa-0.0.6/setup.cfg
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.842242 muheqa-0.0.6/src/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.843615 muheqa-0.0.6/src/muheqa/
--rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.6/src/muheqa/__init__.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.845284 muheqa-0.0.6/src/muheqa/answer/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.845558 muheqa-0.0.6/src/muheqa/answer/analysis/
--rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.6/src/muheqa/answer/analysis/classifier.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.6/src/muheqa/answer/composer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.845885 muheqa-0.0.6/src/muheqa/answer/generation/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.6/src/muheqa/answer/generation/model.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.6/src/muheqa/connection.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      146 2023-06-12 08:13:34.000000 muheqa-0.0.6/src/muheqa/connector.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.846207 muheqa-0.0.6/src/muheqa/evidence/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.846635 muheqa-0.0.6/src/muheqa/evidence/candidates/
--rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.6/src/muheqa/evidence/candidates/ranking.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.6/src/muheqa/evidence/discoverer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.846899 muheqa-0.0.6/src/muheqa/evidence/documents/
--rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.6/src/muheqa/evidence/documents/splitter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.847405 muheqa-0.0.6/src/muheqa/evidence/responses/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1395 2023-06-12 10:17:15.000000 muheqa-0.0.6/src/muheqa/evidence/responses/retriever.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.6/src/muheqa/logformatter.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.847783 muheqa-0.0.6/src/muheqa/summary/
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.848684 muheqa-0.0.6/src/muheqa/summary/keywords/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.6/src/muheqa/summary/keywords/concept.py
--rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.6/src/muheqa/summary/keywords/discovery.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.6/src/muheqa/summary/keywords/entity.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.850009 muheqa-0.0.6/src/muheqa/summary/resources/
--rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.6/src/muheqa/summary/resources/d4c.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     6234 2023-06-12 10:17:01.000000 muheqa-0.0.6/src/muheqa/summary/resources/dbpedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-09 14:59:33.000000 muheqa-0.0.6/src/muheqa/summary/resources/graph.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-12 10:17:08.000000 muheqa-0.0.6/src/muheqa/summary/resources/wikipedia.py
--rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.6/src/muheqa/summary/summarizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.850220 muheqa-0.0.6/src/muheqa/summary/texts/
--rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.6/src/muheqa/summary/texts/verbalizer.py
-drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 10:20:48.845106 muheqa-0.0.6/src/muheqa.egg-info/
--rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 10:20:48.000000 muheqa-0.0.6/src/muheqa.egg-info/PKG-INFO
--rw-r--r--   0 cbadenes   (501) staff       (20)      930 2023-06-12 10:20:48.000000 muheqa-0.0.6/src/muheqa.egg-info/SOURCES.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-12 10:20:48.000000 muheqa-0.0.6/src/muheqa.egg-info/dependency_links.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-12 10:20:48.000000 muheqa-0.0.6/src/muheqa.egg-info/requires.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)       14 2023-06-12 10:20:48.000000 muheqa-0.0.6/src/muheqa.egg-info/top_level.txt
--rw-r--r--   0 cbadenes   (501) staff       (20)      194 2023-06-12 10:17:46.000000 muheqa-0.0.6/src/sample.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.122111 muheqa-0.0.7/
+-rw-r--r--   0 cbadenes   (501) staff       (20)    11357 2023-06-09 14:21:26.000000 muheqa-0.0.7/LICENSE
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 16:10:42.121976 muheqa-0.0.7/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      543 2023-06-10 18:08:18.000000 muheqa-0.0.7/README.md
+-rw-r--r--   0 cbadenes   (501) staff       (20)      945 2023-06-12 16:10:08.000000 muheqa-0.0.7/pyproject.toml
+-rw-r--r--   0 cbadenes   (501) staff       (20)       38 2023-06-12 16:10:42.122152 muheqa-0.0.7/setup.cfg
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.115202 muheqa-0.0.7/src/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.116320 muheqa-0.0.7/src/muheqa/
+-rw-r--r--   0 cbadenes   (501) staff       (20)        0 2023-06-10 14:13:07.000000 muheqa-0.0.7/src/muheqa/__init__.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.117227 muheqa-0.0.7/src/muheqa/answer/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.117522 muheqa-0.0.7/src/muheqa/answer/analysis/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      518 2023-06-09 15:06:05.000000 muheqa-0.0.7/src/muheqa/answer/analysis/classifier.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      634 2023-06-09 14:49:07.000000 muheqa-0.0.7/src/muheqa/answer/composer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.117777 muheqa-0.0.7/src/muheqa/answer/generation/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1312 2022-10-27 14:00:16.000000 muheqa-0.0.7/src/muheqa/answer/generation/model.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1141 2023-06-10 16:48:18.000000 muheqa-0.0.7/src/muheqa/connection.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      146 2023-06-12 08:13:34.000000 muheqa-0.0.7/src/muheqa/connector.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.118064 muheqa-0.0.7/src/muheqa/evidence/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.118473 muheqa-0.0.7/src/muheqa/evidence/candidates/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      884 2023-06-09 14:48:22.000000 muheqa-0.0.7/src/muheqa/evidence/candidates/ranking.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      758 2023-06-09 14:58:33.000000 muheqa-0.0.7/src/muheqa/evidence/discoverer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.118738 muheqa-0.0.7/src/muheqa/evidence/documents/
+-rw-r--r--   0 cbadenes   (501) staff       (20)      843 2023-06-09 14:48:40.000000 muheqa-0.0.7/src/muheqa/evidence/documents/splitter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.119027 muheqa-0.0.7/src/muheqa/evidence/responses/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1395 2023-06-12 10:17:15.000000 muheqa-0.0.7/src/muheqa/evidence/responses/retriever.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      731 2022-08-29 10:15:01.000000 muheqa-0.0.7/src/muheqa/logformatter.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.119293 muheqa-0.0.7/src/muheqa/summary/
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.120165 muheqa-0.0.7/src/muheqa/summary/keywords/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2300 2022-10-27 21:31:49.000000 muheqa-0.0.7/src/muheqa/summary/keywords/concept.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)      862 2023-06-09 14:48:00.000000 muheqa-0.0.7/src/muheqa/summary/keywords/discovery.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1228 2022-09-19 13:11:51.000000 muheqa-0.0.7/src/muheqa/summary/keywords/entity.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.121374 muheqa-0.0.7/src/muheqa/summary/resources/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3151 2023-06-09 14:45:50.000000 muheqa-0.0.7/src/muheqa/summary/resources/d4c.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     6249 2023-06-12 16:10:10.000000 muheqa-0.0.7/src/muheqa/summary/resources/dbpedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     3949 2023-06-12 16:10:13.000000 muheqa-0.0.7/src/muheqa/summary/resources/graph.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     5154 2023-06-12 16:10:14.000000 muheqa-0.0.7/src/muheqa/summary/resources/wikipedia.py
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2294 2023-06-09 14:44:24.000000 muheqa-0.0.7/src/muheqa/summary/summarizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.121626 muheqa-0.0.7/src/muheqa/summary/texts/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     2217 2023-06-09 14:45:06.000000 muheqa-0.0.7/src/muheqa/summary/texts/verbalizer.py
+drwxr-xr-x   0 cbadenes   (501) staff       (20)        0 2023-06-12 16:10:42.117052 muheqa-0.0.7/src/muheqa.egg-info/
+-rw-r--r--   0 cbadenes   (501) staff       (20)     1244 2023-06-12 16:10:42.000000 muheqa-0.0.7/src/muheqa.egg-info/PKG-INFO
+-rw-r--r--   0 cbadenes   (501) staff       (20)      930 2023-06-12 16:10:42.000000 muheqa-0.0.7/src/muheqa.egg-info/SOURCES.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)        1 2023-06-12 16:10:42.000000 muheqa-0.0.7/src/muheqa.egg-info/dependency_links.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       52 2023-06-12 16:10:42.000000 muheqa-0.0.7/src/muheqa.egg-info/requires.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)       14 2023-06-12 16:10:42.000000 muheqa-0.0.7/src/muheqa.egg-info/top_level.txt
+-rw-r--r--   0 cbadenes   (501) staff       (20)      194 2023-06-12 10:17:46.000000 muheqa-0.0.7/src/sample.py
```

### Comparing `muheqa-0.0.6/LICENSE` & `muheqa-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/PKG-INFO` & `muheqa-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.6
+Version: 0.0.7
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `muheqa-0.0.6/README.md` & `muheqa-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/pyproject.toml` & `muheqa-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "sentence-transformers",
     "sparqlwrapper"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "muheqa"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Carlos Badenes-Olmedo", email="carlos.badenes@upm.es" },
 ]
 description = "Multiple and Heterogeneous Question-Answering"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `muheqa-0.0.6/src/muheqa/answer/analysis/classifier.py` & `muheqa-0.0.7/src/muheqa/answer/analysis/classifier.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/answer/composer.py` & `muheqa-0.0.7/src/muheqa/answer/composer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/answer/generation/model.py` & `muheqa-0.0.7/src/muheqa/answer/generation/model.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/connection.py` & `muheqa-0.0.7/src/muheqa/connection.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/evidence/candidates/ranking.py` & `muheqa-0.0.7/src/muheqa/evidence/candidates/ranking.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/evidence/discoverer.py` & `muheqa-0.0.7/src/muheqa/evidence/discoverer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/evidence/documents/splitter.py` & `muheqa-0.0.7/src/muheqa/evidence/documents/splitter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/evidence/responses/retriever.py` & `muheqa-0.0.7/src/muheqa/evidence/responses/retriever.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/logformatter.py` & `muheqa-0.0.7/src/muheqa/logformatter.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/keywords/concept.py` & `muheqa-0.0.7/src/muheqa/summary/keywords/concept.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/keywords/discovery.py` & `muheqa-0.0.7/src/muheqa/summary/keywords/discovery.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/keywords/entity.py` & `muheqa-0.0.7/src/muheqa/summary/keywords/entity.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/resources/d4c.py` & `muheqa-0.0.7/src/muheqa/summary/resources/d4c.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/resources/dbpedia.py` & `muheqa-0.0.7/src/muheqa/summary/resources/dbpedia.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     def __init__(self):
         self.logger = logging.getLogger('muheqa')
         self.logger.debug("initializing DBpedia retriever...")
         self.sparql = SPARQLWrapper(
             "https://dbpedia.org/sparql/", agent='Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/50.0.2661.102 Safari/537.36')
         self.sparql.setReturnFormat(JSON)
         self.sparql.setTimeout(timeout=60)
+        self.graph 		= kg_graph.Graph()
 
     def get_property_value(self, filter):
         query = """
 			PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#> 
 			PREFIX dbr: <http://dbpedia.org/resource/> 
 			select distinct ?object ?label {
 			{ FILTER }
@@ -99,16 +100,17 @@
         request = query_path.replace("QUERY_TEXT", label)
         try:
             r = requests.get(request, headers=headers)
         except:
             self.logger.error("An error getting data from DBpedia lookup service: ")
             return []
         if (len(r.json()['docs']) == 0):
-            r = requests.get(query_path.replace("QUERY_TEXT", lemmatize(label)))
-            self.logger.debug("no resources found in DBpedia for label: " + label + ", retried with: " + lemmatize(label))
+            lemma = self.graph.lemmatize(label)	
+			self.logger.debug("retry search by lemma:" + str(lemma))
+            r = requests.get(query_path.replace("QUERY_TEXT", lemma))
             size = len(label.split(" "))
             index = 1
             while(('search' in r.json()) and (len(r.json()['search']) == 0) and (index < size)):
                 query_label = " ".join(label.split(" ")[index:])
                 index += 1
                 r = requests.get(query_path.replace("QUERY_TEXT", query_label))
                 self.logger.debug("retried with: " + query_label)
```

### Comparing `muheqa-0.0.6/src/muheqa/summary/resources/graph.py` & `muheqa-0.0.7/src/muheqa/summary/resources/graph.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/resources/wikipedia.py` & `muheqa-0.0.7/src/muheqa/summary/resources/wikipedia.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/summarizer.py` & `muheqa-0.0.7/src/muheqa/summary/summarizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa/summary/texts/verbalizer.py` & `muheqa-0.0.7/src/muheqa/summary/texts/verbalizer.py`

 * *Files identical despite different names*

### Comparing `muheqa-0.0.6/src/muheqa.egg-info/PKG-INFO` & `muheqa-0.0.7/src/muheqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muheqa
-Version: 0.0.6
+Version: 0.0.7
 Summary: Multiple and Heterogeneous Question-Answering
 Author-email: Carlos Badenes-Olmedo <carlos.badenes@upm.es>
 Project-URL: Homepage, https://github.com/librairy/muheqa-core
 Project-URL: Bug Tracker, https://github.com/librairy/muheqa-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `muheqa-0.0.6/src/muheqa.egg-info/SOURCES.txt` & `muheqa-0.0.7/src/muheqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

