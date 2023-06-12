# Comparing `tmp/debater_python_api-5.0.1.tar.gz` & `tmp/debater_python_api-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debater_python_api-5.0.1.tar", last modified: Thu Jun  8 10:47:07 2023, max compression
+gzip compressed data, was "debater_python_api-5.0.2.tar", last modified: Mon Jun 12 07:55:17 2023, max compression
```

## Comparing `debater_python_api-5.0.1.tar` & `debater_python_api-5.0.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.989193 debater_python_api-5.0.1/
--rw-r--r--   0 lilache    (501) staff       (20)    11358 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/LICENSE
--rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-08 10:47:07.988965 debater_python_api-5.0.1/PKG-INFO
--rw-r--r--   0 lilache    (501) staff       (20)      169 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/README.md
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.974087 debater_python_api-5.0.1/debater_python_api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.975126 debater_python_api-5.0.1/debater_python_api/api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.978248 debater_python_api-5.0.1/debater_python_api/api/clients/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     4503 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/abstract_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1147 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/argument_quality_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1548 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/claim_and_evidence_detection_client.py
--rw-r--r--   0 lilache    (501) staff       (20)      934 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/claim_boundaries_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     6203 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/clustering_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3034 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/embedding_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1999 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/index_searcher_client.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.979230 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/
--rw-r--r--   0 lilache    (501) staff       (20)      478 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
--rw-r--r--   0 lilache    (501) staff       (20)    35911 2023-06-08 10:37:54.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/KpsResult.py
--rw-r--r--   0 lilache    (501) staff       (20)    13092 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/docx_generator.py
--rw-r--r--   0 lilache    (501) staff       (20)    15390 2023-06-08 10:23:01.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/graph_generator.py
--rw-r--r--   0 lilache    (501) staff       (20)     3923 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/utils.py
--rw-r--r--   0 lilache    (501) staff       (20)     6969 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_admin_client.py
--rw-r--r--   0 lilache    (501) staff       (20)    39175 2023-06-08 10:37:54.000000 debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1894 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_pairs_infer_client.py
--rw-r--r--   0 lilache    (501) staff       (20)    13830 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/narrative_generation_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1230 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/pro_con_client.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.979609 debater_python_api-5.0.1/debater_python_api/api/clients/response_data/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/response_data/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     1597 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/response_data/speech_response.py
--rw-r--r--   0 lilache    (501) staff       (20)     1790 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/term_relater_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1563 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/term_wikifier_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3394 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/theme_extraction_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     3263 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/debater_api.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.979777 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.981181 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      142 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
--rw-r--r--   0 lilache    (501) staff       (20)     5079 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_client.py
--rw-r--r--   0 lilache    (501) staff       (20)     1001 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
--rw-r--r--   0 lilache    (501) staff       (20)     1314 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
--rw-r--r--   0 lilache    (501) staff       (20)     3576 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
--rw-r--r--   0 lilache    (501) staff       (20)     1516 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.984779 debater_python_api-5.0.1/debater_python_api/examples/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      803 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/argument_quality_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      854 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/claim_boundaries_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1002 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/claim_detection_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      932 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/clustering_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      860 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/embedding_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1014 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/evidence_detection_example.py
--rw-r--r--   0 lilache    (501) staff       (20)    85859 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/example_of_sc_args.py
--rw-r--r--   0 lilache    (501) staff       (20)     1480 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/index_searcher_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1204 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/examples/keypoints_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1428 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/pro_con_example.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.985423 debater_python_api-5.0.1/debater_python_api/examples/resources/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)    23817 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/arguments.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.985638 debater_python_api-5.0.1/debater_python_api/examples/resources/filters_output/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/filters_output/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)     2530 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/pro_con_scores.py
--rw-r--r--   0 lilache    (501) staff       (20)     9581 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/run_all_services.py
--rw-r--r--   0 lilache    (501) staff       (20)      870 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/speech_construction_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      480 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/term_relater_example.py
--rw-r--r--   0 lilache    (501) staff       (20)      907 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/term_wikifier_example.py
--rw-r--r--   0 lilache    (501) staff       (20)     1154 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/theme_extraction_example.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.986132 debater_python_api-5.0.1/debater_python_api/examples/usecases/
--rw-r--r--   0 lilache    (501) staff       (20)     4943 2023-06-08 10:37:54.000000 debater_python_api-5.0.1/debater_python_api/examples/usecases/kp_based_survey.py
--rw-r--r--   0 lilache    (501) staff       (20)     6036 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/usecases/mining_to_narrative.py
--rw-r--r--   0 lilache    (501) staff       (20)    10191 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/usecases/survey.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.986318 debater_python_api-5.0.1/debater_python_api/integration_tests/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.986460 debater_python_api-5.0.1/debater_python_api/integration_tests/api/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.987469 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/
--rw-r--r--   0 lilache    (501) staff       (20)     2708 2023-05-22 15:52:47.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
--rw-r--r--   0 lilache    (501) staff       (20)    11791 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesIT.py
--rw-r--r--   0 lilache    (501) staff       (20)     4630 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesLoad.py
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/__init__.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.988554 debater_python_api-5.0.1/debater_python_api/utils/
--rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/utils/__init__.py
--rw-r--r--   0 lilache    (501) staff       (20)      992 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/utils/clusters_refiner.py
--rw-r--r--   0 lilache    (501) staff       (20)     1574 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/utils/general_utils.py
--rw-r--r--   0 lilache    (501) staff       (20)      604 2023-05-22 16:30:58.000000 debater_python_api-5.0.1/debater_python_api/utils/kp_analysis_conf.py
-drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.974867 debater_python_api-5.0.1/debater_python_api.egg-info/
--rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/PKG-INFO
--rw-r--r--   0 lilache    (501) staff       (20)     4041 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 lilache    (501) staff       (20)        1 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 lilache    (501) staff       (20)       87 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/requires.txt
--rw-r--r--   0 lilache    (501) staff       (20)       19 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/top_level.txt
--rw-r--r--   0 lilache    (501) staff       (20)      879 2023-06-08 10:37:43.000000 debater_python_api-5.0.1/pyproject.toml
--rw-r--r--   0 lilache    (501) staff       (20)       38 2023-06-08 10:47:07.989242 debater_python_api-5.0.1/setup.cfg
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.404361 debater_python_api-5.0.2/
+-rw-r--r--   0 lilache    (501) staff       (20)    11358 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/LICENSE
+-rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-12 07:55:17.404159 debater_python_api-5.0.2/PKG-INFO
+-rw-r--r--   0 lilache    (501) staff       (20)      169 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/README.md
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.388774 debater_python_api-5.0.2/debater_python_api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.389747 debater_python_api-5.0.2/debater_python_api/api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.393774 debater_python_api-5.0.2/debater_python_api/api/clients/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4503 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/abstract_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1147 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/argument_quality_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1548 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)      934 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/claim_boundaries_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6203 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/clustering_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3034 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/embedding_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1999 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/index_searcher_client.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.395000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/
+-rw-r--r--   0 lilache    (501) staff       (20)      478 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
+-rw-r--r--   0 lilache    (501) staff       (20)    38133 2023-06-11 20:39:30.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/KpsResult.py
+-rw-r--r--   0 lilache    (501) staff       (20)    12403 2023-06-11 13:30:46.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/docx_generator.py
+-rw-r--r--   0 lilache    (501) staff       (20)    16293 2023-06-11 10:50:55.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/graph_generator.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4239 2023-06-08 21:02:49.000000 debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/utils.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6969 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_admin_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)    39175 2023-06-12 07:51:28.000000 debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1894 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)    13830 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/narrative_generation_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1230 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/pro_con_client.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.395440 debater_python_api-5.0.2/debater_python_api/api/clients/response_data/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/response_data/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1597 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/response_data/speech_response.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1790 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/term_relater_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1563 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/term_wikifier_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3394 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/clients/theme_extraction_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3263 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/api/debater_api.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.395625 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.396760 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      142 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
+-rw-r--r--   0 lilache    (501) staff       (20)     5079 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1001 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1314 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3576 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1516 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.400656 debater_python_api-5.0.2/debater_python_api/examples/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      803 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/argument_quality_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      854 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/claim_boundaries_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1002 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/claim_detection_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      932 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/clustering_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      860 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/embedding_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1014 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/evidence_detection_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)    85859 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/example_of_sc_args.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1480 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/index_searcher_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1204 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/examples/keypoints_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1428 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/pro_con_example.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401150 debater_python_api-5.0.2/debater_python_api/examples/resources/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)    23817 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/arguments.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401331 debater_python_api-5.0.2/debater_python_api/examples/resources/filters_output/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/filters_output/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     2530 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/resources/pro_con_scores.py
+-rw-r--r--   0 lilache    (501) staff       (20)     9581 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/run_all_services.py
+-rw-r--r--   0 lilache    (501) staff       (20)      870 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/speech_construction_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      480 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/term_relater_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      907 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/term_wikifier_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1154 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/theme_extraction_example.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401759 debater_python_api-5.0.2/debater_python_api/examples/usecases/
+-rw-r--r--   0 lilache    (501) staff       (20)     4943 2023-06-12 07:54:01.000000 debater_python_api-5.0.2/debater_python_api/examples/usecases/kp_based_survey.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6036 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/usecases/mining_to_narrative.py
+-rw-r--r--   0 lilache    (501) staff       (20)    10191 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/examples/usecases/survey.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.401931 debater_python_api-5.0.2/debater_python_api/integration_tests/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.402042 debater_python_api-5.0.2/debater_python_api/integration_tests/api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.402939 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/
+-rw-r--r--   0 lilache    (501) staff       (20)     2708 2023-05-22 15:52:47.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
+-rw-r--r--   0 lilache    (501) staff       (20)    11791 2023-06-05 13:38:02.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesIT.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4630 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.403790 debater_python_api-5.0.2/debater_python_api/utils/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/utils/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      992 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/utils/clusters_refiner.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1574 2022-12-12 10:25:59.000000 debater_python_api-5.0.2/debater_python_api/utils/general_utils.py
+-rw-r--r--   0 lilache    (501) staff       (20)      604 2023-05-22 16:30:58.000000 debater_python_api-5.0.2/debater_python_api/utils/kp_analysis_conf.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-12 07:55:17.389473 debater_python_api-5.0.2/debater_python_api.egg-info/
+-rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 lilache    (501) staff       (20)     4041 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lilache    (501) staff       (20)        1 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lilache    (501) staff       (20)       87 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/requires.txt
+-rw-r--r--   0 lilache    (501) staff       (20)       19 2023-06-12 07:55:17.000000 debater_python_api-5.0.2/debater_python_api.egg-info/top_level.txt
+-rw-r--r--   0 lilache    (501) staff       (20)      879 2023-06-12 07:32:46.000000 debater_python_api-5.0.2/pyproject.toml
+-rw-r--r--   0 lilache    (501) staff       (20)       38 2023-06-12 07:55:17.404409 debater_python_api-5.0.2/setup.cfg
```

### Comparing `debater_python_api-5.0.1/LICENSE` & `debater_python_api-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/PKG-INFO` & `debater_python_api-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater_python_api
-Version: 5.0.1
+Version: 5.0.2
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/abstract_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/abstract_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/argument_quality_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/argument_quality_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/claim_and_evidence_detection_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/claim_boundaries_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/claim_boundaries_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/clustering_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/clustering_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/embedding_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/embedding_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/index_searcher_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/index_searcher_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/KpsResult.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/KpsResult.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,68 +14,30 @@
 from debater_python_api.api.clients.key_point_summarization.docx_generator import save_hierarchical_graph_data_to_docx
 from debater_python_api.api.clients.key_point_summarization.graph_generator import create_graph_data, graph_data_to_hierarchical_graph_data, \
     get_hierarchical_graph_from_tree_and_subset_results, get_hierarchical_kps_data
 import os
 CURR_RESULTS_VERSION = "2.0"
 
 
