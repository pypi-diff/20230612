# Comparing `tmp/text2story-1.3.0.tar.gz` & `tmp/text2story-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.3.0.tar", last modified: Mon Jun 12 15:00:19 2023, max compression
+gzip compressed data, was "text2story-1.3.1.tar", last modified: Mon Jun 12 15:31:48 2023, max compression
```

## Comparing `text2story-1.3.0.tar` & `text2story-1.3.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.819371 text2story-1.3.0/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.3.0/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.3.0/MANIFEST.in
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-12 15:00:19.819371 text2story-1.3.0/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7752 2023-05-30 12:31:10.000000 text2story-1.3.0/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2023-06-12 14:59:52.000000 text2story-1.3.0/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      989 2023-06-12 15:00:19.819371 text2story-1.3.0/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-05-26 15:16:02.000000 text2story-1.3.0/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.799371 text2story-1.3.0/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.799371 text2story-1.3.0/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.795371 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.803371 text2story-1.3.0/text2story/annotators/ALLENNLP/cache/
--rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)     4090 2021-03-09 07:42:06.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/cache/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/ALLENNLP/preprocess.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1553 2023-05-29 13:21:32.000000 text2story-1.3.0/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4406 2023-05-25 14:12:26.000000 text2story-1.3.0/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.3.0/text2story/annotators/SPARKNLP/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/annotators/SRLWeakLabeling/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.3.0/text2story/annotators/SRLWeakLabeling/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2394 2023-05-18 09:14:04.000000 text2story-1.3.0/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-05-30 10:06:48.000000 text2story-1.3.0/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.807371 text2story-1.3.0/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9846 2023-06-12 14:58:33.000000 text2story-1.3.0/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.811371 text2story-1.3.0/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.3.0/text2story/core/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.3.0/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2917 2023-06-09 14:36:29.000000 text2story-1.3.0/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      709 2023-06-09 13:29:38.000000 text2story-1.3.0/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2621 2023-06-09 14:35:24.000000 text2story-1.3.0/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    23131 2023-06-09 15:10:17.000000 text2story-1.3.0/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6935 2023-06-09 15:00:43.000000 text2story-1.3.0/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.811371 text2story-1.3.0/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.3.0/text2story/experiments/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/exp.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/exp_en_fn.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/exp_en_pb.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2870 2023-05-29 11:37:16.000000 text2story-1.3.0/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.3.0/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/fn-lirics.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/pb-vn2.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22827 2023-06-07 13:53:21.000000 text2story-1.3.0/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/utils.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/readers/vn-lirics.json
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/select/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/select/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.3.0/text2story/select/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/select/bubble.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.3.0/text2story/select/event.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.3.0/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.815371 text2story-1.3.0/text2story/training/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.3.0/text2story/training/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.3.0/text2story/training/participant_concept.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.819371 text2story-1.3.0/text2story/viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.3.0/text2story/viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15162 2023-06-01 12:14:40.000000 text2story-1.3.0/text2story/viz/bubble_tikz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:00:19.799371 text2story-1.3.0/text2story.egg-info/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2885 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      454 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-06-12 15:00:19.000000 text2story-1.3.0/text2story.egg-info/top_level.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.3.0/text2story.egg-info/zip-safe
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.3.1/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-03-29 14:01:55.000000 text2story-1.3.1/MANIFEST.in
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-12 15:31:48.525915 text2story-1.3.1/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7752 2023-05-30 12:31:10.000000 text2story-1.3.1/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      417 2023-06-12 15:31:36.000000 text2story-1.3.1/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      989 2023-06-12 15:31:48.529915 text2story-1.3.1/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-05-26 15:16:02.000000 text2story-1.3.1/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.517915 text2story-1.3.1/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25595 2023-05-22 15:42:56.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/ALLENNLP/cache/
+-rw-r--r--   0 evelinamorim  (1000) evelinamorim  (1000)     4090 2021-03-09 07:42:06.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/cache/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/ALLENNLP/preprocess.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1553 2023-05-29 13:21:32.000000 text2story-1.3.1/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4406 2023-05-25 14:12:26.000000 text2story-1.3.1/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.3.1/text2story/annotators/SPARKNLP/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/annotators/SRLWeakLabeling/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     3501 2023-05-22 15:42:57.000000 text2story-1.3.1/text2story/annotators/SRLWeakLabeling/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2394 2023-05-18 09:14:04.000000 text2story-1.3.1/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17359 2023-05-30 10:06:48.000000 text2story-1.3.1/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.3.1/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9846 2023-06-12 14:58:33.000000 text2story-1.3.1/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:48:21.000000 text2story-1.3.1/text2story/core/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-03 10:32:35.000000 text2story-1.3.1/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2917 2023-06-12 15:28:35.000000 text2story-1.3.1/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      709 2023-06-09 13:29:38.000000 text2story-1.3.1/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2621 2023-06-09 14:35:24.000000 text2story-1.3.1/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    23368 2023-06-12 15:31:23.000000 text2story-1.3.1/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6935 2023-06-09 15:00:43.000000 text2story-1.3.1/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:04.000000 text2story-1.3.1/text2story/experiments/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      429 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/experiments/exp.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      205 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/experiments/exp_en_fn.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      601 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/experiments/exp_en_pb.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2870 2023-05-29 11:37:16.000000 text2story-1.3.1/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-09 12:20:40.000000 text2story-1.3.1/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22827 2023-06-07 13:53:21.000000 text2story-1.3.1/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-03-27 13:07:12.000000 text2story-1.3.1/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-03-27 13:07:12.000000 text2story-1.3.1/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:09.000000 text2story-1.3.1/text2story/select/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-03-27 13:07:12.000000 text2story-1.3.1/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-03-27 13:07:12.000000 text2story-1.3.1/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.3.1/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/training/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-03 11:20:54.000000 text2story-1.3.1/text2story/training/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14422 2023-05-22 12:41:48.000000 text2story-1.3.1/text2story/training/participant_concept.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.525915 text2story-1.3.1/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-16 11:49:13.000000 text2story-1.3.1/text2story/viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15162 2023-06-01 12:14:40.000000 text2story-1.3.1/text2story/viz/bubble_tikz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-06-12 15:31:48.521915 text2story-1.3.1/text2story.egg-info/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7933 2023-06-12 15:31:48.000000 text2story-1.3.1/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2885 2023-06-12 15:31:48.000000 text2story-1.3.1/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-06-12 15:31:48.000000 text2story-1.3.1/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      454 2023-06-12 15:31:48.000000 text2story-1.3.1/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2023-06-12 15:31:48.000000 text2story-1.3.1/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-26 15:56:54.000000 text2story-1.3.1/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.3.0/LICENSE` & `text2story-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/PKG-INFO` & `text2story-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.3.0
+Version: 1.3.1
 Project-URL: Source, https://github.com/LIAAD/Text2StoryPackage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
