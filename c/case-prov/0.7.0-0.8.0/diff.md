# Comparing `tmp/case_prov-0.7.0.tar.gz` & `tmp/case_prov-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "case_prov-0.7.0.tar", last modified: Tue Apr  4 18:11:55 2023, max compression
+gzip compressed data, was "case_prov-0.8.0.tar", last modified: Mon Jun 12 19:37:08 2023, max compression
```

## Comparing `case_prov-0.7.0.tar` & `case_prov-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:55.925835 case_prov-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-04 18:08:14.000000 case_prov-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 18:11:55.925835 case_prov-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-04 18:08:14.000000 case_prov-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-04 18:08:14.000000 case_prov-0.7.0/README_PyPI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-04 18:08:14.000000 case_prov-0.7.0/THIRD_PARTY_LICENSES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:55.917834 case_prov-0.7.0/case_prov/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/case_prov_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    29166 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/case_prov_dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/case_prov_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:55.921834 case_prov-0.7.0/case_prov/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Activity.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Agent.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Association.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Attribution.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Collection.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Communication.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Delegation.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Derivation.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Entity.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Generation.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Person.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-SoftwareAgent.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-Usage.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-actedOnBehalfOf.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-used-nothing.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-used.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-wasAssociatedWith.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-wasAttributedTo.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-wasDerivedFrom-map.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-wasDerivedFrom.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-wasGeneratedBy.sparql
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-wasInformedBy-map.sparql
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/queries/construct-wasInformedBy.sparql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:55.925835 case_prov-0.7.0/case_prov/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/shapes/case-prov.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-04 18:08:14.000000 case_prov-0.7.0/case_prov/shapes/prov-shapes.ttl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:55.921834 case_prov-0.7.0/case_prov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-04 18:11:55.000000 case_prov-0.7.0/case_prov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-04 18:11:55.000000 case_prov-0.7.0/case_prov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:11:55.000000 case_prov-0.7.0/case_prov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-04 18:11:55.000000 case_prov-0.7.0/case_prov.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 18:11:55.000000 case_prov-0.7.0/case_prov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 18:11:55.000000 case_prov-0.7.0/case_prov.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 18:11:55.925835 case_prov-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-04 18:08:14.000000 case_prov-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:08.563295 case_prov-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-12 19:34:12.000000 case_prov-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 19:37:08.563295 case_prov-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-06-12 19:34:12.000000 case_prov-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-12 19:34:12.000000 case_prov-0.8.0/README_PyPI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-12 19:34:12.000000 case_prov-0.8.0/THIRD_PARTY_LICENSES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:08.563295 case_prov-0.8.0/case_prov/
+-rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/case_prov_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87137 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/case_prov_dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/case_prov_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:08.563295 case_prov-0.8.0/case_prov/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-Activity.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-Agent.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-Collection.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-Entity.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-Person.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-SoftwareAgent.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-actedOnBehalfOf.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-used-nothing.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-used.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-wasAssociatedWith.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-wasAttributedTo.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-wasDerivedFrom-map.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-wasDerivedFrom.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-wasGeneratedBy.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-wasInformedBy-map.sparql
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/queries/construct-wasInformedBy.sparql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:08.563295 case_prov-0.8.0/case_prov/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/shapes/case-prov.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-12 19:34:12.000000 case_prov-0.8.0/case_prov/shapes/prov-shapes.ttl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:37:08.563295 case_prov-0.8.0/case_prov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-12 19:37:08.000000 case_prov-0.8.0/case_prov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-12 19:37:08.000000 case_prov-0.8.0/case_prov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:37:08.000000 case_prov-0.8.0/case_prov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-12 19:37:08.000000 case_prov-0.8.0/case_prov.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 19:37:08.000000 case_prov-0.8.0/case_prov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 19:37:08.000000 case_prov-0.8.0/case_prov.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-12 19:37:08.567295 case_prov-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-12 19:34:12.000000 case_prov-0.8.0/setup.py
```

### Comparing `case_prov-0.7.0/LICENSE` & `case_prov-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/PKG-INFO` & `case_prov-0.8.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: case_prov
-Version: 0.7.0
+Version: 0.8.0
 Summary: A mapping of CASE to W3C PROV