-def _get_comparison_df(results_to_kp_to_n_comments, results_to_total_comments, titles):
-    ordered_kps = []
-    cols = ['key point']
-    for title in titles:
-        n_comments_per_kp_per_title = results_to_kp_to_n_comments[title]
-        new_kps = set(n_comments_per_kp_per_title.keys()).difference(set(ordered_kps))
-        new_kps = sorted(new_kps, key= lambda x:n_comments_per_kp_per_title[x] ,reverse=True)
-        ordered_kps += new_kps
-        cols.extend([f"{title}_n_comments", f"{title}_percent"])
-
-    if "none" in ordered_kps:
-        ordered_kps.remove("none")
-
-    add_change = False
-    if len(titles) == 2:
-        cols.append("change_percent")
-        add_change = True
-
-    rows = []
-    title_to_precent = {}
-    total_row = ["total"]
-    for i,kp in enumerate(ordered_kps):
-        row = [kp]
-        for title in titles:
-            n_comments_title_kp = results_to_kp_to_n_comments[title].get(kp,0)
-            percent_comments_title_kp = (100*n_comments_title_kp/results_to_total_comments[title]) if n_comments_title_kp else 0
-            row.extend([n_comments_title_kp,f'{percent_comments_title_kp:.2f}%'])
-            title_to_precent[title] = percent_comments_title_kp
-            if i == 0:
-                total_row.extend([results_to_total_comments[title] , "1"])
-        if add_change:
-            change_percent = title_to_precent[titles[1]] - title_to_precent[titles[0]]
-            row.append(f'{change_percent:.2f}%')
-            if i==0:
-                total_row.append("")
-        rows.append(row)
-    rows.append(total_row)
-    comparison_df = pd.DataFrame(rows, columns=cols)
-    return comparison_df
-
-
 class KpsResult:
     """
     Class to hold and process the results of a KPS job.
     """
     def __init__(self, result_json, filter_min_relations=0.4):
         """
         :param result_json: the result json returned from the key point client using get_results.
         """
         self.result_json = result_json
