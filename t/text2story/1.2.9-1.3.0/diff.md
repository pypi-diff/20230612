# Comparing `tmp/text2story-1.2.9.tar.gz` & `tmp/text2story-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.2.9.tar", last modified: Wed May 24 22:29:11 2023, max compression
+gzip compressed data, was "text2story-1.3.0.tar", last modified: Mon Jun 12 15:00:19 2023, max compression
```

## Comparing `text2story-1.2.9.tar` & `text2story-1.3.0.tar`

### file list

```diff
@@ -1,101 +1,106 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.2.9/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.2.9/MANIFEST.in
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-24 22:29:11.893532 text2story-1.2.9/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8575 2023-05-17 10:11:38.000000 text2story-1.2.9/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      114 2023-03-29 13:58:48.000000 text2story-1.2.9/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1591 2023-05-24 22:29:11.893532 text2story-1.2.9/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       70 2023-03-29 13:48:56.000000 text2story-1.2.9/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.881533 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/ALLENNLP/preprocess.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2721 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4362 2023-04-28 09:04:12.000000 text2story-1.2.9/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.2.9/text2story/annotators/SPARKNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/annotators/SRLWeakLabeling/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.2.9/text2story/annotators/SRLWeakLabeling/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2394 2023-05-18 09:14:04.000000 text2story-1.2.9/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17253 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4564 2022-11-04 13:39:56.000000 text2story-1.2.9/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.2.9/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.2.9/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2667 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      505 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      529 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17906 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5281 2023-05-03 09:45:52.000000 text2story-1.2.9/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.2.9/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1618 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.889532 text2story-1.2.9/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.2.9/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22674 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.2.9/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.2.9/text2story/select/event.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.2.9/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.2.9/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.2.9/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.893532 text2story-1.2.9/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.2.9/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14759 2023-03-31 13:18:54.000000 text2story-1.2.9/text2story/viz/bubble_tikz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-24 22:29:11.885532 text2story-1.2.9/text2story.egg-info/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9774 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2728 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      238 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-05-24 22:29:11.000000 text2story-1.2.9/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-03-29 13:58:12.000000 text2story-1.2.9/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.819371 text2story-1.3.0/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.3.0/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.3.0/MANIFEST.in
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-12 15:00:19.819371 text2story-1.3.0/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7752 2023-05-30 12:31:10.000000 text2story-1.3.0/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2023-06-12 14:59:52.000000 text2story-1.3.0/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      989 2023-06-12 15:00:19.819371 text2story-1.3.0/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-05-26 15:16:02.000000 text2story-1.3.0/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.799371 text2story-1.3.0/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.799371 text2story-1.3.0/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.795371 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/cache/
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)     4090 2021-03-09 07:42:06.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/cache/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/preprocess.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1553 2023-05-29 13:21:32.000000 text2story-1.3.0/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4406 2023-05-25 14:12:26.000000 text2story-1.3.0/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.3.0/text2story/annotators/SPARKNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/SRLWeakLabeling/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.3.0/text2story/annotators/SRLWeakLabeling/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2394 2023-05-18 09:14:04.000000 text2story-1.3.0/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-05-30 10:06:48.000000 text2story-1.3.0/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9846 2023-06-12 14:58:33.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.811371 text2story-1.3.0/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.3.0/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.3.0/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2917 2023-06-09 14:36:29.000000 text2story-1.3.0/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      709 2023-06-09 13:29:38.000000 text2story-1.3.0/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2621 2023-06-09 14:35:24.000000 text2story-1.3.0/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    23131 2023-06-09 15:10:17.000000 text2story-1.3.0/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6935 2023-06-09 15:00:43.000000 text2story-1.3.0/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.811371 text2story-1.3.0/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.3.0/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/exp.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/exp_en_fn.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/exp_en_pb.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2870 2023-05-29 11:37:16.000000 text2story-1.3.0/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.3.0/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22827 2023-06-07 13:53:21.000000 text2story-1.3.0/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.3.0/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.3.0/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.3.0/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.819371 text2story-1.3.0/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.3.0/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15162 2023-06-01 12:14:40.000000 text2story-1.3.0/text2story/viz/bubble_tikz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.799371 text2story-1.3.0/text2story.egg-info/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2885 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      454 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.3.0/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.2.9/LICENSE` & `text2story-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/README.md` & `text2story-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,195 @@
+Metadata-Version: 2.1
+Name: text2story
+Version: 1.3.0
+Project-URL: Source, https://github.com/LIAAD/Text2StoryPackage
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
 
 - **Relation to Brat2Viz**
 The Text2Story package is a generalization of Brat2Viz and should in fact contain all the funcionalities and variants of the T2S project output.
 
