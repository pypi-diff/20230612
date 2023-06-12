# Comparing `tmp/bcvcontext-0.1.6.tar.gz` & `tmp/bcvcontext-0.1.7.tar.gz`

## Comparing `bcvcontext-0.1.6.tar` & `bcvcontext-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/src/bcvContext/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/src/bcvContext/bcvContext.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/README.md
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/src/bcvContext/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/src/bcvContext/bcvContext.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/README.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.7/PKG-INFO
```

### Comparing `bcvcontext-0.1.6/src/bcvContext/bcvContext.py` & `bcvcontext-0.1.7/src/bcvContext/bcvContext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import json
 from subprocess import call
 
 notarizationPath = ""
-isAudit = 1
+isToCache = 1
 
-def init(_notarizationPath, _isAudit) :
-    global notarizationPath, isAudit
+def init(_notarizationPath, _isToCache) :
+    global notarizationPath, isToCache
     notarizationPath = _notarizationPath
-    isAudit = _isAudit
+    isToCache = _isToCache
 
-def scriptContext(filename) :
-    return filename
+def scriptContext(_filename) :
+    return _filename
 
 def notarizationContextRawfile():
     return "../.." + notarizationPath + "/../rawFile.csv"
 
-def notarizationContext(filename) :
-    return "../.." + notarizationPath + "/" + filename
+def notarizationContext(_filename) :
+    return "../.." + notarizationPath + "/" + _filename
 
 def dayContext(_m, _filename) :
     if (_m >= 0) : raise Exception("No history at J", str(_m))
     day = json.load(open("../.." + notarizationPath + "/.config.json"))["day"] + _m
     if (day < 0) : raise Exception("No history at J", str(day))
     lastNotarization = json.load(open("../.." + notarizationPath + "/../../Day" + str(day) + "/.dayConfig.json"))["lastNotarization"]
     return "../.." + notarizationPath + "/../../Day" + str(day) + "/Notarization" + str(lastNotarization) + "/" + _filename
 
 def finish(*args) :
     call(["rm", "-r","../__cache__"])
-    if isAudit == 1 :
+    if isToCache == 1 :
         call(["mkdir","../__cache__"])
         for i in args :
             call(["mv",str(i),"../__cache__"])
         print("Final result at :", "../__cache__")
 
     else : 
         for i in args :
```

### Comparing `bcvcontext-0.1.6/.gitignore` & `bcvcontext-0.1.7/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
+__cache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
```

### Comparing `bcvcontext-0.1.6/LICENSE` & `bcvcontext-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.6/PKG-INFO` & `bcvcontext-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcvContext
-Version: 0.1.6
+Version: 0.1.7
 Summary: A small package to handle context path for the BCV generic workflow
 Author-email: CEA <thomas.marques@cea.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