+        kps = self.get_key_points()
+        if len(kps) == 0:
+            logging.info("No key points found. Returning empty KpsResult.")
         self.result_df = self._create_result_df()
         self.version = CURR_RESULTS_VERSION
         self.stances = set(result_json["job_metadata"]["per_stance"].keys()).difference({"no-stance"})
-        self.filter_min_relations_for_text = filter_min_relations
+        self.filter_min_relations = filter_min_relations
         self.kp_id_to_hierarchical_data = self._get_kp_id_to_hierarchical_data()
         self.summary_df = self._result_df_to_summary_df()
 
     def get_domain(self):
         return self.result_json["job_metadata"]["general"]["domain"]
 
     def get_stance_to_job_id(self):
@@ -91,24 +53,24 @@
         :param json_file: path to the json file to hold the results
         """
         logging.info(f"Writing results to: {json_file}")
         with open(json_file, 'w') as f:
             json.dump(self.result_json, f)
 
     @staticmethod
-    def load(json_file: str):
+    def load(json_file: str, filter_min_relations:Optional[float] = 0.4):
         """
         Load results from a json file
         :param json_file: the file to load the results from, obtained using the save() method.
         :return: KpsResult object.
         """
         logging.info(f"Loading results from: {json_file}")
         with open(json_file, 'r') as f:
             json_res = json.load(f)
-            return KpsResult.create_from_result_json(json_res)
+            return KpsResult.create_from_result_json(json_res, filter_min_relations)
 
     def _create_result_df(self):
         sentences_data = self.result_json["sentences_data"]
         matchings_rows = []
         kps_have_stance = False
         sentences_have_stance = False
         stance_keys = []
@@ -217,28 +179,35 @@
         total_mapped_row = ["*matched", n_mapped_comments, n_mapped_comments / n_total_comments, n_mapped_sentences,
                     n_mapped_sentences / n_total_sentences, "", "","", ""]
         summary_rows.append(total_mapped_row)
 
         return pd.DataFrame(summary_rows, columns=summary_cols)
 
     @staticmethod
-    def create_from_result_json(result_json, filter_min_relations_for_text=0.4):
+    def create_from_result_json(result_json, filter_min_relations=0.4):
         """
         Create KpsResults from results_json
         :param result_json: the json object obtained from the client via "get_result" or "get_result_from_futures"
