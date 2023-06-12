# Comparing `tmp/dblp_crawler-1.6.3.tar.gz` & `tmp/dblp_crawler-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblp_crawler-1.6.3.tar", last modified: Mon Jun 12 03:38:47 2023, max compression
+gzip compressed data, was "dblp_crawler-1.6.4.tar", last modified: Mon Jun 12 11:46:45 2023, max compression
```

## Comparing `dblp_crawler-1.6.3.tar` & `dblp_crawler-1.6.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.145278 dblp_crawler-1.6.3/dblp_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/arg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.145278 dblp_crawler-1.6.3/dblp_crawler/data/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/dblp_crawler/data/ccf/
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/data/ccf/CCF_A.py
--rw-r--r--   0 runner    (1001) docker     (123)    26883 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/data/ccf/CCF_B.py
--rw-r--r--   0 runner    (1001) docker     (123)    33160 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/data/ccf/CCF_C.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/data/ccf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/data/ccf/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/data/ccf/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/dblp_crawler/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/filter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/dblp_crawler/keyword/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/keyword/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/keyword/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/dblp_crawler/summarizer/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/summarizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/dblp_crawler/summarizer/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/summarizer/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/summarizer/neo4j/n4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/dblp_crawler/summarizer/networkx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/summarizer/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/dblp_crawler/summarizer/networkx/nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 03:38:47.145278 dblp_crawler-1.6.3/dblp_crawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-12 03:38:47.000000 dblp_crawler-1.6.3/dblp_crawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-12 03:38:47.000000 dblp_crawler-1.6.3/dblp_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 03:38:47.000000 dblp_crawler-1.6.3/dblp_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 03:38:47.000000 dblp_crawler-1.6.3/dblp_crawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 03:38:47.000000 dblp_crawler-1.6.3/dblp_crawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 03:38:47.149278 dblp_crawler-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-12 03:38:37.000000 dblp_crawler-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.060004 dblp_crawler-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-12 11:46:45.060004 dblp_crawler-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.056004 dblp_crawler-1.6.4/dblp_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/arg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.056004 dblp_crawler-1.6.4/dblp_crawler/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.056004 dblp_crawler-1.6.4/dblp_crawler/data/ccf/
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/data/ccf/CCF_A.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26883 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/data/ccf/CCF_B.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33160 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/data/ccf/CCF_C.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/data/ccf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/data/ccf/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/data/ccf/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.056004 dblp_crawler-1.6.4/dblp_crawler/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/filter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.056004 dblp_crawler-1.6.4/dblp_crawler/keyword/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/keyword/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/keyword/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.056004 dblp_crawler-1.6.4/dblp_crawler/summarizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/summarizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.060004 dblp_crawler-1.6.4/dblp_crawler/summarizer/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/summarizer/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/summarizer/neo4j/n4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.060004 dblp_crawler-1.6.4/dblp_crawler/summarizer/networkx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/summarizer/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/dblp_crawler/summarizer/networkx/nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:46:45.056004 dblp_crawler-1.6.4/dblp_crawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-12 11:46:44.000000 dblp_crawler-1.6.4/dblp_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-12 11:46:45.000000 dblp_crawler-1.6.4/dblp_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:46:44.000000 dblp_crawler-1.6.4/dblp_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 11:46:44.000000 dblp_crawler-1.6.4/dblp_crawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 11:46:44.000000 dblp_crawler-1.6.4/dblp_crawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 11:46:45.060004 dblp_crawler-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-12 11:46:35.000000 dblp_crawler-1.6.4/setup.py
```

### Comparing `dblp_crawler-1.6.3/LICENSE` & `dblp_crawler-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/PKG-INFO` & `dblp_crawler-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblp_crawler
-Version: 1.6.3
+Version: 1.6.4
 Summary: 异步高并发dblp爬虫，慎用
 Home-page: https://github.com/yindaheng98/dblp-crawler
 Author: yindaheng98
 Author-email: yindaheng98@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dblp_crawler-1.6.3/README.md` & `dblp_crawler-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/__main__.py` & `dblp_crawler-1.6.4/dblp_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/arg.py` & `dblp_crawler-1.6.4/dblp_crawler/arg.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/data/ccf/CCF_A.py` & `dblp_crawler-1.6.4/dblp_crawler/data/ccf/CCF_A.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/data/ccf/CCF_B.py` & `dblp_crawler-1.6.4/dblp_crawler/data/ccf/CCF_B.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/data/ccf/CCF_C.py` & `dblp_crawler-1.6.4/dblp_crawler/data/ccf/CCF_C.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/data/ccf/key.py` & `dblp_crawler-1.6.4/dblp_crawler/data/ccf/key.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/data/ccf/parse.py` & `dblp_crawler-1.6.4/dblp_crawler/data/ccf/parse.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/downloader.py` & `dblp_crawler-1.6.4/dblp_crawler/downloader.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/filter/__init__.py` & `dblp_crawler-1.6.4/dblp_crawler/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/filter/__main__.py` & `dblp_crawler-1.6.4/dblp_crawler/filter/__main__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/filter/utils.py` & `dblp_crawler-1.6.4/dblp_crawler/filter/utils.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/graph.py` & `dblp_crawler-1.6.4/dblp_crawler/graph.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/journal.py` & `dblp_crawler-1.6.4/dblp_crawler/journal.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/keyword/__init__.py` & `dblp_crawler-1.6.4/dblp_crawler/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/keyword/arg.py` & `dblp_crawler-1.6.4/dblp_crawler/keyword/arg.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/parser.py` & `dblp_crawler-1.6.4/dblp_crawler/parser.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler/summarizer/neo4j/n4j.py` & `dblp_crawler-1.6.4/dblp_crawler/summarizer/neo4j/n4j.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import abc
