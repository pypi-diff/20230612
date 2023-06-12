# Comparing `tmp/joeynmt-2.1.0.tar.gz` & `tmp/joeynmt-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joeynmt-2.1.0.tar", last modified: Sun Sep 18 19:23:17 2022, max compression
+gzip compressed data, was "joeynmt-2.2.1.tar", last modified: Mon Jun 12 14:21:24 2023, max compression
```

## Comparing `joeynmt-2.1.0.tar` & `joeynmt-2.2.1.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2022-09-18 19:23:17.114644 joeynmt-2.1.0/
--rw-rw-r--   0 julia     (1000) julia     (1000)      465 2022-09-18 19:23:17.114644 joeynmt-2.1.0/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)    22100 2022-09-18 19:21:15.000000 joeynmt-2.1.0/README.md
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2022-09-18 19:23:17.110644 joeynmt-2.1.0/joeynmt/
--rw-r--r--   0 julia     (1000) julia     (1000)        0 2018-10-15 15:02:14.000000 joeynmt-2.1.0/joeynmt/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     1625 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/__main__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     7757 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/attention.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     6135 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/batch.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    16344 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/builders.py
--rw-rw-r--   0 julia     (1000) julia     (1000)      172 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/constants.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     5708 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/data.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    27341 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/datasets.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    23109 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/decoders.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4108 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/embeddings.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     8877 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/encoders.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    20822 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/helpers.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     8946 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/initialization.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3839 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/loss.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3454 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/metrics.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    12757 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/model.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2476 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/plotting.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    23527 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/prediction.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    35881 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/search.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    13834 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/tokenizers.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    34419 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/training.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    12651 2022-09-18 19:21:15.000000 joeynmt-2.1.0/joeynmt/transformer_layers.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     9306 2022-06-02 17:36:55.000000 joeynmt-2.1.0/joeynmt/vocabulary.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2022-09-18 19:23:17.110644 joeynmt-2.1.0/joeynmt.egg-info/
--rw-rw-r--   0 julia     (1000) julia     (1000)      465 2022-09-18 19:23:16.000000 joeynmt-2.1.0/joeynmt.egg-info/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)     1236 2022-09-18 19:23:17.000000 joeynmt-2.1.0/joeynmt.egg-info/SOURCES.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)        1 2022-09-18 19:23:16.000000 joeynmt-2.1.0/joeynmt.egg-info/dependency_links.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)       20 2022-09-18 19:23:16.000000 joeynmt-2.1.0/joeynmt.egg-info/entry_points.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      245 2022-09-18 19:23:16.000000 joeynmt-2.1.0/joeynmt.egg-info/requires.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)       13 2022-09-18 19:23:16.000000 joeynmt-2.1.0/joeynmt.egg-info/top_level.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      489 2022-09-18 19:23:17.114644 joeynmt-2.1.0/setup.cfg
--rwxrwxr-x   0 julia     (1000) julia     (1000)      777 2022-09-18 19:21:15.000000 joeynmt-2.1.0/setup.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2022-09-18 19:23:17.110644 joeynmt-2.1.0/test/
--rw-r--r--   0 julia     (1000) julia     (1000)        0 2019-04-29 07:53:48.000000 joeynmt-2.1.0/test/__init__.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2022-09-18 19:23:17.114644 joeynmt-2.1.0/test/unit/
--rw-r--r--   0 julia     (1000) julia     (1000)        0 2019-04-29 07:53:48.000000 joeynmt-2.1.0/test/unit/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    17391 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_attention.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     8354 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_batch.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2156 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_data.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    13312 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_dataset.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    11207 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_decoder.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2865 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_embeddings.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     5056 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_encoder.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3249 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_loss.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     1715 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_metric.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3438 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_model_init.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4538 2022-06-02 17:36:55.000000 joeynmt-2.1.0/test/unit/test_prediction.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    19131 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_search.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     7883 2022-06-02 17:36:55.000000 joeynmt-2.1.0/test/unit/test_tokenizer.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     7466 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_transformer_decoder.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4325 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_transformer_encoder.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     1753 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_transformer_utils.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     5939 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_vocabulary.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3770 2022-09-18 19:21:15.000000 joeynmt-2.1.0/test/unit/test_weight_tying.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2023-06-12 14:21:24.600653 joeynmt-2.2.1/
+-rw-rw-r--   0 julia     (1000) julia     (1000)      465 2023-06-12 14:21:24.600653 joeynmt-2.2.1/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)    22697 2023-06-12 14:20:54.000000 joeynmt-2.2.1/README.md
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2023-06-12 14:21:24.596653 joeynmt-2.2.1/joeynmt/
+-rw-r--r--   0 julia     (1000) julia     (1000)        0 2018-10-15 15:02:14.000000 joeynmt-2.2.1/joeynmt/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1759 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/__main__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     7757 2022-06-02 17:36:55.000000 joeynmt-2.2.1/joeynmt/attention.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     6192 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/batch.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    16872 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/builders.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)      172 2022-06-02 17:36:55.000000 joeynmt-2.2.1/joeynmt/constants.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     5708 2022-09-18 19:21:15.000000 joeynmt-2.2.1/joeynmt/data.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    28232 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/datasets.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    23402 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/decoders.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4108 2022-06-02 17:36:55.000000 joeynmt-2.2.1/joeynmt/embeddings.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     9036 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/encoders.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    21339 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/helpers.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     9454 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/hub_interface.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     8946 2022-09-18 19:21:15.000000 joeynmt-2.2.1/joeynmt/initialization.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3839 2022-06-02 17:36:55.000000 joeynmt-2.2.1/joeynmt/loss.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3454 2022-06-02 17:36:55.000000 joeynmt-2.2.1/joeynmt/metrics.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    12757 2022-09-18 19:21:15.000000 joeynmt-2.2.1/joeynmt/model.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2476 2022-06-02 17:36:55.000000 joeynmt-2.2.1/joeynmt/plotting.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    24225 2023-06-12 14:20:54.000000 joeynmt-2.2.1/joeynmt/prediction.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    35881 2022-09-18 19:21:15.000000 joeynmt-2.2.1/joeynmt/search.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    14086 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/tokenizers.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    34075 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/training.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    13169 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/transformer_layers.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/validation.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     9307 2023-06-05 15:59:10.000000 joeynmt-2.2.1/joeynmt/vocabulary.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2023-06-12 14:21:24.596653 joeynmt-2.2.1/joeynmt.egg-info/
+-rw-rw-r--   0 julia     (1000) julia     (1000)      465 2023-06-12 14:21:24.000000 joeynmt-2.2.1/joeynmt.egg-info/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1283 2023-06-12 14:21:24.000000 joeynmt-2.2.1/joeynmt.egg-info/SOURCES.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)        1 2023-06-12 14:21:24.000000 joeynmt-2.2.1/joeynmt.egg-info/dependency_links.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)       20 2023-06-12 14:21:24.000000 joeynmt-2.2.1/joeynmt.egg-info/entry_points.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      252 2023-06-12 14:21:24.000000 joeynmt-2.2.1/joeynmt.egg-info/requires.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)       13 2023-06-12 14:21:24.000000 joeynmt-2.2.1/joeynmt.egg-info/top_level.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      489 2023-06-12 14:21:24.600653 joeynmt-2.2.1/setup.cfg
+-rwxrwxr-x   0 julia     (1000) julia     (1000)      777 2023-06-12 14:20:54.000000 joeynmt-2.2.1/setup.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2023-06-12 14:21:24.596653 joeynmt-2.2.1/test/
+-rw-r--r--   0 julia     (1000) julia     (1000)        0 2019-04-29 07:53:48.000000 joeynmt-2.2.1/test/__init__.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2023-06-12 14:21:24.600653 joeynmt-2.2.1/test/unit/
+-rw-r--r--   0 julia     (1000) julia     (1000)        0 2019-04-29 07:53:48.000000 joeynmt-2.2.1/test/unit/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    17391 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_attention.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     8354 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_batch.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2156 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_data.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    13312 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_dataset.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    11207 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_decoder.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2865 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_embeddings.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     5056 2023-06-05 15:59:11.000000 joeynmt-2.2.1/test/unit/test_encoder.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3249 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_loss.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1715 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_metric.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3437 2023-06-05 15:59:11.000000 joeynmt-2.2.1/test/unit/test_model_init.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4538 2022-06-02 17:36:55.000000 joeynmt-2.2.1/test/unit/test_prediction.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    19131 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_search.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     7943 2023-06-05 15:59:11.000000 joeynmt-2.2.1/test/unit/test_tokenizer.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     7466 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_transformer_decoder.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4325 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_transformer_encoder.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1753 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_transformer_utils.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     5939 2022-09-18 19:21:15.000000 joeynmt-2.2.1/test/unit/test_vocabulary.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3769 2023-06-05 15:59:11.000000 joeynmt-2.2.1/test/unit/test_weight_tying.py
```

### Comparing `joeynmt-2.1.0/README.md` & `joeynmt-2.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # &nbsp; ![Joey-NMT](joey2-small.png) Joey NMT
 [![build](https://github.com/joeynmt/joeynmt/actions/workflows/main.yml/badge.svg)](https://github.com/joeynmt/joeynmt/actions/workflows/main.yml)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-
 ## Goal and Purpose
 :koala: Joey NMT framework is developed for educational purposes.
 It aims to be a **clean** and **minimalistic** code base to help novices 
 find fast answers to the following questions.
 - :grey_question: How to implement classic NMT architectures (RNN and Transformer) in PyTorch?
 - :grey_question: What are the building blocks of these architectures and how do they interact?
 - :grey_question: How to modify these blocks (e.g. deeper, wider, ...)?
@@ -40,25 +39,25 @@
 - Learning curve plotting
 - Scoring hypotheses and references
 
 
 
 ## Installation
 Joey NMT is built on [PyTorch](https://pytorch.org/). Please make sure you have a compatible environment.
-We tested Joey NMT 2.0 with
+We tested Joey NMT v2.2.1 with
 - python 3.10
-- torch 1.12.1
-- cuda 11.6
+- torch 2.0.1
+- cuda 11.7
 
 > :warning: **Warning**
 > When running on **GPU** you need to manually install the suitable PyTorch version 
 > for your [CUDA](https://developer.nvidia.com/cuda-zone) version.
-> For example, you can install PyTorch 1.12.1 with CUDA v11.6 as follows:
+> For example, you can install PyTorch 2.0.1 with CUDA v11.7 as follows:
 > ```
-> $ pip install --upgrade torch==1.12.1 --extra-index-url https://download.pytorch.org/whl/cu116
+> $ pip install --upgrade torch==2.0.1 --extra-index-url https://download.pytorch.org/whl/cu117
 > ```
 > See [PyTorch installation instructions](https://pytorch.org/get-started/locally/).
 
 
 You can install Joey NMT either A. via [pip](https://pypi.org/project/joeynmt/) or B. from source.
 
 ### A. Via pip (the latest stable version)
@@ -80,23 +79,37 @@
 3. Run the unit tests:
   ```bash
   $ python -m unittest
   ```
 
 
 ## Change logs
+
+### v2.2.1
+- compatibility with torch 2.0 tested
+- configurable activation function [#211](https://github.com/joeynmt/joeynmt/pull/211)
+- bug fix [#207](https://github.com/joeynmt/joeynmt/pull/207)
+
+
+<details><summary>previous releases</summary>
+
+### v2.2
+- compatibility with torch 1.13 tested
+- torchhub introduced
+- bugfixes, minor refactoring
+
 ### v2.1
 - upgrade to python 3.10, torch 1.12
 - replace Automated Mixed Precision from NVIDA's amp to Pytorch's amp package
 - replace [discord.py](https://github.com/Rapptz/discord.py) with [pycord](https://github.com/Pycord-Development/pycord) in the Discord Bot demo
-- Data Iterator refactoring
+- data iterator refactoring
 - add wmt14 ende / deen benchmark trained on v2 from scratch
-- bugfixes
+- add tokenizer tutorial
+- minor bugfixes
 
-<details><summary>previous releases</summary>
 
 ### v2.0 *Breaking change!*
 - upgrade to python 3.9, torch 1.11
 - `torchtext.legacy` dependencies are completely replaced by `torch.utils.data`
 - `joeynmt/tokenizers.py`: handles tokenization internally (also supports bpe-dropout!)
 - `joeynmt/datasets.py`: loads data from plaintext, tsv, and huggingface's [datasets](https://github.com/huggingface/datasets)
 - `scripts/build_vocab.py`: trains subwords, creates joint vocab
@@ -129,52 +142,53 @@
 ## Documentation & Tutorials
 
 We also updated the [documentation](https://joeynmt.readthedocs.io) thoroughly for Joey NMT 2.0!
 
 For details, follow the tutorials in [notebooks](notebooks) dir.
 #### v2.x
 - [quick start with joeynmt2](notebooks/joey_v2_demo.ipynb)
+- [fine tuning tutorial](https://github.com/may-/joeynmt/blob/main/notebooks/fine_tuning_tutorial_enja.ipynb)
 - [tokenizer tutorial](https://github.com/may-/joeynmt/blob/main/notebooks/tokenizer_tutorial_en.ipynb)
-- [joeyS2T ASR tutorial](https://github.com/may-/joeynmt/blob/joeyS2T/notebooks/joeyS2T_ASR_tutorial.ipynb) 
+- [joeyS2T ASR tutorial](https://github.com/may-/joeys2t/blob/main/notebooks/joeyS2T_ASR_tutorial.ipynb)
 
 #### v1.x
 - [demo notebook](notebooks/joey_v1_demo.ipynb)
 - [starter notebook](https://github.com/masakhane-io/masakhane-mt/blob/master/starter_notebook-custom-data.ipynb) Masakhane - Machine Translation for African Languages in [masakhane-io](https://github.com/masakhane-io/masakhane-mt)
 - [joeynmt toy models](https://github.com/bricksdont/joeynmt-toy-models) Collection of Joey NMT scripts by [@bricksdont](https://github.com/bricksdont)
 
 ## Usage
 > :warning: **Warning**
 > For Joey NMT v1.x, please refer the archive [here](docs/JoeyNMT_v1.md).
 
 Joey NMT has 3 modes: `train`, `test`, and `translate`, and all of them takes a
 [YAML](https://yaml.org/)-style config file as argument.
 You can find examples in the `configs` directory.
-`small.yaml` contains a detailed explanation of configuration options.
+`transformer_small.yaml` contains a detailed explanation of configuration options.
 
 Most importantly, the configuration contains the description of the model architecture
 (e.g. number of hidden units in the encoder RNN), paths to the training, development and
 test data, and the training hyperparameters (learning rate, validation frequency etc.).
 
 > :memo: **Info**
 > Note that subword model training and joint vocabulary creation is not included
 > in the 3 modes above, has to be done separately.
 > We provide a script that takes care of it: `scritps/build_vocab.py`.
 > ```
-> $ python scripts/build_vocab.py configs/small.yaml --joint
+> $ python scripts/build_vocab.py configs/transformer_small.yaml --joint
 > ```
 
 ### `train` mode
 For training, run 
 ```bash
-$ python -m joeynmt train configs/small.yaml
+$ python -m joeynmt train configs/transformer_small.yaml
 ```
 This will train a model on the training data, validate on validation data, and store
 model parameters, vocabularies, validation outputs. All needed information should be
 specified in the `data`, `training` and `model` section of the config file (here
-`configs/small.yaml`).
+`configs/transformer_small.yaml`).
 
 ```
 model_dir/
 ├── *.ckpt          # checkpoints
 ├── *.hyps          # translated texts at validation
 ├── config.yaml     # config file
 ├── spm.model       # sentencepiece model / subword-nmt codes file
@@ -189,15 +203,15 @@
 
 
 
 ### `test` mode
 This mode will generate translations for validation and test set (as specified in the
 configuration) in `model_dir/out.[dev|test]`.
 ```
-$ python -m joeynmt test configs/small.yaml --ckpt model_dir/avg.ckpt
+$ python -m joeynmt test configs/transformer_small.yaml --ckpt model_dir/avg.ckpt
 ```
 If `--ckpt` is not specified above, the checkpoint path in `load_model` of the config
 file or the best model in `model_dir` will be used to generate translations.
 
 You can specify i.e. [sacrebleu](https://github.com/mjpost/sacrebleu) options in the
 `test` section of the config file.
 
@@ -207,15 +221,15 @@
 > $ python scripts/average_checkpoints.py --inputs model_dir/*00.ckpt --output model_dir/avg.ckpt
 > ```
 
 If you want to output the log-probabilities of the hypotheses or references, you can
 specify `return_score: 'hyp'` or `return_score: 'ref'` in the testing section of the
 config. And run `test` with `--output_path` and `--save_scores` options.
 ```
-$ python -m joeynmt test configs/small.yaml --ckpt model_dir/avg.ckpt --output_path model_dir/pred --save_scores
+$ python -m joeynmt test configs/transformer_small.yaml --ckpt model_dir/avg.ckpt --output_path model_dir/pred --save_scores
 ```
 This will generate `model_dir/pred.{dev|test}.{scores|tokens}` which contains scores and corresponding tokens.
 
 > :memo: **Info**
 > - If you set `return_score: 'hyp'` with greedy decoding, then token-wise scores will be returned. The beam search will return sequence-level scores, because the scores are summed up per sequence during beam exploration.
 > - If you set `return_score: 'ref'`, the model looks up the probabilities of the given ground truth tokens, and both decoding and evaluation will be skipped.
 > - If you specify `n_best` >1 in config, the first translation in the nbest list will be used in the evaluation.
@@ -223,20 +237,20 @@
 
 
 ### `translate` mode
 This mode accepts inputs from stdin and generate translations.
 
 - File translation
   ```
-  $ python -m joeynmt translate configs/small.yaml < my_input.txt > output.txt
+  $ python -m joeynmt translate configs/transformer_small.yaml < my_input.txt > output.txt
   ```
 
 - Interactive translation
   ```
-  $ python -m joeynmt translate configs/small.yaml
+  $ python -m joeynmt translate configs/transformer_small.yaml
   ```
   You'll be prompted to type an input sentence. Joey NMT will then translate with the 
   model specified in `--ckpt` or the config file.
 
   > :bulb: **Tip**
   > Interactive `translate` mode doesn't work with Multi-GPU.
   > Please run it on single GPU or CPU.
@@ -344,15 +358,15 @@
 
 
 ## Projects and Extensions
 Here we'll collect projects and repositories that are based on Joey NMT, so you can find
 inspiration and examples on how to modify and extend the code.
 
 ### Joey NMT v2.x
-- :ear: **JoeyS2T**. Joey NMT is extended for Speech-to-Text tasks! [Code](https://github.com/may-/joeynmt/tree/joeyS2T)
+- :ear: **JoeyS2T**. Joey NMT is extended for Speech-to-Text tasks! Checkout the [code](https://github.com/may-/joeys2t) and the [EMNLP 2022 Paper](https://arxiv.org/abs/2210.02545).
 - :right_anger_bubble: **Discord Joey**. This script demonstrates how to deploy Joey NMT models as a Chatbot on Discord. [Code](scripts/discord_joey.py)
 
 ### Joey NMT v1.x
 - :spider_web: **Masakhane Web**. [@CateGitau](https://github.com/categitau), [@Kabongosalomon](https://github.com/Kabongosalomon), [@vukosim](https://github.com/vukosim) and team built a whole web translation platform for the African NMT models that Masakhane built with Joey NMT. The best is: it's completely open-source, so anyone can contribute new models or features. Try it out [here](http://translate.masakhane.io/), and check out the [code](https://github.com/dsfsi/masakhane-web).
 - :gear: **MutNMT**. [@sjarmero](https://github.com/sjarmero) created a web application to train NMT: it lets the user train, inspect, evaluate and translate with Joey NMT --- perfect for NMT newbies! Code [here](https://github.com/Prompsit/mutnmt). The tool was developed by [Prompsit](https://www.prompsit.com/) in the framework of the European project [MultiTraiNMT](http://www.multitrainmt.eu/).
 - :star2: **Cantonese-Mandarin Translator**. [@evelynkyl](https://github.com/evelynkyl/) trained different NMT models for translating between the low-resourced Cantonese and Mandarin,  with the help of some cool parallel sentence mining tricks! Check out her work [here](https://github.com/evelynkyl/yue_nmt).
 - :book: **Russian-Belarusian Translator**. [@tsimafeip](https://github.com/tsimafeip) built a translator from Russian to Belarusian and adapted it to legal and medical domains. The code can be found [here](https://github.com/tsimafeip/Translator/).
```

### Comparing `joeynmt-2.1.0/joeynmt/__main__.py` & `joeynmt-2.2.1/joeynmt/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,41 @@
 from joeynmt.prediction import test, translate
 from joeynmt.training import train
 
 
 def main():
     ap = argparse.ArgumentParser("Joey NMT")
 
-    ap.add_argument(
-        "mode",
-        choices=["train", "test", "translate"],
-        help="train a model or test or translate",
-    )
+    ap.add_argument("mode",
+                    choices=["train", "test", "translate"],
+                    help="train a model or test or translate")
 
-    ap.add_argument("config_path", type=str, help="path to YAML config file")
+    ap.add_argument("config_path",
+                    metavar="config-path",
+                    type=str,
+                    help="path to YAML config file")
 
     ap.add_argument("-c", "--ckpt", type=str, help="checkpoint for prediction")
 
     ap.add_argument("-o",
-                    "--output_path",
+                    "--output-path",
                     type=str,
                     help="path for saving translation output")
 
-    ap.add_argument(
-        "-a",
-        "--save_attention",
-        action="store_true",
-        help="save attention visualizations",
-    )
-
-    ap.add_argument("-s", "--save_scores", action="store_true", help="save scores")
-
-    ap.add_argument(
-        "-t",
-        "--skip_test",
-        action="store_true",
-        help="Skip test after training",
-    )
+    ap.add_argument("-a",
+                    "--save-attention",
+                    action="store_true",
+                    help="save attention visualizations")
+
+    ap.add_argument("-s", "--save-scores", action="store_true", help="save scores")
+
+    ap.add_argument("-t",
+                    "--skip-test",
+                    action="store_true",
+                    help="Skip test after training")
 
     args = ap.parse_args()
 
     if args.mode == "train":
         train(cfg_file=args.config_path, skip_test=args.skip_test)
     elif args.mode == "test":
         test(
```

### Comparing `joeynmt-2.1.0/joeynmt/attention.py` & `joeynmt-2.2.1/joeynmt/attention.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/batch.py` & `joeynmt-2.2.1/joeynmt/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         self.src = self.src.to(device)
         self.src_length = self.src_length.to(device)
         self.src_mask = self.src_mask.to(device)
 
         if self.has_trg:
             self.trg_input = self.trg_input.to(device)
             self.trg = self.trg.to(device)
+            self.trg_length = self.trg_length.to(device)
             self.trg_mask = self.trg_mask.to(device)
 
     def normalize(
         self,
         tensor: Tensor,
         normalization: str = "none",
         n_gpu: int = 1,
```

### Comparing `joeynmt-2.1.0/joeynmt/builders.py` & `joeynmt-2.2.1/joeynmt/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,32 @@
 )
 
 from joeynmt.helpers import ConfigurationError
 
 logger = logging.getLogger(__name__)
 
 
+def build_activation(activation: str = "relu") -> Callable:
+    """
+    Returns the activation function
+    """
+    # pylint: disable=no-else-return
+    if activation == "relu":
+        return nn.ReLU
+    elif activation == "gelu":
+        return nn.GELU
+    elif activation == "tanh":
+        return torch.tanh
+    elif activation == "swish":
+        return nn.SiLU
+    else:
+        raise ConfigurationError("Invalid activation function. Valid options: "
+                                 "'relu', 'gelu', 'tanh', 'swish'.")
+
+
 def build_gradient_clipper(config: dict) -> Optional[Callable]:
     """
     Define the function for gradient clipping as specified in configuration.
     If not specified, returns None.
 
     Current options:
         - "clip_grad_val": clip the gradients if they exceed this value,
```

### Comparing `joeynmt-2.1.0/joeynmt/data.py` & `joeynmt-2.2.1/joeynmt/data.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/datasets.py` & `joeynmt-2.2.1/joeynmt/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import logging
 import random
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Tuple, Union
 
 import torch
-
 from torch.utils.data import (
     BatchSampler,
     DataLoader,
     Dataset,
     RandomSampler,
     Sampler,
     SequentialSampler,
@@ -43,15 +42,15 @@
     """
 
     def __init__(
         self,
         path: str,
         src_lang: str,
         trg_lang: str,
-        split: int = "train",
+        split: str = "train",
         has_trg: bool = True,
         tokenizer: Dict[str, BasicTokenizer] = None,
         sequence_encoder: Dict[str, Callable] = None,
         random_subset: int = -1,
     ):
         self.path = path
         self.src_lang = src_lang
@@ -210,16 +209,16 @@
                                               drop_last=False)
         else:
             raise ConfigurationError(f"{batch_type}: Unknown batch type")
 
         assert self.sequence_encoder[self.src_lang] is not None
         if self.has_trg:
             assert self.sequence_encoder[self.trg_lang] is not None
-        else:
-            self.sequence_encoder[self.trg_lang] = None
+        # else:
+        #    self.sequence_encoder[self.trg_lang] = None
 
         # data iterator
         return DataLoader(
             dataset=self,
             batch_sampler=batch_sampler,
             collate_fn=partial(self.collate_fn, pad_index=pad_index, device=device),
             num_workers=num_workers,
@@ -311,16 +310,16 @@
     def _look_up_item(self, idx: int, lang: str) -> str:
         try:
             if len(self.idx_map) > 0:
                 idx = self.idx_map[idx]
             line = self.data[lang][idx]
             return line
         except Exception as e:
-            print(idx, self._initial_len)
-            raise Exception from e
+            logger.error(idx, self._initial_len, e)
+            raise ValueError from e
 
     def get_list(self,
                  lang: str,
                  tokenized: bool = False) -> Union[List[str], List[List[str]]]:
         """
         Return list of preprocessed sentences in the given language.
         (not length-filtered, no bpe-dropout)
@@ -444,15 +443,14 @@
         return len(self.df)
 
 
 class StreamDataset(BaseDataset):
     """
     StreamDataset which interacts with stream inputs.
     - called by `translate()` func in `prediction.py`.
-    - src side only, no trg expected.
     """
 
     def __init__(
         self,
         path: str,
         src_lang: str,
         trg_lang: str,
@@ -473,34 +471,45 @@
             tokenizer=tokenizer,
             sequence_encoder=sequence_encoder,
             random_subset=random_subset,
         )
         # place holder
         self.cache = {}
 
-    def set_item(self, line: str) -> None:
+    def set_item(self, src_line: str, trg_line: str = None) -> None:
         """
-        Set source text to the cache.
+        Set input text to the cache.
 
-        :param line: (str)
+        :param src_line: (str)
+        :param trg_line: (str)
         """
-        assert isinstance(line, str) and line.strip() != "", \
+        assert isinstance(src_line, str) and src_line.strip() != "", \
             "The input sentence is empty! Please make sure " \
             "that you are feeding a valid input."
 
         idx = len(self.cache)
-        line = self.tokenizer[self.src_lang].pre_process(line)
-        self.cache[idx] = (line, None)
+        src_line = self.tokenizer[self.src_lang].pre_process(src_line)
+
+        if self.has_trg:
+            trg_line = self.tokenizer[self.trg_lang].pre_process(trg_line)
+        self.cache[idx] = (src_line, trg_line)
 
     def get_item(self, idx: int, lang: str, is_train: bool = None) -> List[str]:
         # pylint: disable=unused-argument
         assert idx in self.cache, (idx, self.cache)
-        assert lang == self.src_lang, (lang, self.src_lang)
-        line, _ = self.cache[idx]
-        item = self.tokenizer[lang](line, is_train=False)
+        assert lang in [self.src_lang, self.trg_lang]
+        if lang == self.trg_lang:
+            assert self.has_trg
+
+        line = {}
+        src_line, trg_line = self.cache[idx]
+        line[self.src_lang] = src_line
+        line[self.trg_lang] = trg_line
+
+        item = self.tokenizer[lang](line[lang], is_train=False)
         return item
 
     def __len__(self) -> int:
         return len(self.cache)
 
     def __repr__(self) -> str:
         return (f"{self.__class__.__name__}(split={self.split}, len={len(self.cache)}, "
@@ -509,14 +518,15 @@
 
 
 class BaseHuggingfaceDataset(BaseDataset):
     """
     Wrapper for Huggingface's dataset object
     cf.) https://huggingface.co/docs/datasets
     """
+    COLUMN_NAME = "sentence"  # dummy column name. should be overriden.
 
     def __init__(
         self,
         path: str,
         src_lang: str,
         trg_lang: str,
         has_trg: bool = True,
@@ -538,18 +548,27 @@
         # load data
         self.dataset = self.load_data(path, **kwargs)
         self._kwargs = kwargs  # should contain arguments passed to `load_dataset()`
 
     def load_data(self, path: str, **kwargs) -> Any:
         # pylint: disable=import-outside-toplevel
         try:
-            from datasets import config, load_dataset, load_from_disk
-            if Path(path, config.DATASET_STATE_JSON_FILENAME).exists():
-                return load_from_disk(path)
-            return load_dataset(path, **kwargs)
+            from datasets import Dataset as Dataset_hf
+            from datasets import DatasetDict, config, load_dataset, load_from_disk
+            if Path(path, config.DATASET_STATE_JSON_FILENAME).exists() \
+                    or Path(path, config.DATASETDICT_JSON_FILENAME).exists():
+                hf_dataset = load_from_disk(path)
+                if isinstance(hf_dataset, DatasetDict):
+                    assert kwargs["split"] in hf_dataset
+                    hf_dataset = hf_dataset[kwargs["split"]]
+            else:
+                hf_dataset = load_dataset(path, **kwargs)
+            assert isinstance(hf_dataset, Dataset_hf)
+            assert self.COLUMN_NAME in hf_dataset.features
+            return hf_dataset
 
         except ImportError as e:
             logger.error(e)
             raise ImportError from e
 
     def sample_random_subset(self, seed: int = 42) -> None:
         super().sample_random_subset(seed)  # check validity
@@ -559,99 +578,91 @@
 
     def reset_random_subset(self) -> None:
         # reload from cache
         self.dataset = self.load_data(self.path, **self._kwargs)
 
     def get_item(self, idx: int, lang: str, is_train: bool = None) -> List[str]:
         # lookup
-        line = self.dataset[idx]
+        line = self.dataset[idx][self.COLUMN_NAME]
         assert lang in line, (line, lang)
 
         # tokenize
         is_train = self.split == "train" if is_train is None else is_train
         item = self.tokenizer[lang](line[lang], is_train=is_train)
         return item
 
     def get_list(self, lang: str, tokenized: bool = False) -> List[str]:
         if tokenized:
-            return self.dataset.map(
-                lambda item: {f"tok_{lang}": self.tokenizer[lang](item[lang])},
-                desc=f"Tokenizing {lang}...",
-            )[f"tok_{lang}"]
-        return self.dataset[lang]
+
+            def _tok(item):
+                item[f'tok_{lang}'] = self.tokenizer[lang](item[self.COLUMN_NAME][lang])
+                return item
+
+            return self.dataset.map(_tok, desc=f"Tokenizing {lang}...")[f'tok_{lang}']
+        return self.dataset.flatten()[f'{self.COLUMN_NAME}.{lang}']
 
     def __len__(self) -> int:
         return self.dataset.num_rows
 
     def __repr__(self) -> str:
         ret = (f"{self.__class__.__name__}(len={self.__len__()}, "
                f"src_lang={self.src_lang}, trg_lang={self.trg_lang}, "
                f"has_trg={self.has_trg}, random_subset={self.random_subset}")
         for k, v in self._kwargs.items():
             ret += f", {k}={v}"
         ret += ")"
         return ret
 
 
-class HuggingfaceDataset(BaseHuggingfaceDataset):
+class HuggingfaceTranslationDataset(BaseHuggingfaceDataset):
     """
     Wrapper for Huggingface's `datasets.features.Translation` class
     cf.) https://github.com/huggingface/datasets/blob/master/src/datasets/features/translation.py
     """  # noqa
+    COLUMN_NAME = "translation"
 
     def load_data(self, path: str, **kwargs) -> Any:
         dataset = super().load_data(path=path, **kwargs)
-
-        # rename columns
-        if "translation" in dataset.features:
-            # check language pair
-            lang_pair = dataset.features["translation"].languages
-            assert self.src_lang in lang_pair, (self.src_lang, lang_pair)
-
-            # rename columns
-            columns = {f"translation.{self.src_lang}": self.src_lang}
-            if self.has_trg:
-                assert self.trg_lang in lang_pair, (self.trg_lang, lang_pair)
-                columns[f"translation.{self.trg_lang}"] = self.trg_lang
-
-            # flatten
-            dataset = dataset.flatten()
-
-        elif f"{self.src_lang}_sentence" in dataset.features:
-            # rename columns
-            columns = {f"{self.src_lang}_sentence": self.src_lang}
+        # pylint: disable=import-outside-toplevel
+        try:
+            from datasets.features import Translation as Translation_hf
+            assert isinstance(dataset.features[self.COLUMN_NAME], Translation_hf), \
+                f"Data type mismatch. Please cast `{self.COLUMN_NAME}` column to " \
+                "datasets.features.Translation class."
+            assert self.src_lang in dataset.features[self.COLUMN_NAME].languages
             if self.has_trg:
-                assert f"{self.trg_lang}_sentence" in dataset.features
-                columns[f"{self.trg_lang}_sentence"] = self.trg_lang
+                assert self.trg_lang in dataset.features[self.COLUMN_NAME].languages
 
-        else:
-            pass
-            # TODO: support other field names
-        dataset = dataset.rename_columns(columns)
+        except ImportError as e:
+            logger.error(e)
+            raise ImportError from e
 
-        # preprocess (lowercase, pretokenize, etc.)
+        # preprocess (lowercase, pretokenize, etc.) + validity check
         def _pre_process(item):
             sl = self.src_lang
-            tl = self.trg_lang
-            ret = {sl: self.tokenizer[sl].pre_process(item[sl])}
+            item[self.COLUMN_NAME][sl] = self.tokenizer[sl].pre_process(
+                item[self.COLUMN_NAME][sl])
             if self.has_trg:
-                ret[tl] = self.tokenizer[tl].pre_process(item[tl])
-            return ret
+                tl = self.trg_lang
+                item[self.COLUMN_NAME][tl] = self.tokenizer[tl].pre_process(
+                    item[self.COLUMN_NAME][tl])
+            return item
 
         def _drop_nan(item):
-            sl = self.src_lang
-            tl = self.trg_lang
-            is_src_valid = item[sl] is not None and len(item[sl]) > 0
+            src_item = item[self.COLUMN_NAME][self.src_lang]
+            is_src_valid = src_item is not None and len(src_item) > 0
             if self.has_trg:
-                is_trg_valid = item[tl] is not None and len(item[tl]) > 0
+                trg_item = item[self.COLUMN_NAME][self.trg_lang]
+                is_trg_valid = trg_item is not None and len(trg_item) > 0
                 return is_src_valid and is_trg_valid
             return is_src_valid
 
         dataset = dataset.filter(_drop_nan, desc="Dropping NaN...")
-        return dataset.map(_pre_process, desc="Preprocessing...")
+        dataset = dataset.map(_pre_process, desc="Preprocessing...")
+        return dataset
 
 
 def build_dataset(
     dataset_type: str,
     path: str,
     src_lang: str,
     trg_lang: str,
@@ -717,26 +728,26 @@
             random_subset=-1,
             **kwargs,
         )
     elif dataset_type == "huggingface":
         # "split" should be specified in kwargs
         if "split" not in kwargs:
             kwargs["split"] = "validation" if split == "dev" else split
-        dataset = HuggingfaceDataset(
+        dataset = HuggingfaceTranslationDataset(
             path=path,
             src_lang=src_lang,
             trg_lang=trg_lang,
             has_trg=has_trg,
             tokenizer=tokenizer,
             sequence_encoder=sequence_encoder,
             random_subset=random_subset,
             **kwargs,
         )
     else:
-        ConfigurationError(f"{dataset_type}: Unknown dataset type.")
+        raise ConfigurationError(f"{dataset_type}: Unknown dataset type.")
     return dataset
 
 
 class SentenceBatchSampler(BatchSampler):
     """
     Wraps another sampler to yield a mini-batch of indices based on num of instances.
     An instance longer than dataset.max_len will be filtered out.
```

### Comparing `joeynmt-2.1.0/joeynmt/decoders.py` & `joeynmt-2.2.1/joeynmt/decoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 from typing import Optional, Tuple
 
 import torch
 from torch import Tensor, nn
 
 from joeynmt.attention import BahdanauAttention, LuongAttention
+from joeynmt.builders import build_activation
 from joeynmt.encoders import Encoder
 from joeynmt.helpers import ConfigurationError, freeze_params, subsequent_mask
 from joeynmt.transformer_layers import PositionalEncoding, TransformerDecoderLayer
 
 
 class Decoder(nn.Module):
     """
@@ -136,14 +137,17 @@
             if encoder.output_size != self.hidden_size:
                 if encoder.output_size != 2 * self.hidden_size:  # bidirectional
                     raise ConfigurationError(
                         f"For initializing the decoder state with the "
                         f"last encoder state, their sizes have to match "
                         f"(encoder: {encoder.output_size} "
                         f"vs. decoder: {self.hidden_size})")
+
+        self.activation = build_activation(kwargs.get("activation", "tanh"))
+
         if freeze:
             freeze_params(self)
 
     def _check_shapes_input_forward_step(
         self,
         prev_embed: Tensor,
         prev_att_vector: Tensor,
@@ -280,15 +284,15 @@
 
         # return attention vector (Luong)
         # combine context with decoder hidden state before prediction
         att_vector_input = torch.cat([query, context], dim=2)
         # batch x 1 x 2*enc_size+hidden_size
         att_vector_input = self.hidden_dropout(att_vector_input)
 
-        att_vector = torch.tanh(self.att_vector_layer(att_vector_input))
+        att_vector = self.activation(self.att_vector_layer(att_vector_input))
 
         # output: batch x 1 x hidden_size
         return att_vector, hidden, att_probs
 
     def forward(
         self,
         trg_embed: Tensor,
@@ -452,16 +456,17 @@
             shape (batch_size, hidden_size)
         """
         batch_size = encoder_final.size(0)
 
         # for multiple layers: is the same for all layers
         if self.init_hidden_option == "bridge" and encoder_final is not None:
             # num_layers x batch_size x hidden_size
-            hidden = (torch.tanh(self.bridge_layer(encoder_final)).unsqueeze(0).repeat(
-                self.num_layers, 1, 1))
+            hidden = (self.activation(
+                self.bridge_layer(encoder_final)).unsqueeze(0).repeat(
+                    self.num_layers, 1, 1))
         elif self.init_hidden_option == "last" and encoder_final is not None:
             # special case: encoder is bidirectional: use only forward state
             if encoder_final.shape[1] == 2 * self.hidden_size:  # bidirectional
                 encoder_final = encoder_final[:, :self.hidden_size]
             hidden = encoder_final.unsqueeze(0).repeat(self.num_layers, 1, 1)
         else:  # initialize with zeros
             with torch.no_grad():
@@ -517,14 +522,15 @@
             TransformerDecoderLayer(
                 size=hidden_size,
                 ff_size=ff_size,
                 num_heads=num_heads,
                 dropout=dropout,
                 alpha=kwargs.get("alpha", 1.0),
                 layer_norm=kwargs.get("layer_norm", "post"),
+                activation=kwargs.get("activation", "relu"),
             ) for _ in range(num_layers)
         ])
 
         self.pe = PositionalEncoding(hidden_size)
         self.layer_norm = (nn.LayerNorm(hidden_size, eps=1e-6) if kwargs.get(
             "layer_norm", "post") == "pre" else None)
 
@@ -585,8 +591,9 @@
         out = self.output_layer(x)
         return out, x, att, None
 
     def __repr__(self):
         return (f"{self.__class__.__name__}(num_layers={len(self.layers)}, "
                 f"num_heads={self.layers[0].trg_trg_att.num_heads}, "
                 f"alpha={self.layers[0].alpha}, "
-                f'layer_norm="{self.layers[0]._layer_norm_position}")')
+                f'layer_norm="{self.layers[0]._layer_norm_position}", '
+                f"activation={self.layers[0].feed_forward.pwff_layer[1]})")
```

### Comparing `joeynmt-2.1.0/joeynmt/embeddings.py` & `joeynmt-2.2.1/joeynmt/embeddings.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/encoders.py` & `joeynmt-2.2.1/joeynmt/encoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,59 +75,59 @@
         )
 
         self._output_size = 2 * hidden_size if bidirectional else hidden_size
 
         if freeze:
             freeze_params(self)
 
-    def _check_shapes_input_forward(self, embed_src: Tensor, src_length: Tensor,
+    def _check_shapes_input_forward(self, src_embed: Tensor, src_length: Tensor,
                                     mask: Tensor) -> None:
         """
         Make sure the shape of the inputs to `self.forward` are correct.
         Same input semantics as `self.forward`.
 
-        :param embed_src: embedded source tokens
+        :param src_embed: embedded source tokens
         :param src_length: source length
         :param mask: source mask
         """
         # pylint: disable=unused-argument
-        assert embed_src.shape[0] == src_length.shape[0]
-        assert embed_src.shape[2] == self.emb_size
-        # assert mask.shape == embed_src.shape
+        assert src_embed.shape[0] == src_length.shape[0]
+        assert src_embed.shape[2] == self.emb_size
+        # assert mask.shape == src_embed.shape
         assert len(src_length.shape) == 1
 
-    def forward(self, embed_src: Tensor, src_length: Tensor, mask: Tensor,
+    def forward(self, src_embed: Tensor, src_length: Tensor, mask: Tensor,
                 **kwargs) -> Tuple[Tensor, Tensor, Tensor]:
         """
         Applies a bidirectional RNN to sequence of embeddings x.
         The input mini-batch x needs to be sorted by src length.
         x and mask should have the same dimensions [batch, time, dim].
 
-        :param embed_src: embedded src inputs,
+        :param src_embed: embedded src inputs,
             shape (batch_size, src_len, embed_size)
         :param src_length: length of src inputs
             (counting tokens before padding), shape (batch_size)
         :param mask: indicates padding areas (zeros where padding), shape
             (batch_size, src_len, embed_size)
         :param kwargs:
         :return:
             - output: hidden states with
                 shape (batch_size, max_length, directions*hidden),
             - hidden_concat: last hidden state with
                 shape (batch_size, directions*hidden)
         """
-        self._check_shapes_input_forward(embed_src=embed_src,
+        self._check_shapes_input_forward(src_embed=src_embed,
                                          src_length=src_length,
                                          mask=mask)
-        total_length = embed_src.size(1)
+        total_length = src_embed.size(1)
 
         # apply dropout to the rnn input
-        embed_src = self.emb_dropout(embed_src)
+        src_embed = self.emb_dropout(src_embed)
 
-        packed = pack_padded_sequence(embed_src, src_length.cpu(), batch_first=True)
+        packed = pack_padded_sequence(src_embed, src_length.cpu(), batch_first=True)
         output, hidden = self.rnn(packed)
 
         if isinstance(hidden, tuple):
             hidden, memory_cell = hidden  # pylint: disable=unused-variable
 
         output, _ = pad_packed_sequence(output,
                                         batch_first=True,
@@ -200,59 +200,62 @@
         self.layers = nn.ModuleList([
             TransformerEncoderLayer(
                 size=hidden_size,
                 ff_size=ff_size,
                 num_heads=num_heads,
                 dropout=dropout,
                 alpha=kwargs.get("alpha", 1.0),
-                layer_norm=kwargs.get("layer_norm", "post"),
+                layer_norm=kwargs.get("layer_norm", "pre"),
+                activation=kwargs.get("activation", "relu"),
             ) for _ in range(num_layers)
         ])
 
         self.pe = PositionalEncoding(hidden_size)
         self.emb_dropout = nn.Dropout(p=emb_dropout)
 
         self.layer_norm = (nn.LayerNorm(hidden_size, eps=1e-6) if kwargs.get(
             "layer_norm", "post") == "pre" else None)
 
         if freeze:
             freeze_params(self)
 
     def forward(
         self,
-        embed_src: Tensor,
+        src_embed: Tensor,
         src_length: Tensor,  # unused
         mask: Tensor = None,
         **kwargs,
     ) -> Tuple[Tensor, Tensor]:
         """
         Pass the input (and mask) through each layer in turn.
         Applies a Transformer encoder to sequence of embeddings x.
         The input mini-batch x needs to be sorted by src length.
         x and mask should have the same dimensions [batch, time, dim].
 
-        :param embed_src: embedded src inputs,
+        :param src_embed: embedded src inputs,
             shape (batch_size, src_len, embed_size)
         :param src_length: length of src inputs
             (counting tokens before padding), shape (batch_size)
         :param mask: indicates padding areas (zeros where padding), shape
             (batch_size, 1, src_len)
+        :param kwargs:
         :return:
             - output: hidden states with shape (batch_size, max_length, hidden)
             - None
         """
         # pylint: disable=unused-argument
-        x = self.pe(embed_src)  # add position encoding to word embeddings
+        x = self.pe(src_embed)  # add position encoding to word embeddings
         x = self.emb_dropout(x)
 
         for layer in self.layers:
             x = layer(x, mask)
 
         if self.layer_norm is not None:
             x = self.layer_norm(x)
         return x, None
 
     def __repr__(self):
         return (f"{self.__class__.__name__}(num_layers={len(self.layers)}, "
                 f"num_heads={self.layers[0].src_src_att.num_heads}, "
                 f"alpha={self.layers[0].alpha}, "
-                f'layer_norm="{self.layers[0]._layer_norm_position}")')
+                f'layer_norm="{self.layers[0]._layer_norm_position}", '
+                f"activation={self.layers[0].feed_forward.pwff_layer[1]})")
```

### Comparing `joeynmt-2.1.0/joeynmt/helpers.py` & `joeynmt-2.2.1/joeynmt/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import shutil
 import sys
 import unicodedata
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
+import packaging.version
 import pkg_resources
 import torch
 import yaml
 from torch import Tensor, nn
 from torch.multiprocessing import cpu_count
 from torch.utils.tensorboard import SummaryWriter
 
@@ -84,14 +85,30 @@
 
         logger.addHandler(sh)
         logger.info("Hello! This is Joey-NMT (version %s).", version)
 
     return version
 
 
+def check_version(pkg_version: str, cfg_version: str) -> None:
+    """
+    Check joeynmt version
+
+    :param pkg_version: package version number
+    :param cfg_version: version number specified in config
+    """
+    joeynmt_version = packaging.version.parse(pkg_version)
+    config_version = packaging.version.parse(cfg_version)
+    # check if the major version number matches
+    # pylint: disable=use-maxsplit-arg
+    assert joeynmt_version.major == config_version.major, (
+        f"You are using JoeyNMT version {str(joeynmt_version)}, "
+        f'but {str(config_version)} is expected in the given config.')
+
+
 def log_cfg(cfg: Dict, prefix: str = "cfg") -> None:
     """
     Write configuration to log.
 
     :param cfg: configuration to log
     :param prefix: prefix for logging
     """
@@ -205,15 +222,15 @@
         )
 
     # model initialization
     def _load_path(path):
         load_path = cfg.get(path, None)
         if load_path is not None:
             load_path = Path(load_path)
-            assert load_path.is_file()
+            assert load_path.is_file(), load_path
         return load_path
 
     load_model: Optional[Path] = _load_path("load_model")
 
     # fp16
     fp16: bool = cfg.get("fp16", False)
 
@@ -466,37 +483,34 @@
 
     :param path: path to checkpoint
     :param device: cuda device name or cpu
     :return: checkpoint (dict)
     """
     logger = logging.getLogger(__name__)
     assert path.is_file(), f"Checkpoint {path} not found."
-    checkpoint = torch.load(path.as_posix(), map_location=device)
+    checkpoint = torch.load(path, map_location=device)
     logger.info("Load model from %s.", path.resolve())
     return checkpoint
 
 
-def resolve_ckpt_path(ckpt: str, load_model: str, model_dir: Path) -> Path:
+def resolve_ckpt_path(load_model: Path, model_dir: Path) -> Path:
     """
     Resolve checkpoint path
 
-    :param ckpt: str passed from stdin args (--ckpt)
-    :param load_model: config entry (cfg['training']['load_model'])
+    :param load_model: config entry (cfg['training']['load_model']) or CLI arg (--ckpt)
     :param model_dir: Path(cfg['training']['model_dir'])
     :return: resolved checkpoint path
     """
-    if ckpt is None:
-        if load_model is None:
-            if (model_dir / "best.ckpt").is_file():
-                ckpt = model_dir / "best.ckpt"
-            else:
-                ckpt = get_latest_checkpoint(model_dir)
+    if load_model is None:
+        if (model_dir / "best.ckpt").is_file():
+            load_model = model_dir / "best.ckpt"
         else:
-            ckpt = Path(load_model)
-    return Path(ckpt)
+            load_model = get_latest_checkpoint(model_dir)
+    assert load_model.is_file(), load_model
+    return load_model
 
 
 # from onmt
 def tile(x: Tensor, count: int, dim=0) -> Tensor:
     """
     Tiles x on dimension dim count times. From OpenNMT. Used for beam search.
 
@@ -512,18 +526,21 @@
     perm = list(range(len(x.size())))
     if dim != 0:
         perm[0], perm[dim] = perm[dim], perm[0]
         x = x.permute(perm).contiguous()
     out_size = list(x.size())
     out_size[0] *= count
     batch = x.size(0)
-    x = (x.view(batch,
-                -1).transpose(0, 1).repeat(count,
-                                           1).transpose(0,
-                                                        1).contiguous().view(*out_size))
+    # yapf: disable
+    x = (x.view(batch, -1)
+         .transpose(0, 1)
+         .repeat(count, 1)
+         .transpose(0, 1)
+         .contiguous()
+         .view(*out_size))
     if dim != 0:
         x = x.permute(perm).contiguous()
     return x
 
 
 def freeze_params(module: nn.Module) -> None:
     """
```

### Comparing `joeynmt-2.1.0/joeynmt/initialization.py` & `joeynmt-2.2.1/joeynmt/initialization.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/loss.py` & `joeynmt-2.2.1/joeynmt/loss.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/metrics.py` & `joeynmt-2.2.1/joeynmt/metrics.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/model.py` & `joeynmt-2.2.1/joeynmt/model.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/plotting.py` & `joeynmt-2.2.1/joeynmt/plotting.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/prediction.py` & `joeynmt-2.2.1/joeynmt/prediction.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 import sys
 import time
 from functools import partial
 from itertools import zip_longest
 from pathlib import Path
 from typing import Dict, List, Tuple
 
-from tqdm import tqdm
 import numpy as np
 import torch
 from torch.utils.data import Dataset
+from tqdm import tqdm
 
 from joeynmt.data import load_data
 from joeynmt.datasets import StreamDataset, build_dataset
 from joeynmt.helpers import (
+    check_version,
     expand_reverse_index,
     load_checkpoint,
     load_config,
     make_logger,
     parse_test_args,
     parse_train_args,
     resolve_ckpt_path,
@@ -45,16 +46,22 @@
     device: torch.device,
     n_gpu: int,
     compute_loss: bool = False,
     normalization: str = "batch",
     num_workers: int = 0,
     cfg: Dict = None,
     fp16: bool = False,
-) -> Tuple[Dict[str, float], List[str], List[str], List[List[str]], List[np.ndarray],
-           List[np.ndarray], ]:
+) -> Tuple[
+        Dict[str, float],
+        List[str],
+        List[str],
+        List[List[str]],
+        List[np.ndarray],
+        List[np.ndarray],
+]:
     """
     Generates translations for the given data.
     If `compute_loss` is True and references are given, also computes the loss.
 
     :param model: model module
     :param data: dataset for validation
     :param device: torch device
@@ -147,23 +154,28 @@
             batch_size = len(sort_reverse_index)  # = batch.nseqs * n_best
 
             # run as during training to get validation loss (e.g. xent)
             if compute_loss and batch.has_trg:
                 assert model.loss_function is not None
 
                 # don't track gradients during validation
-                with torch.no_grad():
-                    batch_loss, log_probs, _, n_correct = model(return_type="loss",
-                                                                **vars(batch))
-                    # sum over multiple gpus
-                    batch_loss = batch.normalize(batch_loss, "sum", n_gpu=n_gpu)
-                    n_correct = batch.normalize(n_correct, "sum", n_gpu=n_gpu)
-                    if return_prob == "ref":
-                        ref_scores = batch.score(log_probs)
-                        output = batch.trg
+                with torch.autocast(device_type=device.type, enabled=fp16):
+                    with torch.no_grad():
+                        batch_loss, log_probs, attn, n_correct = model(
+                            return_type="loss",
+                            return_attention=return_attention,
+                            **vars(batch))
+
+                # sum over multiple gpus
+                batch_loss = batch.normalize(batch_loss, "sum", n_gpu=n_gpu)
+                n_correct = batch.normalize(n_correct, "sum", n_gpu=n_gpu)
+                if return_prob == "ref":
+                    ref_scores = batch.score(log_probs)
+                    attention_scores = attn.detach().cpu().float().numpy()
+                    output = batch.trg
 
                 total_loss += batch_loss.item()  # cast Tensor to float
                 total_n_correct += n_correct.item()  # cast Tensor to int
                 total_ntokens += batch.ntokens
 
             # if return_prob == "ref", then no search needed.
             # (just look up the prob of the ground truth.)
@@ -232,15 +244,22 @@
             "Evaluation result (scoring) %s, duration: %.4f[sec]",
             ", ".join([
                 f"{eval_metric}: {valid_scores[eval_metric]:6.2f}"
                 for eval_metric in ["loss", "ppl", "acc"]
             ]),
             gen_duration,
         )
-        return valid_scores, None, None, decoded_valid, valid_sequence_scores, None
+        return (
+            valid_scores,
+            None,  # valid_ref
+            None,  # valid_hyp
+            decoded_valid,
+            valid_sequence_scores,
+            valid_attention_scores,
+        )
 
     # retrieve detokenized hypotheses and references
     valid_hyp = [
         data.tokenizer[data.trg_lang].post_process(s, generate_unk=generate_unk)
         for s in decoded_valid
     ]
     # references are not length-filtered, not duplicated for n_best > 1
@@ -335,15 +354,17 @@
         n_gpu,
         num_workers,
         normalization,
         fp16,
     ) = parse_train_args(cfg["training"], mode="prediction")
 
     if len(logger.handlers) == 0:
-        _ = make_logger(model_dir, mode="test")  # version string returned
+        pkg_version = make_logger(model_dir, mode="test")  # version string returned
+        if "joeynmt_version" in cfg:
+            check_version(pkg_version, cfg["joeynmt_version"])
 
     # load the data
     if datasets is None:
         src_vocab, trg_vocab, _, dev_data, test_data = load_data(
             data_cfg=cfg["data"], datasets=["dev", "test"])
         data_to_predict = {"dev": dev_data, "test": test_data}
     else:  # avoid to load data again
@@ -374,15 +395,16 @@
                 "Please set `beam_size: 1` in the config.")
             model.loss_function = (  # need to instantiate loss func to compute scores
                 cfg["training"].get("loss", "crossentropy"),
                 cfg["training"].get("label_smoothing", 0.1),
             )
 
     # when checkpoint is not specified, take latest (best) from model dir
-    ckpt = resolve_ckpt_path(ckpt, load_model, model_dir)
+    load_model = load_model if ckpt is None else Path(ckpt)
+    ckpt = resolve_ckpt_path(load_model, model_dir)
 
     # load model checkpoint
     model_checkpoint = load_checkpoint(ckpt, device=device)
 
     # restore model and optimizer parameters
     model.load_state_dict(model_checkpoint["model_state"])
     if device.type == "cuda":
@@ -492,19 +514,21 @@
     # parse and validate cfg
     model_dir, load_model, device, n_gpu, num_workers, _, fp16 = parse_train_args(
         cfg["training"], mode="prediction")
     test_cfg = cfg["testing"]
     src_cfg = cfg["data"]["src"]
     trg_cfg = cfg["data"]["trg"]
 
-    _ = make_logger(model_dir, mode="translate")
-    # version string returned
+    pkg_version = make_logger(model_dir, mode="translate")  # version string returned
+    if "joeynmt_version" in cfg:
+        check_version(pkg_version, cfg["joeynmt_version"])
 
     # when checkpoint is not specified, take latest (best) from model dir
-    ckpt = resolve_ckpt_path(ckpt, load_model, model_dir)
+    load_model = load_model if ckpt is None else Path(ckpt)
+    ckpt = resolve_ckpt_path(load_model, model_dir)
 
     # read vocabs
     src_vocab, trg_vocab = build_vocab(cfg["data"], model_dir=model_dir)
 
     # build model and load parameters into it
     model = build_model(cfg["model"], src_vocab=src_vocab, trg_vocab=trg_vocab)
```

### Comparing `joeynmt-2.1.0/joeynmt/search.py` & `joeynmt-2.2.1/joeynmt/search.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/joeynmt/tokenizers.py` & `joeynmt-2.2.1/joeynmt/tokenizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf-8
 """
 Tokenizer module
 """
+import argparse
 import logging
 import shutil
 from pathlib import Path
 from typing import Dict, List, Union
 
 import sentencepiece as sp
 from subword_nmt import apply_bpe
@@ -45,14 +46,15 @@
             "Currently, we support moses tokenizer only."
         # sacremoses
         if self.pretokenizer == "moses":
             try:
                 from sacremoses import (  # pylint: disable=import-outside-toplevel
                     MosesDetokenizer, MosesPunctNormalizer, MosesTokenizer,
                 )
+
                 # sacremoses package has to be installed.
                 # https://github.com/alvations/sacremoses
             except ImportError as e:
                 logger.error(e)
                 raise ImportError from e
 
             self.lang = kwargs.get("lang", "en")
@@ -209,15 +211,15 @@
         return sequence
 
     def set_vocab(self, itos: List[str]) -> None:
         """Set vocab"""
         self.spm.SetVocabulary(itos)
 
     def copy_cfg_file(self, model_dir: Path) -> None:
-        """Copy confg file to model_dir"""
+        """Copy config file to model_dir"""
         if (model_dir / self.model_file.name).is_file():
             logger.warning(
                 "%s already exists. Stop copying.",
                 (model_dir / self.model_file.name).as_posix(),
             )
         shutil.copy2(self.model_file, (model_dir / self.model_file.name).as_posix())
 
@@ -240,29 +242,34 @@
         max_length: int = -1,
         min_length: int = -1,
         **kwargs,
     ):
         super().__init__(level, lowercase, normalize, max_length, min_length, **kwargs)
         assert self.level == "bpe"
 
-        self.codes: Path = Path(kwargs["codes"])
-        assert self.codes.is_file(), f"codes file {self.codes} not found."
+        codes_file = Path(kwargs["codes"])
+        assert codes_file.is_file(), f"codes file {codes_file} not found."
 
         self.separator: str = kwargs.get("separator", "@@")
+        self.dropout: float = kwargs.get("dropout", 0.0)
+
         bpe_parser = apply_bpe.create_parser()
+        for action in bpe_parser._actions:  # workaround to ensure utf8 encoding
+            if action.dest == "codes":
+                action.type = argparse.FileType('r', encoding='utf8')
         bpe_args = bpe_parser.parse_args(
-            ["--codes", kwargs["codes"], "--separator", self.separator])
+            ["--codes", codes_file.as_posix(), "--separator", self.separator])
         self.bpe = apply_bpe.BPE(
             bpe_args.codes,
             bpe_args.merges,
             bpe_args.separator,
             None,
             bpe_args.glossaries,
         )
-        self.dropout: float = kwargs.get("dropout", 0.0)
+        self.codes: Path = bpe_args.codes
 
     def __call__(self, raw_input: str, is_train: bool = False) -> List[str]:
         """Tokenize"""
         dropout = self.dropout if is_train else 0.0
         tokenized = self.bpe.process_line(raw_input, dropout).strip().split()
         if is_train and self._filter_by_length(len(tokenized)):
             return None
@@ -296,15 +303,15 @@
 
     def set_vocab(self, itos: List[str]) -> None:
         """Set vocab"""
         vocab = set(itos) - set(self.SPECIALS)
         self.bpe.vocab = vocab
 
     def copy_cfg_file(self, model_dir: Path) -> None:
-        """Copy confg file to model_dir"""
+        """Copy config file to model_dir"""
         shutil.copy2(self.codes, (model_dir / self.codes.name).as_posix())
 
     def __repr__(self):
         return (f"{self.__class__.__name__}(level={self.level}, "
                 f"lowercase={self.lowercase}, normalize={self.normalize}, "
                 f"filter_by_length=({self.min_length}, {self.max_length}), "
                 f"pretokenizer={self.pretokenizer}, "
```

### Comparing `joeynmt-2.1.0/joeynmt/training.py` & `joeynmt-2.2.1/joeynmt/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import math
 import shutil
 import time
 from collections import OrderedDict
 from pathlib import Path
 from typing import List, Tuple
 
-import packaging
 import torch
 from torch import Tensor
 from torch.utils.data import Dataset
 from torch.utils.tensorboard import SummaryWriter
 
 from joeynmt.batch import Batch
 from joeynmt.builders import build_gradient_clipper, build_optimizer, build_scheduler
 from joeynmt.data import load_data
 from joeynmt.helpers import (
+    check_version,
     delete_ckpt,
     load_checkpoint,
     load_config,
     log_cfg,
     make_logger,
     make_model_dir,
     parse_train_args,
@@ -784,23 +784,18 @@
     cfg = load_config(Path(cfg_file))
 
     # make logger
     model_dir = make_model_dir(
         Path(cfg["training"]["model_dir"]),
         overwrite=cfg["training"].get("overwrite", False),
     )
-    joeynmt_version = packaging.version.parse(make_logger(model_dir, mode="train"))
-    if "joeynmt_version" in cfg:
-        config_version = packaging.version.parse(cfg["joeynmt_version"])
-        # check if the major version number matches
-        # pylint: disable=use-maxsplit-arg
-        assert joeynmt_version.major == config_version.major, (
-            f"You are using JoeyNMT version {str(joeynmt_version)}, "
-            f'but {str(config_version)} is expected in the given config.')
+    pkg_version = make_logger(model_dir, mode="train")
     # TODO: save version number in model checkpoints
+    if "joeynmt_version" in cfg:
+        check_version(pkg_version, cfg["joeynmt_version"])
 
     # write all entries of config to the log
     log_cfg(cfg)
 
     # store copy of original training config in model dir
     shutil.copy2(cfg_file, (model_dir / "config.yaml").as_posix())
 
@@ -844,15 +839,15 @@
         test(
             cfg_file,
             ckpt=ckpt.as_posix(),
             output_path=output_path.as_posix(),
             datasets=datasets_to_test,
         )
     else:
-        logger.info("Skipping test after training")
+        logger.info("Skipping test after training.")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser("Joey-NMT")
     parser.add_argument(
         "config",
         default="configs/default.yaml",
```

### Comparing `joeynmt-2.1.0/joeynmt/transformer_layers.py` & `joeynmt-2.2.1/joeynmt/transformer_layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 """
 import math
 from typing import Optional
 
 import torch
 from torch import Tensor, nn
 
+from joeynmt.builders import build_activation
+
 
 class MultiHeadedAttention(nn.Module):
     """
     Multi-Head Attention module from "Attention is All You Need"
 
     Implementation modified from OpenNMT-py.
     https://github.com/OpenNMT/OpenNMT-py
@@ -67,15 +69,16 @@
         query_len = q.size(1)
 
         # project the queries (q), keys (k), and values (v)
         k = self.k_layer(k)
         v = self.v_layer(v)
         q = self.q_layer(q)
 
-        # reshape q, k, v for our computation to [batch_size, num_heads, ..]
+        # reshape q, k, v for our computation to
+        # [batch_size, num_heads, seq_len, head_dim]
         k = k.view(batch_size, -1, self.num_heads, self.head_size).transpose(1, 2)
         v = v.view(batch_size, -1, self.num_heads, self.head_size).transpose(1, 2)
         q = q.view(batch_size, -1, self.num_heads, self.head_size).transpose(1, 2)
 
         # compute scores
         q = q / math.sqrt(self.head_size)
 
@@ -116,29 +119,33 @@
     def __init__(
         self,
         input_size: int,
         ff_size: int,
         dropout: float = 0.1,
         alpha: float = 1.0,
         layer_norm: str = "post",
+        activation: str = "relu",
     ) -> None:
         """
         Initializes position-wise feed-forward layer.
         :param input_size: dimensionality of the input.
         :param ff_size: dimensionality of intermediate representation
         :param dropout: dropout probability
         :param alpha: weight factor for residual connection
         :param layer_norm: either "pre" or "post"
+        :param activation: activation function
         """
         super().__init__()
 
+        activation_fnc = build_activation(activation=activation)
+
         self.layer_norm = nn.LayerNorm(input_size, eps=1e-6)
         self.pwff_layer = nn.Sequential(
             nn.Linear(input_size, ff_size),
-            nn.ReLU(),
+            activation_fnc(),
             nn.Dropout(dropout),
             nn.Linear(ff_size, input_size),
             nn.Dropout(dropout),
         )
 
         self.alpha = alpha
         self._layer_norm_position = layer_norm
@@ -209,39 +216,42 @@
         self,
         size: int = 0,
         ff_size: int = 0,
         num_heads: int = 0,
         dropout: float = 0.1,
         alpha: float = 1.0,
         layer_norm: str = "post",
+        activation: str = "relu",
     ) -> None:
         """
         A single Transformer encoder layer.
 
         Note: don't change the name or the order of members!
         otherwise pretrained models cannot be loaded correctly.
 
         :param size: model dimensionality
         :param ff_size: size of the feed-forward intermediate layer
         :param num_heads: number of heads
         :param dropout: dropout to apply to input
         :param alpha: weight factor for residual connection
         :param layer_norm: either "pre" or "post"
+        :param activation: activation function
         """
         super().__init__()
 
         self.layer_norm = nn.LayerNorm(size, eps=1e-6)
         self.src_src_att = MultiHeadedAttention(num_heads, size, dropout=dropout)
 
         self.feed_forward = PositionwiseFeedForward(
             size,
             ff_size=ff_size,
             dropout=dropout,
             alpha=alpha,
             layer_norm=layer_norm,
+            activation=activation,
         )
 
         self.dropout = nn.Dropout(dropout)
         self.size = size
 
         self.alpha = alpha
         self._layer_norm_position = layer_norm
@@ -283,41 +293,44 @@
         self,
         size: int = 0,
         ff_size: int = 0,
         num_heads: int = 0,
         dropout: float = 0.1,
         alpha: float = 1.0,
         layer_norm: str = "post",
+        activation: str = "relu",
     ) -> None:
         """
         Represents a single Transformer decoder layer.
         It attends to the source representation and the previous decoder states.
 
         Note: don't change the name or the order of members!
         otherwise pretrained models cannot be loaded correctly.
 
         :param size: model dimensionality
         :param ff_size: size of the feed-forward intermediate layer
         :param num_heads: number of heads
         :param dropout: dropout to apply to input
         :param alpha: weight factor for residual connection
         :param layer_norm: either "pre" or "post"
+        :param activation: activation function
         """
         super().__init__()
         self.size = size
 
         self.trg_trg_att = MultiHeadedAttention(num_heads, size, dropout=dropout)
         self.src_trg_att = MultiHeadedAttention(num_heads, size, dropout=dropout)
 
         self.feed_forward = PositionwiseFeedForward(
             size,
             ff_size=ff_size,
             dropout=dropout,
             alpha=alpha,
             layer_norm=layer_norm,
+            activation=activation,
         )
 
         self.x_layer_norm = nn.LayerNorm(size, eps=1e-6)
         self.dec_layer_norm = nn.LayerNorm(size, eps=1e-6)
 
         self.dropout = nn.Dropout(dropout)
         self.alpha = alpha
@@ -328,14 +341,15 @@
     def forward(
         self,
         x: Tensor,
         memory: Tensor,
         src_mask: Tensor,
         trg_mask: Tensor,
         return_attention: bool = False,
+        **kwargs,
     ) -> Tensor:
         """
         Forward pass of a single Transformer decoder layer.
 
         First applies target-target self-attention, dropout with residual connection
         (adding the input to the result), and layer norm.
 
@@ -349,14 +363,15 @@
         :param src_mask: source mask
         :param trg_mask: target mask (so as to not condition on future steps)
         :param return_attention: whether to return the attention weights
         :return:
             - output tensor
             - attention weights
         """
+        # pylint: disable=unused-argument
         # 1. target-target self-attention
         residual = x
         if self._layer_norm_position == "pre":
             x = self.x_layer_norm(x)
 
         h1, _ = self.trg_trg_att(x, x, x, mask=trg_mask)
         h1 = self.dropout(h1) + self.alpha * residual
```

### Comparing `joeynmt-2.1.0/joeynmt/vocabulary.py` & `joeynmt-2.2.1/joeynmt/vocabulary.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         # tokenize sentences
         sents = dataset.get_list(lang=cfg["lang"], tokenized=True)
 
         # newly create unique token list (language-wise)
         counter = Counter(flatten(sents))
         unique_tokens = sort_and_cut(counter, max_size, min_freq)
     else:
-        raise Exception("Please provide a vocab file path or dataset.")
+        raise ValueError("Please provide a vocab file path or dataset.")
 
     vocab = Vocabulary(unique_tokens)
     assert len(vocab) <= max_size + len(vocab.specials), (len(vocab), max_size)
 
     # check for all except for UNK token whether they are OOVs
     for s in vocab.specials[1:]:
         assert not vocab.is_unk(s)
```

### Comparing `joeynmt-2.1.0/joeynmt.egg-info/SOURCES.txt` & `joeynmt-2.2.1/joeynmt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 joeynmt/constants.py
 joeynmt/data.py
 joeynmt/datasets.py
 joeynmt/decoders.py
 joeynmt/embeddings.py
 joeynmt/encoders.py
 joeynmt/helpers.py
+joeynmt/hub_interface.py
 joeynmt/initialization.py
 joeynmt/loss.py
 joeynmt/metrics.py
 joeynmt/model.py
 joeynmt/plotting.py
 joeynmt/prediction.py
 joeynmt/search.py
 joeynmt/tokenizers.py
 joeynmt/training.py
 joeynmt/transformer_layers.py
+joeynmt/validation.py
 joeynmt/vocabulary.py
 joeynmt.egg-info/PKG-INFO
 joeynmt.egg-info/SOURCES.txt
 joeynmt.egg-info/dependency_links.txt
 joeynmt.egg-info/entry_points.txt
 joeynmt.egg-info/requires.txt
 joeynmt.egg-info/top_level.txt
```

### Comparing `joeynmt-2.1.0/setup.py` & `joeynmt-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("requirements.txt", encoding="utf-8") as req_fp:
     install_requires = req_fp.readlines()
 
 setup(
     name='joeynmt',
-    version='2.1.0',
+    version='2.2.1',
     description='Minimalist NMT for educational purposes',
     author='Jasmijn Bastings and Julia Kreutzer',
     url='https://github.com/joeynmt/joeynmt',
     license='Apache License',
     install_requires=install_requires,
     packages=find_packages(exclude=[]),
     python_requires='>=3.7',
```

### Comparing `joeynmt-2.1.0/test/unit/test_attention.py` & `joeynmt-2.2.1/test/unit/test_attention.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_batch.py` & `joeynmt-2.2.1/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_data.py` & `joeynmt-2.2.1/test/unit/test_data.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_dataset.py` & `joeynmt-2.2.1/test/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_decoder.py` & `joeynmt-2.2.1/test/unit/test_decoder.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_embeddings.py` & `joeynmt-2.2.1/test/unit/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_encoder.py` & `joeynmt-2.2.1/test/unit/test_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             hidden_size=self.hidden_size,
             bidirectional=bidirectional,
         )
         x = torch.rand(size=(batch_size, time_dim, self.emb_size))
         # no padding, no mask
         x_length = torch.Tensor([time_dim] * batch_size).int()
         mask = torch.ones_like(x)
-        output, hidden = encoder(embed_src=x, src_length=x_length, mask=mask)
+        output, hidden = encoder(src_embed=x, src_length=x_length, mask=mask)
         self.assertEqual(
             output.shape,
             torch.Size([batch_size, time_dim, directions * self.hidden_size]),
         )
         self.assertEqual(
             hidden.shape,
             torch.Size([batch_size, directions * self.hidden_size]),
```

### Comparing `joeynmt-2.1.0/test/unit/test_loss.py` & `joeynmt-2.2.1/test/unit/test_loss.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_metric.py` & `joeynmt-2.2.1/test/unit/test_metric.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_model_init.py` & `joeynmt-2.2.1/test/unit/test_model_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import unittest
-
 import copy
+import unittest
 
 import torch
 from torch import nn
 
 from joeynmt.model import build_model
 from joeynmt.vocabulary import Vocabulary
```

### Comparing `joeynmt-2.1.0/test/unit/test_prediction.py` & `joeynmt-2.2.1/test/unit/test_prediction.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_search.py` & `joeynmt-2.2.1/test/unit/test_search.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_tokenizer.py` & `joeynmt-2.2.1/test/unit/test_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import random
 import unittest
 
-import sentencepiece as spm
-
 from joeynmt.data import load_data
 from joeynmt.tokenizers import (
     BasicTokenizer,
     SentencePieceTokenizer,
     SubwordNMTTokenizer,
 )
 
@@ -35,15 +33,14 @@
             },
             "dataset_type": "plain",
         }
 
         # set seed
         seed = 42
         random.seed(seed)
-        spm.set_random_generator_seed(seed)
 
     def testBasicTokenizer(self):
         # first valid example from the training set after filtering
         expected_srcs = {
             "char": "Danke.",
             "word": "David Gallo: Das ist Bill Lange. Ich bin Dave Gallo.",
         }
@@ -148,18 +145,20 @@
             # check tokenized sequence
             self.assertEqual(tokenized, expected[lang]['tokenized'])
 
             # check detokenized sequence
             detokenized = tokenizer.post_process(tokenized)
             self.assertEqual(detokenized, expected[lang]['detokenized'])
 
-            tokenizer.nbest_size = -1
-            tokenizer.alpha = 0.8
-            dropout = tokenizer(detokenized, is_train=True)
-            self.assertEqual(dropout, expected[lang]['dropout'])
+            # we cannot set a random seed for sampling.
+            # cf) https://github.com/google/sentencepiece/issues/609
+            # tokenizer.nbest_size = -1
+            # tokenizer.alpha = 0.8
+            # dropout = tokenizer(detokenized, is_train=True)
+            # self.assertEqual(dropout, expected[lang]['dropout'])
 
     def testSubwordNMTTokenizer(self):
         cfg = self.data_cfg.copy()
         for side in ["src", "trg"]:
             cfg[side]["max_length"] = 30
             cfg[side]["level"] = "bpe"
             cfg[side]["tokenizer_type"] = "subword-nmt"
```

### Comparing `joeynmt-2.1.0/test/unit/test_transformer_decoder.py` & `joeynmt-2.2.1/test/unit/test_transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_transformer_encoder.py` & `joeynmt-2.2.1/test/unit/test_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_transformer_utils.py` & `joeynmt-2.2.1/test/unit/test_transformer_utils.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_vocabulary.py` & `joeynmt-2.2.1/test/unit/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `joeynmt-2.1.0/test/unit/test_weight_tying.py` & `joeynmt-2.2.1/test/unit/test_weight_tying.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import unittest
-
 import copy
+import unittest
 
 import torch
 
 from joeynmt.model import build_model
 from joeynmt.vocabulary import Vocabulary
```

