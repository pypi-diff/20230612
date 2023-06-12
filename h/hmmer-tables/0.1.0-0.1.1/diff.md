# Comparing `tmp/hmmer_tables-0.1.0.tar.gz` & `tmp/hmmer_tables-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmer_tables-0.1.0.tar", max compression
+gzip compressed data, was "hmmer_tables-0.1.1.tar", max compression
```

## Comparing `hmmer_tables-0.1.0.tar` & `hmmer_tables-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-06-12 15:39:46.426268 hmmer_tables-0.1.0/LICENSE
--rw-r--r--   0        0        0       15 2023-06-12 15:39:46.427467 hmmer_tables-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 15:39:56.207600 hmmer_tables-0.1.0/hmmer_tables/__init__.py
--rw-r--r--   0        0        0      319 2023-06-12 15:39:56.208378 hmmer_tables-0.1.0/hmmer_tables/csv_iter.py
--rw-r--r--   0        0        0     2902 2023-06-12 15:39:56.207289 hmmer_tables-0.1.0/hmmer_tables/domtbl.py
--rw-r--r--   0        0        0     1866 2023-06-12 15:39:56.206656 hmmer_tables-0.1.0/hmmer_tables/interval.py
--rw-r--r--   0        0        0       72 2023-06-12 15:39:56.205996 hmmer_tables-0.1.0/hmmer_tables/path_like.py
--rw-r--r--   0        0        0     1646 2023-06-12 15:39:56.208036 hmmer_tables-0.1.0/hmmer_tables/tbl.py
--rw-r--r--   0        0        0      468 2023-06-12 15:39:46.427127 hmmer_tables-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hmmer_tables-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-12 15:39:46.426268 hmmer_tables-0.1.1/LICENSE
+-rw-r--r--   0        0        0       15 2023-06-12 15:39:46.427467 hmmer_tables-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 15:39:56.207600 hmmer_tables-0.1.1/hmmer_tables/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-12 15:39:56.208378 hmmer_tables-0.1.1/hmmer_tables/csv_iter.py
+-rw-r--r--   0        0        0     3038 2023-06-12 15:49:25.111691 hmmer_tables-0.1.1/hmmer_tables/domtbl.py
+-rw-r--r--   0        0        0     1866 2023-06-12 15:39:56.206656 hmmer_tables-0.1.1/hmmer_tables/interval.py
+-rw-r--r--   0        0        0       72 2023-06-12 15:39:56.205996 hmmer_tables-0.1.1/hmmer_tables/path_like.py
+-rw-r--r--   0        0        0     1747 2023-06-12 15:51:43.511951 hmmer_tables-0.1.1/hmmer_tables/tbl.py
+-rw-r--r--   0        0        0      468 2023-06-12 15:52:49.194535 hmmer_tables-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 hmmer_tables-0.1.1/PKG-INFO
```

### Comparing `hmmer_tables-0.1.0/LICENSE` & `hmmer_tables-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.1.0/hmmer_tables/domtbl.py` & `hmmer_tables-0.1.1/hmmer_tables/domtbl.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 class DomTBLIndex(BaseModel):
     name: str
     accession: str
     length: int
 
 
 class DomTBLSeqScore(BaseModel):
-    e_value: str
-    score: str
-    bias: str
+    e_value: float
+    score: float
+    bias: float
 
 
 class DomTBLDomScore(BaseModel):
     id: int
     size: int
-    c_value: str
-    i_value: str
-    score: str
-    bias: str
+    c_value: float
+    i_value: float
+    score: float
+    bias: float
 
 
 class DomTBLCoord(BaseModel):
     """
     Coordinates.
 
     Parameters
@@ -72,15 +72,15 @@
     target: DomTBLIndex
     query: DomTBLIndex
     full_sequence: DomTBLSeqScore
     domain: DomTBLDomScore
     hmm_coord: DomTBLCoord
     ali_coord: DomTBLCoord
     env_coord: DomTBLCoord
-    acc: str
+    acc: float
     description: str
 
     def _asdict(self):
         return dataclasses.asdict(self)
 
     def __iter__(self):
         return iter(self._asdict().values())
@@ -97,27 +97,31 @@
     ----------
     file
         File path or file stream.
     """
     rows = []
     with open(filename, "r") as file:
         for x in csv_iter(file):
+            seq_score = DomTBLSeqScore(
+                e_value=float(x[6]), score=float(x[7]), bias=float(x[8])
+            )
+            domain = DomTBLDomScore(
+                id=int(x[9]),
+                size=int(x[10]),
+                c_value=float(x[11]),
+                i_value=float(x[12]),
+                score=float(x[13]),
+                bias=float(x[14]),
+            )
             row = DomTBLRow(
                 target=DomTBLIndex(name=x[0], accession=x[1], length=int(x[2])),
                 query=DomTBLIndex(name=x[3], accession=x[4], length=int(x[5])),
-                full_sequence=DomTBLSeqScore(e_value=x[6], score=x[7], bias=x[8]),
-                domain=DomTBLDomScore(
-                    id=int(x[9]),
-                    size=int(x[10]),
-                    c_value=x[11],
-                    i_value=x[12],
-                    score=x[13],
-                    bias=x[14],
-                ),
+                full_sequence=seq_score,
+                domain=domain,
                 hmm_coord=DomTBLCoord(start=int(x[15]), stop=int(x[16])),
                 ali_coord=DomTBLCoord(start=int(x[17]), stop=int(x[18])),
                 env_coord=DomTBLCoord(start=int(x[19]), stop=int(x[20])),
-                acc=x[21],
+                acc=float(x[21]),
                 description=" ".join(x[22:]),
             )
             rows.append(row)
     return rows
```

### Comparing `hmmer_tables-0.1.0/hmmer_tables/interval.py` & `hmmer_tables-0.1.1/hmmer_tables/interval.py`

 * *Files identical despite different names*

### Comparing `hmmer_tables-0.1.0/PKG-INFO` & `hmmer_tables-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmer-tables
-Version: 0.1.0
+Version: 0.1.1
 Summary: Read tables produced by HMMER software.
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