-Home-page: https://github.com/casework/CASE-Implementation-PROV
+Home-page: https://github.com/casework/CASE-Implementation-PROV-O
 Author: Alex Nelson
 Author-email: alexander.nelson@nist.gov
-License: UNKNOWN
-Description: # CASE Implementation: PROV-O
-        
-        This repository maps [CASE](https://caseontology.org/) to [W3C PROV-O](https://www.w3.org/TR/prov-o/).  Note that contrary to other CASE implementations, this maps CASE out to another data model, instead of mapping another data model or tool into CASE.
-        
-        Full documentation is available at the [project homepage](https://github.com/casework/CASE-Implementation-PROV-O).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+License-File: THIRD_PARTY_LICENSES.md
+
+# CASE Implementation: PROV-O
+
+This repository maps [CASE](https://caseontology.org/) to [W3C PROV-O](https://www.w3.org/TR/prov-o/) and [OWL-Time](https://www.w3.org/TR/owl-time/).  Note that contrary to other CASE implementations, this maps CASE out to another data model, instead of mapping another data model or tool into CASE.
+
+Full documentation is available at the [project homepage](https://github.com/casework/CASE-Implementation-PROV-O).
```

### Comparing `case_prov-0.7.0/THIRD_PARTY_LICENSES.md` & `case_prov-0.8.0/THIRD_PARTY_LICENSES.md`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/__init__.py` & `case_prov-0.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,11 @@
 # protection and is in the public domain. NIST assumes no
 # responsibility whatsoever for its use by other parties, and makes
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
-__version__ = "0.7.0"
+import setuptools
+
+if __name__ == "__main__":
+    setuptools.setup()
```

### Comparing `case_prov-0.7.0/case_prov/case_prov_check.py` & `case_prov-0.8.0/case_prov/case_prov_check.py`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/py.typed` & `case_prov-0.8.0/case_prov/py.typed`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/queries/__init__.py` & `case_prov-0.8.0/case_prov/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Activity.sparql` & `case_prov-0.8.0/case_prov/queries/construct-Activity.sparql`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 CONSTRUCT
 {
   # Augment CASE InvestigativeActions as PROV Activities.
   ?nAction
     a prov:Activity ;
     prov:endedAtTime ?lEndTime ;
     prov:startedAtTime ?lStartTime ;
-    rdfs:comment ?lDescription ;
+    uco-core:description ?lDescription ;
+    uco-core:name ?lName ;
     .
 }
 WHERE {
   ?nAction
     a case-investigation:InvestigativeAction ;
     .
 
@@ -37,8 +38,14 @@
   }
 
   OPTIONAL {
     ?nAction
       uco-core:description ?lDescription ;
       .
   }
+
+  OPTIONAL {
+    ?nAction
+      uco-core:name ?lName ;
+      .
+  }
 }
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Agent.sparql` & `case_prov-0.8.0/case_prov/queries/construct-Agent.sparql`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,28 @@
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
   # Designate InvestigativeAction performers, and the instruments they use, as Agents.
   ?nAgent a prov:Agent .
-  ?nAgent rdfs:comment ?lDescription ;
+  ?nAgent uco-core:description ?lDescription .
+  ?nAgent uco-core:name ?lName .
 }
 WHERE {
   ?nInvestigativeAction
     a case-investigation:InvestigativeAction ;
     (uco-action:instrument|uco-action:performer) ?nAgent ;
     .
 
   OPTIONAL {
     ?nAgent
       uco-core:description ?lDescription ;
       .
   }
+
+  OPTIONAL {
+    ?nAgent
+      uco-core:name ?lName ;
+      .
+  }
 }
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Association.sparql` & `case_prov-0.8.0/case_prov/queries/construct-wasAssociatedWith.sparql`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,24 @@
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
-  ?nInvestigativeAction
-    prov:qualifiedAssociation [
-      a prov:Association ;
-      prov:agent ?nAgent ;
-      # TODO - A role enactment can go here, under prov:hadRole.
-    ] ;
-    .
+  # Designate InvestigativeAction performers as Agents.
+  ?nInvestigativeAction prov:wasAssociatedWith ?nAgent .
 }
 WHERE {
   ?nInvestigativeAction
     a case-investigation:InvestigativeAction ;
     .
 
   {
-    SELECT ?nAction ?nAgent
+    SELECT ?nInvestigativeAction ?nAgent
     WHERE {
       ?nInvestigativeAction
         uco-action:instrument ?nAgent ;
         .
       FILTER NOT EXISTS {
         ?nInvestigativeAction
           uco-action:performer ?nPerformer ;
@@ -43,23 +38,21 @@
     WHERE {
       ?nInvestigativeAction
         uco-action:performer ?nAgent ;
         .
       FILTER NOT EXISTS {
         ?nInvestigativeAction
           uco-action:instrument ?nInstrument ;
-          .
       }
     }
   }
   UNION
   {
     SELECT ?nInvestigativeAction ?nAgent
     WHERE {
       ?nInvestigativeAction
         uco-action:performer ?nPerformer ;
         uco-action:instrument ?nAgent ;
         .
     }
   }
 }
-
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Attribution.sparql` & `case_prov-0.8.0/case_prov/queries/construct-wasAttributedTo.sparql`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
-  ?nResult
-    prov:qualifiedAttribution [
-      a prov:Attribution ;
-      prov:agent ?nAgent ;
-    ] ;
-    .
+  # Designate InvestigativeAction results as associated with the action
+  # performer or the tool operating on their behalf.
+  ?nResult prov:wasAttributedTo ?nAgent .
 }
 WHERE {
   ?nInvestigativeAction
     a case-investigation:InvestigativeAction ;
     uco-action:result ?nResult ;
     .
 
@@ -29,29 +26,27 @@
     WHERE {
       ?nInvestigativeAction
         uco-action:instrument ?nAgent ;
         .
       FILTER NOT EXISTS {
         ?nInvestigativeAction
           uco-action:performer ?nPerformer ;
-          .
       }
     }
   }
   UNION
   {
     SELECT ?nInvestigativeAction ?nAgent
     WHERE {
       ?nInvestigativeAction
         uco-action:performer ?nAgent ;
         .
       FILTER NOT EXISTS {
         ?nInvestigativeAction
           uco-action:instrument ?nInstrument ;
-          .
       }
     }
   }
   UNION
   {
     SELECT ?nInvestigativeAction ?nAgent
     WHERE {
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Collection.sparql` & `case_prov-0.8.0/case_prov/queries/construct-Collection.sparql`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Delegation.sparql` & `case_prov-0.8.0/case_prov/queries/construct-actedOnBehalfOf.sparql`

 * *Files 21% similar despite different names*

```diff
@@ -7,21 +7,16 @@
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
-  ?nInstrument
-    prov:qualifiedDelegation [
-      a prov:Delegation ;
-      prov:agent ?nPerformer ;
-      prov:hadActivity ?nInvestigativeAction ;
-    ] ;
-  .
+  # Designate InvestigativeAction instruments as Agents acting on behalf of the action performer.
+  ?nInstrument prov:actedOnBehalfOf ?nPerformer .
 
 }
 WHERE {
   ?nInvestigativeAction
     a case-investigation:InvestigativeAction ;
     uco-action:instrument ?nInstrument ;
     uco-action:performer ?nPerformer ;
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Derivation.sparql` & `case_prov-0.8.0/case_prov/queries/construct-wasDerivedFrom.sparql`

 * *Files 24% similar despite different names*

```diff
@@ -7,27 +7,17 @@
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
-  # A lengthy explanation on why Generation and Usage are not made here
-  # is inlined in case_prov_dot.py.
-  # Also note that this query intentionally creates a Derivation node
-  # per ?nObjectA binding.  A test done in prov-check raises a
-  # PROV-CONSTRAINTs error (though, the test ID has not yet been
-  # determined) if a Derivation houses two prov:entity values.
-  ?nObjectB
-    prov:qualifiedDerivation [
-      a prov:Derivation ;
-      prov:entity ?nObjectA ;
-      prov:hadActivity ?nAction ;
-    ] ;
-    .
+  # Identify all objects that are outputs of an InvestigativeAction as
+  # wasDerivedFrom each of the action's inputs.
+  ?nObjectB prov:wasDerivedFrom ?nObjectA
 }
 WHERE {
   ?nAction
     a case-investigation:InvestigativeAction ;
     uco-action:result ?nObjectB ;
     .
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Generation.sparql` & `case_prov-0.8.0/case_prov/queries/construct-used-nothing.sparql`

 * *Files 14% similar despite different names*

```diff
@@ -7,27 +7,21 @@
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
-  ?nObject
-    prov:qualifiedGeneration [
-      a prov:Generation ;
-      prov:activity ?nAction ;
-      prov:atTime ?lTime ;
-    ] ;
-    .
+  # Augment PROV Activities with explicit no-input declarations.
+  ?nAction prov:used prov:EmptyCollection .
 }
 WHERE {
   ?nAction
     a case-investigation:InvestigativeAction ;
-    uco-action:result ?nObject ;
     .
 
-  OPTIONAL {
+  FILTER NOT EXISTS {
     ?nAction
-      uco-action:endTime ?lTime ;
+      uco-action:object ?nInput ;
       .
   }
 }
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-Person.sparql` & `case_prov-0.8.0/case_prov/queries/construct-Person.sparql`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/queries/construct-SoftwareAgent.sparql` & `case_prov-0.8.0/case_prov/queries/construct-SoftwareAgent.sparql`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/queries/construct-actedOnBehalfOf.sparql` & `case_prov-0.8.0/case_prov/queries/construct-wasGeneratedBy.sparql`

 * *Files 21% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
-  # Designate InvestigativeAction instruments as Agents acting on behalf of the action performer.
-  ?nInstrument prov:actedOnBehalfOf ?nPerformer .
-
+  # Identify all objects that are outputs of an InvestigativeAction as
+  # wasGeneratedBy the action.
+  ?nObject prov:wasGeneratedBy ?nAction .
 }
 WHERE {
-  ?nInvestigativeAction
+  ?nAction
     a case-investigation:InvestigativeAction ;
-    uco-action:instrument ?nInstrument ;
-    uco-action:performer ?nPerformer ;
+    uco-action:result ?nObject ;
     .
 }
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-used-nothing.sparql` & `case_prov-0.8.0/case_prov/queries/construct-used.sparql`

 * *Files 25% similar despite different names*

```diff
@@ -7,21 +7,16 @@
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
 CONSTRUCT
 {
-  # Augment PROV Activities with explicit no-input declarations.
-  ?nAction prov:used prov:EmptyCollection .
+  # Augment PROV Activities with inputs.
+  ?nAction prov:used ?nInput .
 }
 WHERE {
   ?nAction
     a case-investigation:InvestigativeAction ;
+    uco-action:object ?nInput ;
     .
-
-  FILTER NOT EXISTS {
-    ?nAction
-      uco-action:object ?nInput ;
-      .
-  }
 }
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-used.sparql` & `case_prov-0.8.0/case_prov/queries/construct-wasInformedBy-map.sparql`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 # protection and is in the public domain. NIST assumes no
 # responsibility whatsoever for its use by other parties, and makes
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
-CONSTRUCT
-{
-  # Augment PROV Activities with inputs.
-  ?nAction prov:used ?nInput .
+CONSTRUCT {
+  ?x prov:wasInformedBy ?y .
+  ?x a prov:Activity .
+  ?y a prov:Activity .
 }
 WHERE {
-  ?nAction
-    a case-investigation:InvestigativeAction ;
-    uco-action:object ?nInput ;
-    .
+  ?x case-investigation:wasInformedBy ?y .
 }
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-wasDerivedFrom-map.sparql` & `case_prov-0.8.0/case_prov/queries/construct-wasDerivedFrom-map.sparql`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/queries/construct-wasInformedBy-map.sparql` & `case_prov-0.8.0/case_prov/shapes/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,7 @@
 # United States Code this software is not subject to copyright
 # protection and is in the public domain. NIST assumes no
 # responsibility whatsoever for its use by other parties, and makes
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
-
-CONSTRUCT {
-  ?x prov:wasInformedBy ?y .
-  ?x a prov:Activity .
-  ?y a prov:Activity .
-}
-WHERE {
-  ?x case-investigation:wasInformedBy ?y .
-}
```

### Comparing `case_prov-0.7.0/case_prov/queries/construct-wasInformedBy.sparql` & `case_prov-0.8.0/case_prov/queries/construct-wasInformedBy.sparql`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/shapes/case-prov.ttl` & `case_prov-0.8.0/case_prov/shapes/case-prov.ttl`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov/shapes/prov-shapes.ttl` & `case_prov-0.8.0/case_prov/shapes/prov-shapes.ttl`

 * *Files identical despite different names*

### Comparing `case_prov-0.7.0/case_prov.egg-info/PKG-INFO` & `case_prov-0.8.0/case_prov.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: case-prov
-Version: 0.7.0
+Version: 0.8.0
 Summary: A mapping of CASE to W3C PROV
-Home-page: https://github.com/casework/CASE-Implementation-PROV
+Home-page: https://github.com/casework/CASE-Implementation-PROV-O
 Author: Alex Nelson
 Author-email: alexander.nelson@nist.gov
-License: UNKNOWN
-Description: # CASE Implementation: PROV-O
-        
-        This repository maps [CASE](https://caseontology.org/) to [W3C PROV-O](https://www.w3.org/TR/prov-o/).  Note that contrary to other CASE implementations, this maps CASE out to another data model, instead of mapping another data model or tool into CASE.
-        
-        Full documentation is available at the [project homepage](https://github.com/casework/CASE-Implementation-PROV-O).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+License-File: THIRD_PARTY_LICENSES.md
+
+# CASE Implementation: PROV-O
+
+This repository maps [CASE](https://caseontology.org/) to [W3C PROV-O](https://www.w3.org/TR/prov-o/) and [OWL-Time](https://www.w3.org/TR/owl-time/).  Note that contrary to other CASE implementations, this maps CASE out to another data model, instead of mapping another data model or tool into CASE.
+
+Full documentation is available at the [project homepage](https://github.com/casework/CASE-Implementation-PROV-O).
```

### Comparing `case_prov-0.7.0/case_prov.egg-info/SOURCES.txt` & `case_prov-0.8.0/case_prov.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,25 +14,18 @@
 case_prov.egg-info/dependency_links.txt
 case_prov.egg-info/entry_points.txt
 case_prov.egg-info/requires.txt
 case_prov.egg-info/top_level.txt
 case_prov/queries/__init__.py
 case_prov/queries/construct-Activity.sparql
 case_prov/queries/construct-Agent.sparql
-case_prov/queries/construct-Association.sparql
-case_prov/queries/construct-Attribution.sparql
 case_prov/queries/construct-Collection.sparql
-case_prov/queries/construct-Communication.sparql
-case_prov/queries/construct-Delegation.sparql
-case_prov/queries/construct-Derivation.sparql
 case_prov/queries/construct-Entity.sparql
-case_prov/queries/construct-Generation.sparql
 case_prov/queries/construct-Person.sparql
 case_prov/queries/construct-SoftwareAgent.sparql
-case_prov/queries/construct-Usage.sparql
 case_prov/queries/construct-actedOnBehalfOf.sparql
 case_prov/queries/construct-used-nothing.sparql
 case_prov/queries/construct-used.sparql
 case_prov/queries/construct-wasAssociatedWith.sparql
 case_prov/queries/construct-wasAttributedTo.sparql
 case_prov/queries/construct-wasDerivedFrom-map.sparql
 case_prov/queries/construct-wasDerivedFrom.sparql
```

### Comparing `case_prov-0.7.0/setup.cfg` & `case_prov-0.8.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -2,39 +2,43 @@
 name = case_prov
 version = attr: case_prov.__version__
 author = Alex Nelson
 author_email = alexander.nelson@nist.gov
 description = A mapping of CASE to W3C PROV
 long_description = file: README_PyPI.md
 long_description_content_type = text/markdown
-url = https://github.com/casework/CASE-Implementation-PROV
+url = https://github.com/casework/CASE-Implementation-PROV-O
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 license_files = 
 	LICENSE
 	THIRD_PARTY_LICENSES.md
 
 [options]
 include_package_data = true
 install_requires = 
-	case_utils >=0.10.0,< 0.11.0
+	case_utils >=0.11.0,< 0.12.0
 	prov
 	pydot
 packages = find:
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	case_prov_check = case_prov.case_prov_check:main
 	case_prov_dot = case_prov.case_prov_dot:main
 	case_prov_rdf = case_prov.case_prov_rdf:main
 
+[options.extras_require]
+testing = 
+	case_utils[testing]
+
 [options.package_data]
 case_prov = py.typed
 case_prov.queries = *.sparql
 case_prov.shapes = *.ttl
 
 [flake8]
 extend-ignore =
```

