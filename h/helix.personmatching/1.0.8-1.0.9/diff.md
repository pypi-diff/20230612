# Comparing `tmp/helix.personmatching-1.0.8.tar.gz` & `tmp/helix.personmatching-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/helix.personmatching-1.0.8.tar", last modified: Wed Dec 21 19:04:50 2022, max compression
+gzip compressed data, was "dist/helix.personmatching-1.0.9.tar", last modified: Wed Dec 21 19:19:24 2022, max compression
```

## Comparing `helix.personmatching-1.0.8.tar` & `helix.personmatching-1.0.9.tar`

### file list

```diff
@@ -1,70 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      521 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix.personmatching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix.personmatching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix.personmatching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix.personmatching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix.personmatching.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix.personmatching.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix.personmatching.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/fhir_to_dict_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/test_fhir_to_dict_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/logics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/match_score.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/match_score_without_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/rule_attribute_score.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/rule_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/rules_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/score_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/logics/scoring_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match/test_exact_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_bundle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_bundle/test_exact_match_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_list/test_exact_match_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/human_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/human_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/human_api/partial_match/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/human_api/partial_match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/human_api/partial_match/test_hapi_partial_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/walgreens/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/walgreens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/walgreens/partial_match/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/walgreens/partial_match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/matchers/test/walgreens/partial_match/test_walgreens_partial_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/models/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/helix_personmatching/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/helix_personmatching/utils/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2022-12-21 19:04:49.000000 helix.personmatching-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:50.000000 helix.personmatching-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:04:05.000000 helix.personmatching-1.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix.personmatching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix.personmatching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix.personmatching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix.personmatching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix.personmatching.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix.personmatching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix.personmatching.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/fhir_to_dict_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/test_fhir_to_dict_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/logics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/match_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/match_score_without_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/rule_attribute_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/rule_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/rules_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/score_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/logics/scoring_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match/test_exact_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_bundle/test_exact_match_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_list/test_exact_match_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/human_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/human_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/human_api/partial_match/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/human_api/partial_match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/human_api/partial_match/test_hapi_partial_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match/test_walgreens_partial_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match_with_extra_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match_with_extra_rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match_with_extra_rule/test_walgreens_partial_match_with_extra_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match_with_extra_rule_and_custom_weights/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match_with_extra_rule_and_custom_weights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match_with_extra_rule_and_custom_weights/test_walgreens_partial_match_with_extra_rule_and_custom_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/models/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/models/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/models/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/models/rules/attribute_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/models/rules/fixed_score_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/models/scoring_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/helix_personmatching/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/helix_personmatching/utils/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 19:19:24.000000 helix.personmatching-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 19:18:25.000000 helix.personmatching-1.0.9/tests/__init__.py
```

### Comparing `helix.personmatching-1.0.8/LICENSE` & `helix.personmatching-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/Makefile` & `helix.personmatching-1.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/PKG-INFO` & `helix.personmatching-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.personmatching
-Version: 1.0.8
+Version: 1.0.9
 Summary: helix.personmatching
 Home-page: https://github.com/icanbwell/helix.personmatching
 Author: Imran Qureshi
 Author-email: imran@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `helix.personmatching-1.0.8/helix.personmatching.egg-info/PKG-INFO` & `helix.personmatching-1.0.9/helix.personmatching.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.personmatching
-Version: 1.0.8
+Version: 1.0.9
 Summary: helix.personmatching
 Home-page: https://github.com/icanbwell/helix.personmatching
 Author: Imran Qureshi
 Author-email: imran@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_loader.py` & `helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_loader.py`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/fhir_to_dict_manager.py` & `helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/fhir_to_dict_manager.py`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/test_fhir_to_dict_manager.py` & `helix.personmatching-1.0.9/helix_personmatching/fhir_manager/fhir_to_dict_manager/test/test_fhir_to_dict_manager.py`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/helix_personmatching/logics/rules_generator.py` & `helix.personmatching-1.0.9/helix_personmatching/logics/rules_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,240 +1,265 @@
-from typing import List
+from typing import List, Optional
 
+from helix_personmatching.models.rules.attribute_rule import AttributeRule
 from helix_personmatching.models.constants import Attribute
+from helix_personmatching.models.rules.fixed_score_rule import FixedScoreRule
 from helix_personmatching.models.rule import Rule
+from helix_personmatching.models.scoring_option import ScoringOption
 
 
 class RulesGenerator:
     @staticmethod