-## Installation
-
-
-### Language and OS Requirements
-
-Text2Story package is written entirely in Python 3.8 modules ensuring compatibility with UNIX type Operating systems.
-
-### Swap Size
-
-T2S is an NLP project, which means that is intended to operate over large amounts of data using complex models, some of the third-party libraries that demand great computing resources.
-
-To ensure enough computation power, you should use a computer where the sum of physical and virtual RAM should be at least 16GB.
-
-* ####  [How to increase swap/virtual memory size in Linux systems](https://askubuntu.com/questions/178712/how-to-increase-swap-space)
-
-### Steps for installation
-
-1. Create a virtual enviroment with the following command
-   ```bash
-   python3.8 -m venv venv    
-   ```
-2. Activate the virtual enviroment with the following command
-   ```bash
-   source venv/bin/activate 
-   ```
-3. Installation of py_heideltime package (more detailed instructions in https://github.com/JMendes1995/py_heideltime)
-   ```bash
-    pip install git+https://github.com/JMendes1995/py_heideltime.git
-   ```
-4. Give tree parser of py_heideltime package permission to execute
-   ```bash
-    chmod +x $(VENV_HOME)/lib/python3.8/site-packages/py_heideltime/Heideltime/TreeTaggerLinux/bin/tree-tagger
-   ```
-5. Installation of plantuml package, which is used in the visualization.
-   ```
-   pip install git+https://github.com/SamuelMarks/python-plantuml#egg=plantuml
-   ```
-6. Installation of the text2story package.
-   ```bash
-     python -m pip install text2story
-   ```
-
-The following steps are optional to use the text2story package, but essential to run the our TLDR Python notebook locally (https://bit.ly/3s36Bxf).
-
-7. Adding virtual enviroment to Jupyter Notebook.
-   ```bash
-      python3.8 -m pip install --user ipykernel
-   ```
-
-8. Adding your virtual enviroment to Jupyter.
-   ```bash
-      python -m ipykernel install --user --name=venv
-   ```
-
-9. Changing the kernel in the Jupyter, by cliking in Kernel -> Change Kernel -> (kernel name).
-
-
-
-### Usage
-
-
-```python
-import text2story as t2s # Import the package
-
-t2s.start('en') # Load the pipelines in en language
-
-text = 'On Friday morning, Max Healthcare, which runs 10 private hospitals around Delhi, put out an "SOS" message, saying it had less than an hour\'s supply remaining at two of its sites. The shortage was later resolved.'
-
-doc = t2s.Narrative('en', text, '2020-05-30')
-
-doc.extract_actors('spacy') # Extraction done with just the SPACY tool.
-
-doc.extract_times() # Extraction done with all tools (same as specifying 'py_heideltime', since we have just one tool to extract timexs)
-
-
-doc.extract_events('allennlp') # Extraction of events with allennlp tool
-doc.extract_semantic_role_link('allennlp') # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
-
-doc.ISO_annotation('annotations.ann') # Outputs ISO annotation in .ann format (txt) in a file called 'annotations.ann', which is a standard of BRAT annotation tool
-
-
-```
-
-## Examples: Python Notebooks
-
-A  basic notebook that teaches how to use our reader of annotations, which format is assumed is to be in the BRAT format is in the following link: [How to read a BRAT file](https://colab.research.google.com/drive/1_jc6SJNAdWMYBMVlGPldFDmGNg4gFUCs?usp=sharing).
-
-There is the TLDR Python notebook, which extracts the main narrative elements and draw an MSC visulization:  [Too Long Didn't Read Tutorial](https://bit.ly/3s36Bxf).
-
-Finally, there is a notebook that shows how to produce a bubble visualization: [How To: Bubble Visualization](https://colab.research.google.com/drive/1V2DCuP1qAlwUXThTKNUnZ98WxARZXC_v?usp=sharing).
 
 ## Structure
+```
 .
 │   README.md
 |   env.yml
 │   requirements.txt
-|   pyproject.toml
-|   MANIFEST.in
-|   LICENSE
 |
-└── src
-    └─ text2story
-        └─ core
-         │   annotator.py (META-annotator)
-         │   entity_structures.py (ActorEntity, TimexEntity and EventEntity classes)
-         |   exceptions.py (Exceptions raised by the package)
-         |   link_structures.py (TemporalLink, AspectualLink, SubordinationLink, SemanticRoleLink and ObjectalLink classes)
-         |   narrative.py (Narrative class)
-         |   utils.py (Utility functions)
-         
-        └─ annotators (tools supported by the package to do the extractions)
-         |   NLTK
-         │   PY_HEIDELTIME
-         |   SPACY
-	 |   ALLENNLP
-	 |   CUSTOMPT (A CRF customized model to detect events in the Portuguese language)
-         
-        └─ brat2viz (tool devoted to create visual representations of ann files)
-         |   brat2drs (scripts that do a conversion from a brat stand off format (.ann) to DRS format)
-         │   drs2viz (scripts that do a conversion from drs format to a visual representation)
-
-        └─ readers (module dedicated to read different kind of corpora)
-         |   fn-lirics.json (conversion map from framenet to lirics: semlink project -> https://github.com/cu-clear/semlink)
-         |   pb-vn2.json   (conversion map from propbank to verbnet: semlink project -> https://github.com/cu-clear/semlink)
-         |   vn-lirics.json (conversion map from verbnet to lirics: semlink project -> https://github.com/cu-clear/semlink)
-         |   read_brat.py  (read brat stand off format)
-         |   read_ecb.py  (read ecb+ format)
-         |   read_framenet.py  (read nltk data of framenet dataset)
-         |   read_propbank.py  (read nltk data of propbank dataset)
-         |   read.py  (META-reader)
-         |   token_corpus.py  (Token representation of data)
-         |   utils.py  (Utility functions for readers)
-
-        └─ experiments (module dedicated to perform batch experiments with narrative datasets)
-         |   evaluation.py  (It performs experiments in only one dataset)
-         |   metrics.py   (It implements some metrics for classification recall, precision, and f1. Strict and relaxed versions (ref. Semeval-2013 task 1: Tempeval-3))
-         |   run_experiments.py  (It implements batch experiments for narrative datasets)
-         |   stats.py (It implements methods to evaluate some statistics of narrative datasets)
+└──Text2Story
+      └──core
+      │   │   annotator.py (META-annotator)
+      │   │   entity_structures.py (ActorEntity, TimexEntity and EventEntity classes)
+      │   |   exceptions.py (Exceptions raised by the package)
+      │   |   link_structures.py (TemporalLink, AspectualLink, SubordinationLink, SemanticRoleLink and ObjectalLink classes)
+      │   |   narrative.py (Narrative class)
+      │   |   utils.py (Utility functions)
+      │   
+      └───annotators (tools supported by the package to do the extractions)
+      |   |   NLTK
+      |   │   PY_HEIDELTIME
+      |   |   SPACY
+|
+└── Webapp
+      |  backend.py
+      |  main.py
+      |  session_state.py
+      |  input_phase.py
+      |  output_phase.py
 
+```
 
+## Classes
+### Entity classes
+- **ActorEntity** 🟢
+    - attributes
+        - text : str
+        - character_span : (int, int)
+        - value : str
+        - type : str
+        - individuation : str (HARDCODED)
+        - involvement : str  (HARDCODED)
+
+- **TimexEntity** 🟢
+    - attributes
+        - text : str
+        - character_span : (int, int)
+        - value : str
+        - type : str
+        - temporal_function : boolean (HARDCODED)
+        - anchor_time : str (HARDCODED)
+
+- **EventEntity** 🟢
+    - attributes
+        - text : str
+        - character_span : str
+        - event_class : str (HARDCODED)
+        - polarity : str (HARDCODED)
+        - factuality : str (HARDCODED)
+        - tense : str (HARDCODED)
+
+### Link classes
+
+- **TemporalLink** 🔴
+
+- **AspectualLink** 🔴
+
+- **SubordinationLink** 🔴
+
+- **SemanticRoleLink** 🟢
+    - attributes
+        - type : str
+        - actor : str
+        - event : str
+
+- **ObjectalLink** 🟢
+    - attributes
+        - type : str  (HARDCODED)
+        - arg1 : str
+        - arg2 : str
+
+### Other classes
+- **Narrative**
+    - attributes
+        - lang : str 🟢
+        - text : str 🟢
+        - publication_time : str 🟢
+        - actors : {str -> ActorEntity} 🟢
+        - timex : {str -> TimexEntity} 🟢
+        - events : {str -> EventEntity} 🟢
+        - tlinks : 🔴
+        - ref_rels : 🔴
+        - obj_links : {str -> SemanticRoleLink} 🟢
+        - sem_links : {str -> ObjectalLink} 🟢
+    - methods
+        - extract_actors: given a list of tools to do the extraction with, updates self.actors and returns it 🟢
+        - extract_times: given a list of tools to do the extraction with, updates self.timexs and returns it 🟢
+        - extract_events: given a list of tools to do the extraction with, updates self.events and returns it 🟢
+        - extract_semantic_role_links: given a list of tools to do the extraction with, finds semantic role links between extracted actors (self.actors) and events (self.events), updates self.sem_links and returns it. 🟢
+        - extract_objectal_links: given a list of tools to do the extraction with, updates self.obj_links and returns it 🟢
+        - tempsort_events: given two or more events (spans?), outputs the temporal relationship between them. Output ISO dictionary. 🔴
+        - ISO_annotation: returns ISO annotation in .ann format 🟢
+        - import_ISO_annotation: imports ISO annotation from file (may not be trivial, because of the organization by type) 🔴
+        - drs: outputs list with drs formulae (txt) 🔴
+        - compare_annotations: compare ISO annotation given with the one here (should annotation be an attribute) 🔴
+
+- **drs** 🔴
+    - attributes
+        - drs: list with text or structure with formulae
+    - methods
+        - msc: plot msc
+        - kowledge_graph: plot knowledge_graph
+        - icons: plot icon strip
+        - pretty_print:
 
 ### Annotators
 All annotators have the same interface: they implement a function called 'extract_' followed by the name of the particular extraction.
 E.g., if they are extracting actors, then they implement a function named 'extract_actors', with two arguments: the language of text and the text itself.
 
-|  Extractions |           Interface                                      |     Supporting tools  |
+|  Extractions |           Interface                                      |     Supporting tools |
 |      ---     |             ---                                          |           ---         |
-|     Actor    | extract_actors(lang, text)                               | SPACY, NLTK 	  |
-|    Timexs    | extract_timexs(lang, text, publication_time)             |      PY_HEIDELTIME    |
-| ObjectalLink | extract_objectal_links(lang, text, publication_time)     |        ALLENNLP       |
-|     Event    | extract_events(lang, text, publication_time)             | ALLENNLP, CUSTOMPT    |
-| SemanticLink | extract_semantic_role_link(lang, text, publication_time) |        ALLENNLP       |
+|     Actor    | extract_actors(lang, text)                               | SPACY,  NLTK |
+|    Timexs    | extract_timexs(lang, text, publication_time)             |      PY_HEIDELTIME |
+| ObjectalLink | extract_objectal_links(lang, text, publication_time)     |        ALLENNLP |
+|     Event    | extract_events(lang, text, publication_time)             |        ALLENNLP |
+| SemanticLink | extract_semantic_role_link(lang, text, publication_time) |        ALLENNLP |
 
 To **change some model used in the supported tools**, just go to text2story/annotators/ANNOTATOR_TO_BE_CHANGED and change the model in the file: \_\_init\_\_.py.
 
 To **add a new tool**, add a folder to text2story/annotators with the name of the annotator all capitalized (just a convention; useful to avoid name colisions).
 In that folder, create a file called '\_\_init\_\_.py' and there implement a function load() and the desired extraction functions.
 The function load() should load the pipeline to some variable defined by you, so that, every time we do an extraction, we don't need to load the pipeline all over again. (Implement it, even if your annotator doesn't load anything. Leave it with an empty body.)
 
 In the text2story.annotators.\_\_init\_\_.py file, add a call to the load() function, and to the extract functions.
 (See the already implemented tools for guidance.)
 
 And it should be done.
 
 PS: Don't forget to normalize the labels to our semantic framework!
 
+### Usage
+
+#### Installation
+
+The installation requires graphviz software.
+
+* Ubuntu: sudo apt install graphviz-dev
+* Windows: https://graphviz.org/download/#windows
+* Mac OS: brew install graphviz
+
+
+#### Terminal
+```python
+import text2story as t2s # Import the package
+
+t2s.start() # Load the pipelines
+
+text = 'On Friday morning, Max Healthcare, which runs 10 private hospitals around Delhi, put out an "SOS" message, saying it had less than an hour\'s supply remaining at two of its sites. The shortage was later resolved.'
+
+doc = t2s.Narrative('en', text, '2020-05-30')
+
+doc.extract_actors() # Extraction done with all tools.
+doc.extract_actors('spacy', 'nltk') # Extraction done with the SPACY and NLTK tools.
+doc.extract_actors('allennlp') # Extraction done with just the ALLENNLP tool.
+
+doc.extract_times() # Extraction done with all tools (same as specifying 'py_heideltime', since we have just one tool to extract timexs)
+
+doc.extract_objectal_links() # Extraction of objectal links from the text with all tools (needs to be done after extracting actors, since it requires actors to make the co-reference resolution)
+
+doc.extract_events() # Extraction of events with all tools
+doc.extract_semantic_role_link() # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
+
+ann_str = doc.ISO_annotation() # Outputs ISO annotation in .ann format (txt) in a file called 'annotations.ann'
+with open('annotations.ann', "w") as fd:
+    fd.write(ann_str)
+```
+#### Web app
+```ssh
+python backend.py
+streamlit run main.py
+```
+and a page on your browser will open!
+
```

### Comparing `text2story-1.2.9/text2story/__init__.py` & `text2story-1.3.0/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.3.0/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.3.0/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.3.0/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.3.0/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.3.0/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.3.0/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.3.0/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.3.0/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.3.0/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/NLTK/__init__.py` & `text2story-1.3.0/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/SPACY/__init__.py` & `text2story-1.3.0/text2story/annotators/SPACY/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
     if lang == "pt":
         if not(spacy.util.is_package('pt_core_news_lg')):
             spacy.cli.download('pt_core_news_lg')
         pipeline['pt'] = spacy.load('pt_core_news_lg')
 
     elif lang == "en":
-
+        spacy.cli.download('en_core_web_sm')
         if not(spacy.util.is_package('en_core_web_lg')):
             spacy.cli.download('en_core_web_lg')
 
         pipeline['en'] = spacy.load('en_core_web_lg')
     else:
         raise InvalidLanguage(lang)
```

### Comparing `text2story-1.2.9/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.3.0/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/SRLWeakLabeling/__init__.py` & `text2story-1.3.0/text2story/annotators/SRLWeakLabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/annotators/__init__.py` & `text2story-1.3.0/text2story/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/brat2viz/README.md` & `text2story-1.3.0/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.3.0/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # %%
 # Brat2DRT
 
 import re
 import glob
 import os
+import string
 
 import platform
 
 from pathlib import Path
 
 # DRT
 from nltk.sem import logic
@@ -230,16 +231,17 @@
             for x in dexpr_list:
 
                 if "event_str" not in x[0].keys():
                     continue
 
                 var = dexpr('%s' % x[0].get('event_var'))
                 event_str = ''.join([x.capitalize() for x in x[0].get('event_str').split()])
+                #event_str = event_str.replace('-', '')
+                event_str = "".join([c for c in event_str if c not in string.punctuation])
                 event_str = event_str + '=' + x[0].get('event_var')
-                event_str = event_str.replace('-', '')
                 var_ = dexpr('%s' % event_str)
                 tmp_dr = []
 
                 for y in dr_set:
                     tmp_dr = tmp_dr + [str(y) for x in list(x)
                     [1:-1] if re.search(y, str(x))]
```

### Comparing `text2story-1.2.9/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.3.0/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/brat2viz/drs2viz/app.py` & `text2story-1.3.0/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.3.0/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/core/annotator.py` & `text2story-1.3.0/text2story/core/annotator.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/core/entity_structures.py` & `text2story-1.3.0/text2story/core/entity_structures.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,28 +56,39 @@
     type: str
         The type of the time.
         Possible values are: 'Date', 'Time', 'Duration' and 'Set'.
     temporal_function: str
         Possible values are: 'None' or 'Publication_Time'.
     """
 
-    def __init__(self, text, character_span, value, timex_type, temporal_function='Publication_Time'):
+    def __init__(self, text, character_span, timex_type, temporal_function='Publication_Time'):
         self.text = text
         self.character_span = character_span
-        self.value = value
+        #self.value = value
         self.type = timex_type
         self.temporal_function = temporal_function
 
 
 class EventEntity:
     """
     Representation of an event entity.
         TODO: Annotations (A)
     """
 
-    def __init__(self, text, character_span, event_class="Occurrence", polarity="Pos"):
+    def __init__(self, text, character_span,**kwargs):
         self.text = text
         self.character_span = character_span
-        self.event_class = event_class
-        self.polarity = polarity
+
+        for attr_name, attr_value in kwargs.items():
+            setattr(self,attr_name, attr_value)
+
         self.factuality = "Factual"
         self.tense = "Pres"
+
+class SpatialRelationEntity:
+    def __init__(self, text, character_span,**kwargs):
+        self.text = text
+        self.character_span = character_span
+
+        for attr_name, attr_value in kwargs.items():
+            setattr(self,attr_name, attr_value)
+
```

### Comparing `text2story-1.2.9/text2story/core/narrative.py` & `text2story-1.3.0/text2story/core/narrative.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 	text2story.core.narrative
 
 	Narrative class
 """
+import warnings
 
 from text2story.core.annotator import Annotator
 from text2story.core.entity_structures import *
 from text2story.core.link_structures import *
-from text2story.core.utils import pairwise
+from text2story.core.utils import pairwise, capfirst, join_tokens
 
 
 class Narrative:
     """
     Representation of a narrative.
 
     Attributes
@@ -70,16 +71,142 @@
         self._id = 1
         self._event_id = 1
         self._rel_id = 1
 
         self.actors = {}
         self.times = {}
         self.events = {}
-        self.obj_links = {}
-        self.sem_links = {}
+        self.spatial_relations = {}
+
+        self.links = {}
+        #self.obj_links = {}
+        #self.sem_links = {}
+
+        #self.temp_links = {}
+        #self.subordination_links = {}
+        #self.qualitative_spatial_links = {}
+        #self.movement_links = {}
+        # self.measure_links = {}
+
+
+
+    @classmethod
+    def fromTokenCorpus(cls, lang,  doc):
+        """
+        build a narrative object from a list of TokenCorpus objects
+
+        @return: a narrative object
+
+        """
+
+        cls.lang = lang
+        cls.publication_time = None
+
+        cls.actors = {}
+        cls.times = {}
+        cls.events = {}
+        cls.spatial_relations = {}
+        cls.links = {}
+
+        # first collect only the annotations
+        n = len(doc)
+        i = 0
+        map_id_tok = {}
+        rel_set = set()
+        doc_txt = ""
+        while i < n:
+
+            for idx, id_ann in enumerate(doc[i].id_ann):
+                if id_ann in map_id_tok:
+                    map_id_tok[id_ann] = (map_id_tok[id_ann][0] + [i],\
+                                          map_id_tok[id_ann][1],\
+                                          map_id_tok[id_ann][2])
+                else:
+                    ann_type, ann_map = doc[i].attr[idx]
+                    map_id_tok[id_ann] = ([i], ann_type, ann_map)
+
+            # collect relations
+            for rel in doc[i].relations:
+                if rel.rel_id not in rel_set:
+
+                    rel_type = rel.rel_type.split("_")
+
+                    main_type = rel_type[0]
+                    subtype = rel_type[1]
+                    if rel.argn == "arg2":
+                        arg1 = doc[i].id_ann[0]
+                        arg2 = rel.toks[0].id_ann[0]
+                    else:
+                        arg2 = doc[i].id_ann[0]
+                        arg1 = rel.toks[0].id_ann[0]
+
+                    linkObj = createLinkObject(arg1,arg2,main_type, subtype, rel.rel_id)
+                    if main_type in cls.links:
+                        cls.links[main_type].append(linkObj)
+                    else:
+                        cls.links[main_type] = [linkObj]
+
+                    rel_set.add(rel.rel_id)
+
+            doc_txt = doc_txt + doc[i].text + " "
+            i += 1
+
+        for id_ann in map_id_tok:
+            # the tokens of this annotation
+            idx_lst, ann_type, ann_map = map_id_tok[id_ann]
+            text = [doc[i].text for i in idx_lst]
+            text = join_tokens(text)
+
+            span_start = doc[idx_lst[0]].offset
+            span_end = doc[idx_lst[-1]].offset + len(doc[idx_lst[-1]].text)
+
+            if ann_type == "Participant":
+
+                lexical_head = ann_map.get("Lexical_Head","")
+
+                participant_type = ann_map.get("Participant_Type_Domain","")
+                cls.actors[id_ann] = ActorEntity(text, (span_start, span_end), lexical_head, actor_type=participant_type)
+            elif ann_type == "Event":
+                event_class = ann_map.get("Class", "")
+                event_polarity = ann_map.get("Polarity","Pos")
+                event_type = ann_map.get("Event_Type","Occurrence")
+                event_pos = ann_map.get("Pos","Verb")
+                event_tense = ann_map.get("Tense","Pres")
+                event_aspect = ann_map.get("Aspect","Perfective")
+
+                cls.events[id_ann] = EventEntity(text, (span_start, span_end),event_class=event_class,\
+                                                 polarity=event_polarity,type=event_type,pos=event_pos,\
+                                                 tense=event_tense,aspect=event_aspect)
+            elif ann_type == "Time":
+                # annotations :: [(TimeStartOffset, TimeEndOffset, TimeType, TimeValue)]
+                time_type = ann_map.get("Time_Type","Time")
+                temporal_function = ann_map.get("TemporalFunction","Publication_Time")
+                cls.times[id_ann] = TimeEntity(text,(span_start,span_end),
+                                                                 time_type, temporal_function=temporal_function)
+            elif ann_type == "Spatial_Relation":
+                spatial_relation_type = ann_map.get("Type","Topological")
+                topological = ann_map.get("Topological","Equal")
+                pathDefining = ann_map.get("PathDefining","Starts")
+                cls.spatial_relations[id_ann] = SpatialRelationEntity(text, (span_start, span_end),\
+                                                                      type=spatial_relation_type,\
+                                                                      topological=topological,
+                                                                      pathDefining=pathDefining)
+
+            else:
+                warnings.warn("Annotation type not recognized: %s -> %s" % (id_ann, ann_type))
+
+
+
+        narrativeSelf = cls(lang,doc_txt,"2023")
+        narrativeSelf.actors = cls.actors
+        narrativeSelf.events = cls.events
+        narrativeSelf.times = cls.times
+        narrativeSelf.spatial_relations = cls.spatial_relations
+        narrativeSelf.links = cls.links
+        return narrativeSelf
 
     def extract_actors(self, *tools):
         """
         Parameters
         ----------
         tools : str, ...
                 the tools to be used in the annotation
@@ -152,14 +279,15 @@
         -------
                 self.obj_rels updated
         """
 
         # annotations ::
         clusters = Annotator(tools).extract_objectal_links(
             self.lang, self.text)
+        obj_links = {}
 
         for cluster in clusters:
             for i in range(0, len(cluster) - 1):
                 e1 = cluster[i]
                 e2 = cluster[i + 1]
 
                 # Get the actors
@@ -168,19 +296,20 @@
                 # If one of them wasn't identified in the actor extration, add it as a new actor
                 if arg1 == None:
                     arg1 = self._add_actor(e1)
                 if arg2 == None:
                     arg2 = self._add_actor(e2)
 
                 # (Type (sameHead, partOf, ...), Arg1, Arg2)
-                self.obj_links['R' + str(self._rel_id)
-                               ] = ObjectalLink(arg1, arg2)
+                obj_links['R' + str(self._rel_id)
+                               ] = ObjectalLink(arg1, arg2, "R" + str(self._rel_id))
                 self._rel_id += 1
 
-        return self.obj_links
+        self.links["OLINK"] = obj_links
+        return obj_links
 
     def extract_semantic_role_links(self, *tools):
         """
         Find semantic role links between extracted actors and events.
         Since the SRL model is different from the NER model, this function maps actors found by the SRL model into
         actors that were already extracted. If the actor was not yet extracted, it adds a new one.
 
@@ -226,37 +355,39 @@
                 #    actor_key = self._add_actor(
                 #        row.char_span, lexical_head="Noun", actor_type="Other")
                 #    key_list.append(actor_key)
             
             sentence_df["key"] = key_list
 
         # MAKE SEMANTIC ROLE LINK ENTITIES
+        sem_links = {}
         for sentence_df in srl_by_sentence:
             for row1, row2 in pairwise(sentence_df.itertuples()):
                 sem1 = row1.sem_role_type
                 sem2 = row2.sem_role_type
 
                 if (sem1 == "EVENT") | (sem2 == "EVENT"):
                     if sem1 != "EVENT":
                         sem_role, actor, event = sem1, row1.key, row2.key
                     else:
                         sem_role, actor, event = sem2, row2.key, row1.key
 
                     if actor == "None" or event == "None":
                         continue
 
-                    self.sem_links["R" + str(self._rel_id)] = SemanticRoleLink(
-                        actor, event, sem_role.lower())
+                    sem_links["R" + str(self._rel_id)] = SemanticRoleLink(
+                        actor, event, sem_role.lower(), "R" + str(self._rel_id))
                     self._rel_id += 1
 
-        return self.sem_links
+        self.links["SRLINK"] =sem_links
+        return sem_links
 
     def _add_srlink(self, actor, event, sem_role):
-        self.sem_links["R" + str(self._rel_id)
-                       ] = SemanticRoleLink(actor, event, sem_role.lower())
+        self.links["SRLINKS"]["R" + str(self._rel_id)
+                       ] = SemanticRoleLink(actor, event, sem_role.lower(), "R" + str(self._rel_id))
         self._rel_id += 1
 
     def _get_actor_key(self, char_span, match_type="exact"):
         """
         Parameters
         ----------
         char_span : (int, int)
@@ -431,14 +562,26 @@
 
             # A107 FunctionInDocument T4 Publication_Time
             # r += ('A' + str(attribute_id) + '\t' + 'FunctionInDocument' + ' ' + time_id + ' ' + time.temporal_function + '\n')
             r += ('A' + str(attribute_id) + '\t' + 'TemporalFunction' +
                   ' ' + time_id + ' ' + time.temporal_function + '\n')
             attribute_id += 1
 
+        for spatialRelation_id in self.spatial_relations:
+            spatialRelation = self.spatial_relations[spatialRelation_id]
+
+            r += (spatialRelation_id + '\t' + 'Spatial_Relation' + ' ' + str(spatialRelation.character_span[0]) + ' ' + str(
+                spatialRelation.character_span[1]) + '\t' + spatialRelation.text + '\n')
+
+            attr_dct = vars(spatialRelation)
+            for att in attr_dct:
+                if att != "character_span" and att != "text":
+                    r +=(f"A{attribute_id}\t{capfirst(att)} {spatialRelation_id} {attr_dct[att]}\n")
+                    attribute_id += 1
+
         for event_id in self.events:
 
             event = self.events[event_id]
             if len(event.text.strip()) == 0:
                 continue
             # T22 EVENT 312 328 is strengthening
             r += (event_id + '\t' + 'Event' + ' ' + str(event.character_span[0]) + ' ' + str(
@@ -457,23 +600,12 @@
             attribute_id += 1
 
             #r += (f"A{attribute_id}\tFactuality {event_id} {event.factuality}\n")
             #import pdb
             # pdb.set_trace()
             attribute_id += 1
 
-        for objectal_link_id in self.obj_links:
-            obj_link = self.obj_links[objectal_link_id]
-
-            # R34 OBJ_REL_objIdentity Arg1:T3 Arg2:T1
-            #r += (objectal_link_id + '\t' + 'OBJ_REL_' + obj_link.type + ' ' + 'Arg1:' + obj_link.arg1 + ' ' + 'Arg2:' + obj_link.arg2 + '\n')
-            r += (objectal_link_id + '\t' + 'OLINK_' + obj_link.type + ' ' +
-                  'Arg1:' + obj_link.arg1 + ' ' + 'Arg2:' + obj_link.arg2 + '\n')
-
-        for sem_link_id in self.sem_links:
-            sem_link = self.sem_links[sem_link_id]
-
-            # R35 SEMROLE_theme Arg1:E1 Arg2:T1
-        #	r += (f"{sem_link_id}\tSEMROLE_{sem_link.type} Arg1:{sem_link.event} Arg2:{sem_link.actor}\n")
-            r += (f"{sem_link_id}\tSRLINK_{sem_link.type} Arg1:{sem_link.event} Arg2:{sem_link.actor}\n")
+        for link_type in self.links:
+            for link in self.links[link_type]:
+                r += str(link) + "\n"
 
         return r
```

### Comparing `text2story-1.2.9/text2story/experiments/evaluation.py` & `text2story-1.3.0/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/experiments/metrics.py` & `text2story-1.3.0/text2story/experiments/metrics.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/experiments/run_experiments.py` & `text2story-1.3.0/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/readers/pb-vn2.json` & `text2story-1.3.0/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/readers/read.py` & `text2story-1.3.0/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/readers/read_brat.py` & `text2story-1.3.0/text2story/readers/read_brat.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,15 +515,19 @@
 
 
                 elif line[0] == 'A':
 
                     ref = line_toks[2]
                     if ref in ann_ref:
                         #ann_ref[ref][1].append((line[1], line[3]))
-                        ann_ref[ref][line_toks[1]] = line_toks[3]
+                        if len(line_toks) > 3:
+                            ann_ref[ref][line_toks[1]] = line_toks[3]
+                        else:
+                            ann_ref[ref][line_toks[1]] = line_toks[1]
+
                     else:
                         ann_ref[ref] = {line_toks[1]:line_toks[3]}
 
         idx_lst = ann.keys()
 
         idx_lst = sorted(idx_lst, key=lambda elem: elem[0])
 
@@ -630,14 +634,15 @@
             m = int((b + e) / 2)
 
         return pos
 
     def __process_annotations(self, file_ann, ann, ann_ref):
         pass
 
+
     def fileToColumnFormat(self, ann_file, output_file):
         """
         Convert only one file to the column format.
 
         @param string: path of annotation file
         @param string: path of output file
```

### Comparing `text2story-1.2.9/text2story/readers/read_ecb.py` & `text2story-1.3.0/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/readers/read_framenet.py` & `text2story-1.3.0/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/readers/read_propbank.py` & `text2story-1.3.0/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/readers/token_corpus.py` & `text2story-1.3.0/text2story/readers/token_corpus.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/readers/utils.py` & `text2story-1.3.0/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/select/bubble.py` & `text2story-1.3.0/text2story/select/bubble.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/select/event.py` & `text2story-1.3.0/text2story/select/event.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/text2viz/Text2Viz.py` & `text2story-1.3.0/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/text2viz/visualization.py` & `text2story-1.3.0/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/training/participant_concept.py` & `text2story-1.3.0/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.2.9/text2story/viz/bubble_tikz.py` & `text2story-1.3.0/text2story/viz/bubble_tikz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from text2story.select.bubble import BubbleMap, BigBubble, Bubble 
 from text2story.readers.read_brat import ReadBrat
-import pdflatex as ptex
 from pdf2image import convert_from_path
 
 import os
 import re
 import sys
 
+from latexcompiler import LC
+
 tikz_doc = "\\documentclass{standalone}\n\\usepackage{pgf,tikz}\n\\usetikzlibrary{arrows}\n\\usepackage{listofitems} % for \\readlist to create arrays"
 
 def bubble_header():
     return '''
 \\usepackage[T1]{fontenc}
 \\usetikzlibrary{calc}
 \\usetikzlibrary{arrows.meta}
@@ -400,35 +401,39 @@
 
     reader = ReadBrat()
     data = reader.process_file(ann_file)
 
     #Serao apenas as relações temporais que nao envolvam reporting events ligado pelo TLINK identity.
     tikz_str, bubble_map = build_fig(data, "Reporting", ["TLINK"])
 
-    bubble_map.to_json("output.txt")
+    bubble_map.to_json(os.path.join(output_dir,"output.txt"))
 
     ann_file_base = os.path.basename(ann_file)
 
     output_file = os.path.join(output_dir, "%s.tex" % ann_file_base)
     with open(output_file, "w") as fd:
         fd.write(tikz_str)
 
-    pdfl = ptex.PDFLaTeX.from_texfile(output_file)
+    LC.compile_document(tex_engine="pdflatex", bib_engine="bibtex",no_bib=True, path=output_file, folder_name=output_dir)
+    #pdfl = ptex.PDFLaTeX.from_texfile(output_file)
     #os.system("pdflatex -halt-on-error -output-directory %s %s" % (output_dir, output_file))
 
     pdf_file = os.path.join(output_dir, "%s.pdf" % ann_file_base)
 
-    pdf, log, completed_process = pdfl.create_pdf()
-    with open(pdf_file, 'wb') as pdfout:
-        pdfout.write(pdf)
+    #pdf, log, completed_process = pdfl.create_pdf()
+    #with open(pdf_file, 'wb') as pdfout:
+    #    pdfout.write(pdf)
 
     png_file = os.path.join(output_dir, "%s.png" % ann_file_base)
+    log_file = os.path.join(output_dir, "%s.log" % ann_file_base)
+    aux_file = os.path.join(output_dir, "%s.aux" % ann_file_base)
+    sync_file = os.path.join(output_dir, "%s.synctex.gz" % ann_file_base)
 
     pages = convert_from_path(pdf_file, 500)
     for page in pages:
         # usually only one page
         page.save(png_file, 'PNG')
 
     #os.system("convert  -density 600 %s  %s" % (pdf_file, png_file))
-    os.system("rm %s" % (pdf_file))
+    os.system("rm %s %s %s %s" % (pdf_file, log_file, aux_file, sync_file))
```

### Comparing `text2story-1.2.9/text2story.egg-info/SOURCES.txt` & `text2story-1.3.0/text2story.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 text2story/annotators/ALLENNLP/my_model.py
 text2story/annotators/ALLENNLP/my_reader.py
 text2story/annotators/ALLENNLP/preprocess.py
 text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
 text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
 text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
 text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+text2story/annotators/ALLENNLP/cache/config.json
 text2story/annotators/CUSTOMPT/__init__.py
 text2story/annotators/CUSTOMPT/crf_v2.1.joblib
 text2story/annotators/CUSTOMPT/event_model.py
 text2story/annotators/CUSTOMPT/feature_extractor.py
 text2story/annotators/NLTK/__init__.py
 text2story/annotators/PY_HEIDELTIME/__init__.py
 text2story/annotators/SPACY/__init__.py
@@ -45,14 +46,17 @@
 text2story/core/entity_structures.py
 text2story/core/exceptions.py
 text2story/core/link_structures.py
 text2story/core/narrative.py
 text2story/core/utils.py
 text2story/experiments/__init__.py
 text2story/experiments/evaluation.py
+text2story/experiments/exp.json
+text2story/experiments/exp_en_fn.json
+text2story/experiments/exp_en_pb.json
 text2story/experiments/metrics.py
 text2story/experiments/run_experiments.py
 text2story/experiments/stats.py
 text2story/readers/__init__.py
 text2story/readers/fn-lirics.json
 text2story/readers/pb-vn2.json
 text2story/readers/read.py
```