```

### Comparing `text2story-1.3.0/README.md` & `text2story-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/setup.cfg` & `text2story-1.3.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description-file = README.md
 name = text2story
-version = 1.3.0
+version = 1.3.1
 project_urls = 
 	Source =  https://github.com/LIAAD/Text2StoryPackage
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
```

### Comparing `text2story-1.3.0/text2story/__init__.py` & `text2story-1.3.1/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.3.1/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.3.1/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.3.1/text2story/annotators/ALLENNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/cache/config.json` & `text2story-1.3.1/text2story/annotators/ALLENNLP/cache/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.3.1/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.3.1/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.3.1/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.3.1/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.3.1/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.3.1/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.3.1/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/NLTK/__init__.py` & `text2story-1.3.1/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.3.1/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/SPACY/__init__.py` & `text2story-1.3.1/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.3.1/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/SRLWeakLabeling/__init__.py` & `text2story-1.3.1/text2story/annotators/SRLWeakLabeling/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/annotators/__init__.py` & `text2story-1.3.1/text2story/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/brat2viz/README.md` & `text2story-1.3.1/text2story/brat2viz/README.md`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.3.1/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.3.1/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/brat2viz/drs2viz/app.py` & `text2story-1.3.1/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.3.1/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.3.1/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/core/annotator.py` & `text2story-1.3.1/text2story/core/annotator.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/core/entity_structures.py` & `text2story-1.3.1/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/core/exceptions.py` & `text2story-1.3.1/text2story/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/core/link_structures.py` & `text2story-1.3.1/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/core/narrative.py` & `text2story-1.3.1/text2story/core/narrative.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,16 @@
         events = Annotator(tools).extract_events(self.lang, self.text)
         if len(events) == 0:
             self.events = []
             return []
 
         for event in events.itertuples():
             self.events["T" + str(self._id)
-                        ] = EventEntity(event.actor, event.char_span)
+                        ] = EventEntity(event.actor, event.char_span, event_class="Occurrence",\
+                                        polarity="Pos", factuality="Factual",tense="Pres")
             self._id += 1
 
         return self.events
 
     def extract_objectal_links(self, *tools):
         """
         Parameters
@@ -474,15 +475,16 @@
 
         @param char_span: tuple of characters (first_char, last_char) that delimit the event
 
         @return: The key of the new added event
         """
         key = 'T' + str(self._id)
         self.events[key] = EventEntity(
-            self.text[char_span[0]:char_span[1]], char_span)
+            self.text[char_span[0]:char_span[1]], char_span,  event_class="Occurrence",\
+                                        polarity="Pos", factuality="Factual",tense="Pres")
 
         self._id += 1
 
         return key
 
     def _add_time(self, char_span):
         """
```

