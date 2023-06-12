# Comparing `tmp/rxn-reaction-preprocessing-2.0.3.tar.gz` & `tmp/rxn-reaction-preprocessing-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-reaction-preprocessing-2.0.3.tar", last modified: Wed May  3 08:55:28 2023, max compression
+gzip compressed data, was "rxn-reaction-preprocessing-2.1.0.tar", last modified: Mon Jun 12 15:11:58 2023, max compression
```

## Comparing `rxn-reaction-preprocessing-2.0.3.tar` & `rxn-reaction-preprocessing-2.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.576044 rxn-reaction-preprocessing-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-03 08:55:28.576044 rxn-reaction-preprocessing-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-03 08:55:28.576044 rxn-reaction-preprocessing-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.556044 rxn-reaction-preprocessing-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.556044 rxn-reaction-preprocessing-2.0.3/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.564044 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.564044 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/annotation_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/annotation_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/missing_annotation_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/molecule_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/molecule_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/rejected_molecules_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.556044 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.568044 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/
--rw-r--r--   0 runner    (1001) docker     (123)   483074 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210428.json
--rw-r--r--   0 runner    (1001) docker     (123)   116582 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210826.json
--rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-200302.json
--rw-r--r--   0 runner    (1001) docker     (123)    18321 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-210428.json
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/importer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2930 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/mixed_reaction_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/molecule_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/pistachio_record_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/reaction_standardizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.568044 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/annotation_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/combine_class_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/find_missing_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/standardize_pistachio_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/smiles_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/special_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/stable_data_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.572044 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-03 08:55:28.000000 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-03 08:55:28.000000 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:55:28.000000 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 08:55:28.000000 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:55:28.000000 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 08:55:28.000000 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 08:55:28.000000 rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:55:28.572044 rxn-reaction-preprocessing-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_mixed_reaction_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_molecule_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_pistachio_record_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_reaction_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_smiles_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_special_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_stable_data_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-03 08:55:17.000000 rxn-reaction-preprocessing-2.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.308712 rxn-reaction-preprocessing-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-12 15:11:58.308712 rxn-reaction-preprocessing-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-12 15:11:58.308712 rxn-reaction-preprocessing-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.296712 rxn-reaction-preprocessing-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.296712 rxn-reaction-preprocessing-2.1.0/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.300712 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.304712 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/annotation_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/annotation_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/missing_annotation_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/molecule_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/molecule_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/rejected_molecules_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.296712 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.304712 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/
+-rw-r--r--   0 runner    (1001) docker     (123)   483074 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210428.json
+-rw-r--r--   0 runner    (1001) docker     (123)   116582 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210826.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-200302.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18321 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-210428.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/importer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2930 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/mixed_reaction_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/molecule_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/pistachio_record_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/reaction_standardizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.304712 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/annotation_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/combine_class_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/find_missing_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/standardize_pistachio_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/smiles_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/special_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/stable_data_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.304712 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-12 15:11:58.000000 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-12 15:11:58.000000 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:11:58.000000 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-12 15:11:58.000000 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:11:58.000000 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-12 15:11:58.000000 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 15:11:58.000000 rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:11:58.308712 rxn-reaction-preprocessing-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_mixed_reaction_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_molecule_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_pistachio_record_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_reaction_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_smiles_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_special_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_stable_data_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-12 15:11:49.000000 rxn-reaction-preprocessing-2.1.0/tests/test_utils.py
```

### Comparing `rxn-reaction-preprocessing-2.0.3/LICENSE` & `rxn-reaction-preprocessing-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/PKG-INFO` & `rxn-reaction-preprocessing-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: rxn-reaction-preprocessing
-Version: 2.0.3
+Version: 2.1.0
 Summary: Reaction preprocessing tools
