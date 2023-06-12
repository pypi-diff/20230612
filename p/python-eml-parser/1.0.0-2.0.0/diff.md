# Comparing `tmp/python_eml_parser-1.0.0.tar.gz` & `tmp/python_eml_parser-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_eml_parser-1.0.0.tar", last modified: Sat Oct 30 22:01:16 2021, max compression
+gzip compressed data, was "python_eml_parser-2.0.0.tar", last modified: Mon Jun 12 10:25:19 2023, max compression
```

## Comparing `python_eml_parser-1.0.0.tar` & `python_eml_parser-2.0.0.tar`

### file list

```diff
@@ -1,59 +1,29 @@
-drwxr-xr-x   0 markrozeboom   (501) staff       (20)        0 2021-10-30 22:01:16.131589 python_eml_parser-1.0.0/
-drwxr-xr-x   0 markrozeboom   (501) staff       (20)        0 2021-10-30 22:01:15.914073 python_eml_parser-1.0.0/.github/
--rw-r--r--   0 markrozeboom   (501) staff       (20)      245 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/.github/pull_request_template.md
--rw-r--r--   0 markrozeboom   (501) staff       (20)       91 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/.gitignore
--rw-r--r--   0 markrozeboom   (501) staff       (20)      126 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1063 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/LICENSE
--rw-r--r--   0 markrozeboom   (501) staff       (20)      329 2021-10-30 22:01:14.000000 python_eml_parser-1.0.0/Makefile
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1898 2021-10-30 22:01:16.131252 python_eml_parser-1.0.0/PKG-INFO
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1312 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/README.md
-drwxr-xr-x   0 markrozeboom   (501) staff       (20)        0 2021-10-30 22:01:15.920877 python_eml_parser-1.0.0/eml_parser/
--rw-r--r--   0 markrozeboom   (501) staff       (20)        0 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/__init__.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)      561 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/email_cleaner.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)    13786 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/email_parser.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)      129 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/exceptions.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1677 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/helper.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)     5589 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/icon_email.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1340 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/icon_file.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1187 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/indicators.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)      611 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/eml_parser/microsoft_newline_cleaner.py
-drwxr-xr-x   0 markrozeboom   (501) staff       (20)        0 2021-10-30 22:01:15.923073 python_eml_parser-1.0.0/python_eml_parser.egg-info/
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1898 2021-10-30 22:01:15.000000 python_eml_parser-1.0.0/python_eml_parser.egg-info/PKG-INFO
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1879 2021-10-30 22:01:15.000000 python_eml_parser-1.0.0/python_eml_parser.egg-info/SOURCES.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)        1 2021-10-30 22:01:15.000000 python_eml_parser-1.0.0/python_eml_parser.egg-info/dependency_links.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)       57 2021-10-30 22:01:15.000000 python_eml_parser-1.0.0/python_eml_parser.egg-info/entry_points.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)       21 2021-10-30 22:01:15.000000 python_eml_parser-1.0.0/python_eml_parser.egg-info/top_level.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)       22 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/requirements.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)       38 2021-10-30 22:01:16.131669 python_eml_parser-1.0.0/setup.cfg
--rw-r--r--   0 markrozeboom   (501) staff       (20)      911 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/setup.py
-drwxr-xr-x   0 markrozeboom   (501) staff       (20)        0 2021-10-30 22:01:15.947615 python_eml_parser-1.0.0/unit_test/
--rw-r--r--   0 markrozeboom   (501) staff       (20)        0 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/__init__.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1266 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payload_cleaner.py
-drwxr-xr-x   0 markrozeboom   (501) staff       (20)        0 2021-10-30 22:01:16.129813 python_eml_parser-1.0.0/unit_test/payloads/
--rw-r--r--   0 markrozeboom   (501) staff       (20)    34675 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/2 level deep email attached.eml
--rw-r--r--   0 markrozeboom   (501) staff       (20)    12073 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/3_deep_with_text_attachment.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)    39679 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/API Security Survey (please take this important survey) .eml
--rw-r--r--   0 markrozeboom   (501) staff       (20)    34753 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/Grüße_von_Stefan_Appel.eml
--rw-r--r--   0 markrozeboom   (501) staff       (20)      394 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/basic_email.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)    11388 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/basic_email_attachment.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)    25616 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/double_attached_with_images.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)   933104 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/email_with_nested_attachments_python_object.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)    55116 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/encoded_ms_eml.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)   179783 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/evil_email.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)   257102 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/four_deep_with_pic.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)    22277 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_attachment_email_payload.json
--rw-r--r--   0 markrozeboom   (501) staff       (20)    22119 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_attachment_email_with_attachment_payload.json
--rw-r--r--   0 markrozeboom   (501) staff       (20)      951 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_attachments_file_payload.json
--rw-r--r--   0 markrozeboom   (501) staff       (20)     4872 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_folders_payload.json
--rw-r--r--   0 markrozeboom   (501) staff       (20)    15149 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_headers_payload.json
--rw-r--r--   0 markrozeboom   (501) staff       (20)    78372 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_messages_payload.json
--rw-r--r--   0 markrozeboom   (501) staff       (20)     3006 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_messages_payload_one_basic_message.json
--rw-r--r--   0 markrozeboom   (501) staff       (20)    23375 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_raw_attachment_test.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)    23264 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/get_raw_attachment_test_no_content_type.txt
--rw-r--r--   0 markrozeboom   (501) staff       (20)   199687 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/hash_crash.eml
--rw-r--r--   0 markrozeboom   (501) staff       (20)  1623445 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/lots_of_eml_attached.eml
--rw-r--r--   0 markrozeboom   (501) staff       (20)     5948 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/payloads/quoted_printable.eml
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1536 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/test_email_cleaner.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)    16944 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/test_email_parser.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)     8846 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/test_icon_email.py
--rw-r--r--   0 markrozeboom   (501) staff       (20)     1512 2021-10-30 18:35:22.000000 python_eml_parser-1.0.0/unit_test/test_icon_file.py
+drwxr-xr-x   0 ablakley   (503) staff       (20)        0 2023-06-12 10:25:19.066214 python_eml_parser-2.0.0/
+-rw-r--r--   0 ablakley   (503) staff       (20)     1063 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/LICENSE
+-rw-r--r--   0 ablakley   (503) staff       (20)     1985 2023-06-12 10:25:19.065774 python_eml_parser-2.0.0/PKG-INFO
+-rw-r--r--   0 ablakley   (503) staff       (20)     1419 2023-03-24 09:55:54.000000 python_eml_parser-2.0.0/README.md
+drwxr-xr-x   0 ablakley   (503) staff       (20)        0 2023-06-12 10:25:19.053143 python_eml_parser-2.0.0/eml_parser/
+-rw-r--r--   0 ablakley   (503) staff       (20)        0 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/eml_parser/__init__.py
+-rw-r--r--   0 ablakley   (503) staff       (20)      561 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/eml_parser/email_cleaner.py
+-rw-r--r--   0 ablakley   (503) staff       (20)    13855 2023-03-24 10:19:12.000000 python_eml_parser-2.0.0/eml_parser/email_parser.py
+-rw-r--r--   0 ablakley   (503) staff       (20)      129 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/eml_parser/exceptions.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     1677 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/eml_parser/helper.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     5584 2023-03-24 10:19:31.000000 python_eml_parser-2.0.0/eml_parser/icon_email.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     1450 2023-03-24 10:19:25.000000 python_eml_parser-2.0.0/eml_parser/icon_file.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     1369 2023-03-24 09:50:46.000000 python_eml_parser-2.0.0/eml_parser/indicators.py
+-rw-r--r--   0 ablakley   (503) staff       (20)      611 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/eml_parser/microsoft_newline_cleaner.py
+drwxr-xr-x   0 ablakley   (503) staff       (20)        0 2023-06-12 10:25:19.058175 python_eml_parser-2.0.0/python_eml_parser.egg-info/
+-rw-r--r--   0 ablakley   (503) staff       (20)     1985 2023-06-12 10:25:19.000000 python_eml_parser-2.0.0/python_eml_parser.egg-info/PKG-INFO
+-rw-r--r--   0 ablakley   (503) staff       (20)      643 2023-06-12 10:25:19.000000 python_eml_parser-2.0.0/python_eml_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 ablakley   (503) staff       (20)        1 2023-06-12 10:25:19.000000 python_eml_parser-2.0.0/python_eml_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 ablakley   (503) staff       (20)       56 2023-06-12 10:25:19.000000 python_eml_parser-2.0.0/python_eml_parser.egg-info/entry_points.txt
+-rw-r--r--   0 ablakley   (503) staff       (20)       21 2023-06-12 10:25:19.000000 python_eml_parser-2.0.0/python_eml_parser.egg-info/top_level.txt
+-rw-r--r--   0 ablakley   (503) staff       (20)       38 2023-06-12 10:25:19.066358 python_eml_parser-2.0.0/setup.cfg
+-rw-r--r--   0 ablakley   (503) staff       (20)      911 2023-03-24 09:55:54.000000 python_eml_parser-2.0.0/setup.py
+drwxr-xr-x   0 ablakley   (503) staff       (20)        0 2023-06-12 10:25:19.064530 python_eml_parser-2.0.0/unit_test/
+-rw-r--r--   0 ablakley   (503) staff       (20)        0 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/unit_test/__init__.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     1266 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/unit_test/payload_cleaner.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     1536 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/unit_test/test_email_cleaner.py
+-rw-r--r--   0 ablakley   (503) staff       (20)    16943 2023-03-28 09:58:59.000000 python_eml_parser-2.0.0/unit_test/test_email_parser.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     8846 2023-03-22 11:27:39.000000 python_eml_parser-2.0.0/unit_test/test_icon_email.py
+-rw-r--r--   0 ablakley   (503) staff       (20)     1511 2023-03-24 09:39:08.000000 python_eml_parser-2.0.0/unit_test/test_icon_file.py
```

### Comparing `python_eml_parser-1.0.0/LICENSE` & `python_eml_parser-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_eml_parser-1.0.0/PKG-INFO` & `python_eml_parser-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: python_eml_parser
-Version: 1.0.0
+Version: 2.0.0
 Summary: Rapid7 InsightConnect email parser for email plugins
 Home-page: https://github.com/rapid7/python-eml-parser
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -54,10 +53,9 @@
 and [pre-commit](https://pre-commit.com/) for handling code
 style. Simply follow the instructions for installing pre-commit and 
 run `pre-commit install` in the repository after cloning and you will
 be on your way to contributing!
 
 ## Changelog
 
+* 2.0.0 - MD5, SHA1, and SHA256 Indicators for Base64 Content are now hashes of the decoded Base64 Content
 * 1.0.0 - Initial release
-
-
```

### Comparing `python_eml_parser-1.0.0/README.md` & `python_eml_parser-2.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 and [pre-commit](https://pre-commit.com/) for handling code
 style. Simply follow the instructions for installing pre-commit and 
 run `pre-commit install` in the repository after cloning and you will
 be on your way to contributing!
 
 ## Changelog
 
+* 2.0.0 - MD5, SHA1, and SHA256 Indicators for Base64 Content are now hashes of the decoded Base64 Content
 * 1.0.0 - Initial release
```

### Comparing `python_eml_parser-1.0.0/eml_parser/email_cleaner.py` & `python_eml_parser-2.0.0/eml_parser/email_cleaner.py`

 * *Files identical despite different names*

### Comparing `python_eml_parser-1.0.0/eml_parser/email_parser.py` & `python_eml_parser-2.0.0/eml_parser/email_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,15 @@
             if content_transfer_encoding.lower() == "base64":
                 content = content.replace("\n", "")
 
             icon_file = IconFile(
                 file_name=filename,
                 content_type=part.get_content_type(),
                 content=content,
+                content_transfer_encoding=content_transfer_encoding,
             )
 
             #################
             #  Attached .eml
             #################
             icon_file.name = str(make_header(decode_header(icon_file.name)))
             if icon_file.name.endswith(".eml"):
```

### Comparing `python_eml_parser-1.0.0/eml_parser/helper.py` & `python_eml_parser-2.0.0/eml_parser/helper.py`

 * *Files identical despite different names*

### Comparing `python_eml_parser-1.0.0/eml_parser/icon_email.py` & `python_eml_parser-2.0.0/eml_parser/icon_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,28 +114,28 @@
 
         return ret_val
 
     # These functions are needed for equality and hashing. They
     # are used to remove duplicates in the flattened lists.
 
     def __eq__(self, other):
-        """ Check for equality """
+        """Check for equality"""
         return (
             self.id == other.id
             and self.subject == other.subject
             and self.body == other.body
             and self.date_received == other.date_received
             and self.recipients == other.recipients
             and self.sender == other.sender
             and self.account == other.account
             and self.categories == other.categories
         )
 
     def __hash__(self):
-        """ Return a unique hash """
+        """Return a unique hash"""
 
         # 'Tue, 13 Aug 2019 12:56:31 -0500'
         return hash(
             (
                 "id",
                 self.id,
                 "subject",
@@ -152,9 +152,9 @@
                 self.account,
                 "categories",
                 str(self.categories),
             )
         )
 
     def __lt__(self, other):
-        """ Less than, allows class to be sorted"""
+        """Less than, allows class to be sorted"""
         return self.subject < other.subject
```

### Comparing `python_eml_parser-1.0.0/eml_parser/icon_file.py` & `python_eml_parser-2.0.0/eml_parser/icon_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import json
 
 import eml_parser.helper as helper
 from eml_parser.indicators import Indicators
 
 
 class IconFile(object):
-    def __init__(self, file_name: str = "", content_type: str = "", content: str = ""):
+    def __init__(
+        self,
+        file_name: str = "",
+        content_type: str = "",
+        content: str = "",
+        content_transfer_encoding: str = "",
+    ):
         self.name = file_name
         self.content = content
         self.content_type = content_type
-        self.indicators = Indicators(content)
+        self.indicators = Indicators(content, content_transfer_encoding)
 
     # May not need this
     def make_serializable(self) -> dict:
         """Converts the File to a JSON-serializable, cleaned dict"""
         message_json = json.dumps(
             self, default=lambda o: o.__dict__, sort_keys=True, indent=4
         )
@@ -38,9 +44,9 @@
                 self.content,
                 "content_type",
                 self.content_type,
             )
         )
 
     def __lt__(self, other):
