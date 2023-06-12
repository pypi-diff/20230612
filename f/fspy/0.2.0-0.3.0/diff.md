# Comparing `tmp/fspy-0.2.0-py2.py3-none-any.whl.zip` & `tmp/fspy-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 29947 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      202 b- defN 23-Jun-11 16:35 fspy/__init__.py
+Zip file size: 29860 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       33 b- defN 23-Jun-12 11:01 fspy/__init__.py
 -rw-rw-r--  2.0 unx     2067 b- defN 23-Jun-11 16:35 fspy/response_models.py
 -rw-rw-r--  2.0 unx     9604 b- defN 23-Jun-12 10:39 fspy/solver.py
 -rw-rw-r--  2.0 unx      441 b- defN 23-Jun-11 16:35 fspy/solver_exceptions.py
--rw-rw-r--  2.0 unx    35128 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    42723 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      677 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/RECORD
-9 files, 90957 bytes uncompressed, 28797 bytes compressed:  68.3%
+-rw-rw-r--  2.0 unx    35128 b- defN 23-Jun-12 11:03 fspy-0.3.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    42723 b- defN 23-Jun-12 11:03 fspy-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 11:03 fspy-0.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-12 11:03 fspy-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-12 11:03 fspy-0.3.0.dist-info/RECORD
+9 files, 90787 bytes uncompressed, 28710 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fspy/solver.py
 Comment: 
 
 Filename: fspy/solver_exceptions.py
 Comment: 
 
-Filename: fspy-0.2.0.dist-info/LICENSE
+Filename: fspy-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fspy-0.2.0.dist-info/METADATA
+Filename: fspy-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fspy-0.2.0.dist-info/WHEEL
+Filename: fspy-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fspy-0.2.0.dist-info/top_level.txt
+Filename: fspy-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fspy-0.2.0.dist-info/RECORD
+Filename: fspy-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fspy/__init__.py

```diff
@@ -1,3 +1 @@
 from .solver import FlareSolverr
-from response_models import FlareSolverOK, SessionsListResponse, SesssionCreateResponse, Solution, GetPostRequestResponse
-from solver_exceptions import FlareSolverError
```

## Comparing `fspy-0.2.0.dist-info/LICENSE` & `fspy-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fspy-0.2.0.dist-info/METADATA` & `fspy-0.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fspy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A FlareSolverr wrapper for Python.
 Author: NandeMD
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

## Comparing `fspy-0.2.0.dist-info/RECORD` & `fspy-0.3.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-fspy/__init__.py,sha256=sCMqKfzICfxVyMhd1jaq6Ymh1bBp1qgwJuMCJkupMXs,202
+fspy/__init__.py,sha256=k8lV1pMolDm8RyQ6zQawW4JNb0G42bxEq0nZHZxl5vM,33
 fspy/response_models.py,sha256=UnjQBBKZUXdpUFXy4kiOtF6LWs_yMgxwhkdT6qoKtoc,2067
 fspy/solver.py,sha256=_YuJWJs3gZEdAJMRQHtWpLFWVBKPv1QyjmGtBub3I40,9604
 fspy/solver_exceptions.py,sha256=swvJMAe-FhA4jWHfjFwa5X3-WNncXnmWamQYlcPS-_8,441
-fspy-0.2.0.dist-info/LICENSE,sha256=N0P3pKtRMvfb64jmgJdlerg3TnS0a2QC776AzPsbZIg,35128
-fspy-0.2.0.dist-info/METADATA,sha256=4BnFvT7CGJKuOiOsSQLXGkZy5rt15OUbWWQYz5uPTaU,42723
-fspy-0.2.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-fspy-0.2.0.dist-info/top_level.txt,sha256=Dob_Di7XjCRx78eckkRUpwVVhopDqUIvkxZmLwUaiUk,5
-fspy-0.2.0.dist-info/RECORD,,
+fspy-0.3.0.dist-info/LICENSE,sha256=N0P3pKtRMvfb64jmgJdlerg3TnS0a2QC776AzPsbZIg,35128
+fspy-0.3.0.dist-info/METADATA,sha256=WjvMZVrj2HoXaRTcALVvnyWChJTlonHNkdkhyNw5CZA,42723
+fspy-0.3.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+fspy-0.3.0.dist-info/top_level.txt,sha256=Dob_Di7XjCRx78eckkRUpwVVhopDqUIvkxZmLwUaiUk,5
+fspy-0.3.0.dist-info/RECORD,,
```