+        :param filter_min_relations: minimal relation score between key points to be considered related in the hierarchy
         :return: KpsResult object
         """
         if 'keypoint_matchings' not in result_json:
-            raise KpsIllegalInputException("Faulty results json provided: does not contain 'keypoint_matchings'. returning empty results")
+            raise KpsIllegalInputException("Faulty results json provided: does not contain 'keypoint_matching'.")
+        if "job_metadata" not in result_json:
+            raise KpsIllegalInputException("Faulty result_json provided: does not contain 'job_metadata'. result_json must be"
+                                           "the json object returned by the server when running with SDK version >= 5.0.0."
+                                           "Converting older json results is not supported. to generate the old"
+                                           "results for the given json object please use SDK version <= 4.3.2. To generate new result"
+                                           "please rerun the KPS job using the current SDK")
         else:
             try:
                 version = result_json.get("version", "1.0")
                 if version != CURR_RESULTS_VERSION:
                     result_json = KpsResult._convert_to_new_version(result_json, version, CURR_RESULTS_VERSION)
-                return KpsResult(result_json, filter_min_relations_for_text)
+                return KpsResult(result_json, filter_min_relations)
             except Exception as e:
                 logging.error("Could not create KpsResults from json.")
                 raise e
 
     def get_job_metadata(self):
         """ Return the metadata associated with the (or jobs in case of merged results)"""
         return self.result_json['job_metadata']
@@ -297,17 +266,17 @@
         :param min_n_matches_in_docx: optional, remove key points with less than min_n_matches_in_docx matching sentences.
         '''
         graph_full_data = create_graph_data(full_results.result_df, full_results._get_number_of_unique_sentences())
         hierarchical_graph_full_data = graph_data_to_hierarchical_graph_data(graph_data=graph_full_data)
 
         new_hierarchical_graph_data = get_hierarchical_graph_from_tree_and_subset_results(
             hierarchical_graph_full_data,
-            self.result_df, self.filter_min_relations_for_text, n_top_matches_in_graph)
+            self.result_df, self.filter_min_relations, n_top_matches_in_graph)
 
-        new_kp_id_to_hierarchical_data = get_hierarchical_kps_data(self.result_df, new_hierarchical_graph_data, self.filter_min_relations_for_text)
+        new_kp_id_to_hierarchical_data = get_hierarchical_kps_data(self.result_df, new_hierarchical_graph_data, self.filter_min_relations)
         self.generate_docx_report(output_dir, result_name,
                             n_matches_in_docx=n_matches_in_docx,
                             include_match_score_in_docx=include_match_score_in_docx,
                             min_n_matches_in_docx=min_n_matches_in_docx,
                             kp_id_to_hierarchical_data = new_kp_id_to_hierarchical_data)
 
     def export_to_all_outputs(self, output_dir: str, result_name: str,
@@ -435,14 +404,61 @@
             total_sentences = set()
             for i, keypoint_matching in enumerate(self.result_json['keypoint_matchings']):
                 matching_sents_ids = set([get_unique_sent_id(d) for d in keypoint_matching['matching']])
                 if keypoint_matching['keypoint'] != 'none':
                     total_sentences = total_sentences.union(matching_sents_ids)
             return len(total_sentences)
 
+    def _get_comparison_df(self, results_to_kp_to_n_comments, results_to_total_comments, titles, kp_to_stance):
+        ordered_kps = []
+        cols = ['key point', 'stance']
+
+        for title in titles:
+            n_comments_per_kp_per_title = results_to_kp_to_n_comments[title]
+            new_kps = set(n_comments_per_kp_per_title.keys()).difference(set(ordered_kps))
+            new_kps = sorted(new_kps, key=lambda x: n_comments_per_kp_per_title[x], reverse=True)
+            ordered_kps += new_kps
+            cols.extend([f"{title}_n_comments", f"{title}_percent"])
+
+        if "none" in ordered_kps:
+            ordered_kps.remove("none")
+
+        add_change = False
+        if len(titles) == 2:
+            cols.append("change_percent")
+            add_change = True
+
+        rows = []
+        title_to_precent = {}
+        total_row = ["total", ""]
+        for i, kp in enumerate(ordered_kps):
+            row = [kp, kp_to_stance[kp]]
+
+            for title in titles:
+                n_comments_title_kp = results_to_kp_to_n_comments[title].get(kp, 0)
+                percent_comments_title_kp = (
+                            100 * n_comments_title_kp / results_to_total_comments[title]) if n_comments_title_kp else 0
+                row.extend([n_comments_title_kp, f'{percent_comments_title_kp:.2f}%'])
+                title_to_precent[title] = percent_comments_title_kp
+                if i == 0:
+                    total_row.extend([results_to_total_comments[title], "1"])
+            if add_change:
+                change_percent = title_to_precent[titles[1]] - title_to_precent[titles[0]]
+                row.append(f'{change_percent:.2f}%')
+                if i == 0:
+                    total_row.append("")
+
+            rows.append(row)
+        rows.append(total_row)
+        comparison_df = pd.DataFrame(rows, columns=cols)
+
+        if len(set(kp_to_stance.values()).difference({"no-stance", None})) == 0:
+            comparison_df = comparison_df[[c for c in comparison_df.columns if c != "stance"]]
+        return comparison_df
+
     def compare_with_comment_subsets(self, comments_subsets_dict:Dict[str, List[str]], include_full:Optional[bool] = True):
         """
         Compare the full result with the results generated from comment subsets. This is useful in order to compare the
         key points' prevalence among different subsets of the full data.
         :param comments_subsets_dict: dictionary of string titles as keys and the set of comment ids that corresponds to each title.
         Comment ids that are not part of this result are ignored.
         :param include_full: Optional, default True, whether to include the full results in the comparison.
@@ -453,15 +469,17 @@
         results_to_total_comments.update({title: len(comments_subsets_dict[title]) for title in comments_subsets_dict})
 
         titles = (["full"] if include_full else []) + sorted(comments_subsets_dict.keys(), key=lambda x: results_to_total_comments[x], reverse=True)
 
         results_to_kp_to_n_comments = {"full": self._get_kp_to_n_matched_comments()} if include_full else {}
         results_to_kp_to_n_comments.update(
             {title: self._get_kp_to_n_matched_comments(comments_subset=comment_ids) for title, comment_ids in comments_subsets_dict.items()})