-        """ Less than, allows class to be sorted"""
+        """Less than, allows class to be sorted"""
         return self.name < other.name
```

### Comparing `python_eml_parser-1.0.0/eml_parser/microsoft_newline_cleaner.py` & `python_eml_parser-2.0.0/eml_parser/microsoft_newline_cleaner.py`

 * *Files identical despite different names*

### Comparing `python_eml_parser-1.0.0/python_eml_parser.egg-info/PKG-INFO` & `python_eml_parser-2.0.0/python_eml_parser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: python-eml-parser
-Version: 1.0.0
+Version: 2.0.0
 Summary: Rapid7 InsightConnect email parser for email plugins
 Home-page: https://github.com/rapid7/python-eml-parser
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -54,10 +53,9 @@
 and [pre-commit](https://pre-commit.com/) for handling code
 style. Simply follow the instructions for installing pre-commit and 
 run `pre-commit install` in the repository after cloning and you will
 be on your way to contributing!
 
 ## Changelog
 
+* 2.0.0 - MD5, SHA1, and SHA256 Indicators for Base64 Content are now hashes of the decoded Base64 Content
 * 1.0.0 - Initial release
-
-
```

### Comparing `python_eml_parser-1.0.0/setup.py` & `python_eml_parser-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="python_eml_parser",
-    version="1.0.0",
+    version="2.0.0",
     description="Rapid7 InsightConnect email parser for email plugins",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rapid7 Integrations Alliance",
     author_email="integrationalliance@rapid7.com",
     url="https://github.com/rapid7/python-eml-parser",
     packages=find_packages(),
```

### Comparing `python_eml_parser-1.0.0/unit_test/payload_cleaner.py` & `python_eml_parser-2.0.0/unit_test/payload_cleaner.py`

 * *Files identical despite different names*

### Comparing `python_eml_parser-1.0.0/unit_test/test_email_cleaner.py` & `python_eml_parser-2.0.0/unit_test/test_email_cleaner.py`

 * *Files identical despite different names*

### Comparing `python_eml_parser-1.0.0/unit_test/test_email_parser.py` & `python_eml_parser-2.0.0/unit_test/test_email_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from eml_parser.email_parser import EmailParser
 from unittest import TestCase
 import logging
 import os
 from email import message_from_string
-
 TEST_MAILBOX_ID = "somedude@hotmail.com"
 
 CURRENT_DIR = os.path.dirname(__file__)
 GET_RAW_ATTACHMENT_PAYLOAD = f"{CURRENT_DIR}/payloads/four_deep_with_pic.txt"
 GET_RAW_ATTACHMENT_PAYLOAD2 = f"{CURRENT_DIR}/payloads/get_raw_attachment_test.txt"
 GET_RAW_ATTACHMENT_PAYLOAD3 = f"{CURRENT_DIR}/payloads/3_deep_with_text_attachment.txt"
 GET_RAW_ATTACHMENT_PAYLOAD4 = f"{CURRENT_DIR}/payloads/basic_email_attachment.txt"
@@ -81,22 +80,22 @@
         self.assertEqual(attached_email_of_attached_email.subject, "Pic attached")
 
         attached_file = email.attached_files[0]
         self.assertEqual(attached_file.content[:5], "iVBOR")
         self.assertEqual(attached_file.content_type, "image/png")
         self.assertEqual(attached_file.name, "example.com")
         self.assertEqual(
-            attached_file.indicators.md5, "539cefc749ed1d78e3c821307f7c1b0a"
+            attached_file.indicators.md5, "4e6b332381785e918147874620c9a778"
         )
         self.assertEqual(
-            attached_file.indicators.sha1, "9a95c01f15c461708733dac2b3fbe10901801582"
+            attached_file.indicators.sha1, "843feb4b836778969c6370dc0a6afba409a09f34"
         )
         self.assertEqual(
             attached_file.indicators.sha256,
-            "ac92883cdc6cda0735f9c3f968e6103f8dd93f705cc077dce70924eda523a916",
+            "a8ed7fe07252c245e2cf3ae606f3051ea14e47840b5883f6bdc1cafd88bf4871",
         )
 
     def test_parse_from_raw2(self):
         raw_email = read_file_to_string(GET_RAW_ATTACHMENT_PAYLOAD2)
         email_parser = EmailParser(self.log)
         email = email_parser.make_email_from_raw(
             message_from_string(raw_email), TEST_MAILBOX_ID
@@ -156,21 +155,21 @@
         self.assertEqual(email.sender, "user@example.com")
 
         attachment = email.attached_files[0]
         self.assertEqual(attachment.content_type, "text/plain")
         expected_content = "VGhpcyBpcyBhIHRlc3QgYXR0YWNobWVudA0KDQpJdCBoYXMgc29tZSB0ZXh0IGluIGl0LiANCg0KYWFkcm9pZC5uZXQNCg=="
         self.assertEqual(attachment.content, expected_content)
         self.assertEqual(attachment.name, "test_example.com")
-        self.assertEqual(attachment.indicators.md5, "593aa3b46e3902094303b7ef1349d9ff")
+        self.assertEqual(attachment.indicators.md5, "17ee38189af19fa3c7047bdab0042cae")
         self.assertEqual(
-            attachment.indicators.sha1, "d1181c07e87d73803bf5786b37e8f03a176290a2"
+            attachment.indicators.sha1, "54df9bfd77f891c8181c1105bef9247c61d56e0a"
         )
         self.assertEqual(
             attachment.indicators.sha256,
-            "c08eb82e5383760cad3a4b4863dfb871b4c4252eba039c64a90ffc818907de27",
+            "a1485e471988b56478ca36c592638f225bb9c0f171e83148cfdd996ab099262c",
         )
 
     def test_parse_from_raw4(self):
         raw_email = read_file_to_string(GET_RAW_ATTACHMENT_PAYLOAD4)
         email_parser = EmailParser(self.log)
         email = email_parser.make_email_from_raw(
             message_from_string(raw_email), TEST_MAILBOX_ID
@@ -281,22 +280,22 @@
         email2 = email.attached_emails[1]
 
         self.assertTrue(email1.subject, "Pic and eml attached")
         self.assertTrue(email2.subject, "Test Email")
 
         attached_file = email.attached_files[0]
         self.assertEqual(
-            attached_file.indicators.md5, "2fca7949ad1004cefe685b81c3889e1c"
+            attached_file.indicators.md5, "7e7fbad36024562ff3e0f04b191463ad"
         )
         self.assertEqual(
-            attached_file.indicators.sha1, "b7e20bc9d4eb40adb1c4f103821bd461deab9d3f"
+            attached_file.indicators.sha1, "7e9c25b3bd8537d7dde9602633835137a2e4f1d0"
         )
         self.assertEqual(
             attached_file.indicators.sha256,
-            "8477aeb65fe7985cc82bc8f231ebfc519b8178d1050a9cee7f1b450e6c370240",
+            "f1c3e8c51308fdd82b6da7e7691f0fecf05a76cdafb014091ebe0aaab0b0cc47",
         )
 
     def test_single_recipient(self):
         email_parser = EmailParser(self.log)
         msg = {"To": "bob@hotmail.com"}
         rcpt = email_parser.get_recipients(msg)
         self.assertEqual(rcpt, ["bob@hotmail.com"])
```

### Comparing `python_eml_parser-1.0.0/unit_test/test_icon_email.py` & `python_eml_parser-2.0.0/unit_test/test_icon_email.py`

 * *Files identical despite different names*

### Comparing `python_eml_parser-1.0.0/unit_test/test_icon_file.py` & `python_eml_parser-2.0.0/unit_test/test_icon_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from eml_parser.icon_file import IconFile
 from unittest import TestCase
 
-
 # This class tests icon file
 class TestIconFile(TestCase):
     def setUp(self) -> None:
         pass
 
     def test_create_file(self):
         icon_file = IconFile(
```

