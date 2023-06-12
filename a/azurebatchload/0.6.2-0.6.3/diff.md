# Comparing `tmp/azurebatchload-0.6.2.tar.gz` & `tmp/azurebatchload-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azurebatchload-0.6.2.tar", last modified: Thu Jul 21 06:43:40 2022, max compression
+gzip compressed data, was "azurebatchload-0.6.3.tar", last modified: Mon Jun 12 07:56:07 2023, max compression
```

## Comparing `azurebatchload-0.6.2.tar` & `azurebatchload-0.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 06:43:40.963264 azurebatchload-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6649 2022-07-21 06:43:40.963264 azurebatchload-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5965 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 06:43:40.963264 azurebatchload-0.6.2/azurebatchload/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/azurebatchload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/azurebatchload/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/azurebatchload/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/azurebatchload/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     3515 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/azurebatchload/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/azurebatchload/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 06:43:40.963264 azurebatchload-0.6.2/azurebatchload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6649 2022-07-21 06:43:40.000000 azurebatchload-0.6.2/azurebatchload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-07-21 06:43:40.000000 azurebatchload-0.6.2/azurebatchload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 06:43:40.000000 azurebatchload-0.6.2/azurebatchload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-21 06:43:40.000000 azurebatchload-0.6.2/azurebatchload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-21 06:43:40.000000 azurebatchload-0.6.2/azurebatchload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-07-21 06:43:23.000000 azurebatchload-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-07-21 06:43:40.963264 azurebatchload-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:56:07.479307 azurebatchload-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-12 07:56:07.479307 azurebatchload-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:56:07.479307 azurebatchload-0.6.3/azurebatchload/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/azurebatchload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/azurebatchload/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/azurebatchload/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/azurebatchload/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/azurebatchload/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/azurebatchload/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:56:07.479307 azurebatchload-0.6.3/azurebatchload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-12 07:56:07.000000 azurebatchload-0.6.3/azurebatchload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-12 07:56:07.000000 azurebatchload-0.6.3/azurebatchload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:56:07.000000 azurebatchload-0.6.3/azurebatchload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 07:56:07.000000 azurebatchload-0.6.3/azurebatchload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 07:56:07.000000 azurebatchload-0.6.3/azurebatchload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 07:55:48.000000 azurebatchload-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-12 07:56:07.483307 azurebatchload-0.6.3/setup.cfg
```

### Comparing `azurebatchload-0.6.2/LICENSE` & `azurebatchload-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `azurebatchload-0.6.2/PKG-INFO` & `azurebatchload-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurebatchload
-Version: 0.6.2
+Version: 0.6.3
 Summary: Download and upload files in batches from Azure Blob Storage Containers
 Home-page: https://github.com/zypp-io/azure-batch-load
 Author: Erfan Nariman, Melvin Folkers
 Author-email: hello@zypp.io
 Project-URL: Bug Tracker, https://github.com/zypp-io/azure-batch-load/issues
 Project-URL: Source, https://github.com/zypp-io/azure-batch-load
 Keywords: python,azure,blob,download,upload,batch
```

### Comparing `azurebatchload-0.6.2/README.md` & `azurebatchload-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `azurebatchload-0.6.2/azurebatchload/checks.py` & `azurebatchload-0.6.3/azurebatchload/checks.py`

 * *Files identical despite different names*

### Comparing `azurebatchload-0.6.2/azurebatchload/core.py` & `azurebatchload-0.6.3/azurebatchload/core.py`

 * *Files identical despite different names*

### Comparing `azurebatchload-0.6.2/azurebatchload/download.py` & `azurebatchload-0.6.3/azurebatchload/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
                 download_file.write(blob_client.download_blob().readall())
 
             n_files += 1
 
         logging.info(f"Downloaded total of {n_files} files")
 
     def download(self):
-
         # for batch load we use the Azure CLI
         if self.method == "batch":
             self._download_batch()
 
         # for single load we use Python SDK
         else:
             self._download_single()
```

### Comparing `azurebatchload-0.6.2/azurebatchload/upload.py` & `azurebatchload-0.6.3/azurebatchload/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
     def upload_single(self):
         blob_service_client = BlobServiceClient.from_connection_string(self.connection_string)
         download_links = {}
 
         for root, dirs, files in os.walk(self.folder):
             for file in files:
-
                 full_path = os.path.join(root, file)
 
                 # ignore hidden files
                 if file.startswith("."):
                     continue
 
                 # if list_files is given, only upload matched files
```

### Comparing `azurebatchload-0.6.2/azurebatchload/utils.py` & `azurebatchload-0.6.3/azurebatchload/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         return files
 
     @staticmethod
     def _get_file_names_simple(files):
         return [file.get("name") for file in files]
 
     def _list_blobs_not_extended(self, files):
-
         file_names = self._get_file_names_simple(files)
         # 1. dataframe = False, return just a list of file names
         if not self.dataframe:
             return file_names
         # 2. dataframe = True, dataframe with one column filenames
         else:
             return DataFrame({"filename": file_names})
```

### Comparing `azurebatchload-0.6.2/azurebatchload.egg-info/PKG-INFO` & `azurebatchload-0.6.3/azurebatchload.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azurebatchload
-Version: 0.6.2
+Version: 0.6.3
 Summary: Download and upload files in batches from Azure Blob Storage Containers
 Home-page: https://github.com/zypp-io/azure-batch-load
 Author: Erfan Nariman, Melvin Folkers
 Author-email: hello@zypp.io
 Project-URL: Bug Tracker, https://github.com/zypp-io/azure-batch-load/issues
 Project-URL: Source, https://github.com/zypp-io/azure-batch-load
 Keywords: python,azure,blob,download,upload,batch
```

### Comparing `azurebatchload-0.6.2/setup.cfg` & `azurebatchload-0.6.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = azurebatchload
-version = 0.6.2
+version = 0.6.3
 author = Erfan Nariman, Melvin Folkers
 author_email = hello@zypp.io
 description = Download and upload files in batches from Azure Blob Storage Containers
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = python, azure, blob, download, upload, batch
 url = https://github.com/zypp-io/azure-batch-load
@@ -16,16 +16,16 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = azurebatchload
 python_requires = >=3.7
 install_requires = 
-	azure-storage-blob~=12.8.1
-	pandas~=1.4.1
+	azure-storage-blob>=12.8.1
+	pandas>=1.4.1
 
 [flake8]
 statistics = True
 count = True
 max-complexity = 12
 max-line-length = 120
 per-file-ignores = __init__.py: F401
```