+Home-page: https://github.com/rxn4chemistry/rxn-reaction-preprocessing
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
+Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-reaction-preprocessing/
+Project-URL: Repository, https://github.com/rxn4chemistry/rxn-reaction-preprocessing
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `rxn-reaction-preprocessing-2.0.3/README.md` & `rxn-reaction-preprocessing-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/setup.cfg` & `rxn-reaction-preprocessing-2.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 version = attr: rxn.reaction_preprocessing.__version__
 description = Reaction preprocessing tools
 author = IBM RXN team
 author_email = rxn4chemistry@zurich.ibm.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
+url = https://github.com/rxn4chemistry/rxn-reaction-preprocessing
+project_urls = 
+	Documentation = https://rxn4chemistry.github.io/rxn-reaction-preprocessing/
+	Repository = https://github.com/rxn4chemistry/rxn-reaction-preprocessing
 classifiers = 
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
+	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
@@ -62,15 +67,15 @@
 	pytest-cov>=2.10.1
 	pytest>=6.1.2
 	types-click>=7.1.1
 	types-dataclasses>=0.1.4
 	types-setuptools>=57.4.2
 	types-tabulate>=0.1.0
 rdkit = 
-	rdkit-pypi>=2021.3.2
+	rdkit>=2022.3.3
 
 [flake8]
 extend-ignore = E501
 exclude = __init__.py
 
 [egg_info]
 tag_build =
```

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/__init__.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .preprocessor import Preprocessor
 from .smiles_tokenizer import SmilesTokenizer
 from .stable_data_splitter import StableDataSplitter
 from .standardizer import Standardizer
 from .utils import RandomType
 
 __name__ = "rxn-reaction-preprocessing"
