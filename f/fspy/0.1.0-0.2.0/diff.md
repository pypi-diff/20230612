# Comparing `tmp/fspy-0.1.0-py2.py3-none-any.whl.zip` & `tmp/fspy-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 29778 bytes, number of entries: 9
+Zip file size: 29947 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      202 b- defN 23-Jun-11 16:35 fspy/__init__.py
 -rw-rw-r--  2.0 unx     2067 b- defN 23-Jun-11 16:35 fspy/response_models.py
--rw-rw-r--  2.0 unx     8996 b- defN 23-Jun-11 16:35 fspy/solver.py
+-rw-rw-r--  2.0 unx     9604 b- defN 23-Jun-12 10:39 fspy/solver.py
 -rw-rw-r--  2.0 unx      441 b- defN 23-Jun-11 16:35 fspy/solver_exceptions.py
--rw-rw-r--  2.0 unx    35128 b- defN 23-Jun-11 16:47 fspy-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx    42736 b- defN 23-Jun-11 16:47 fspy-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-11 16:47 fspy-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-11 16:47 fspy-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      677 b- defN 23-Jun-11 16:47 fspy-0.1.0.dist-info/RECORD
-9 files, 90362 bytes uncompressed, 28628 bytes compressed:  68.3%
+-rw-rw-r--  2.0 unx    35128 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    42723 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      677 b- defN 23-Jun-12 10:53 fspy-0.2.0.dist-info/RECORD
+9 files, 90957 bytes uncompressed, 28797 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fspy/solver.py
 Comment: 
 
 Filename: fspy/solver_exceptions.py
 Comment: 
 
-Filename: fspy-0.1.0.dist-info/LICENSE
+Filename: fspy-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: fspy-0.1.0.dist-info/METADATA
+Filename: fspy-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: fspy-0.1.0.dist-info/WHEEL
+Filename: fspy-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: fspy-0.1.0.dist-info/top_level.txt
+Filename: fspy-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fspy-0.1.0.dist-info/RECORD
+Filename: fspy-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fspy/solver.py

```diff
@@ -18,14 +18,26 @@
             self,
             host: str = "127.0.0.1",
             port: Optional[Union[str, int]] = "8191",
             http_schema: Literal["http", "https"] = "http",
             additional_headers: dict = None,
             v: str = "v1"
     ) -> None:
+        """
+        :param host: Host address for FlareSolverr. Default: localhost.
+        :type host: str
+        :param port:  Host port for FlareSolverr. Defaul: 8191.
+        :type port: str | int
+        :param http_schema: Http schema for the requests module. Default: http
+        :type http_schema: Literal["http", "https"]
+        :param additional_headers: Additional headers you want to include while sending requests to FlareSolverr.
+        :type additional_headers: dict
+        :param v: FlareSolverr endpoint version. Do not change until strictly necessary.
+        :type v: str
+        """
         self.req_session = requests.Session()
         ah = additional_headers if additional_headers is not None else {}
         self.req_session.headers.update = {"Content-Type": "application/json", **ah}
 
         self.host = host
         self.port = str(port) if port is not None else None
         self.http_schema = http_schema
```

## Comparing `fspy-0.1.0.dist-info/LICENSE` & `fspy-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fspy-0.1.0.dist-info/METADATA` & `fspy-0.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fspy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A FlareSolverr wrapper for Python.
 Author: NandeMD
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,15 +676,15 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/NandeMD/FSPy
 Project-URL: Repository, https://github.com/NandeMD/FSPy
 Keywords: wrapper,flaresolverr
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