### Comparing `text2story-1.3.0/text2story/core/utils.py` & `text2story-1.3.1/text2story/core/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/experiments/evaluation.py` & `text2story-1.3.1/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/experiments/exp_en_pb.json` & `text2story-1.3.1/text2story/experiments/exp_en_pb.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/experiments/metrics.py` & `text2story-1.3.1/text2story/experiments/metrics.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/experiments/run_experiments.py` & `text2story-1.3.1/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/experiments/stats.py` & `text2story-1.3.1/text2story/experiments/stats.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/pb-vn2.json` & `text2story-1.3.1/text2story/readers/pb-vn2.json`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/read.py` & `text2story-1.3.1/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/read_brat.py` & `text2story-1.3.1/text2story/readers/read_brat.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/read_ecb.py` & `text2story-1.3.1/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/read_framenet.py` & `text2story-1.3.1/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/read_propbank.py` & `text2story-1.3.1/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/token_corpus.py` & `text2story-1.3.1/text2story/readers/token_corpus.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/readers/utils.py` & `text2story-1.3.1/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/select/bubble.py` & `text2story-1.3.1/text2story/select/bubble.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/select/event.py` & `text2story-1.3.1/text2story/select/event.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/text2viz/Text2Viz.py` & `text2story-1.3.1/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/text2viz/visualization.py` & `text2story-1.3.1/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/training/participant_concept.py` & `text2story-1.3.1/text2story/training/participant_concept.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story/viz/bubble_tikz.py` & `text2story-1.3.1/text2story/viz/bubble_tikz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.3.0/text2story.egg-info/PKG-INFO` & `text2story-1.3.1/text2story.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.3.0
+Version: 1.3.1
 Project-URL: Source, https://github.com/LIAAD/Text2StoryPackage
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
```

### Comparing `text2story-1.3.0/text2story.egg-info/SOURCES.txt` & `text2story-1.3.1/text2story.egg-info/SOURCES.txt`

 * *Files identical despite different names*