-__version__ = "2.0.3"  # managed by bump2version
+__version__ = "2.1.0"  # managed by bump2version
 __all__ = [
     "Augmenter",
     "MixedReactionFilter",
     "Preprocessor",
     "RandomType",
     "SmilesTokenizer",
     "StableDataSplitter",
```

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/annotation_criterion.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/annotation_criterion.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/annotation_info.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/annotation_info.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/missing_annotation_detector.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/missing_annotation_detector.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/molecule_annotation.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/molecule_annotation.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/molecule_replacer.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/molecule_replacer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/annotations/rejected_molecules_filter.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/annotations/rejected_molecules_filter.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/augmenter.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/config.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 @dataclass
 class RxnImportConfig:
     """Configuration for the initial import of the reaction data.
 
     Fields:
         input_file: the input file path (.txt, .csv).
-        output_csv: the ouptut file path.
+        output_csv: the output file path.
         initial_data_format: whether the input file is in TXT or CSV format.
         reaction_column_name: name the column containing the reactions if the input
             is in CSV format. The value is ignored if the input is not in CSV format.
         reaction_column_name: how to name the column with the reaction SMILES in
             the output CSV.
         fragment_bond: token denoting a fragment bond in the reaction SMILES (after import).
         remove_atom_mapping: whether to remove the atom mapping from the input reaction SMILES.
@@ -210,25 +210,26 @@
     """Configuration for the split transformation step.
 
     Fields:
         input_file_path: The input file path.
         output_directory: The directory containing the files after splitting.
         split_ratio: The split ratio between training, and test and validation sets.
         reaction_column_name: Name of the reaction column for the data file.
-        index_column: Name of the column used to generate the hash ensuring
-            stable splitting.
+        index_column: The name of the column used to generate the hash which ensures
+            stable splitting. "products" and "precursors" are also allowed even if
+            they do not exist as columns.
         hash_seed: Seed for the hashing function used for splitting.
         shuffle_seed: Seed for shuffling the train split.
     """
 
     input_file_path: str = SI("${preprocess.output_file_path}")
     output_directory: str = SI("${data.proc_dir}")
     split_ratio: float = 0.05
     reaction_column_name: str = SI("${common.reaction_column_name}")
-    index_column: str = SI("${split.reaction_column_name}")
+    index_column: str = "products"
     hash_seed: int = 42
     shuffle_seed: int = 42
 
 
 @dataclass
 class InputOutputTuple:
     inp: str = MISSING
```

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210428.json` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210428.json`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210826.json` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/catalyst-annotation-210826.json`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-200302.json` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-200302.json`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-210428.json` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/data/standardization-files/pistachio-210428.json`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/importer.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/importer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/main.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/main.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/mixed_reaction_filter.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/mixed_reaction_filter.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/molecule_standardizer.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/molecule_standardizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/pistachio_record_standardizer.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/pistachio_record_standardizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/preprocessor.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/preprocessor.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/reaction_standardizer.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/reaction_standardizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/annotation_check.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/annotation_check.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/combine_class_token.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/combine_class_token.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/find_missing_annotations.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/find_missing_annotations.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/scripts/standardize_pistachio_records.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/scripts/standardize_pistachio_records.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/smiles_tokenizer.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/special_tokens.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/special_tokens.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/stable_data_splitter.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/stable_data_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         """Creates a stable split into training, validation, and test sets. Returns a boolean mask
         for each set, to not duplicate the DataFrame while preserving the original.
 
         Args:
             df: The pandas DataFrame to be split into training, validation, and test sets.
             reaction_column_name: Name of the reaction column for the data file.
             index_column: The name of the column used to generate the hash which ensures
-                stable splitting.
+                stable splitting. "products" and "precursors" are also allowed even if
+                they do not exist as columns.
             split_ratio: The split ratio. Defaults to 0.05.
             hash_seed: seed to use for hashing. The default of 0 corresponds to
                 the default value in the xxhash implementation.
             shuffle_seed: Seed for shuffling the train split.
 
         Returns:
             A tuple of three pandas DataFrames for the three splits.
```

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/standardizer.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/standardizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn/reaction_preprocessing/utils.py` & `rxn-reaction-preprocessing-2.1.0/src/rxn/reaction_preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/PKG-INFO` & `rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: rxn-reaction-preprocessing
-Version: 2.0.3
+Version: 2.1.0
 Summary: Reaction preprocessing tools
+Home-page: https://github.com/rxn4chemistry/rxn-reaction-preprocessing
 Author: IBM RXN team
 Author-email: rxn4chemistry@zurich.ibm.com
 License: MIT
+Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-reaction-preprocessing/
+Project-URL: Repository, https://github.com/rxn4chemistry/rxn-reaction-preprocessing
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `rxn-reaction-preprocessing-2.0.3/src/rxn_reaction_preprocessing.egg-info/SOURCES.txt` & `rxn-reaction-preprocessing-2.1.0/src/rxn_reaction_preprocessing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_augmenter.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_augmenter.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_importer.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_mixed_reaction_filter.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_mixed_reaction_filter.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_molecule_standardizer.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_molecule_standardizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_pistachio_record_standardizer.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_pistachio_record_standardizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_preprocessor.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_reaction_standardizer.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_reaction_standardizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_smiles_tokenizer.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_special_tokens.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_special_tokens.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_stable_data_splitter.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_stable_data_splitter.py`

 * *Files identical despite different names*

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_standardizer.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_standardizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         {
             "rxn": [
                 "O=C1CCC2(CC1)OCCO2>>O=C1CCC2(C[C@H]1C)OCCO2",  # stereo only in product
                 "O=C1CCC2(CC1)OCCO2>>O=C1CCC2(C[C@@H]1C)OCCO2",  # stereo only in product
                 "[Na]Cl.CC[Zn]CC~Cc1ccccc1>>[Na]Cl",  # substitution needed
                 "[Na]Cl.Cc1ccccc1~CC[Zn]CC>>[Na]Cl",  # substitution needed but performed only if canonicalization
                 "CC.CCC>>CCO",  # no substitution
-                "CC.[Na+5].CC>>[Na+]~[OH-]",  # invalid smiles -> '>>'
+                "CC.[NaK].CC>>[Na+]~[OH-]",  # invalid smiles -> '>>'
                 "CC(C)(C)O[K].CCO~CCO>>[Li]O",  # rejected reaction -> '>>'
                 r"CC(=O)/C=C(\C)O[V](=O)O/C(C)=C/C(C)=O.CCCC[N+](CCCC)(CCCC)CCCC~CCCC[N+](CCCC)(CCCC)CCCC~C1(=C(SC(=S)S1)[S-])[S-]~C1(=C(SC(=S)S1)[S-])[S-]~[Pd+2]>>O[K]",
                 # requires annotation -> '>>'
             ],
         }
     )
     annotations = load_annotations(annotations_file)
```

### Comparing `rxn-reaction-preprocessing-2.0.3/tests/test_utils.py` & `rxn-reaction-preprocessing-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