-        return _get_comparison_df(results_to_kp_to_n_comments, results_to_total_comments, titles)
+
+        kp_to_stance = self.get_kp_to_stance()
+        return self._get_comparison_df(results_to_kp_to_n_comments, results_to_total_comments, titles, kp_to_stance)
 
     def compare_with_other_results(self, this_title : str, other_results_dict : Dict[str,'KpsResult']):
         """
         Compare this result with other results.
         :param this_title: title to be associated with the current result.
         :param other_results_dict: dictionary of result titles as keys and KpsResult objects as values.
         :return: a dataframe containing the number and percentage of the comments matched to each key point in each result,
@@ -469,24 +487,30 @@
         """
         results_to_total_comments = {this_title:self._get_number_of_unique_comments()}
         results_to_total_comments.update({title:result._get_number_of_unique_comments() for title,result in other_results_dict.items()})
         titles = [this_title] + sorted(other_results_dict.keys(), key=lambda x:results_to_total_comments[x], reverse=True)
 
         results_to_kp_to_n_comments = {this_title:self._get_kp_to_n_matched_comments()}
         results_to_kp_to_n_comments.update({title:result._get_kp_to_n_matched_comments()  for title,result in other_results_dict.items()})
-        return _get_comparison_df(results_to_kp_to_n_comments, results_to_total_comments, titles)
+
+        kp_to_stance = self.get_kp_to_stance()
+        for result in other_results_dict.values():
+            kp_to_stance.update(result.get_kp_to_stance())
+
+        return self._get_comparison_df(results_to_kp_to_n_comments, results_to_total_comments, titles, kp_to_stance)
 
     @staticmethod
     def get_merged_pro_con_results(pro_result: 'KpsResult', con_result: 'KpsResult'):
         """
         Merge a pro KpsResult and a con KpsResult to a single merged KpsResult.
         The two results must be obtained by the same user, over the same domain and the same set of comments.
         :param pro_result: KpsResult generated from running on stance "PRO".
         :param con_result: KpsResult generated from running on stance "CON".
         """
+        logging.info("Merging positive and negative KpsResults.")
         assert pro_result.stances == {"pro"}, f"pro_result must be generated from running on stance 'PRO', given {pro_result.stances}"
         assert con_result.stances == {"con"}, f"con_result must be generated from running on stance 'CON', given {con_result.stances}"
         con_meta = con_result.result_json["job_metadata"]["general"]
         pro_meta = pro_result.result_json["job_metadata"]["general"]
         for k in ["user_id","domain"]:
             assert con_meta[k] == pro_meta[k], f'pro_result and con_result must have the same {k}, but given {pro_meta[k]} for pro and {con_meta[k]} for con'
         assert con_meta["n_comments"] == pro_meta['n_comments'], f'pro_result and con_result must be generated from running on' \
@@ -514,15 +538,16 @@
         pro_metadata = pro_result.result_json["job_metadata"]
         con_metadata = con_result.result_json["job_metadata"]
         new_metadata = {"general":pro_metadata["general"],
                         "per_stance":{"pro":pro_metadata["per_stance"]["pro"], "con":con_metadata["per_stance"]["con"]}}
         combined_results_json = {'keypoint_matchings':keypoint_matchings, "sentences_data":sentences_data,
                                  "version":CURR_RESULTS_VERSION,
                                  "job_metadata":new_metadata}
-        return KpsResult.create_from_result_json(combined_results_json)
+        filter_min_relations = np.min([pro_result.filter_min_relations, con_result.filter_min_relations])
+        return KpsResult.create_from_result_json(combined_results_json, filter_min_relations=filter_min_relations)
 
     @staticmethod
     # If result_json is of the old server version, convert to version 2.0
     # 1.0 - received from the server, must have only one stance (merging pro_con is only on v2)
     def _convert_v1_to_v2(result_json):
         metadata = result_json["job_metadata"]
         kps_stance = KpsResult._get_stance_from_server_stances(metadata["stances"])
@@ -587,18 +612,22 @@
             if comments_subset:
                 matching_comments_set = set(filter(lambda x:x in comments_subset, matching_comments_set))
 
             n_matches = len(matching_comments_set)
             kp_n_comments[kp] = n_matches
         return kp_n_comments
 
+    def get_key_points(self):
+        return [keypoint_matching["keypoint"] for keypoint_matching in self.result_json['keypoint_matchings'] if keypoint_matching["keypoint"] != "none"]
+
+
     def _get_kp_id_to_hierarchical_data(self):
         graph_data = create_graph_data(self.result_df, n_sentences=self._get_number_of_unique_sentences())
-        hierarchical_graph_data = graph_data_to_hierarchical_graph_data(graph_data=graph_data)
-        return get_hierarchical_kps_data(self.result_df, hierarchical_graph_data, self.filter_min_relations_for_text)
+        hierarchical_graph_data = graph_data_to_hierarchical_graph_data(graph_data=graph_data, filter_min_relations=self.filter_min_relations)
+        return get_hierarchical_kps_data(self.result_df, hierarchical_graph_data, self.filter_min_relations)
 
     @staticmethod
     def _get_stance_from_server_stances(server_stances):
 
         if not server_stances or len(server_stances) == 0:
             return "no-stance"
         if server_stances == ["pos"]:
@@ -639,7 +668,11 @@
 
     def get_stance_str(self):
         if len(self.stances) == 0:
             return "no-stance"
         elif len(self.stances) == 1:
             return list(self.stances)[0]
         return "pro and con"
