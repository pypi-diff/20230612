# Comparing `tmp/bloboluni-2.0.0.tar.gz` & `tmp/bloboluni-2.0.1.tar.gz`

## Comparing `bloboluni-2.0.0.tar` & `bloboluni-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloboluni-2.0.0/GitVersion.yml
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 bloboluni-2.0.0/test.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 bloboluni-2.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 bloboluni-2.0.0/bloboluni/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-2.0.0/bloboluni/serializers.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 bloboluni-2.0.0/bloboluni/storage.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-2.0.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-2.0.0/LICENSE
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 bloboluni-2.0.0/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bloboluni-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 bloboluni-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloboluni-2.0.1/GitVersion.yml
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 bloboluni-2.0.1/test.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 bloboluni-2.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 bloboluni-2.0.1/bloboluni/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloboluni-2.0.1/bloboluni/serializers.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 bloboluni-2.0.1/bloboluni/storage.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 bloboluni-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 bloboluni-2.0.1/LICENSE
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 bloboluni-2.0.1/README.md
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 bloboluni-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 bloboluni-2.0.1/PKG-INFO
```

### Comparing `bloboluni-2.0.0/test.py` & `bloboluni-2.0.1/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     def amethod(self):
         return "A method"
 
 if __name__ == "__main__":
     data = MyClass("blob", 30, MyProfession("Developer", "A developer"))
 
     connectionstring = os.environ["AZURE_STORAGE_CONNECTION_STRING"]
+    print(connectionstring)
     storage = BlobStorage(connectionstring, "mycontainer")
     
     key = uuid.uuid4().hex
     blob = storage.get(key)
     assert blob is None
     storage.upsert(key, data)
     blob = storage.get(key)
```

### Comparing `bloboluni-2.0.0/.github/workflows/python-publish.yml` & `bloboluni-2.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bloboluni-2.0.0/bloboluni/serializers.py` & `bloboluni-2.0.1/bloboluni/serializers.py`

 * *Files identical despite different names*

### Comparing `bloboluni-2.0.0/bloboluni/storage.py` & `bloboluni-2.0.1/bloboluni/storage.py`

 * *Files identical despite different names*

### Comparing `bloboluni-2.0.0/.gitignore` & `bloboluni-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bloboluni-2.0.0/LICENSE` & `bloboluni-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bloboluni-2.0.0/README.md` & `bloboluni-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bloboluni-2.0.0/pyproject.toml` & `bloboluni-2.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bloboluni"
-version = "2.0.0"
+version = "2.0.1"
 description = "A simple package for storing and retrieving blobs of data from Azure Blob Storage"
 authors = [
   { name = "Martin Moan", email = "martin.moan1@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 dependencies = [
   "requests>2",
   "python-dotenv>=1",
   "azure-storage-blob>=1",
   "azure-identity>=1",
+  "jsonpickle>=3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/MartinMoan/blobstorage"
 "Bug Tracker" = "https://github.com/MartinMoan/blobstorage/issues"
```

### Comparing `bloboluni-2.0.0/PKG-INFO` & `bloboluni-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloboluni
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple package for storing and retrieving blobs of data from Azure Blob Storage
 Project-URL: Homepage, https://github.com/MartinMoan/blobstorage
 Project-URL: Bug Tracker, https://github.com/MartinMoan/blobstorage/issues
 Author-email: Martin Moan <martin.moan1@gmail.com>
 License: Copyright (c) 2023 Martin Hoff Moan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,17 +24,18 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Requires-Dist: azure-identity>=1
 Requires-Dist: azure-storage-blob>=1
+Requires-Dist: jsonpickle>=3
 Requires-Dist: python-dotenv>=1
 Requires-Dist: requests>2
 Description-Content-Type: text/markdown
 
 # bloboluni: Azure blob storage wrapper
 `bloboluni` is a simple python module for interacting with Azure blob storage.
```

