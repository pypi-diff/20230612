# Comparing `tmp/unstructured-0.7.3.tar.gz` & `tmp/unstructured-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.3.tar", last modified: Fri Jun  9 18:21:51 2023, max compression
+gzip compressed data, was "unstructured-0.7.4.tar", last modified: Mon Jun 12 18:57:23 2023, max compression
```

## Comparing `unstructured-0.7.3.tar` & `unstructured-0.7.4.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.852471 unstructured-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-09 18:21:39.000000 unstructured-0.7.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-09 18:21:39.000000 unstructured-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-09 18:21:51.852471 unstructured-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-09 18:21:39.000000 unstructured-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 18:21:39.000000 unstructured-0.7.3/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 18:21:51.856471 unstructured-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-09 18:21:39.000000 unstructured-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-09 18:21:39.000000 unstructured-0.7.3/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.836471 unstructured-0.7.3/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.840471 unstructured-0.7.3/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.840471 unstructured-0.7.3/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.840471 unstructured-0.7.3/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.848471 unstructured-0.7.3/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.852471 unstructured-0.7.3/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.852471 unstructured-0.7.3/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-09 18:21:39.000000 unstructured-0.7.3/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:21:51.832471 unstructured-0.7.3/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 18:21:51.000000 unstructured-0.7.3/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.223657 unstructured-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-12 18:57:12.000000 unstructured-0.7.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 18:57:12.000000 unstructured-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-12 18:57:23.223657 unstructured-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-12 18:57:12.000000 unstructured-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.199657 unstructured-0.7.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 18:57:23.223657 unstructured-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-12 18:57:12.000000 unstructured-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.199657 unstructured-0.7.4/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.207657 unstructured-0.7.4/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.207657 unstructured-0.7.4/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.207657 unstructured-0.7.4/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.211657 unstructured-0.7.4/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.211657 unstructured-0.7.4/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.211657 unstructured-0.7.4/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.215657 unstructured-0.7.4/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.219657 unstructured-0.7.4/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.223657 unstructured-0.7.4/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-12 18:57:23.000000 unstructured-0.7.4/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.3/LICENSE.md` & `unstructured-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/PKG-INFO` & `unstructured-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.3
+Version: 0.7.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.3 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.4 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.7.3/README.md` & `unstructured-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/setup.py` & `unstructured-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.4/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.4/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/test_unstructured/test_utils.py` & `unstructured-0.7.4/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/cleaners/core.py` & `unstructured-0.7.4/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/cleaners/extract.py` & `unstructured-0.7.4/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/cleaners/translate.py` & `unstructured-0.7.4/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/documents/base.py` & `unstructured-0.7.4/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/documents/elements.py` & `unstructured-0.7.4/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/documents/email_elements.py` & `unstructured-0.7.4/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/documents/html.py` & `unstructured-0.7.4/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/documents/xml.py` & `unstructured-0.7.4/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/file_utils/encoding.py` & `unstructured-0.7.4/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/file_utils/exploration.py` & `unstructured-0.7.4/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.4/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/file_utils/filetype.py` & `unstructured-0.7.4/unstructured/file_utils/filetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import os
 import re
 import zipfile
 from enum import Enum
 from functools import wraps
 from typing import IO, Callable, List, Optional
 
+import filetype as ft
+
 from unstructured.documents.elements import Element, PageBreak
 from unstructured.file_utils.encoding import detect_file_encoding
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import (
     _add_element_metadata,
     _remove_element_metadata,
     exactly_one,
@@ -46,14 +48,15 @@
     "docProps/core.xml",
     "ppt/presentation.xml",
 ]
 
 
 class FileType(Enum):
     UNK = 0
+    EMPTY = 1
 
     # MS Office Types
     DOC = 10
     DOCX = 11
     XLS = 12
     XLSX = 13
     PPT = 14
@@ -117,14 +120,15 @@
     "application/vnd.openxmlformats-officedocument.presentationml.presentation": FileType.PPTX,
     "application/vnd.ms-powerpoint": FileType.PPT,
     "application/xml": FileType.XML,
     "application/vnd.oasis.opendocument.text": FileType.ODT,
     "message/rfc822": FileType.EML,
     "application/x-ole-storage": FileType.MSG,
     "application/vnd.ms-outlook": FileType.MSG,
