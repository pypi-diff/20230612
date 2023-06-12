# Comparing `tmp/clayrs-0.4.0.tar.gz` & `tmp/clayrs-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clayrs-0.4.0.tar", last modified: Wed Nov 30 17:27:53 2022, max compression
+gzip compressed data, was "clayrs-0.4.1.tar", last modified: Mon Jun 12 09:58:37 2023, max compression
```

## Comparing `clayrs-0.4.0.tar` & `clayrs-0.4.1.tar`

### file list

```diff
@@ -1,269 +1,269 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.422887 clayrs-0.4.0/
--rw-rw-rw-   0        0        0    35823 2022-06-07 21:08:29.000000 clayrs-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       25 2022-07-01 17:25:27.000000 clayrs-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8098 2022-11-30 17:27:53.422887 clayrs-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     6964 2022-07-01 17:52:41.000000 clayrs-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:51.976038 clayrs-0.4.0/clayrs/
--rw-rw-rw-   0        0        0       80 2022-10-18 17:10:14.000000 clayrs-0.4.0/clayrs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.055991 clayrs-0.4.0/clayrs/content_analyzer/
--rw-rw-rw-   0        0        0      777 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/__init__.py
--rw-rw-rw-   0        0        0    19919 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/config.py
--rw-rw-rw-   0        0        0    13001 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/content_analyzer_main.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.081208 clayrs-0.4.0/clayrs/content_analyzer/content_representation/
--rw-rw-rw-   0        0        0       28 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/content_representation/__init__.py
--rw-rw-rw-   0        0        0    17711 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/content_representation/content.py
--rw-rw-rw-   0        0        0     9660 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/content_representation/representation_container.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.096992 clayrs-0.4.0/clayrs/content_analyzer/embeddings/
--rw-rw-rw-   0        0        0      134 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.163154 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/
--rw-rw-rw-   0        0        0      259 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/__init__.py
--rw-rw-rw-   0        0        0     2015 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py
--rw-rw-rw-   0        0        0    12971 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py
--rw-rw-rw-   0        0        0     1918 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py
--rw-rw-rw-   0        0        0     2999 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py
--rw-rw-rw-   0        0        0     2716 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/lda.py
--rw-rw-rw-   0        0        0     2961 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py
--rw-rw-rw-   0        0        0     1791 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.192273 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/
--rw-rw-rw-   0        0        0      182 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/__init__.py
--rw-rw-rw-   0        0        0     3502 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py
--rw-rw-rw-   0        0        0     1265 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py
--rw-rw-rw-   0        0        0     1362 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py
--rw-rw-rw-   0        0        0     6168 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py
--rw-rw-rw-   0        0        0     2327 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py
--rw-rw-rw-   0        0        0     4182 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_source.py
--rw-rw-rw-   0        0        0      659 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/exceptions.py
--rw-rw-rw-   0        0        0    27437 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/exogenous_properties_retrieval.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.231202 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/
--rw-rw-rw-   0        0        0      251 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.255393 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/
--rw-rw-rw-   0        0        0      271 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
--rw-rw-rw-   0        0        0     3402 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py
--rw-rw-rw-   0        0        0    22732 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py
--rw-rw-rw-   0        0        0    17916 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py
--rw-rw-rw-   0        0        0     3346 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py
--rw-rw-rw-   0        0        0     7598 2022-11-30 17:09:26.000000 clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.286790 clayrs-0.4.0/clayrs/content_analyzer/information_processor/
--rw-rw-rw-   0        0        0       84 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/information_processor/__init__.py
--rw-rw-rw-   0        0        0    11229 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/information_processor/ekphrasis.py
--rw-rw-rw-   0        0        0     2402 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/information_processor/information_processor.py
--rw-rw-rw-   0        0        0    11713 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/information_processor/nltk.py
--rw-rw-rw-   0        0        0    11797 2022-11-22 22:28:31.000000 clayrs-0.4.0/clayrs/content_analyzer/information_processor/spacy.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.318699 clayrs-0.4.0/clayrs/content_analyzer/memory_interfaces/
--rw-rw-rw-   0        0        0       55 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/memory_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5433 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py
--rw-rw-rw-   0        0        0    12924 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/memory_interfaces/text_interface.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.343215 clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/
--rw-rw-rw-   0        0        0      154 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/__init__.py
--rw-rw-rw-   0        0        0    31916 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/ratings.py
--rw-rw-rw-   0        0        0     2776 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/score_processor.py
--rw-rw-rw-   0        0        0     1163 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py
--rw-rw-rw-   0        0        0    14008 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/content_analyzer/raw_information_source.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.357235 clayrs-0.4.0/clayrs/content_analyzer/utils/
--rw-rw-rw-   0        0        0        0 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/utils/__init__.py
--rw-rw-rw-   0        0        0     1070 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/utils/check_tokenization.py
--rw-rw-rw-   0        0        0     1252 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/content_analyzer/utils/id_merger.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.384117 clayrs-0.4.0/clayrs/evaluation/
--rw-rw-rw-   0        0        0      206 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/evaluation/__init__.py
--rw-rw-rw-   0        0        0     6053 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/eval_model.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.398143 clayrs-0.4.0/clayrs/evaluation/eval_pipeline_modules/
--rw-rw-rw-   0        0        0        2 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/evaluation/eval_pipeline_modules/__init__.py
--rw-rw-rw-   0        0        0     7634 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py
--rw-rw-rw-   0        0        0      158 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/evaluation/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.458527 clayrs-0.4.0/clayrs/evaluation/metrics/
--rw-rw-rw-   0        0        0      412 2022-09-20 11:34:40.000000 clayrs-0.4.0/clayrs/evaluation/metrics/__init__.py
--rw-rw-rw-   0        0        0    23860 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/metrics/classification_metrics.py
--rw-rw-rw-   0        0        0     7918 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/metrics/error_metrics.py
--rw-rw-rw-   0        0        0    23608 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/metrics/fairness_metrics.py
--rw-rw-rw-   0        0        0     1043 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/metrics/metrics.py
--rw-rw-rw-   0        0        0    26717 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/metrics/plot_metrics.py
--rw-rw-rw-   0        0        0    20138 2022-11-30 17:09:26.000000 clayrs-0.4.0/clayrs/evaluation/metrics/ranking_metrics.py
--rw-rw-rw-   0        0        0     5220 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/evaluation/statistical_test.py
--rw-rw-rw-   0        0        0     3696 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/evaluation/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.492469 clayrs-0.4.0/clayrs/recsys/
--rw-rw-rw-   0        0        0      528 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/__init__.py
--rw-rw-rw-   0        0        0      967 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/algorithm.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.523825 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/
--rw-rw-rw-   0        0        0      224 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.540095 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/centroid_vector/
--rw-rw-rw-   0        0        0       89 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/centroid_vector/__init__.py
--rw-rw-rw-   0        0        0    12467 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py
--rw-rw-rw-   0        0        0     1262 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/centroid_vector/similarities.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.571168 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/classifier/
--rw-rw-rw-   0        0        0      171 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/classifier/__init__.py
--rw-rw-rw-   0        0        0    13108 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py
--rw-rw-rw-   0        0        0    12738 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/classifier/classifiers.py
--rw-rw-rw-   0        0        0    13336 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/content_based_algorithm.py
--rw-rw-rw-   0        0        0     3369 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/contents_loader.py
--rw-rw-rw-   0        0        0     1291 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.587587 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/index_query/
--rw-rw-rw-   0        0        0       37 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/index_query/__init__.py
--rw-rw-rw-   0        0        0    13239 2022-09-20 11:34:40.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/index_query/index_query.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.618405 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/regressor/
--rw-rw-rw-   0        0        0      204 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/regressor/__init__.py
--rw-rw-rw-   0        0        0    13600 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py
--rw-rw-rw-   0        0        0    12396 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/recsys/content_based_algorithm/regressor/regressors.py
--rw-rw-rw-   0        0        0    32721 2022-11-30 17:09:26.000000 clayrs-0.4.0/clayrs/recsys/experiment.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.637756 clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/
--rw-rw-rw-   0        0        0       55 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/__init__.py
--rw-rw-rw-   0        0        0     5848 2022-11-22 11:49:37.000000 clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.647100 clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/page_rank/
--rw-rw-rw-   0        0        0       38 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/page_rank/__init__.py
--rw-rw-rw-   0        0        0    14333 2022-11-30 17:09:26.000000 clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py
--rw-rw-rw-   0        0        0     3864 2022-11-30 17:09:26.000000 clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/page_rank/page_rank.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.665692 clayrs-0.4.0/clayrs/recsys/graphs/
--rw-rw-rw-   0        0        0      123 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.697035 clayrs-0.4.0/clayrs/recsys/graphs/feature_selection/
--rw-rw-rw-   0        0        0      201 2022-07-01 12:58:18.000000 clayrs-0.4.0/clayrs/recsys/graphs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0      138 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/graphs/feature_selection/exceptions.py
--rw-rw-rw-   0        0        0    12098 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py
--rw-rw-rw-   0        0        0     7116 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py
--rw-rw-rw-   0        0        0    10668 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/graphs/graph.py
--rw-rw-rw-   0        0        0      390 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/graphs/graph_metrics.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.728595 clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/
--rw-rw-rw-   0        0        0      145 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/__init__.py
--rw-rw-rw-   0        0        0    12188 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py
--rw-rw-rw-   0        0        0    11042 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py
--rw-rw-rw-   0        0        0    14361 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py
--rw-rw-rw-   0        0        0    12052 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/methodology.py
--rw-rw-rw-   0        0        0    14672 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/recsys/partitioning.py
--rw-rw-rw-   0        0        0    31969 2022-11-22 11:49:37.000000 clayrs-0.4.0/clayrs/recsys/recsys.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.807955 clayrs-0.4.0/clayrs/utils/
--rw-rw-rw-   0        0        0       77 2022-10-18 17:41:50.000000 clayrs-0.4.0/clayrs/utils/__init__.py
--rw-rw-rw-   0        0        0     1223 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/utils/automatic_methods.py
--rw-rw-rw-   0        0        0     1422 2022-06-07 21:08:29.000000 clayrs-0.4.0/clayrs/utils/class_utils.py
--rw-rw-rw-   0        0        0      327 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/utils/const.py
--rw-rw-rw-   0        0        0     1784 2022-11-28 11:11:59.000000 clayrs-0.4.0/clayrs/utils/context_managers.py
--rw-rw-rw-   0        0        0     1313 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/utils/custom_logger.py
--rw-rw-rw-   0        0        0     1852 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/utils/load_content.py
--rw-rw-rw-   0        0        0    16554 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/utils/report.py
--rw-rw-rw-   0        0        0     4166 2022-10-18 22:52:53.000000 clayrs-0.4.0/clayrs/utils/save_content.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.002687 clayrs-0.4.0/clayrs.egg-info/
--rw-rw-rw-   0        0        0     8098 2022-11-30 17:27:51.000000 clayrs-0.4.0/clayrs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11194 2022-11-30 17:27:51.000000 clayrs-0.4.0/clayrs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-30 17:27:51.000000 clayrs-0.4.0/clayrs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      440 2022-11-30 17:27:51.000000 clayrs-0.4.0/clayrs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-30 17:27:51.000000 clayrs-0.4.0/clayrs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2022-06-07 21:08:29.000000 clayrs-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      467 2022-11-09 12:20:46.000000 clayrs-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2022-11-30 17:27:53.422887 clayrs-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1636 2022-11-30 17:09:16.000000 clayrs-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.807955 clayrs-0.4.0/test/
--rw-rw-rw-   0        0        0       85 2022-08-23 14:07:43.000000 clayrs-0.4.0/test/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.855780 clayrs-0.4.0/test/content_analyzer/
--rw-rw-rw-   0        0        0      114 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.877325 clayrs-0.4.0/test/content_analyzer/content_representation/
--rw-rw-rw-   0        0        0      114 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/content_representation/__init__.py
--rw-rw-rw-   0        0        0     6125 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/content_representation/test_content.py
--rw-rw-rw-   0        0        0     3165 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/content_representation/test_representation_container.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.887342 clayrs-0.4.0/test/content_analyzer/embeddings/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.955274 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/__init__.py
--rw-rw-rw-   0        0        0      837 2022-11-22 22:28:31.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py
--rw-rw-rw-   0        0        0     5370 2022-11-22 22:28:31.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py
--rw-rw-rw-   0        0        0      837 2022-11-22 22:28:31.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py
--rw-rw-rw-   0        0        0     2596 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py
--rw-rw-rw-   0        0        0     2578 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_lda.py
--rw-rw-rw-   0        0        0     2492 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py
--rw-rw-rw-   0        0        0      835 2022-11-22 22:28:31.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:52.999431 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/__init__.py
--rw-rw-rw-   0        0        0     1682 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py
--rw-rw-rw-   0        0        0     1015 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/test_sbert.py
--rw-rw-rw-   0        0        0     7373 2022-07-01 12:58:18.000000 clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/test_transformer.py
--rw-rw-rw-   0        0        0     1464 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/embeddings/test_embedding_source.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.032448 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.045305 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/embedding_technique/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
--rw-rw-rw-   0        0        0     1839 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py
--rw-rw-rw-   0        0        0     5328 2022-07-01 12:58:18.000000 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py
--rw-rw-rw-   0        0        0     5441 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/test_field_content_production_technique.py
--rw-rw-rw-   0        0        0      761 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py
--rw-rw-rw-   0        0        0     1123 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/test_tf_idf.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.076814 clayrs-0.4.0/test/content_analyzer/information_processor/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/information_processor/__init__.py
--rw-rw-rw-   0        0        0     6760 2022-11-22 22:28:31.000000 clayrs-0.4.0/test/content_analyzer/information_processor/test_ekphrasis.py
--rw-rw-rw-   0        0        0     4666 2022-11-22 22:28:31.000000 clayrs-0.4.0/test/content_analyzer/information_processor/test_nlp.py
--rw-rw-rw-   0        0        0     5417 2022-11-22 22:28:31.000000 clayrs-0.4.0/test/content_analyzer/information_processor/test_spacy.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.092715 clayrs-0.4.0/test/content_analyzer/memory_interfaces/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/memory_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5970 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/memory_interfaces/test_text_interface.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.108497 clayrs-0.4.0/test/content_analyzer/ratings_manager/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/ratings_manager/__init__.py
--rw-rw-rw-   0        0        0     1634 2022-07-01 12:58:18.000000 clayrs-0.4.0/test/content_analyzer/ratings_manager/test_rating_processor.py
--rw-rw-rw-   0        0        0    16379 2022-09-20 11:34:40.000000 clayrs-0.4.0/test/content_analyzer/ratings_manager/test_ratings.py
--rw-rw-rw-   0        0        0      878 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/ratings_manager/test_sentiment_analysis.py
--rw-rw-rw-   0        0        0     2861 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/test_config.py
--rw-rw-rw-   0        0        0    13832 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/content_analyzer/test_content_analyzer_main.py
--rw-rw-rw-   0        0        0    12250 2022-11-22 11:49:37.000000 clayrs-0.4.0/test/content_analyzer/test_exogenous_properties_retrieval.py
--rw-rw-rw-   0        0        0    16062 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/content_analyzer/test_raw_information_source.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.125223 clayrs-0.4.0/test/content_analyzer/utils/
--rw-rw-rw-   0        0        0        0 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/content_analyzer/utils/__init__.py
--rw-rw-rw-   0        0        0      630 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/content_analyzer/utils/test_check_tokenization.py
--rw-rw-rw-   0        0        0      769 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/content_analyzer/utils/test_id_merger.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.156394 clayrs-0.4.0/test/evaluation/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.173949 clayrs-0.4.0/test/evaluation/eval_pipeline_modules/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/evaluation/eval_pipeline_modules/__init__.py
--rw-rw-rw-   0        0        0     7197 2022-09-20 11:34:40.000000 clayrs-0.4.0/test/evaluation/eval_pipeline_modules/test_metric_evaluator.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.219219 clayrs-0.4.0/test/evaluation/metrics/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/evaluation/metrics/__init__.py
--rw-rw-rw-   0        0        0    37484 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/evaluation/metrics/test_classification_metrics.py
--rw-rw-rw-   0        0        0     9022 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/evaluation/metrics/test_error_metrics.py
--rw-rw-rw-   0        0        0    30699 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/evaluation/metrics/test_fairness_metrics.py
--rw-rw-rw-   0        0        0    24104 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/evaluation/metrics/test_plot_metrics.py
--rw-rw-rw-   0        0        0    18261 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/evaluation/metrics/test_ranking_metrics.py
--rw-rw-rw-   0        0        0    11551 2022-08-26 22:39:15.000000 clayrs-0.4.0/test/evaluation/test_eval_model.py
--rw-rw-rw-   0        0        0    15955 2022-06-24 10:21:32.000000 clayrs-0.4.0/test/evaluation/test_statistical_tests.py
--rw-rw-rw-   0        0        0     3818 2022-07-01 12:58:18.000000 clayrs-0.4.0/test/evaluation/test_utils.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.250707 clayrs-0.4.0/test/recsys/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.266348 clayrs-0.4.0/test/recsys/content_based_algorithm/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.281971 clayrs-0.4.0/test/recsys/content_based_algorithm/centroid_vector/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/centroid_vector/__init__.py
--rw-rw-rw-   0        0        0     7435 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py
--rw-rw-rw-   0        0        0     1020 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/centroid_vector/test_similarities.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.297595 clayrs-0.4.0/test/recsys/content_based_algorithm/classifier/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/classifier/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/classifier/test_classifier.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.297595 clayrs-0.4.0/test/recsys/content_based_algorithm/index_query/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/index_query/__init__.py
--rw-rw-rw-   0        0        0     7134 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/index_query/test_index_query.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.313890 clayrs-0.4.0/test/recsys/content_based_algorithm/regressor/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/regressor/__init__.py
--rw-rw-rw-   0        0        0     9912 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/regressor/test_regression.py
--rw-rw-rw-   0        0        0     4739 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/test_content_based_algorithm.py
--rw-rw-rw-   0        0        0     1887 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/content_based_algorithm/test_contents_loader.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.328905 clayrs-0.4.0/test/recsys/graph_based_algorithm/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graph_based_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.334744 clayrs-0.4.0/test/recsys/graph_based_algorithm/page_rank/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graph_based_algorithm/page_rank/__init__.py
--rw-rw-rw-   0        0        0     6780 2022-11-30 17:09:26.000000 clayrs-0.4.0/test/recsys/graph_based_algorithm/page_rank/test_nx_page_rank.py
--rw-rw-rw-   0        0        0     5312 2022-11-30 17:09:26.000000 clayrs-0.4.0/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py
--rw-rw-rw-   0        0        0     3161 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.334744 clayrs-0.4.0/test/recsys/graphs/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.344754 clayrs-0.4.0/test/recsys/graphs/feature_selection/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graphs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0     6561 2022-07-01 12:58:18.000000 clayrs-0.4.0/test/recsys/graphs/feature_selection/test_feature_selection.py
--rw-rw-rw-   0        0        0     7296 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graphs/feature_selection/test_feature_selection_alg.py
--rw-rw-rw-   0        0        0     2288 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graphs/test_graph.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.376011 clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/
--rw-rw-rw-   0        0        0        0 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/__init__.py
--rw-rw-rw-   0        0        0    16619 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py
--rw-rw-rw-   0        0        0    14057 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py
--rw-rw-rw-   0        0        0    15747 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py
--rw-rw-rw-   0        0        0    19963 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/recsys/test_experiment.py
--rw-rw-rw-   0        0        0    17658 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/recsys/test_methodology.py
--rw-rw-rw-   0        0        0     8271 2022-09-20 11:34:40.000000 clayrs-0.4.0/test/recsys/test_partitioning.py
--rw-rw-rw-   0        0        0    15538 2022-09-20 11:34:40.000000 clayrs-0.4.0/test/recsys/test_recsys.py
-drwxrwxrwx   0        0        0        0 2022-11-30 17:27:53.422887 clayrs-0.4.0/test/utils/
--rw-rw-rw-   0        0        0      115 2022-10-18 22:52:53.000000 clayrs-0.4.0/test/utils/__init__.py
--rw-rw-rw-   0        0        0     2663 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/utils/test_automatic_methods.py
--rw-rw-rw-   0        0        0     1105 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/utils/test_class_utils.py
--rw-rw-rw-   0        0        0     1495 2022-09-20 11:34:40.000000 clayrs-0.4.0/test/utils/test_context_managers.py
--rw-rw-rw-   0        0        0      451 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/utils/test_load_content.py
--rw-rw-rw-   0        0        0    10245 2022-06-07 21:08:29.000000 clayrs-0.4.0/test/utils/test_report.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.777305 clayrs-0.4.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-12 09:52:17.000000 clayrs-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-06-12 09:52:17.000000 clayrs-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8186 2023-06-12 09:58:37.777305 clayrs-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6977 2023-06-12 09:52:17.000000 clayrs-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.452087 clayrs-0.4.1/clayrs/
+-rw-rw-rw-   0        0        0       80 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.497641 clayrs-0.4.1/clayrs/content_analyzer/
+-rw-rw-rw-   0        0        0      777 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/__init__.py
+-rw-rw-rw-   0        0        0    19919 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/config.py
+-rw-rw-rw-   0        0        0    13001 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_analyzer_main.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.501662 clayrs-0.4.1/clayrs/content_analyzer/content_representation/
+-rw-rw-rw-   0        0        0       28 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_representation/__init__.py
+-rw-rw-rw-   0        0        0    17711 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_representation/content.py
+-rw-rw-rw-   0        0        0     9660 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_representation/representation_container.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.504662 clayrs-0.4.1/clayrs/content_analyzer/embeddings/
+-rw-rw-rw-   0        0        0      134 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.516769 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/
+-rw-rw-rw-   0        0        0      259 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/__init__.py
+-rw-rw-rw-   0        0        0     2015 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py
+-rw-rw-rw-   0        0        0    12971 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py
+-rw-rw-rw-   0        0        0     1918 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py
+-rw-rw-rw-   0        0        0     2999 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py
+-rw-rw-rw-   0        0        0     2716 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/lda.py
+-rw-rw-rw-   0        0        0     2961 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py
+-rw-rw-rw-   0        0        0     1791 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.525175 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/
+-rw-rw-rw-   0        0        0      182 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/__init__.py
+-rw-rw-rw-   0        0        0     3502 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py
+-rw-rw-rw-   0        0        0     1265 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py
+-rw-rw-rw-   0        0        0     1362 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py
+-rw-rw-rw-   0        0        0     6168 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py
+-rw-rw-rw-   0        0        0     2327 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py
+-rw-rw-rw-   0        0        0     4182 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_source.py
+-rw-rw-rw-   0        0        0      659 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/exceptions.py
+-rw-rw-rw-   0        0        0    27437 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/exogenous_properties_retrieval.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.532183 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/
+-rw-rw-rw-   0        0        0      251 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.536472 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/
+-rw-rw-rw-   0        0        0      271 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py
+-rw-rw-rw-   0        0        0    22732 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py
+-rw-rw-rw-   0        0        0    17916 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py
+-rw-rw-rw-   0        0        0     3346 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py
+-rw-rw-rw-   0        0        0     7598 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.544383 clayrs-0.4.1/clayrs/content_analyzer/information_processor/
+-rw-rw-rw-   0        0        0       84 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/__init__.py
+-rw-rw-rw-   0        0        0    11229 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/ekphrasis.py
+-rw-rw-rw-   0        0        0     2402 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/information_processor.py
+-rw-rw-rw-   0        0        0    11713 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/nltk.py
+-rw-rw-rw-   0        0        0    11797 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/spacy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.548856 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/
+-rw-rw-rw-   0        0        0       55 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5433 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py
+-rw-rw-rw-   0        0        0    12924 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/text_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.555330 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/
+-rw-rw-rw-   0        0        0      154 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/__init__.py
+-rw-rw-rw-   0        0        0    31916 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/ratings.py
+-rw-rw-rw-   0        0        0     2776 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/score_processor.py
+-rw-rw-rw-   0        0        0     1163 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py
+-rw-rw-rw-   0        0        0    14008 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/raw_information_source.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.559810 clayrs-0.4.1/clayrs/content_analyzer/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/utils/__init__.py
+-rw-rw-rw-   0        0        0     1070 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/utils/check_tokenization.py
+-rw-rw-rw-   0        0        0     1252 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/utils/id_merger.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.567256 clayrs-0.4.1/clayrs/evaluation/
+-rw-rw-rw-   0        0        0      206 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     6053 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/eval_model.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.569324 clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/
+-rw-rw-rw-   0        0        0        2 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/__init__.py
+-rw-rw-rw-   0        0        0     7634 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py
+-rw-rw-rw-   0        0        0      158 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.580837 clayrs-0.4.1/clayrs/evaluation/metrics/
+-rw-rw-rw-   0        0        0      412 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0    23860 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/classification_metrics.py
+-rw-rw-rw-   0        0        0     7918 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/error_metrics.py
+-rw-rw-rw-   0        0        0    23608 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/fairness_metrics.py
+-rw-rw-rw-   0        0        0     1043 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/metrics.py
+-rw-rw-rw-   0        0        0    26717 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/plot_metrics.py
+-rw-rw-rw-   0        0        0    20138 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/ranking_metrics.py
+-rw-rw-rw-   0        0        0     5220 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/statistical_test.py
+-rw-rw-rw-   0        0        0     3696 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.589179 clayrs-0.4.1/clayrs/recsys/
+-rw-rw-rw-   0        0        0      528 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.594184 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/
+-rw-rw-rw-   0        0        0      224 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.598183 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/
+-rw-rw-rw-   0        0        0       89 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/__init__.py
+-rw-rw-rw-   0        0        0    12467 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py
+-rw-rw-rw-   0        0        0     1262 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/similarities.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.603180 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/
+-rw-rw-rw-   0        0        0      171 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/__init__.py
+-rw-rw-rw-   0        0        0    13108 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py
+-rw-rw-rw-   0        0        0    12738 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifiers.py
+-rw-rw-rw-   0        0        0    13336 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/content_based_algorithm.py
+-rw-rw-rw-   0        0        0     3369 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/contents_loader.py
+-rw-rw-rw-   0        0        0     1291 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.606183 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/
+-rw-rw-rw-   0        0        0       37 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/__init__.py
+-rw-rw-rw-   0        0        0    13239 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/index_query.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.610183 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/
+-rw-rw-rw-   0        0        0      204 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/__init__.py
+-rw-rw-rw-   0        0        0    13600 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py
+-rw-rw-rw-   0        0        0    12396 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/regressors.py
+-rw-rw-rw-   0        0        0    32721 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/experiment.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.613178 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/
+-rw-rw-rw-   0        0        0       55 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/__init__.py
+-rw-rw-rw-   0        0        0     5848 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.618328 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/
+-rw-rw-rw-   0        0        0       38 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/__init__.py
+-rw-rw-rw-   0        0        0    14333 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py
+-rw-rw-rw-   0        0        0     3864 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/page_rank.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.622328 clayrs-0.4.1/clayrs/recsys/graphs/
+-rw-rw-rw-   0        0        0      123 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.628330 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/
+-rw-rw-rw-   0        0        0      201 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/exceptions.py
+-rw-rw-rw-   0        0        0    12098 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py
+-rw-rw-rw-   0        0        0     7116 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py
+-rw-rw-rw-   0        0        0    10668 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/graph.py
+-rw-rw-rw-   0        0        0      390 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/graph_metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.633660 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/
+-rw-rw-rw-   0        0        0      145 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/__init__.py
+-rw-rw-rw-   0        0        0    12188 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py
+-rw-rw-rw-   0        0        0    11042 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py
+-rw-rw-rw-   0        0        0    14361 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py
+-rw-rw-rw-   0        0        0    12052 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/methodology.py
+-rw-rw-rw-   0        0        0    14672 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/partitioning.py
+-rw-rw-rw-   0        0        0    31969 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/recsys.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.646727 clayrs-0.4.1/clayrs/utils/
+-rw-rw-rw-   0        0        0       77 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1223 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/automatic_methods.py
+-rw-rw-rw-   0        0        0     1422 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/class_utils.py
+-rw-rw-rw-   0        0        0      327 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/const.py
+-rw-rw-rw-   0        0        0     1784 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/context_managers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/custom_logger.py
+-rw-rw-rw-   0        0        0     1852 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/load_content.py
+-rw-rw-rw-   0        0        0    16554 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/report.py
+-rw-rw-rw-   0        0        0     4166 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/save_content.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.488671 clayrs-0.4.1/clayrs.egg-info/
+-rw-rw-rw-   0        0        0     8186 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11194 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      440 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2023-06-12 09:52:18.000000 clayrs-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0      467 2023-06-12 09:52:18.000000 clayrs-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 09:58:37.779575 clayrs-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1691 2023-06-12 09:58:30.000000 clayrs-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.648738 clayrs-0.4.1/test/
+-rw-rw-rw-   0        0        0       85 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.655269 clayrs-0.4.1/test/content_analyzer/
+-rw-rw-rw-   0        0        0      114 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.660259 clayrs-0.4.1/test/content_analyzer/content_representation/
+-rw-rw-rw-   0        0        0      114 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/content_representation/__init__.py
+-rw-rw-rw-   0        0        0     6125 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/content_representation/test_content.py
+-rw-rw-rw-   0        0        0     3165 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/content_representation/test_representation_container.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.662262 clayrs-0.4.1/test/content_analyzer/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.674038 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py
+-rw-rw-rw-   0        0        0     5370 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py
+-rw-rw-rw-   0        0        0      837 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py
+-rw-rw-rw-   0        0        0     2596 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py
+-rw-rw-rw-   0        0        0     2578 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_lda.py
+-rw-rw-rw-   0        0        0     2492 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py
+-rw-rw-rw-   0        0        0      835 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.679042 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/__init__.py
+-rw-rw-rw-   0        0        0     1682 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py
+-rw-rw-rw-   0        0        0     1015 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_sbert.py
+-rw-rw-rw-   0        0        0     7373 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_transformer.py
+-rw-rw-rw-   0        0        0     1464 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/test_embedding_source.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.685241 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.689243 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
+-rw-rw-rw-   0        0        0     1839 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py
+-rw-rw-rw-   0        0        0     5328 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py
+-rw-rw-rw-   0        0        0     5441 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_field_content_production_technique.py
+-rw-rw-rw-   0        0        0      761 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py
+-rw-rw-rw-   0        0        0     1123 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_tf_idf.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.694672 clayrs-0.4.1/test/content_analyzer/information_processor/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/__init__.py
+-rw-rw-rw-   0        0        0     6760 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/test_ekphrasis.py
+-rw-rw-rw-   0        0        0     4666 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/test_nlp.py
+-rw-rw-rw-   0        0        0     5417 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/test_spacy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.697676 clayrs-0.4.1/test/content_analyzer/memory_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/memory_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5970 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/memory_interfaces/test_text_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.703334 clayrs-0.4.1/test/content_analyzer/ratings_manager/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/test_rating_processor.py
+-rw-rw-rw-   0        0        0    16379 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/test_ratings.py
+-rw-rw-rw-   0        0        0      878 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/test_sentiment_analysis.py
+-rw-rw-rw-   0        0        0     2861 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_config.py
+-rw-rw-rw-   0        0        0    13832 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_content_analyzer_main.py
+-rw-rw-rw-   0        0        0    12250 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_exogenous_properties_retrieval.py
+-rw-rw-rw-   0        0        0    16062 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_raw_information_source.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.706735 clayrs-0.4.1/test/content_analyzer/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/utils/__init__.py
+-rw-rw-rw-   0        0        0      630 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/utils/test_check_tokenization.py
+-rw-rw-rw-   0        0        0      769 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/utils/test_id_merger.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.712530 clayrs-0.4.1/test/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.715633 clayrs-0.4.1/test/evaluation/eval_pipeline_modules/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/eval_pipeline_modules/__init__.py
+-rw-rw-rw-   0        0        0     7197 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/eval_pipeline_modules/test_metric_evaluator.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.722831 clayrs-0.4.1/test/evaluation/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0    37484 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_classification_metrics.py
+-rw-rw-rw-   0        0        0     9022 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_error_metrics.py
+-rw-rw-rw-   0        0        0    30699 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_fairness_metrics.py
+-rw-rw-rw-   0        0        0    24104 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_plot_metrics.py
+-rw-rw-rw-   0        0        0    18261 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_ranking_metrics.py
+-rw-rw-rw-   0        0        0    11551 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/test_eval_model.py
+-rw-rw-rw-   0        0        0    15955 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/test_statistical_tests.py
+-rw-rw-rw-   0        0        0     3818 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.730845 clayrs-0.4.1/test/recsys/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.734847 clayrs-0.4.1/test/recsys/content_based_algorithm/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.738842 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/__init__.py
+-rw-rw-rw-   0        0        0     7435 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py
+-rw-rw-rw-   0        0        0     1020 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/test_similarities.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.741844 clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/__init__.py
+-rw-rw-rw-   0        0        0     8845 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/test_classifier.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.745116 clayrs-0.4.1/test/recsys/content_based_algorithm/index_query/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/index_query/__init__.py
+-rw-rw-rw-   0        0        0     7134 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/index_query/test_index_query.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.747113 clayrs-0.4.1/test/recsys/content_based_algorithm/regressor/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/regressor/__init__.py
+-rw-rw-rw-   0        0        0     9912 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/regressor/test_regression.py
+-rw-rw-rw-   0        0        0     4739 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/test_content_based_algorithm.py
+-rw-rw-rw-   0        0        0     1887 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/test_contents_loader.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.750115 clayrs-0.4.1/test/recsys/graph_based_algorithm/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.754113 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/__init__.py
+-rw-rw-rw-   0        0        0     6780 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/test_nx_page_rank.py
+-rw-rw-rw-   0        0        0     5312 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py
+-rw-rw-rw-   0        0        0     3161 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.756360 clayrs-0.4.1/test/recsys/graphs/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.760439 clayrs-0.4.1/test/recsys/graphs/feature_selection/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0     6561 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection.py
+-rw-rw-rw-   0        0        0     7296 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection_alg.py
+-rw-rw-rw-   0        0        0     2288 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_graph.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.765582 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/__init__.py
+-rw-rw-rw-   0        0        0    16619 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py
+-rw-rw-rw-   0        0        0    14057 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py
+-rw-rw-rw-   0        0        0    15747 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py
+-rw-rw-rw-   0        0        0    19963 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_experiment.py
+-rw-rw-rw-   0        0        0    17658 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_methodology.py
+-rw-rw-rw-   0        0        0     8271 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_partitioning.py
+-rw-rw-rw-   0        0        0    15538 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_recsys.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.775301 clayrs-0.4.1/test/utils/
+-rw-rw-rw-   0        0        0      115 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/__init__.py
+-rw-rw-rw-   0        0        0     2663 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_automatic_methods.py
+-rw-rw-rw-   0        0        0     1105 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_class_utils.py
+-rw-rw-rw-   0        0        0     1495 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_context_managers.py
+-rw-rw-rw-   0        0        0      451 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_load_content.py
+-rw-rw-rw-   0        0        0    10245 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_report.py
```

### Comparing `clayrs-0.4.0/LICENSE` & `clayrs-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/PKG-INFO` & `clayrs-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: clayrs
-Version: 0.4.0
+Version: 0.4.1
 Summary: Complexly represent contents, build recommender systems, evaluate them. All in one place!
 Home-page: https://github.com/swapUniba/ClayRS
 Author: Antonio Silletti, Elio Musacchio, Roberta Sallustio
 License: GPL-3.0
 Keywords: recommender system,cbrs,evaluation,recsys
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -29,15 +31,15 @@
 
 
 # ClayRS
 
 [![Build Status](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml/badge.svg)](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml)&nbsp;&nbsp;
 [![Docs](https://github.com/swapUniba/ClayRS/actions/workflows/docs_building.yml/badge.svg)](https://swapuniba.github.io/ClayRS/)&nbsp;&nbsp;
 [![codecov](https://codecov.io/gh/swapUniba/ClayRS/branch/master/graph/badge.svg?token=dftmT3QD8D)](https://codecov.io/gh/swapUniba/ClayRS)&nbsp;&nbsp;
-[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
 
 
 ***ClayRS*** is a python framework for (mainly) content-based recommender systems which allows you to perform several operations, starting from a raw representation of users and items to building and evaluating a recommender system. It also supports graph-based recommendation with feature selection algorithms and graph manipulation methods.
 
 The framework has three main modules, which you can also use individually:
 
 <p align="center">
@@ -205,7 +207,9 @@
 
 ```python
 sys_result, users_result =  em.fit()
 ```
 
 Note that the EvalModel is able to compute evaluation of recommendations generated by other tools/frameworks, check
 documentation for more
+
+
```

### Comparing `clayrs-0.4.0/README.md` & `clayrs-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # ClayRS
 
 [![Build Status](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml/badge.svg)](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml)&nbsp;&nbsp;
 [![Docs](https://github.com/swapUniba/ClayRS/actions/workflows/docs_building.yml/badge.svg)](https://swapuniba.github.io/ClayRS/)&nbsp;&nbsp;
 [![codecov](https://codecov.io/gh/swapUniba/ClayRS/branch/master/graph/badge.svg?token=dftmT3QD8D)](https://codecov.io/gh/swapUniba/ClayRS)&nbsp;&nbsp;
-[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
 
 
 ***ClayRS*** is a python framework for (mainly) content-based recommender systems which allows you to perform several operations, starting from a raw representation of users and items to building and evaluating a recommender system. It also supports graph-based recommendation with feature selection algorithms and graph manipulation methods.
 
 The framework has three main modules, which you can also use individually:
 
 <p align="center">
```

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/__init__.py` & `clayrs-0.4.1/clayrs/content_analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/config.py` & `clayrs-0.4.1/clayrs/content_analyzer/config.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/content_analyzer_main.py` & `clayrs-0.4.1/clayrs/content_analyzer/content_analyzer_main.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/content_representation/content.py` & `clayrs-0.4.1/clayrs/content_analyzer/content_representation/content.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/content_representation/representation_container.py` & `clayrs-0.4.1/clayrs/content_analyzer/content_representation/representation_container.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/lda.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/lda.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/embeddings/embedding_source.py` & `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_source.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/exceptions.py` & `clayrs-0.4.1/clayrs/content_analyzer/exceptions.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/exogenous_properties_retrieval.py` & `clayrs-0.4.1/clayrs/content_analyzer/exogenous_properties_retrieval.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py` & `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py` & `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py` & `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py` & `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py` & `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/information_processor/ekphrasis.py` & `clayrs-0.4.1/clayrs/content_analyzer/information_processor/ekphrasis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/information_processor/information_processor.py` & `clayrs-0.4.1/clayrs/content_analyzer/information_processor/information_processor.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/information_processor/nltk.py` & `clayrs-0.4.1/clayrs/content_analyzer/information_processor/nltk.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/information_processor/spacy.py` & `clayrs-0.4.1/clayrs/content_analyzer/information_processor/spacy.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py` & `clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/memory_interfaces/text_interface.py` & `clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/text_interface.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/ratings.py` & `clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/ratings.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/score_processor.py` & `clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/score_processor.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py` & `clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/raw_information_source.py` & `clayrs-0.4.1/clayrs/content_analyzer/raw_information_source.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/utils/check_tokenization.py` & `clayrs-0.4.1/clayrs/content_analyzer/utils/check_tokenization.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/content_analyzer/utils/id_merger.py` & `clayrs-0.4.1/clayrs/content_analyzer/utils/id_merger.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/eval_model.py` & `clayrs-0.4.1/clayrs/evaluation/eval_model.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py` & `clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/metrics/classification_metrics.py` & `clayrs-0.4.1/clayrs/evaluation/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/metrics/error_metrics.py` & `clayrs-0.4.1/clayrs/evaluation/metrics/error_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/metrics/fairness_metrics.py` & `clayrs-0.4.1/clayrs/evaluation/metrics/fairness_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/metrics/metrics.py` & `clayrs-0.4.1/clayrs/evaluation/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/metrics/plot_metrics.py` & `clayrs-0.4.1/clayrs/evaluation/metrics/plot_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/metrics/ranking_metrics.py` & `clayrs-0.4.1/clayrs/evaluation/metrics/ranking_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/statistical_test.py` & `clayrs-0.4.1/clayrs/evaluation/statistical_test.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/evaluation/utils.py` & `clayrs-0.4.1/clayrs/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/__init__.py` & `clayrs-0.4.1/clayrs/recsys/__init__.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/algorithm.py` & `clayrs-0.4.1/clayrs/recsys/algorithm.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/centroid_vector/similarities.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/similarities.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/classifier/classifiers.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifiers.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/content_based_algorithm.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/content_based_algorithm.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/contents_loader.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/contents_loader.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/exceptions.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/exceptions.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/index_query/index_query.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/index_query.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/content_based_algorithm/regressor/regressors.py` & `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/regressors.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/experiment.py` & `clayrs-0.4.1/clayrs/recsys/experiment.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py` & `clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py` & `clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graph_based_algorithm/page_rank/page_rank.py` & `clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/page_rank.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py` & `clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py` & `clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graphs/graph.py` & `clayrs-0.4.1/clayrs/recsys/graphs/graph.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py` & `clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py` & `clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py` & `clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/methodology.py` & `clayrs-0.4.1/clayrs/recsys/methodology.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/partitioning.py` & `clayrs-0.4.1/clayrs/recsys/partitioning.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/recsys/recsys.py` & `clayrs-0.4.1/clayrs/recsys/recsys.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/utils/automatic_methods.py` & `clayrs-0.4.1/clayrs/utils/automatic_methods.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/utils/class_utils.py` & `clayrs-0.4.1/clayrs/utils/class_utils.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/utils/context_managers.py` & `clayrs-0.4.1/clayrs/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/utils/custom_logger.py` & `clayrs-0.4.1/clayrs/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/utils/load_content.py` & `clayrs-0.4.1/clayrs/utils/load_content.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/utils/report.py` & `clayrs-0.4.1/clayrs/utils/report.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs/utils/save_content.py` & `clayrs-0.4.1/clayrs/utils/save_content.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/clayrs.egg-info/PKG-INFO` & `clayrs-0.4.1/clayrs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: clayrs
-Version: 0.4.0
+Version: 0.4.1
 Summary: Complexly represent contents, build recommender systems, evaluate them. All in one place!
 Home-page: https://github.com/swapUniba/ClayRS
 Author: Antonio Silletti, Elio Musacchio, Roberta Sallustio
 License: GPL-3.0
 Keywords: recommender system,cbrs,evaluation,recsys
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -29,15 +31,15 @@
 
 
 # ClayRS
 
 [![Build Status](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml/badge.svg)](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml)&nbsp;&nbsp;
 [![Docs](https://github.com/swapUniba/ClayRS/actions/workflows/docs_building.yml/badge.svg)](https://swapuniba.github.io/ClayRS/)&nbsp;&nbsp;
 [![codecov](https://codecov.io/gh/swapUniba/ClayRS/branch/master/graph/badge.svg?token=dftmT3QD8D)](https://codecov.io/gh/swapUniba/ClayRS)&nbsp;&nbsp;
-[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
 
 
 ***ClayRS*** is a python framework for (mainly) content-based recommender systems which allows you to perform several operations, starting from a raw representation of users and items to building and evaluating a recommender system. It also supports graph-based recommendation with feature selection algorithms and graph manipulation methods.
 
 The framework has three main modules, which you can also use individually:
 
 <p align="center">
@@ -205,7 +207,9 @@
 
 ```python
 sys_result, users_result =  em.fit()
 ```
 
 Note that the EvalModel is able to compute evaluation of recommendations generated by other tools/frameworks, check
 documentation for more
+
+
```

### Comparing `clayrs-0.4.0/clayrs.egg-info/SOURCES.txt` & `clayrs-0.4.1/clayrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/setup.py` & `clayrs-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.4.0"
+VERSION = "0.4.1"
 
 setup(name='clayrs',
       version=VERSION,
       license='GPL-3.0',
       author='Antonio Silletti, Elio Musacchio, Roberta Sallustio',
       install_requires=requirements,
       description='Complexly represent contents, build recommender systems, evaluate them. All in one place!',
@@ -30,13 +30,14 @@
             'Operating System :: OS Independent',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3 :: Only',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
             'Topic :: Software Development :: Libraries',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Software Development :: Testing :: Unit'
       ]
 
       )
```

### Comparing `clayrs-0.4.0/test/content_analyzer/content_representation/test_content.py` & `clayrs-0.4.1/test/content_analyzer/content_representation/test_content.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/content_representation/test_representation_container.py` & `clayrs-0.4.1/test/content_analyzer/content_representation/test_representation_container.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_lda.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_lda.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/test_sbert.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_sbert.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/embedding_loader/test_transformer.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_transformer.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/embeddings/test_embedding_source.py` & `clayrs-0.4.1/test/content_analyzer/embeddings/test_embedding_source.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py` & `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py` & `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/test_field_content_production_technique.py` & `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_field_content_production_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py` & `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/field_content_production_techniques/test_tf_idf.py` & `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_tf_idf.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/information_processor/test_ekphrasis.py` & `clayrs-0.4.1/test/content_analyzer/information_processor/test_ekphrasis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/information_processor/test_nlp.py` & `clayrs-0.4.1/test/content_analyzer/information_processor/test_nlp.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/information_processor/test_spacy.py` & `clayrs-0.4.1/test/content_analyzer/information_processor/test_spacy.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/memory_interfaces/test_text_interface.py` & `clayrs-0.4.1/test/content_analyzer/memory_interfaces/test_text_interface.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/ratings_manager/test_rating_processor.py` & `clayrs-0.4.1/test/content_analyzer/ratings_manager/test_rating_processor.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/ratings_manager/test_ratings.py` & `clayrs-0.4.1/test/content_analyzer/ratings_manager/test_ratings.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/ratings_manager/test_sentiment_analysis.py` & `clayrs-0.4.1/test/content_analyzer/ratings_manager/test_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/test_config.py` & `clayrs-0.4.1/test/content_analyzer/test_config.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/test_content_analyzer_main.py` & `clayrs-0.4.1/test/content_analyzer/test_content_analyzer_main.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/test_exogenous_properties_retrieval.py` & `clayrs-0.4.1/test/content_analyzer/test_exogenous_properties_retrieval.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/test_raw_information_source.py` & `clayrs-0.4.1/test/content_analyzer/test_raw_information_source.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/utils/test_check_tokenization.py` & `clayrs-0.4.1/test/content_analyzer/utils/test_check_tokenization.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/content_analyzer/utils/test_id_merger.py` & `clayrs-0.4.1/test/content_analyzer/utils/test_id_merger.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/eval_pipeline_modules/test_metric_evaluator.py` & `clayrs-0.4.1/test/evaluation/eval_pipeline_modules/test_metric_evaluator.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/metrics/test_classification_metrics.py` & `clayrs-0.4.1/test/evaluation/metrics/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/metrics/test_error_metrics.py` & `clayrs-0.4.1/test/evaluation/metrics/test_error_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/metrics/test_fairness_metrics.py` & `clayrs-0.4.1/test/evaluation/metrics/test_fairness_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/metrics/test_plot_metrics.py` & `clayrs-0.4.1/test/evaluation/metrics/test_plot_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/metrics/test_ranking_metrics.py` & `clayrs-0.4.1/test/evaluation/metrics/test_ranking_metrics.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/test_eval_model.py` & `clayrs-0.4.1/test/evaluation/test_eval_model.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/test_statistical_tests.py` & `clayrs-0.4.1/test/evaluation/test_statistical_tests.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/evaluation/test_utils.py` & `clayrs-0.4.1/test/evaluation/test_utils.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py` & `clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/content_based_algorithm/centroid_vector/test_similarities.py` & `clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/test_similarities.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/content_based_algorithm/classifier/test_classifier.py` & `clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/test_classifier.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/content_based_algorithm/index_query/test_index_query.py` & `clayrs-0.4.1/test/recsys/content_based_algorithm/index_query/test_index_query.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/content_based_algorithm/regressor/test_regression.py` & `clayrs-0.4.1/test/recsys/content_based_algorithm/regressor/test_regression.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/content_based_algorithm/test_content_based_algorithm.py` & `clayrs-0.4.1/test/recsys/content_based_algorithm/test_content_based_algorithm.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/content_based_algorithm/test_contents_loader.py` & `clayrs-0.4.1/test/recsys/content_based_algorithm/test_contents_loader.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graph_based_algorithm/page_rank/test_nx_page_rank.py` & `clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/test_nx_page_rank.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py` & `clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py` & `clayrs-0.4.1/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graphs/feature_selection/test_feature_selection.py` & `clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graphs/feature_selection/test_feature_selection_alg.py` & `clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection_alg.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graphs/test_graph.py` & `clayrs-0.4.1/test/recsys/graphs/test_graph.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py` & `clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py` & `clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py` & `clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/test_experiment.py` & `clayrs-0.4.1/test/recsys/test_experiment.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/test_methodology.py` & `clayrs-0.4.1/test/recsys/test_methodology.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/test_partitioning.py` & `clayrs-0.4.1/test/recsys/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/recsys/test_recsys.py` & `clayrs-0.4.1/test/recsys/test_recsys.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/utils/test_automatic_methods.py` & `clayrs-0.4.1/test/utils/test_automatic_methods.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/utils/test_class_utils.py` & `clayrs-0.4.1/test/utils/test_class_utils.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/utils/test_context_managers.py` & `clayrs-0.4.1/test/utils/test_context_managers.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.0/test/utils/test_report.py` & `clayrs-0.4.1/test/utils/test_report.py`

 * *Files identical despite different names*