+
+    def get_kp_to_stance(self):
+         keypoint_matchings = self.result_json["keypoint_matchings"]
+         return {keypoint_matching['keypoint']:keypoint_matching.get("stance", None) for keypoint_matching in keypoint_matchings}
```

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/docx_generator.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/docx_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import random
 
 import docx
+import numpy as np
 from docx.enum.dml import MSO_THEME_COLOR_INDEX
 from docx.shared import Inches, Pt, RGBColor
 from docx import Document
 
 from debater_python_api.api.clients.key_point_summarization.KpsExceptions import KpsIllegalInputException
 from debater_python_api.api.clients.key_point_summarization.utils import create_dict_to_list, \
     trunc_float, read_dicts_from_df, get_unique_sent_id
@@ -25,15 +26,15 @@
     if len(stances) == 1:
         return stance_to_stance_str[list(stances)[0]]
     if set(stances) == set(["pro","con"]):
         return "Positive and Negative"
     raise KpsIllegalInputException(f"unsupported stances {stances}")
 
 def get_kp_stance_if_needed(id_data, stances):
-    return id_data["kp_stance"].capitalize() + ", " if stances == {"pro", "con"} else ""
+    return id_data["kp_stance"].capitalize() + ", " if set(stances) == {"pro", "con"} else ""
 
 def insertHR(paragraph):
     p = paragraph._p  # p is the <w:p> XML element
     pPr = p.get_or_add_pPr()
     pBdr = OxmlElement('w:pBdr')
     pPr.insert_element_before(pBdr,
         'w:shd', 'w:tabs', 'w:suppressAutoHyphens', 'w:kinsoku', 'w:wordWrap',
@@ -98,43 +99,34 @@
     paragraph_format.keep_together = False
 
 def add_data_stats(meta_data, dicts, kp_id_to_data, document, stances, min_n_matches):
     n_kps = len(kp_id_to_data)
     n_total_sentences = meta_data["general"]["n_sentences"]
     n_total_comments = meta_data["general"]["n_comments"]
     dicts_not_none = list(filter(lambda r: r["kp"] != "none", dicts))
-    n_matches_sentences = len(set([get_unique_sent_id(d) for d in dicts_not_none]))
     n_matches_comments = len(set([d["comment_id"] for d in dicts_not_none])) # Todo: this includes matches to smaller, filtered kps!
-    rate_matched_sents = 100*n_matches_sentences / n_total_sentences
     rate_matched_comments = 100*n_matches_comments / n_total_comments
 
-    stances_str = get_stance_to_stance_str(stances).lower()
-
     heading = document.add_heading('Data Statistics', 1)
     set_heading(heading)
-    s = f'Analyzed {n_total_comments} comments ({n_total_sentences} sentences).\n' \
-        f'Identified {n_kps} {stances_str.lower()} key points with at least {min_n_matches or 1} matching sentences.\n' \
-        f'{int(rate_matched_comments)}% of the comments (and {int(rate_matched_sents)}%' \
-        f' of the sentences) were matched to at least one key point.\n'
+    s = f'Analyzed {n_total_comments} comments with {n_total_sentences} sentences.\n' \
+        f'Identified {n_kps} key points with at least {min_n_matches or 1} matching sentences.\n' \
+        f'{int(np.round(rate_matched_comments, 0))}% of the comments were matched to at least one key point.\n'
     for stance in ["pro","con"]:
         if stance in stances:
             stance_str = get_stance_to_stance_str(stance).lower()
             n_kps_stance = len(list(filter(lambda kp_id:kp_id_to_data[kp_id].get("kp_stance")==stance, kp_id_to_data)))
             kp_stance_str = f"of {n_kps_stance} {stance_str} key points." if len(stances) > 1 else "key point."
 
-            n_stance_sentences = meta_data["per_stance"][stance]["n_sentences_stance"]
             n_stance_comments = meta_data["per_stance"][stance]["n_comments_stance"]
             dicts_stance = list(filter(lambda r: r["kp_stance"] == stance, dicts_not_none))
-            n_matches_sentences_stance = len(set([get_unique_sent_id(d) for d in dicts_stance]))
             n_matches_comments_stance = len(set([d["comment_id"] for d in dicts_stance]))
-            matched_sentences_stance_rate = 100*n_matches_sentences_stance/n_stance_sentences if n_stance_sentences > 0 else 0
             matched_comments_stance_rate = 100*n_matches_comments_stance / n_stance_comments if n_stance_comments > 0 else 0
-            s += f'Identified {n_stance_comments} {stance_str} comments (and {n_stance_sentences} {stance_str} sentences).\n'\
-                 f'{int(matched_comments_stance_rate)}% of these comments (and {int(matched_sentences_stance_rate)}% of these sentences)' \
-                f' were matched to at least one {kp_stance_str}\n'
+            s += f'\nIdentified {n_stance_comments} {stance_str} comments.\n'\
+                 f'{int(matched_comments_stance_rate)}% of these comments were matched to at least one {kp_stance_str}\n'
     p = document.add_paragraph()
     run = p.add_run(s)
     run.font.size = Pt(12)
 
 
 def sample_list_keep_order(list_to_sample, n_to_sample, seed=0):
     rng = random.Random(seed)
@@ -270,15 +262,15 @@
 
     for id, paragraph in id_to_paragraph1.items():
         id_data = kp_id_to_data[id]
         kp = id_data['kp']
         kp_stance_str = get_kp_stance_if_needed(id_data, stances)
         n_matches = int(id_data["n_matching_sentences"])
         if n_matches == id_data["n_matching_sents_in_subtree"]:
-            msg = f'{kp} ({n_matches} matches)'
+            msg = f'{kp} ({kp_stance_str}{n_matches} matches)'
         else:
             if sort_by_subtree:
                 msg = f'{kp} ({kp_stance_str}{id_data["n_matching_sents_in_subtree"]} matching sentences in subtree, {n_matches} matches)'
             else:
                 msg = f'{kp} ({kp_stance_str}{n_matches} matches, {id_data["n_matching_sents_in_subtree"]} in subtree)'
         add_link(paragraph=paragraph, link_to=f'table_bookmark{id}', text=msg, tool_tip="Click to view top matching sentences")
```

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/graph_generator.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/graph_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import itertools
 import json
 import logging
 import pandas as pd
 import numpy as np
 from debater_python_api.api.clients.key_point_summarization.utils import create_dict_to_list, read_dicts_from_df, \