-    def generate_rules() -> List[Rule]:
+    def generate_rules(*, options: Optional[List[ScoringOption]] = None) -> List[Rule]:
         """
         generate default match rules
         :return: generated rules for matching
         """
 
         rules: List[Rule] = [
-            Rule(
+            AttributeRule(
                 name="Rule-001",
                 description="given name, family name, gender, dob, zip",
                 number=1,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.NAME_FAMILY,
                     Attribute.GENDER,
                     Attribute.BIRTH_DATE,
                     Attribute.ADDRESS_POSTAL_CODE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-002",
                 description="given name, dob, address 1, zip",
                 number=2,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.BIRTH_DATE,
                     Attribute.ADDRESS_LINE_1,
                     Attribute.ADDRESS_POSTAL_CODE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-003",
                 description="given name, date of birth, email",
                 number=3,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.BIRTH_DATE,
                     Attribute.EMAIL,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-004",
                 description="given name, date of birth, phone",
                 number=4,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.BIRTH_DATE,
                     Attribute.PHONE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-005",
                 description="given name, family name, year of date of birth, gender, address 1, zip",
                 number=5,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.NAME_FAMILY,
                     Attribute.BIRTH_DATE_YEAR,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1,
                     Attribute.ADDRESS_POSTAL_CODE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-006",
                 description="given name, family name, dob month, dob date, gender, address 1, zip",
                 number=6,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.NAME_FAMILY,
                     Attribute.BIRTH_DATE_MONTH,
                     Attribute.BIRTH_DATE_DAY,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1,
                     Attribute.ADDRESS_POSTAL_CODE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-007",
                 description="given name, family name, date of birth, gender, phone",
                 number=7,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.NAME_FAMILY,
                     Attribute.BIRTH_DATE,
                     Attribute.GENDER,
                     Attribute.PHONE_AREA,
                     Attribute.PHONE_LOCAL,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-008",
                 description="first name, last name, date of birth, gender, phone local exchange, phone line",
                 number=8,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.NAME_FAMILY,
                     Attribute.BIRTH_DATE,
                     Attribute.GENDER,
                     Attribute.PHONE_LOCAL,
                     Attribute.PHONE_LINE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-009",
                 description="first name, last name, date of birth, gender, phone area code, phone line",
                 number=9,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.NAME_FAMILY,
                     Attribute.BIRTH_DATE,
                     Attribute.GENDER,
                     Attribute.PHONE_AREA,
                     Attribute.PHONE_LINE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-010",
                 description="given name, dob, gender, address 1 street number, zip, email username, phone line",
                 number=10,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.BIRTH_DATE,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1_ST_NUM,
                     Attribute.ADDRESS_POSTAL_CODE,
                     Attribute.EMAIL_USERNAME,
                     Attribute.PHONE_LINE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-011",
                 description="given name, dob, gender, address 1 street number, zip, "
                 + "phone area code, phone local exchange code",
                 number=11,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.BIRTH_DATE,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1_ST_NUM,
                     Attribute.ADDRESS_POSTAL_CODE,
                     Attribute.PHONE_AREA,
                     Attribute.PHONE_LOCAL,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-012",
                 description="given name, dob, gender, address 1 street number, zip, phone area code, phone line number",
                 number=12,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.BIRTH_DATE,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1_ST_NUM,
                     Attribute.ADDRESS_POSTAL_CODE,
                     Attribute.PHONE_AREA,
                     Attribute.PHONE_LINE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-013",
                 description="given name, dob, gender, address 1 street number, zip, "
                 + "phone local exchange code, phone line number",
                 number=13,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.BIRTH_DATE,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1_ST_NUM,
                     Attribute.ADDRESS_POSTAL_CODE,
                     Attribute.PHONE_LOCAL,
                     Attribute.PHONE_LINE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-014",
                 description="family name, date of birth, is adult today flag, gender, address 1, zip, phone",
                 number=14,
                 attributes=[
                     Attribute.NAME_FAMILY,
                     Attribute.BIRTH_DATE,
                     Attribute.IS_ADULT_TODAY,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1,
                     Attribute.ADDRESS_POSTAL_CODE,
                     Attribute.PHONE,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-015",
                 description="family name, date of birth, is adult today flag, gender, address 1, zip, email",
                 number=15,
                 attributes=[
                     Attribute.NAME_FAMILY,
                     Attribute.BIRTH_DATE,
                     Attribute.IS_ADULT_TODAY,
                     Attribute.GENDER,
                     Attribute.ADDRESS_LINE_1,
                     Attribute.ADDRESS_POSTAL_CODE,
                     Attribute.EMAIL,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
-            Rule(
+            AttributeRule(
                 name="Rule-016",
                 description="given name, email, phone, dob_year",
                 number=16,
                 attributes=[
                     Attribute.NAME_GIVEN,
                     Attribute.EMAIL,
                     Attribute.PHONE,
                     Attribute.BIRTH_DATE_YEAR,
                 ],
-                score=0.0,
+                weight=1.0,
             ),
         ]
 
+        if options and len(options) > 0:
+            available_extra_rules = [
+                FixedScoreRule(
+                    name="Rule-050", description="fixed score", number=50, weight=1.0
+                )
+            ]
+            rules.extend(
+                [
+                    rule
+                    for rule in available_extra_rules
+                    if any([r for r in options if rule.name == r.rule_name])
+                ]
+            )
+
+            for option in options:
+                matching_rules = [
+                    rule for rule in rules if rule.name == option.rule_name
+                ]
+                if len(matching_rules) > 0:
+                    matching_rule = matching_rules[0]
+                    matching_rule.weight = option.weight
+
         return rules
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/logics/score_calculator.py` & `helix.personmatching-1.0.9/helix_personmatching/logics/score_calculator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from typing import Any, List, Optional
+from typing import List, Optional
 
-from rapidfuzz import fuzz
 
 from helix_personmatching.logics.match_score_without_threshold import (
     MatchScoreWithoutThreshold,
 )
-from helix_personmatching.logics.rule_attribute_score import RuleAttributeScore
 from helix_personmatching.logics.rule_score import RuleScore
 from helix_personmatching.logics.scoring_input import ScoringInput
 from helix_personmatching.models.rule import Rule
 
 
 class ScoreCalculator:
     @staticmethod
     def initialize_score(rules: List[Rule]) -> None:
-        for rule in rules:
-            rule.score = 0.0
+        pass
 
     @staticmethod
     def calculate_total_score(
         rules: List[Rule], source: ScoringInput, target: ScoringInput
     ) -> MatchScoreWithoutThreshold:
         match_results: List[RuleScore] = ScoreCalculator.calculate_score(
             rules=rules, source=source, target=target
@@ -102,54 +99,8 @@
 
         return rules_score_results
 
     @staticmethod
     def calculate_score_for_rule(
         rule: Rule, source: ScoringInput, target: ScoringInput
     ) -> Optional[RuleScore]:
-        """
-        Calculate a matching score for one rule between FHIR Person-Person, or Person-Patient, or Person/Patient-AppUser
-        :param rule: one rule in the generated rules by RulesGenerator
-        :param source: Dictionary of Pii data for FHIR Person/Patient data, or AppUser data
-        :param target: Dictionary of Pii data for FHIR Person/Patient data, or AppUser data
-        :return: Dictionary of 1 rule score result
-        """
-
-        id_data_source: Optional[Any] = source.id_
-        id_data_target: Optional[Any] = target.id_
-        if not (id_data_source and id_data_target):
-            return None
-
-        rule_attribute_scores: List[RuleAttributeScore] = []
-        score_avg: float = 0.0
-        for attribute in rule.attributes:
-            rule_attribute_score: RuleAttributeScore = RuleAttributeScore(
-                attribute=attribute, score=0.0, present=False, source=None, target=None
-            )
-            val_source: Optional[str] = getattr(source, attribute)
-            val_target: Optional[str] = getattr(target, attribute)
-
-            if val_source and val_target:
-                rule_attribute_score.present = True
-                # calculate exact string match on "trimmed lower" string values
-                score_for_attribute = fuzz.ratio(
-                    str(val_source).strip().lower(), str(val_target).strip().lower()
-                )
-                score_avg += score_for_attribute
-                rule_attribute_score.score = score_for_attribute
-                rule_attribute_score.source = val_source
-                rule_attribute_score.target = val_target
-            rule_attribute_scores.append(rule_attribute_score)
-
-        score_avg /= len(rule.attributes)
-        rule.score = score_avg
-
-        rule_score: RuleScore = RuleScore(
-            id_source=str(id_data_source),
-            id_target=str(id_data_target),
-            rule_name=rule.name,
-            rule_description=rule.description,
-            rule_score=rule.score,
-            attribute_scores=rule_attribute_scores,
-        )
-
-        return rule_score
+        return rule.score(source=source, target=target)
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/logics/scoring_input.py` & `helix.personmatching-1.0.9/helix_personmatching/logics/scoring_input.py`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/helix_personmatching/matchers/matcher.py` & `helix.personmatching-1.0.9/helix_personmatching/matchers/matcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Optional, Union
 
 # noinspection PyPackageRequirements
 from fhir.resources.bundle import Bundle
 
 # noinspection PyPackageRequirements
 from fhir.resources.patient import Patient
 
@@ -17,24 +17,29 @@
 from helix_personmatching.logics.match_score_without_threshold import (
     MatchScoreWithoutThreshold,
 )
 from helix_personmatching.logics.rules_generator import RulesGenerator
 from helix_personmatching.logics.score_calculator import ScoreCalculator
 from helix_personmatching.logics.scoring_input import ScoringInput
 from helix_personmatching.models.rule import Rule
+from helix_personmatching.models.scoring_option import ScoringOption
 
 
 class Matcher:
     # noinspection PyMethodMayBeStatic
     def score_inputs(
-        self, *, source: List[ScoringInput], target: List[ScoringInput]
+        self,
+        *,
+        source: List[ScoringInput],
+        target: List[ScoringInput],
+        options: Optional[List[ScoringOption]] = None
     ) -> List[MatchScoreWithoutThreshold]:
         assert source
         assert target
-        rules: List[Rule] = RulesGenerator.generate_rules()
+        rules: List[Rule] = RulesGenerator.generate_rules(options=options)
 
         result: List[MatchScoreWithoutThreshold] = []
 
         for source_resource in source:
             for target_resource in target:
                 result.append(
                     ScoreCalculator.calculate_total_score(
@@ -46,14 +51,15 @@
     def match_scoring_inputs(
         self,
         *,
         source: List[ScoringInput],
         target: List[ScoringInput],
         threshold: float = 80.0,
         verbose: bool = False,
+        options: Optional[List[ScoringOption]] = None
     ) -> List[MatchScore]:
         assert source
         assert isinstance(source, list)
         assert target
         assert isinstance(target, list)
 
         return [
@@ -61,54 +67,63 @@
                 id_source=score.id_source,
                 id_target=score.id_target,
                 rule_scores=score.rule_scores if verbose else [],
                 total_score=score.total_score,
                 threshold=threshold,
                 matched=(score.total_score >= threshold),
             )
-            for score in self.score_inputs(source=source, target=target)
+            for score in self.score_inputs(
+                source=source, target=target, options=options
+            )
         ]
 
     def match(
         self,
         *,
         source_json: Union[str, List[str]],
         target_json: Union[str, List[str]],
         threshold: float = 80.0,
         verbose: bool = False,
+        options: Optional[List[ScoringOption]] = None
     ) -> List[MatchScore]:
         assert source_json
         assert isinstance(source_json, str) or isinstance(source_json, list)
         assert target_json
         assert isinstance(target_json, str) or isinstance(target_json, list)
 
         source: List[ScoringInput] = FhirLoader.get_scoring_inputs(
             resource_json=source_json
         )
         target: List[ScoringInput] = FhirLoader.get_scoring_inputs(
             resource_json=target_json
         )
         match_score: List[MatchScore] = self.match_scoring_inputs(
-            source=source, target=target, threshold=threshold, verbose=verbose
+            source=source,
+            target=target,
+            threshold=threshold,
+            verbose=verbose,
+            options=options,
         )
         return match_score
 
     def match_resources(
         self,
         *,
         source: Union[Patient, Person, Bundle],
         target: Union[Patient, Person, Bundle],
         threshold: float = 80.0,
         verbose: bool = False,
+        options: Optional[List[ScoringOption]] = None
     ) -> List[MatchScore]:
         source_scoring_inputs: List[
             ScoringInput
         ] = FhirToAttributeDict.get_scoring_inputs_for_resource(resource=source)
         target_scoring_inputs: List[
             ScoringInput
         ] = FhirToAttributeDict.get_scoring_inputs_for_resource(resource=target)
         return self.match_scoring_inputs(
             source=source_scoring_inputs,
             target=target_scoring_inputs,
             threshold=threshold,
             verbose=verbose,
+            options=options,
         )
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match/test_exact_match.py` & `helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_bundle/test_exact_match_bundle.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 from typing import List
 
 from helix_personmatching.logics.match_score import MatchScore
 from helix_personmatching.matchers.matcher import Matcher
 
 
-def test_exact_match() -> None:
+def test_exact_match_bundle() -> None:
+    print("")
     data_dir: Path = Path(__file__).parent.joinpath("./")
 
     with open(data_dir.joinpath("patient1.json")) as file:
         resource1_json = file.read()
 
     with open(data_dir.joinpath("patient2.json")) as file:
         resource2_json = file.read()
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_bundle/test_exact_match_bundle.py` & `helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match_list/test_exact_match_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from pathlib import Path
 from typing import List
 
 from helix_personmatching.logics.match_score import MatchScore
 from helix_personmatching.matchers.matcher import Matcher
 
 
-def test_exact_match_bundle() -> None:
+def test_exact_match_list() -> None:
+    print("")
     data_dir: Path = Path(__file__).parent.joinpath("./")
 
     with open(data_dir.joinpath("patient1.json")) as file:
         resource1_json = file.read()
 
     with open(data_dir.joinpath("patient2.json")) as file:
         resource2_json = file.read()
 
     matcher = Matcher()
 
     scores: List[MatchScore] = matcher.match(
-        source_json=resource1_json, target_json=resource2_json, verbose=True
+        source_json=[resource1_json], target_json=[resource2_json], verbose=True
     )
 
     assert len(scores) == 1
     score = scores[0]
     assert score.matched is True
 
     assert score.total_score == 94.56845238095238
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/matchers/test/exact_match_list/test_exact_match_list.py` & `helix.personmatching-1.0.9/helix_personmatching/matchers/test/exact_match/test_exact_match.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from pathlib import Path
 from typing import List
 
 from helix_personmatching.logics.match_score import MatchScore
 from helix_personmatching.matchers.matcher import Matcher
 
 
-def test_exact_match_list() -> None:
+def test_exact_match() -> None:
+    print("")
     data_dir: Path = Path(__file__).parent.joinpath("./")
 
     with open(data_dir.joinpath("patient1.json")) as file:
         resource1_json = file.read()
 
     with open(data_dir.joinpath("patient2.json")) as file:
         resource2_json = file.read()
 
     matcher = Matcher()
 
     scores: List[MatchScore] = matcher.match(
-        source_json=[resource1_json], target_json=[resource2_json], verbose=True
+        source_json=resource1_json, target_json=resource2_json, verbose=True
     )
 
     assert len(scores) == 1
     score = scores[0]
     assert score.matched is True
 
     assert score.total_score == 94.56845238095238
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/matchers/test/human_api/partial_match/test_hapi_partial_match.py` & `helix.personmatching-1.0.9/helix_personmatching/matchers/test/human_api/partial_match/test_hapi_partial_match.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import List
 
 from helix_personmatching.logics.match_score import MatchScore
 from helix_personmatching.matchers.matcher import Matcher
 
 
 def test_hapi_partial_match() -> None:
+    print("")
     data_dir: Path = Path(__file__).parent.joinpath("./person_data")
 
     with open(data_dir.joinpath("bwell_master_person.json")) as file:
         bwell_master_person_json = file.read()
 
     with open(data_dir.joinpath("hapi_person.json")) as file:
         hapi_person_json = file.read()
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/matchers/test/walgreens/partial_match/test_walgreens_partial_match.py` & `helix.personmatching-1.0.9/helix_personmatching/matchers/test/walgreens/partial_match_with_extra_rule/test_walgreens_partial_match_with_extra_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import dataclasses
 import json
 from pathlib import Path
 from typing import List
 
 from helix_personmatching.logics.match_score import MatchScore
 from helix_personmatching.matchers.matcher import Matcher
+from helix_personmatching.models.scoring_option import ScoringOption
 
 
-def test_walgreens_partial_match() -> None:
+def test_walgreens_partial_match_with_extra_rule() -> None:
+    print("")
     data_dir: Path = Path(__file__).parent.joinpath("./person_data")
 
     with open(data_dir.joinpath("bwell_master_person.json")) as file:
         bwell_master_person_json = file.read()
 
     with open(data_dir.joinpath("walgreens_person.json")) as file:
         walgreens_person_json = file.read()
 
     matcher = Matcher()
 
     scores: List[MatchScore] = matcher.match(
         source_json=walgreens_person_json,
         target_json=bwell_master_person_json,
         verbose=True,
+        options=[ScoringOption(rule_name="Rule-050", weight=1.0)],
     )
 
     assert len(scores) == 1
     score = scores[0]
 
     print(f"score.matched: {score.matched}")
     assert score.matched is False
 
     print(f"score.total_score: {score.total_score}")
-    assert score.total_score == 30.69940476190476
+    assert score.total_score == 36.94940476190476
 
     score_dict = dataclasses.asdict(score)
 
     scores_json = json.dumps(score_dict, default=str)
     print(scores_json)
 
     with open(data_dir.joinpath("expected_scores.json")) as file:
```

### Comparing `helix.personmatching-1.0.8/helix_personmatching/models/constants.py` & `helix.personmatching-1.0.9/helix_personmatching/models/constants.py`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/helix_personmatching/utils/json_serializer.py` & `helix.personmatching-1.0.9/helix_personmatching/utils/json_serializer.py`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/setup.cfg` & `helix.personmatching-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `helix.personmatching-1.0.8/setup.py` & `helix.personmatching-1.0.9/setup.py`

 * *Files identical despite different names*

