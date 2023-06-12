# Comparing `tmp/mlopspython-extraction-74126878396677081493445.tar.gz` & `tmp/mlopspython-extraction-84376237332458489677065070.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlopspython-extraction-74126878396677081493445.tar", last modified: Fri Apr  7 20:15:49 2023, max compression
+gzip compressed data, was "mlopspython-extraction-84376237332458489677065070.tar", last modified: Mon Jun 12 16:05:27 2023, max compression
```

## Comparing `mlopspython-extraction-74126878396677081493445.tar` & `mlopspython-extraction-84376237332458489677065070.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-07 20:15:24.000000 mlopspython-extraction-74126878396677081493445/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:24.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-07 20:15:24.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:15:49.885375 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 20:15:49.000000 mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:05:27.431306 mlopspython-extraction-84376237332458489677065070/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-12 16:05:27.431306 mlopspython-extraction-84376237332458489677065070/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:05:27.431306 mlopspython-extraction-84376237332458489677065070/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-12 16:05:08.000000 mlopspython-extraction-84376237332458489677065070/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:05:27.431306 mlopspython-extraction-84376237332458489677065070/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:05:27.431306 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:05:08.000000 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-12 16:05:08.000000 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:05:27.431306 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-12 16:05:27.000000 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 16:05:27.000000 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:05:27.000000 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 16:05:27.000000 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 16:05:27.000000 mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction.egg-info/top_level.txt
```

### Comparing `mlopspython-extraction-74126878396677081493445/setup.py` & `mlopspython-extraction-84376237332458489677065070/setup.py`

 * *Files identical despite different names*

### Comparing `mlopspython-extraction-74126878396677081493445/src/mlopspython_extraction/extraction.py` & `mlopspython-extraction-84376237332458489677065070/src/mlopspython_extraction/extraction.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 @dataclass
 class ImageResult:
     image_bytes_io: BytesIO
     index_page: int
     index_image: int
 
+
 def extract_images_stream(pdf_bytes) -> Iterable[ImageResult]:
     with fitz.open(stream=pdf_bytes, filetype="pdf") as document:
         number_pages = len(document) - 1
         for index_page in range(number_pages):
             images = document.get_page_images(index_page)
             for index_image, image in enumerate(images):
                 xref = image[0]
@@ -48,13 +49,7 @@
         for image_stream in extract_images_stream(pdf_bytes):
             filename = "{0}_page{1}_index{2}.png".format(pdf_path.stem, str(image_stream.index_page), str(image_stream.index_image))
             number_images_output = number_images_output + 1
             with open(Path(images_directory_path) / filename, "wb") as file_stream:
                 file_stream.write(image_stream.image_bytes_io.getbuffer())
 
     return ExtractImagesResult(number_files_input=len(pdfs), number_images_output=number_images_output)
-
-
-if __name__ == "__main__":
-    pdfs_directory_path = ".\\dataset-cats-dogs-others"
-    images_directory_path = ".\\extracted_images"
-    extract_images(pdfs_directory_path, images_directory_path)
```