-    get_unique_sent_id
-
+    get_unique_sent_id, sort_dict_items_by_value_then_key
+import networkx as nx
 
 def create_graph_data(full_results_df, n_sentences, min_n_similar_matches=5, n_matches_samples=20):
     def graph_to_graph_data(graph, n_sentences):
         for node in graph['nodes']:
             node['relative_val'] = float(node['n_matches']) / float(n_sentences)
 
         graph_data = []
@@ -61,28 +62,27 @@
                 continue
             else:
                 kp_i = all_kps[i]
                 kp_j = all_kps[j]
                 sents_i = kp_to_sentences[kp_i]
                 sents_j = kp_to_sentences[kp_j]
                 n_sentences_i_in_j = len([s for s in sents_i if s in sents_j])
-                if n_sentences_i_in_j > min_n_similar_matches:
+                if n_sentences_i_in_j >= min_n_similar_matches:
                     edge_to_score[(i, j)] = n_sentences_i_in_j / len(sents_i)
     nodes = [get_node(i, kp, kp_to_dicts, n_matches_samples) for i, kp in enumerate(all_kps)]
     edges = [{'source': i, 'target': j, 'score': edge_to_score[i, j]} for (i, j) in edge_to_score]
     graph = {'nodes': nodes, 'edges': edges}
 
     return graph_to_graph_data(graph, n_sentences)
 
 
 def graph_data_to_hierarchical_graph_data(graph_data_json_file=None,
                                           graph_data=None,
                                           filter_small_nodes=-1.0,
-                                          filter_min_relations=-1.0,
-                                          filter_big_to_small_edges=True):
+                                          filter_min_relations=-1.0):
     if (graph_data_json_file is None and graph_data is None) or (
             graph_data_json_file is not None and graph_data is not None):
         logging.error('Please pass either graph_data_json_file or graph_data')
 
     if graph_data_json_file is not None:
         print(f'creating hierarchical graph from file: {graph_data_json_file}')
         graph_data = json.load(open(graph_data_json_file))
@@ -98,25 +98,41 @@
     id_to_node = {d['data']['id']: d for d in nodes}
 
     if filter_min_relations > 0.0:
         edges = [e for e in edges if float(e['data']['score']) >= filter_min_relations]
 
     edges = [e for e in edges if (e['data']['source'] in nodes_ids and e['data']['target'] in nodes_ids)]
 
-    if filter_big_to_small_edges:
-        edges = [e for e in edges if int(id_to_node[e['data']['source']]['data']['n_matches']) <= int(
-            id_to_node[e['data']['target']]['data']['n_matches'])]
-
-        # if source and target have the same number of matches - a cycle can still remain
-        edges_source_target = [(e['data']['source'], e['data']['target']) for e in edges]
-        to_remove = []
-        for (s_id, t_id) in edges_source_target:
-            if s_id < t_id and (t_id, s_id) in edges_source_target:
-                to_remove.append((s_id, t_id))
-        edges = [e for e in edges if (e['data']['source'], e['data']['target']) not in to_remove]
+    # filter big to_small edges:
+    edges = [e for e in edges if int(id_to_node[e['data']['source']]['data']['n_matches']) <= int(
+        id_to_node[e['data']['target']]['data']['n_matches'])]
+
+    # find cycles of same size nodes and break them
+    source_target_to_score = {(e['data']['source'], e['data']['target']): e['data']['score'] for e in edges}
+    n_matches_to_node_ids = create_dict_to_list([(n['data']['n_matches'],n['data']['id']) for n in nodes])
+
+    to_remove = set()
+    for n, sub_node_ids in n_matches_to_node_ids.items():
+         if len(sub_node_ids) < 2:
+             continue
+         sub_edges = [e for e in source_target_to_score.keys() if e[0] in sub_node_ids and e[1] in sub_node_ids]
+         if len(sub_edges) > 1:
+            graph = nx.DiGraph(incoming_graph_data=sub_edges)
+            cycles = list(nx.simple_cycles(graph))
+            cycle_to_edges_ids = {i : tuple([(c[i], c[(i+1)%len(c)]) for i in range(len(c))]) for i,c in enumerate(cycles)}
+
+            while len(cycle_to_edges_ids) > 0:
+                edges_in_cycles = set(itertools.chain(*cycle_to_edges_ids.values()))
+                edges_in_cycles_to_scores = {e: source_target_to_score[e] for e in edges_in_cycles}
+                edges_in_cycles = [x[0] for x in sort_dict_items_by_value_then_key(edges_in_cycles_to_scores)]
+                e = edges_in_cycles[-1]
+                to_remove.add(e)
+                cycle_to_edges_ids = dict(filter(lambda x: e not in x[1], cycle_to_edges_ids.items()))
+
+    edges = [e for e in edges if (e['data']['source'], e['data']['target']) not in to_remove]
 
     source_target_to_score = {(e['data']['source'], e['data']['target']): e['data']['score'] for e in edges}
 
     # keep only edges to max parent
     id_to_parents = create_dict_to_list([(e['data']['source'], e['data']['target']) for e in edges])
     id_to_max_parent = {}
     for id, parents in id_to_parents.items():