-import asyncio
 import logging
 from typing import Optional
 
 from neo4j import Session
 
 from dblp_crawler import Graph, DBLPPerson, Publication
 
 logger = logging.getLogger("graph")
 
+def add_publication(tx, publication):
+    n4jset = "MERGE (p:Publication {key:$key}) SET p.title=$title, p.journal_key=$journal_key, p.journal=$journal, p.year=$year"
+    if publication.doi():
+        n4jset += ", p.doi=$doi"
+    tx.run(n4jset,
+            key=publication.key(),
+            title=publication.title(),
+            journal_key=publication.journal_key() or "",
+            journal=publication.journal() or "",
+            year=publication.year(),
+            doi=publication.doi())
+
 
 def add_person(tx, person: DBLPPerson, added_pubs: set):
     tx.run("MERGE (a:Person {pid: $pid, name: $name})", pid=person.pid(), name=person.name())
     for publication in person.publications():
         if publication.key() in added_pubs:
             continue
         added_pubs.add(publication.key())
-        tx.run("MATCH (a:Person) WHERE a.pid = $pid "
-               "MERGE (p:Publication {key:$key, title:$title, journal_key:$journal_key, journal:$journal, year:$year}) "
+        tx.run("MERGE (a:Person {pid: $pid}) "
+               "MERGE (p:Publication {key: $key}) "
                "MERGE (a)-[:WRITE]->(p)",
                pid=person.pid(),
-               key=publication.key(),
-               title=publication.title(),
-               journal_key=publication.journal_key() or "",
-               journal=publication.journal() or "",
-               year=publication.year())
-        if publication.doi():
-            tx.run("MATCH (p:Publication {key:$key}) SET p.doi=$doi",
-                key=publication.key(),
-                doi=publication.doi())
+               key=publication.key())
+        add_publication(tx, publication)
 
 
 def add_edge(tx, a: str, b: str, publication: Publication):
-    tx.run("MATCH (a:Person) WHERE a.pid = $a "
-           "MATCH (b:Person) WHERE b.pid = $b "
-           "MATCH (p:Publication) WHERE p.key = $key "
+    tx.run("MERGE (a:Person {pid: $a}) "
+           "MERGE (b:Person {pid: $b}) "
+           "MERGE (p:Publication {key: $key}) "
            "MERGE (a)-[:WRITE]->(p)"
            "MERGE (b)-[:WRITE]->(p)",
            a=a, b=b,
-           key=publication.key(),
-           title=publication.title(),
-           journal_key=publication.journal_key(),
-           journal=publication.journal(),
-           year=publication.year())
+           key=publication.key())
+    add_publication(tx, publication)
 
 
 class Neo4jGraph(Graph, metaclass=abc.ABCMeta):
     def __init__(self, session: Session, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.session = session
         self.added_pubs = set()
```

### Comparing `dblp_crawler-1.6.3/dblp_crawler/summarizer/networkx/nx.py` & `dblp_crawler-1.6.4/dblp_crawler/summarizer/networkx/nx.py`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/dblp_crawler.egg-info/PKG-INFO` & `dblp_crawler-1.6.4/dblp_crawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblp-crawler
-Version: 1.6.3
+Version: 1.6.4
 Summary: 异步高并发dblp爬虫，慎用
 Home-page: https://github.com/yindaheng98/dblp-crawler
 Author: yindaheng98
 Author-email: yindaheng98@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dblp_crawler-1.6.3/dblp_crawler.egg-info/SOURCES.txt` & `dblp_crawler-1.6.4/dblp_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblp_crawler-1.6.3/setup.py` & `dblp_crawler-1.6.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'dblp_crawler.summarizer': 'dblp_crawler/summarizer',
     'dblp_crawler.summarizer.networkx': 'dblp_crawler/summarizer/networkx',
     'dblp_crawler.summarizer.neo4j': 'dblp_crawler/summarizer/neo4j',
 }
 
 setup(
     name='dblp_crawler',
-    version='1.6.3',
+    version='1.6.4',
     author='yindaheng98',
     author_email='yindaheng98@163.com',
     url='https://github.com/yindaheng98/dblp-crawler',
     description=u'异步高并发dblp爬虫，慎用',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir=package_dir,
```