+    "inode/x-empty": FileType.EMPTY,
 }
 
 MIMETYPES_TO_EXCLUDE = [
     "text/x-markdown",
     "application/epub+zip",
     "text/x-csv",
     "application/csv",
@@ -192,51 +196,60 @@
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
     encoding: Optional[str] = "utf-8",
 ) -> Optional[FileType]:
     """Use libmagic to determine a file's type. Helps determine which partition brick
     to use for a given file. A return value of None indicates a non-supported file type.
     """
+    mime_type = None
     exactly_one(filename=filename, file=file)
 
+    # first check (content_type)
     if content_type:
         filetype = STR_TO_FILETYPE.get(content_type)
         if filetype:
             return filetype
 
+    # second check (filename/file_name/file)
+    # continue if successfully define mime_type
     if filename or file_filename:
         _filename = filename or file_filename or ""
         _, extension = os.path.splitext(_filename)
         extension = extension.lower()
         if os.path.isfile(_filename) and LIBMAGIC_AVAILABLE:
             mime_type = magic.from_file(
                 _resolve_symlink(filename or file_filename),
                 mime=True,
             )  # type: ignore
-        else:
-            return EXT_TO_FILETYPE.get(extension.lower(), FileType.UNK)
+        elif os.path.isfile(_filename):
+            mime_type = ft.guess_mime(filename)
+        if mime_type is None:
+            return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
     elif file is not None:
         extension = None
         # NOTE(robinson) - the python-magic docs recommend reading at least the first 2048 bytes
         # Increased to 4096 because otherwise .xlsx files get detected as a zip file
         # ref: https://github.com/ahupp/python-magic#usage
         if LIBMAGIC_AVAILABLE:
             mime_type = magic.from_buffer(file.read(4096), mime=True)
         else:
-            raise ImportError(
-                "libmagic is unavailable. "
-                "Filetype detection on file-like objects requires libmagic. "
-                "Please install libmagic and try again.",
+            mime_type = ft.guess_mime(file.read(4096))
+        if mime_type is None:
+            logger.warning(
+                "libmagic is unavailable but assists in filetype detection on file-like objects."
+                "Please consider installing libmagic for better results.",
             )
+            return EXT_TO_FILETYPE.get(extension, FileType.UNK)
+
     else:
         raise ValueError("No filename, file, nor file_filename were specified.")
 
     """Mime type special cases."""
-
+    # third check (mime_type)
     # NOTE(crag): for older versions of the OS libmagic package, such as is currently
     # installed on the Unstructured docker image, .json files resolve to "text/plain"
     # rather than "application/json". this corrects for that case.
     if mime_type == "text/plain" and extension == ".json":
         return FileType.JSON
 
     # NOTE(Crag): older magic lib does not differentiate between xls and doc
@@ -296,14 +309,17 @@
 
     elif _is_code_mime_type(mime_type):
         # NOTE(robinson) - we'll treat all code files as plain text for now.
         # we can update this logic and add filetypes for specific languages
         # later if needed.
         return FileType.TXT
 
+    elif mime_type.endswith("empty"):
+        return FileType.EMPTY
+
     # For everything else
     elif mime_type in STR_TO_FILETYPE:
         return STR_TO_FILETYPE[mime_type]
 
     logger.warning(
         f"The MIME type{f' of {filename!r}' if filename else ''} is {mime_type!r}. "
         "This file type is not currently supported in unstructured.",
```

### Comparing `unstructured-0.7.3/unstructured/file_utils/metadata.py` & `unstructured-0.7.4/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/azure.py` & `unstructured-0.7.4/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.4/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/discord.py` & `unstructured-0.7.4/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.4/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/git.py` & `unstructured-0.7.4/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/github.py` & `unstructured-0.7.4/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.4/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.4/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/local.py` & `unstructured-0.7.4/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.4/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/s3.py` & `unstructured-0.7.4/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/slack.py` & `unstructured-0.7.4/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.4/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.4/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/interfaces.py` & `unstructured-0.7.4/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/ingest/main.py` & `unstructured-0.7.4/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/nlp/english-words.txt` & `unstructured-0.7.4/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/nlp/english_words.py` & `unstructured-0.7.4/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/nlp/patterns.py` & `unstructured-0.7.4/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/nlp/tokenize.py` & `unstructured-0.7.4/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/__init__.py` & `unstructured-0.7.4/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/api.py` & `unstructured-0.7.4/unstructured/partition/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 
 def partition_via_api(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
-    strategy: str = "hi_res",
     api_url: str = "https://api.unstructured.io/general/v0/general",
     api_key: str = "",
+    **request_kwargs,
 ) -> List[Element]:
     """Partitions a document using the Unstructured REST API. This is equivalent to
     running the document through partition.
 
     See https://api.unstructured.io/general/docs for the hosted API documentation or
     https://github.com/Unstructured-IO/unstructured-api for instructions on how to run
     the API locally as a container.
@@ -34,72 +34,76 @@
         A string defining the target filename path.
     content_type
         A string defining the file content in MIME type
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     file_filename
         When file is not None, the filename (string) to store in element metadata. E.g. "foo.txt"
-    strategy
-        The strategy to use for partitioning the PDF. Uses a layout detection model if set
-        to 'hi_res', otherwise partition_pdf simply extracts the text from the document
-        and processes it.
     api_url
         The URL for the Unstructured API. Defaults to the hosted Unstructured API.
     api_key
         The API key to pass to the Unstructured API.
+    request_kwargs
+        Additional parameters to pass to the data field of the request to the Unstructured API.
+        For example the `strategy` parameter.
     """
     exactly_one(filename=filename, file=file)
 
     headers = {
         "ACCEPT": "application/json",
         "UNSTRUCTURED-API-KEY": api_key,
     }
 
-    data = {
-        "strategy": strategy,
-    }
+    # set default values for kwargs
+    strategy = request_kwargs.pop("strategy", "hi_res")
+    request_kwargs["strategy"] = strategy
 
     if filename is not None:
         with open(filename, "rb") as f:
             files = [
                 ("files", (filename, f, content_type)),
             ]
             response = requests.post(
                 api_url,
                 headers=headers,
-                data=data,
+                data=request_kwargs,
                 files=files,  # type: ignore
             )
     elif file is not None:
         if file_filename is None:
             raise ValueError(
                 "If file is specified in partition_via_api, "
                 "file_filename must be specified as well.",
             )
         files = [
             ("files", (file_filename, file, content_type)),  # type: ignore
         ]
-        response = requests.post(api_url, headers=headers, data=data, files=files)  # type: ignore
+        response = requests.post(
+            api_url,
+            headers=headers,
+            data=request_kwargs,
+            files=files,  # type: ignore
+        )
 
     if response.status_code == 200:
         return elements_from_json(text=response.text)
     else:
         raise ValueError(
             f"Receive unexpected status code {response.status_code} from the API.",
         )
 
 
 def partition_multiple_via_api(
     filenames: Optional[List[str]] = None,
     content_types: Optional[List[str]] = None,
     files: Optional[List[str]] = None,
     file_filenames: Optional[List[str]] = None,
-    strategy: str = "hi_res",
     api_url: str = "https://api.unstructured.io/general/v0/general",
     api_key: str = "",
+    **request_kwargs,
 ) -> List[List[Element]]:
     """Partitions multiple document using the Unstructured REST API by batching
     the documents into a single HTTP request.
 
     See https://api.unstructured.io/general/docs for the hosted API documentation or
     https://github.com/Unstructured-IO/unstructured-api for instructions on how to run
     the API locally as a container.
@@ -118,23 +122,26 @@
         The strategy to use for partitioning the PDF. Uses a layout detection model if set
         to 'hi_res', otherwise partition_pdf simply extracts the text from the document
         and processes it.
     api_url
         The URL for the Unstructured API. Defaults to the hosted Unstructured API.
     api_key
         The API key to pass to the Unstructured API.
+    request_kwargs
+        Additional parameters to pass to the data field of the request to the Unstructured API.
+        For example the `strategy` parameter.
     """
     headers = {
         "ACCEPT": "application/json",
         "UNSTRUCTURED-API-KEY": api_key,
     }
 
-    data = {
-        "strategy": strategy,
-    }
+    # set default values for kwargs
+    strategy = request_kwargs.pop("strategy", "hi_res")
+    request_kwargs["strategy"] = strategy
 
     if filenames is not None:
         if content_types and len(content_types) != len(filenames):
             raise ValueError("content_types and filenames must have the same length.")
 
         with contextlib.ExitStack() as stack:
             files = [stack.enter_context(open(f, "rb")) for f in filenames]  # type: ignore
@@ -144,15 +151,15 @@
                 filename = filenames[i]
                 content_type = content_types[i] if content_types is not None else None
                 _files.append(("files", (filename, file, content_type)))
 
             response = requests.post(
                 api_url,
                 headers=headers,
-                data=data,
+                data=request_kwargs,
                 files=_files,  # type: ignore
             )
 
     elif files is not None:
         if content_types and len(content_types) != len(files):
             raise ValueError("content_types and files must have the same length.")
 
@@ -163,15 +170,20 @@
 
         _files = []
         for i, _file in enumerate(files):  # type: ignore
             content_type = content_types[i] if content_types is not None else None
             filename = file_filenames[i]
             _files.append(("files", (filename, _file, content_type)))
 
-        response = requests.post(api_url, headers=headers, data=data, files=_files)  # type: ignore
+        response = requests.post(
+            api_url,
+            headers=headers,
+            data=request_kwargs,
+            files=_files,  # type: ignore
+        )
 
     if response.status_code == 200:
         documents = []
         response_list = response.json()
         # NOTE(robinson) - this check is because if only one filename is passed, the return
         # type from the API is a list of objects instead of a list of lists
         if not isinstance(response_list[0], list):
```

### Comparing `unstructured-0.7.3/unstructured/partition/auto.py` & `unstructured-0.7.4/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,16 @@
         )
     elif filetype == FileType.JSON:
         elements = partition_json(filename=filename, file=file)
     elif (filetype == FileType.XLSX) or (filetype == FileType.XLS):
         elements = partition_xlsx(filename=filename, file=file)
     elif filetype == FileType.CSV:
         elements = partition_csv(filename=filename, file=file)
+    elif filetype == FileType.EMPTY:
+        elements = []
     else:
         msg = "Invalid file" if not filename else f"Invalid file {filename}"
         raise ValueError(f"{msg}. The {filetype} file type is not supported in partition.")
 
     for element in elements:
         element.metadata.url = url
         element.metadata.data_source = data_source_metadata
```

### Comparing `unstructured-0.7.3/unstructured/partition/common.py` & `unstructured-0.7.4/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/csv.py` & `unstructured-0.7.4/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/doc.py` & `unstructured-0.7.4/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/docx.py` & `unstructured-0.7.4/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/email.py` & `unstructured-0.7.4/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/epub.py` & `unstructured-0.7.4/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/html.py` & `unstructured-0.7.4/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/image.py` & `unstructured-0.7.4/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/json.py` & `unstructured-0.7.4/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/md.py` & `unstructured-0.7.4/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/msg.py` & `unstructured-0.7.4/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/odt.py` & `unstructured-0.7.4/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/pdf.py` & `unstructured-0.7.4/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/ppt.py` & `unstructured-0.7.4/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/pptx.py` & `unstructured-0.7.4/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/rtf.py` & `unstructured-0.7.4/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/strategies.py` & `unstructured-0.7.4/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/text.py` & `unstructured-0.7.4/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/text_type.py` & `unstructured-0.7.4/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/xlsx.py` & `unstructured-0.7.4/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/partition/xml.py` & `unstructured-0.7.4/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/argilla.py` & `unstructured-0.7.4/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/base.py` & `unstructured-0.7.4/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/baseplate.py` & `unstructured-0.7.4/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/datasaur.py` & `unstructured-0.7.4/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/huggingface.py` & `unstructured-0.7.4/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/label_box.py` & `unstructured-0.7.4/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/label_studio.py` & `unstructured-0.7.4/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/prodigy.py` & `unstructured-0.7.4/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/staging/weaviate.py` & `unstructured-0.7.4/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured/utils.py` & `unstructured-0.7.4/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.3/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.4/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.3
+Version: 0.7.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.3 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.4 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.7.3/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.4/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