@@ -182,24 +198,24 @@
         edges = [d for d in graph_data if d['type'] == 'edge']
         edges = [e for e in edges if float(e['data']['score']) >= min_relation_strength]
         graph_data = nodes + edges
     return graph_data
 
 
 def get_hierarchical_graph_from_tree_and_subset_results(graph_data_hierarchical, subset_results_df,
-                                                        filter_min_relations_for_text=0.4,
+                                                        filter_min_relations=0.4,
                                                         n_top_matches_in_graph=20):
 
     n_sentences = len(set(subset_results_df["sentence_text"]))
     results_kps = [kp for kp in set(subset_results_df["kp"]) if kp != "none"]
 
     nodes = [d for d in graph_data_hierarchical if d['type'] == 'node']
     edges = [d for d in graph_data_hierarchical if d['type'] == 'edge']
-    if filter_min_relations_for_text > 0:
-        edges = [e for e in edges if float(e['data']['score']) >= filter_min_relations_for_text]
+    if filter_min_relations > 0:
+        edges = [e for e in edges if float(e['data']['score']) >= filter_min_relations]
 
     # change graph nodes to match new results:
     n_kps_in_new_only = len(set(results_kps).difference(set(n["data"]['kp'] for n in nodes)))
     if n_kps_in_new_only > 0:  # no new kps in results
         logging.warning(
             f"New result file contains {n_kps_in_new_only} key points not in the graph data. Not creating summaries.")
         return None
@@ -313,8 +329,8 @@
     for id in kp_id_to_data:
         kp_id_to_data[id].update({'parent':id_to_parent.get(id),
                                   'n_matching_sents_in_subtree':id_to_n_matches_subtree_sent.get(id),
                                   'n_matching_comments_in_subtree':id_to_n_matches_subtree_comments.get(id),
                                   "kids":id_to_kids.get(id, []),
                                   'kp_stance':kp_to_stance[kp_id_to_data[id]['kp']],
                                   'n_matching_comments':kp_to_n_matching_comments[kp_id_to_data[id]['kp']]})
-    return kp_id_to_data
+    return kp_id_to_data
```

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/utils.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/key_point_summarization/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,7 +122,14 @@
 
 def filter_dict_by_keys(d, keys):
     return {k:d[k] for k in keys}
 
 
 def is_list_of_strings(lst):
     return isinstance(lst, list) and len([a for a in lst if not isinstance(a, str)]) == 0
+
+# sort by val (descending), with key (ascending) as tie breaker
+def sort_dict_items_by_value_then_key(d, val_reverse = True, key_reverse = False):
+    d_items = list(d.items())
+    d_items.sort(key=lambda x: x[0], reverse = key_reverse)
+    d_items.sort(key=lambda x: x[1], reverse = val_reverse)
+    return d_items
```

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_admin_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_admin_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_pairs_infer_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/narrative_generation_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/narrative_generation_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/pro_con_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/pro_con_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/response_data/speech_response.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/response_data/speech_response.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/term_relater_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/term_relater_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/term_wikifier_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/term_wikifier_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/clients/theme_extraction_client.py` & `debater_python_api-5.0.2/debater_python_api/api/clients/theme_extraction_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/debater_api.py` & `debater_python_api-5.0.2/debater_python_api/api/debater_api.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_client.py` & `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py` & `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py` & `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_base.py` & `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_request.py` & `debater_python_api-5.0.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/argument_quality_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/argument_quality_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/claim_boundaries_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/claim_boundaries_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/claim_detection_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/claim_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/clustering_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/clustering_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/embedding_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/embedding_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/evidence_detection_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/evidence_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/example_of_sc_args.py` & `debater_python_api-5.0.2/debater_python_api/examples/example_of_sc_args.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/index_searcher_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/index_searcher_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/keypoints_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/keypoints_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/pro_con_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/pro_con_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/resources/arguments.py` & `debater_python_api-5.0.2/debater_python_api/examples/resources/arguments.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/resources/pro_con_scores.py` & `debater_python_api-5.0.2/debater_python_api/examples/resources/pro_con_scores.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/run_all_services.py` & `debater_python_api-5.0.2/debater_python_api/examples/run_all_services.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/speech_construction_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/speech_construction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/term_wikifier_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/term_wikifier_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/theme_extraction_example.py` & `debater_python_api-5.0.2/debater_python_api/examples/theme_extraction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/usecases/kp_based_survey.py` & `debater_python_api-5.0.2/debater_python_api/examples/usecases/kp_based_survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/usecases/mining_to_narrative.py` & `debater_python_api-5.0.2/debater_python_api/examples/usecases/mining_to_narrative.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/examples/usecases/survey.py` & `debater_python_api-5.0.2/debater_python_api/examples/usecases/survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py` & `debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesIT.py` & `debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesIT.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesLoad.py` & `debater_python_api-5.0.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/utils/clusters_refiner.py` & `debater_python_api-5.0.2/debater_python_api/utils/clusters_refiner.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/utils/general_utils.py` & `debater_python_api-5.0.2/debater_python_api/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api/utils/kp_analysis_conf.py` & `debater_python_api-5.0.2/debater_python_api/utils/kp_analysis_conf.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/debater_python_api.egg-info/PKG-INFO` & `debater_python_api-5.0.2/debater_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater-python-api
-Version: 5.0.1
+Version: 5.0.2
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.1/debater_python_api.egg-info/SOURCES.txt` & `debater_python_api-5.0.2/debater_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.1/pyproject.toml` & `debater_python_api-5.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debater_python_api"
-version = "5.0.1"
+version = "5.0.2"
 description = "Project Debater Early Access Program API sdk for python"
 readme = "README.md"
 authors = [{ name = "Elad Venezian", email = "eladv@il.ibm.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

