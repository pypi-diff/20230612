# Comparing `tmp/gabarit-1.3.1.tar.gz` & `tmp/gabarit-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gabarit-1.3.1.tar", last modified: Tue Apr  4 09:13:15 2023, max compression
+gzip compressed data, was "gabarit-1.3.2.tar", last modified: Mon Jun 12 09:59:51 2023, max compression
```

## Comparing `gabarit-1.3.1.tar` & `gabarit-1.3.2.tar`

### file list

```diff
@@ -1,628 +1,628 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    31709 2023-04-04 09:13:12.000000 gabarit-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-04 09:13:12.000000 gabarit-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-04 09:13:15.415192 gabarit-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-04 09:13:12.000000 gabarit-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.355191 gabarit-1.3.1/gabarit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.355191 gabarit-1.3.1/gabarit/template_api/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.355191 gabarit-1.3.1/gabarit/template_api/api_project/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/.env
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/Dockerfile.svc
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/launch.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.355191 gabarit-1.3.1/gabarit/template_api/api_project/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.355191 gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/logtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_api/api_project/package_name/model/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/model/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/model/model_gabarit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/technical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/technical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_api/api_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/create_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/test_routers_functionnal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/test_routers_technical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/api_project/tests/test_schemas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_api/generate_api_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/default_model_upload_instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/generate_nlp_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/.dvc/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/nose_setup_coverage.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.367192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.367192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/f1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)    22904 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/model_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/model_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/model_huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.371192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_gbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_sgdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_svm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.371192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_gru.py
--rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    34177 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_tfidf_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/utils_deep_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/utils_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.371192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/monitoring/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/monitoring/model_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.371192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/preprocessing/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.347191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.359192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/
--rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/EDA.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.363191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/
--rw-r--r--   0 runner    (1001) docker     (123)  2071556 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/ds.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    54736 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    12778 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/negative.png
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/positive.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.363191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.363191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/post-checkout
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-push
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    60469 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/nlp.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.363191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/1_preprocess_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    25413 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/2_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/3_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/4_demonstrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.363191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_create_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_get_embedding_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_merge_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_reload_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_split_train_valid_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_sweetviz_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.347191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.347191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.363191 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/
--rw-r--r--   0 runner    (1001) docker     (123)    42642 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/Tutorial_fr.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.367192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/
--rw-r--r--   0 runner    (1001) docker     (123)   482890 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   483855 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/model_author.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/utils_tutorial_fr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.367192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/
--rw-r--r--   0 runner    (1001) docker     (123)    29124 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/Tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.367192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/
--rw-r--r--   0 runner    (1001) docker     (123)   104645 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/demonstrator.png
--rw-r--r--   0 runner    (1001) docker     (123)    51937 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/lstm_choice.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   111052 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1.png
--rw-r--r--   0 runner    (1001) docker     (123)    76097 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1_path.png
--rw-r--r--   0 runner    (1001) docker     (123)   244424 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model2.png
--rw-r--r--   0 runner    (1001) docker     (123)   205552 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/predictions.png
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/utils_main_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_dataset2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    70476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38695 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25490 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    26393 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    25921 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_gru.py
--rw-r--r--   0 runner    (1001) docker     (123)    37280 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    44562 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)    45397 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_gbt.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_sgdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29146 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_svm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26271 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_utils_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_nlp/nlp_project/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/default_model_upload_instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/generate_num_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/num_project/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/num_project/.dvc/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/nose_setup_coverage.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23285 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/model_aggregation_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    29275 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/model_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    19018 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/model_xgboost_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_gbt_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_knn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_lgbm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_logistic_regression_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_rf_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_ridge_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_sgd_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_svm_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/model_dense_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/model_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    30916 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/model_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/model_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/model_aggregation_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/model_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/model_xgboost_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.383192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_bayesian_ridge_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_elasticnet_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_gbt_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_kernel_ridge_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_knn_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_lgbm_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_pls_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_rf_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_sgd_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_svr_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.383192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/model_dense_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/utils_deep_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/utils_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.383192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/monitoring/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/monitoring/model_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.383192 gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/column_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/outlier_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.351191 gabarit-1.3.1/gabarit/template_num/num_project/package_name-exploration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/num_project/package_name-exploration/EDA/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-exploration/EDA/EDA.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/post-checkout
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-push
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    60469 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/robot.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.375192 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/1_preprocess_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/2_apply_existing_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28062 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/3_training_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22805 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/3_training_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/4_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/5_demonstrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_create_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    27678 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_fairness_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_merge_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_reload_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_split_train_valid_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_sweetviz_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.379192 gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/answers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    40496 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_num.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.387192 gabarit-1.3.1/gabarit/template_num/num_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_column_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_dataset2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    68571 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_aggregation_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    35247 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_aggregation_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_bayesian_ridge_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    51453 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    26116 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    30194 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_dense_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_dense_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_elasticnet_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_gbt_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_gbt_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    44315 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_kernel_ridge_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    38435 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_knn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_knn_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    38628 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_lgbm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_lgbm_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    39411 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_logistic_regression_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    28002 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_pls_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    38250 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_rf_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_rf_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    38696 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_ridge_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_sgd_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_sgd_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    38352 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_svm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_svr_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_xgboost_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_xgboost_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_outlier_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40962 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/tests/test_utils_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_num/num_project/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.387192 gabarit-1.3.1/gabarit/template_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/default_model_upload_instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/generate_vision_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.387192 gabarit-1.3.1/gabarit/template_vision/vision_project/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.387192 gabarit-1.3.1/gabarit/template_vision/vision_project/.dvc/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/nose_setup_coverage.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.387192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_cnn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    20699 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_transfer_learning_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/model_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/model_keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59082 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_detectron_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_keras_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    80849 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_object_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/utils_deep_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/utils_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.395192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/monitoring/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/monitoring/model_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.395192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/preprocessing/manage_white_borders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/preprocessing/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    26500 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.387192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/post-checkout
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-push
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    60469 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/robot.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/1_preprocess_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/2_training_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/2_training_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/3_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/4_demonstrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/utils/0_create_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/utils/0_reload_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/utils/0_split_train_valid_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.391192 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/answers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    34014 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_vision.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.395192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.395192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/apple_36.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.395192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/apple.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Bombay_19.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_34.jpg
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/toto.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_4.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_3.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_34.jpg
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/toto.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.351191 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_4.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.399192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/toto/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/toto/titi.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.403192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_3.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.403192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.403192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.403192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Bombay_19.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.403192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.403192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Bombay_19.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.407192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.407192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Bombay_19.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.407192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/preprocess_pipeline.conf
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.407192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Bombay_19.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.411192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.411192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.411192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/preprocess_pipeline.conf
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.355191 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.411192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_4.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.411192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_3.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_36.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_4.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/
--rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_19.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/preprocess_pipeline.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_15.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_30.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_31.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_34.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/metadata_bboxes.csv
--rw-r--r--   0 runner    (1001) docker     (123)   270880 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/mixed_22.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fake_metrics.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.415192 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/
--rw-r--r--   0 runner    (1001) docker     (123)    32016 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/apple_76.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/banana_76.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/metadata_bboxes.csv
--rw-r--r--   0 runner    (1001) docker     (123)   270880 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/mixed_22.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    48870 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/orange_77.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13984 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_map.json
--rw-r--r--   0 runner    (1001) docker     (123)    23879 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_manage_white_borders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_cnn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    89016 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_detectron_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_explainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    56452 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)    98567 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_keras_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)   131251 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_transfer_learning_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    21119 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils_faster_rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    22490 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    55754 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 09:13:12.000000 gabarit-1.3.1/gabarit/template_vision/vision_project/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:13:15.355191 gabarit-1.3.1/gabarit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-04 09:13:15.000000 gabarit-1.3.1/gabarit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    44358 2023-04-04 09:13:15.000000 gabarit-1.3.1/gabarit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:13:15.000000 gabarit-1.3.1/gabarit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-04 09:13:15.000000 gabarit-1.3.1/gabarit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 09:13:15.000000 gabarit-1.3.1/gabarit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 09:13:15.000000 gabarit-1.3.1/gabarit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 09:13:15.415192 gabarit-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-04 09:13:12.000000 gabarit-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.761584 gabarit-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    31709 2023-06-12 09:59:46.000000 gabarit-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-12 09:59:46.000000 gabarit-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-06-12 09:59:51.761584 gabarit-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-06-12 09:59:46.000000 gabarit-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.705584 gabarit-1.3.2/gabarit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.705584 gabarit-1.3.2/gabarit/template_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.705584 gabarit-1.3.2/gabarit/template_api/api_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/.env
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/launch.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.705584 gabarit-1.3.2/gabarit/template_api/api_project/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_api/api_project/package_name/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/model/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/model/model_gabarit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/technical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/technical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_api/api_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/create_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/test_routers_functionnal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/test_routers_technical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/api_project/tests/test_schemas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_api/generate_api_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/default_model_upload_instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/generate_nlp_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/nose_setup_coverage.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.709584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.721584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.721584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/f1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24253 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/model_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43711 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/model_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34984 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/model_huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.721584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_gbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_sgdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_svm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.721584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17723 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34572 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_tfidf_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15135 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/utils_deep_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/utils_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.721584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/monitoring/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/monitoring/model_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.721584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/preprocessing/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.689584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.713584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/
+-rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/EDA.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.713584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  2071556 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/ds.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    54736 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12778 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/negative.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/positive.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.713584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.713584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/post-checkout
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-push
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    60469 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/nlp.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.717584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/1_preprocess_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25413 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/2_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/3_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/4_demonstrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.717584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_create_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_get_embedding_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_merge_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_reload_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_split_train_valid_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_sweetviz_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.693584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.689584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.717584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/
+-rw-r--r--   0 runner    (1001) docker     (123)    42642 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/Tutorial_fr.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.717584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   482890 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   483855 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/model_author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/utils_tutorial_fr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.717584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/
+-rw-r--r--   0 runner    (1001) docker     (123)    29124 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/Tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.717584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   104645 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/demonstrator.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51937 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/lstm_choice.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   111052 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76097 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1_path.png
+-rw-r--r--   0 runner    (1001) docker     (123)   244424 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   205552 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/predictions.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/utils_main_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_dataset2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73923 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38695 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25706 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25770 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26673 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26201 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37560 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45686 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47919 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_gbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29816 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_sgdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29146 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_utils_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_nlp/nlp_project/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_num/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/default_model_upload_instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/generate_num_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_num/num_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_num/num_project/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/nose_setup_coverage.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24634 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/model_aggregation_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29295 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/model_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19018 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/model_xgboost_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_gbt_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_knn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_lgbm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_logistic_regression_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_rf_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_ridge_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_sgd_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_svm_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/model_dense_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/model_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31521 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/model_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/model_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15947 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/model_aggregation_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/model_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/model_xgboost_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.733584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_bayesian_ridge_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_elasticnet_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_gbt_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_kernel_ridge_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_knn_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_lgbm_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_pls_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_rf_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_sgd_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_svr_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.733584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/model_dense_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/utils_deep_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/utils_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.733584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/monitoring/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/monitoring/model_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.733584 gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/column_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/outlier_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.693584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-exploration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-exploration/EDA/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-exploration/EDA/EDA.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.725584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/post-checkout
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-push
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    60469 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/robot.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/1_preprocess_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/2_apply_existing_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28062 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/3_training_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22805 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/3_training_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/4_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/5_demonstrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_create_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27678 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_fairness_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_merge_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_reload_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_split_train_valid_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_sweetviz_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.729584 gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/answers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40496 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_num.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_num/num_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_column_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_dataset2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71994 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_aggregation_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36003 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_aggregation_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_bayesian_ridge_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51453 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26116 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30972 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_dense_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_dense_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_elasticnet_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_gbt_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_gbt_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46256 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_kernel_ridge_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38435 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_knn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_knn_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38628 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_lgbm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_lgbm_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39411 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_logistic_regression_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28002 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_pls_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38250 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_rf_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_rf_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38696 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_ridge_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_sgd_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_sgd_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38352 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_svm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_svr_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35388 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_xgboost_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_xgboost_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_outlier_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43413 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/tests/test_utils_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_num/num_project/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/default_model_upload_instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/generate_vision_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/nose_setup_coverage.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.741584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.741584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_cnn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20699 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_transfer_learning_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/model_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/model_keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.741584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59082 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_detectron_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_keras_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80849 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_object_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/utils_deep_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/utils_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.741584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/monitoring/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/monitoring/model_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.741584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/preprocessing/manage_white_borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/preprocessing/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26500 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/post-checkout
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-push
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    60469 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/robot.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/1_preprocess_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/2_training_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/2_training_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/3_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/4_demonstrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/utils/0_create_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/utils/0_reload_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/utils/0_split_train_valid_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.737584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.741584 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/answers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34014 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_vision.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/apple_36.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/apple.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Bombay_19.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_34.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/toto.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_4.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.745584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_3.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.749584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_34.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/toto.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.701584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.749584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_4.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.749584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/toto/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/toto/titi.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.749584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_3.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.749584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.749584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.749584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Bombay_19.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.753584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.753584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Bombay_19.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.753584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.753584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Bombay_19.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.753584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/preprocess_pipeline.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.753584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Bombay_19.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.757584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.757584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.757584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/preprocess_pipeline.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.705584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.757584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_4.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.757584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_3.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.757584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.757584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.761584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_36.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_4.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.761584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/
+-rw-r--r--   0 runner    (1001) docker     (123)   104013 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_10.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_19.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/preprocess_pipeline.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.761584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_15.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_30.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_31.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_34.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.761584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.761584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/metadata_bboxes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   270880 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/mixed_22.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fake_metrics.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.761584 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/
+-rw-r--r--   0 runner    (1001) docker     (123)    32016 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/apple_76.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/banana_76.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/metadata_bboxes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   270880 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/mixed_22.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    48870 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/orange_77.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13984 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23879 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_manage_white_borders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28641 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_cnn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89016 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_detectron_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57572 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98567 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_keras_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131251 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_transfer_learning_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21119 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils_faster_rcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22490 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55754 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 09:59:46.000000 gabarit-1.3.2/gabarit/template_vision/vision_project/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:59:51.705584 gabarit-1.3.2/gabarit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-06-12 09:59:51.000000 gabarit-1.3.2/gabarit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    44354 2023-06-12 09:59:51.000000 gabarit-1.3.2/gabarit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:59:51.000000 gabarit-1.3.2/gabarit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-12 09:59:51.000000 gabarit-1.3.2/gabarit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 09:59:51.000000 gabarit-1.3.2/gabarit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 09:59:51.000000 gabarit-1.3.2/gabarit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:59:51.761584 gabarit-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-12 09:59:46.000000 gabarit-1.3.2/setup.py
```

### Comparing `gabarit-1.3.1/LICENSE` & `gabarit-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/MANIFEST.in` & `gabarit-1.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/PKG-INFO` & `gabarit-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gabarit
-Version: 1.3.1
+Version: 1.3.2
 Summary: Kickstart your AI project as code
 Home-page: https://github.com/OSS-Pole-Emploi/gabarit
 Author: Agence Data Services PE Nantes
 Author-email: contactadsaiframeworks.00619@pole-emploi.fr
 License: AGPL-3.0
 Description: [![pypi badge](https://img.shields.io/pypi/v/gabarit.svg)](https://pypi.python.org/pypi/gabarit)
         ![NLP tests](https://github.com/OSS-Pole-Emploi/gabarit/actions/workflows/nlp_build_tests.yaml/badge.svg)
```

### Comparing `gabarit-1.3.1/README.md` & `gabarit-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/__init__.py` & `gabarit-1.3.2/gabarit/template_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/README.md` & `gabarit-1.3.2/gabarit/template_api/api_project/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 ├─ tests
 │   └─ ...
 .
 .
 .
 ├─ .env                         # environement variables for settings
 ├─ makefile
-├─ Dockerfile.svc
+├─ Dockerfile
 ├─ pyproject.toml               # your package dependencies and infos
 ├─ setup.py
 ├─ launch.sh                    # start your application
 └─ README.md
 ```
 
 
@@ -241,15 +241,15 @@
 
 You can use routes from {{package_name}}.routers.technical as examples of how to create
 requests and responses schemas thanks to pydantic or have a look at the
 [FastAPI documentation](https://fastapi.tiangolo.com/tutorial/response-model/).
 
 ### Dockerfile
 
-A minimal `Dockerfile.svc` is provided by the template. You should have a look a it, especially
+A minimal `Dockerfile` is provided by the template. You should have a look a it, especially
 if you have to download your model in your containers.
 
 <!--
 The "omit from toc" comments are here for the Markdown All in One VSCode extension :
 it permits to remove a title from the auto table of content
 
 See https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one
```

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/makefile` & `gabarit-1.3.2/gabarit/template_api/api_project/makefile`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,14 @@
 	./launch.sh
 
 ####################################################
 # Build docker image
 ####################################################
 
 build-d:
-	docker build -t {{package_name}}_api -f Dockerfile.svc .
+	docker build -t {{package_name}}_api -f Dockerfile .
 
 run-d:
 	docker container run --rm -p 5000:5000 {{package_name}}_api
 
 run-d-it:
 	docker container run --rm -p 5000:5000 -i -t {{package_name}}_api
```

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/__init__.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/application.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/application.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/__init__.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/config.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/config.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/logtools.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/logtools.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/core/resources.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/core/resources.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/model/__init__.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/model/model_base.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/model/model_base.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/model/model_gabarit.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/model/model_gabarit.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/__init__.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/functional.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/functional.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/__init__.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/functional.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/functional.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/technical.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/technical.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/schemas/utils.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/package_name/routers/technical.py` & `gabarit-1.3.2/gabarit/template_api/api_project/package_name/routers/technical.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/pyproject.toml` & `gabarit-1.3.2/gabarit/template_api/api_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/__init__.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/conftest.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 > More details about test_base_client and test_complete_client:
 >
 > By default a TestClient does not fire events so the startup and shutdown events are never fired
 > and the model is never loaded.
 > We can fire thoses events by using TestClient as a context manager so we use two TestClient in
 > our tests : a test_base_client that does not load the model and test_complete_client that does
 > load the model thanks to a context manager. It allows us to test the behavior of our application
-> when a model is not loaded (which should not happend).
+> when a model is not loaded (which should not happen).
 
 """
 
 import os
 import pytest
 from pathlib import Path
 from fastapi.testclient import TestClient
```

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/create_test_model.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/create_test_model.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/test_config.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/test_model.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/test_routers_functionnal.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/test_routers_functionnal.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/test_routers_technical.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/test_routers_technical.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/api_project/tests/test_schemas_utils.py` & `gabarit-1.3.2/gabarit/template_api/api_project/tests/test_schemas_utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_api/generate_api_project.py` & `gabarit-1.3.2/gabarit/template_api/generate_api_project.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/default_config.ini` & `gabarit-1.3.2/gabarit/template_nlp/default_config.ini`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/generate_nlp_project.py` & `gabarit-1.3.2/gabarit/template_nlp/generate_nlp_project.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/Makefile` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/Makefile`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/README.md` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/README.md`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/nose_setup_coverage.cfg` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/nose_setup_coverage.cfg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/__init__.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/__init__.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/__init__.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/accuracy.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/f1.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/f1.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/precision.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/precision.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/recall.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/hf_metrics/recall.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/model_aggregation.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/model_aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,92 +248,104 @@
             self.nb_fit = 1
 
         # Update attributes
         self.trained, self.list_classes, self.dict_classes = self._check_trained()
 
     @utils.data_agnostic_str_to_list
     @utils.trained_needed
-    def predict(self, x_test, return_proba: bool = False, **kwargs) -> np.ndarray:
+    def predict(self, x_test, return_proba: bool = False, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Prediction
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
             return_proba (bool): If the function should return the probabilities instead of the classes
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: array of shape = [n_samples]
         '''
         # We decide whether to rely on each model's probas or their predictions
         if return_proba:
-            return self.predict_proba(x_test)
+            return self.predict_proba(x_test, alternative_version=alternative_version)
         else:
             # Get what we want (probas or preds) and use the aggregation function
             if self.using_proba:
-                preds_or_probas = self._predict_probas_sub_models(x_test, **kwargs)
+                preds_or_probas = self._predict_probas_sub_models(x_test, alternative_version=alternative_version, **kwargs)
             else:
-                preds_or_probas = self._predict_sub_models(x_test, **kwargs)
+                preds_or_probas = self._predict_sub_models(x_test, alternative_version=alternative_version, **kwargs)
             return np.array([self.aggregation_function(array, list_classes=self.list_classes) for array in preds_or_probas])  # type: ignore
 
     @utils.data_agnostic_str_to_list
     @utils.trained_needed
-    def predict_proba(self, x_test, **kwargs) -> np.ndarray:
+    def predict_proba(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Predicts the probabilities on the test set
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: array of shape = [n_samples, n_classes]
         '''
-        probas_sub_models = self._predict_probas_sub_models(x_test, **kwargs)
+        probas_sub_models = self._predict_probas_sub_models(x_test, alternative_version=alternative_version, **kwargs)
         # The probas of all models are averaged
         return np.sum(probas_sub_models, axis=1) / probas_sub_models.shape[1]
 
     @utils.trained_needed
-    def _predict_probas_sub_models(self, x_test, **kwargs) -> np.ndarray:
+    def _predict_probas_sub_models(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Recover the probabilities of each model being aggregated
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: array of shape = [n_samples, nb_model, nb_classes]
         '''
-        array_probas = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=True) for sub_model in self.sub_models])
+        array_probas = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=True, alternative_version=alternative_version)
+                                 for sub_model in self.sub_models])
         array_probas = np.transpose(array_probas, (1, 0, 2))
         return array_probas
 
     @utils.trained_needed
-    def _predict_sub_models(self, x_test, **kwargs) -> np.ndarray:
+    def _predict_sub_models(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Recover the predictions of each model being aggregated
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: not multi_label : array of shape = [n_samples, nb_model]
                         multi_label : array of shape = [n_samples, nb_model, n_classes]
         '''
         if self.multi_label:
-            array_predict = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=False) for sub_model in self.sub_models])
+            array_predict = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=False, alternative_version=alternative_version)
+                                      for sub_model in self.sub_models])
             array_predict = np.transpose(array_predict, (1, 0, 2))
         else:
-            array_predict = np.array([sub_model['model'].predict(x_test) for sub_model in self.sub_models])
+            array_predict = np.array([sub_model['model'].predict(x_test, alternative_version=alternative_version) for sub_model in self.sub_models])
             array_predict = np.transpose(array_predict, (1, 0))
         return array_predict
 
-    def _predict_full_list_classes(self, model: Type[ModelClass], x_test, return_proba: bool = False) -> np.ndarray:
+    def _predict_full_list_classes(self, model: Type[ModelClass], x_test, return_proba: bool = False, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''For multi_label: adds missing columns in the prediction of model (class missing in their list_classes)
         Or, if return_proba, adds a proba of zero to the missing classes in their list_classes
 
         Args:
             model (ModelClass): Model to use
             x_test (?): Array-like or sparse matrix of shape = [n_samples, n_features]
             return_proba (bool): If the function should return the probabilities instead of the classes
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: The array with the missing columns added
         '''
         # Get predictions or probas
-        preds_or_probas = model.predict(x_test, return_proba=return_proba)
+        preds_or_probas = model.predict(x_test, return_proba=return_proba, alternative_version=alternative_version)
 
         # Manage each cases. Reorder predictions or probas according to aggregation model list_classes
         # Multi label, proba = True
         # Multi label, proba = False
         # Mono label, proba = True
         if model.multi_label or return_proba:
             df_all = pd.DataFrame(np.zeros((len(preds_or_probas), len(self.list_classes))), columns=self.list_classes)  # type: ignore
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/model_class.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/model_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             x_test (?): Array-like or sparse matrix, shape = [n_samples, n_features]
         Returns:
             (np.ndarray): Array, shape = [n_samples, n_classes]
         '''
         raise NotImplementedError("'predict_proba' needs to be overridden")
 
     @utils.trained_needed
-    def predict_with_proba(self, x_test) -> Tuple[np.ndarray, np.ndarray]:
+    def predict_with_proba(self, x_test, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         '''Predicts on the test set with probabilities
 
         Args:
             x_test (?): Array-like or sparse matrix, shape = [n_samples, n_features]
         Returns:
             predicted_class (np.ndarray): The predicted classes, shape = [n_samples, n_classes]
             predicted_proba (np.ndarray): The predicted probabilities for each class, shape = [n_samples, n_classes]
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/model_huggingface.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/model_huggingface.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.epochs = epochs
         self.validation_split = validation_split
         self.patience = patience
         self.transformer_name = transformer_name
         self.model_max_length = model_max_length
 
         # transformer_params has no use as of 14/12/2022
-        # we still leave it for compatibility with keras models and future usage
+        # we still leave it for compatibility with Keras models and future usage
         self.transformer_params = transformer_params
 
         # Trainer params
         if trainer_params is None:
             trainer_params = {
                 'output_dir': self.model_dir,
                 'learning_rate': 2e-5,
@@ -571,15 +571,15 @@
                         plt.plot(fit_history_dict[f'{dataset}_{metric}'])
                         legend += ['Train'] if dataset == 'train_metrics' else ['Validation']
                 plt.title(f"Model {title}")
                 plt.ylabel(title)
                 plt.xlabel('Epoch')
                 plt.legend(legend, loc='upper left')
                 # Save
-                filename == f"{filename}.jpeg"
+                filename = f"{filename}.jpeg"
                 plt.savefig(os.path.join(plots_path, filename))
 
                 # Close figures
                 plt.close('all')
 
     @no_type_check  # We do not check the type, because it is complicated with managing custom_objects_str
     def save(self, json_data: Union[dict, None] = None) -> None:
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/__init__.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_pipeline.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_gbt.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_gbt.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_lgbm.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_lgbm.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_sgdc.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_sgdc.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_svm.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_sklearn/model_tfidf_svm.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/__init__.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_cnn.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_cnn.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_attention.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_attention.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_gru.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_gru.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_structured_attention.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_embedding_lstm_structured_attention.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_keras.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         Kwargs:
             batch_size (int): Batch size
             epochs (int): Number of epochs
             validation_split (float): Percentage for the validation set split
                 Only used if no input validation set when fitting
             patience (int): Early stopping patience
             embedding_name (str) : The name of the embedding matrix to use
-            keras_params (dict): Parameters used by keras models.
+            keras_params (dict): Parameters used by Keras models.
                 e.g. learning_rate, nb_lstm_units, etc...
                 The purpose of this dictionary is for the user to use it as they wants in the _get_model function
                 This parameter was initially added in order to do an hyperparameters search
         '''
         # TODO: learning rate should be an attribute !
         # Init.
         super().__init__(**kwargs)
@@ -309,73 +309,80 @@
 
         # Set trained
         self.trained = True
         self.nb_fit += 1
 
     @utils.data_agnostic_str_to_list
     @utils.trained_needed
-    def predict(self, x_test, return_proba: bool = False, **kwargs) -> np.ndarray:
+    def predict(self, x_test, return_proba: bool = False, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Predictions on test set
 
         Args:
             x_test (?): Array-like or sparse matrix, shape = [n_samples]
         Kwargs:
             return_proba (bool): If the function should return the probabilities instead of the classes
+            alternative_version (bool): If an alternative predict version must be used. Should be faster with low nb of inputs.
         Returns:
             (np.ndarray): Array, shape = [n_samples, n_classes]
         '''
         # Cast in pd.Series
         x_test = pd.Series(x_test)
 
         # Predict
-        predicted_proba = self.predict_proba(x_test)
+        predicted_proba = self.predict_proba(x_test, alternative_version=alternative_version)
 
         # We return the probabilities if wanted
         if return_proba:
             return predicted_proba
 
         # Finally, we get the classes predictions
         return self.get_classes_from_proba(predicted_proba)
 
     @utils.data_agnostic_str_to_list
     @utils.trained_needed
-    def predict_proba(self, x_test, experimental_version: bool = False, **kwargs) -> np.ndarray:
+    def predict_proba(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Predicts probabilities on the test dataset
 
         Args:
             x_test (?): Array-like or sparse matrix, shape = [n_samples, n_features]
         Kwargs:
-            experimental_version (bool): If an experimental (but faster) version must be used
+            alternative_version (bool): If an alternative predict version must be used. Should be faster with low nb of inputs.
         Returns:
             (np.ndarray): Array, shape = [n_samples, n_classes]
         '''
         # Prepare input
         x_test = self._prepare_x_test(x_test)
         # Process
-        if experimental_version:
-            return self.experimental_predict_proba(x_test)
+        if alternative_version:
+            return self._alternative_predict_proba(x_test)
         else:
             return self.model.predict(x_test, batch_size=128, verbose=1)  # type: ignore
 
     @utils.trained_needed
-    def experimental_predict_proba(self, x_test, **kwargs) -> np.ndarray:
-        '''Predicts probabilities on the test dataset - Experimental function
-        Preprocessings must be done before (in predict_proba)
-        Here we only do the prediction and return the result
+    def _alternative_predict_proba(self, x_test, **kwargs) -> np.ndarray:
+        '''Predicts probabilities on the test dataset - Alternative version
+        Should be faster with low nb of inputs.
 
         Args:
             x_test (?): Array-like or sparse matrix, shape = [n_samples]
         Returns:
             (np.ndarray): Array, shape = [n_samples, n_classes]
         '''
-        @tf.function
-        def serve(x):
-            return self.model(x, training=False)
+        return self._serve(x_test).numpy()
 
-        return serve(x_test).numpy()
+    @tf.function
+    def _serve(self, x: np.ndarray):
+        '''Improves predict function using tf.function (cf. https://www.tensorflow.org/guide/function)
+
+        Args:
+            x (np.ndarray): input data
+        Returns:
+            tf.tensor: model's output
+        '''
+        return self.model(x, training=False)
 
     def _prepare_x_train(self, x_train) -> np.ndarray:
         '''Prepares the input data for the model
 
         Args:
             x_train (?): Array-like, shape = [n_samples, n_features]
         Returns:
@@ -572,15 +579,15 @@
                 plt.plot(fit_history.history[metric])
                 plt.plot(fit_history.history[f'val_{metric}'])
                 plt.title(f"Model {title}")
                 plt.ylabel(title)
                 plt.xlabel('Epoch')
                 plt.legend(['Train', 'Validation'], loc='upper left')
                 # Save
-                filename == f"{filename}.jpeg"
+                filename = f"{filename}.jpeg"
                 plt.savefig(os.path.join(plots_path, filename))
 
                 # Close figures
                 plt.close('all')
 
     def _save_model_png(self, model) -> None:
         '''Tries to save the structure of the model in png format
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_tfidf_dense.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/model_tfidf_dense.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/utils_deep_keras.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/models_tensorflow/utils_deep_keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-## Utils - tools-functions for deep_learning keras models
+## Utils - tools-functions for deep_learning Keras models
 # Copyright (C) <2018-2022>  <Agence Data Services, DSI Pôle Emploi>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
@@ -266,15 +266,15 @@
     return fn
 
 
 # ** EXPERIMENTAL **
 # ** EXPERIMENTAL **
 # ** EXPERIMENTAL **
 
-# From Gaëlle JOUIS Thesis
+# From Gaëlle JOUIS' PhD Thesis
 
 class AttentionAverage(Layer):
     def __init__(self, attention_hops, **kwargs) -> None:
         self.attention_hops = attention_hops
         self.applied_axis = 1
         super(AttentionAverage, self).__init__()
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/models_training/utils_models.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/models_training/utils_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -274,21 +274,24 @@
     # Load model
     model, model_conf = ModelClass.load_model(model_dir=model_dir, **kwargs)
 
     # Return model & its configs
     return model, model_conf
 
 
-def predict(content: Union[str, list], model, model_conf: dict, **kwargs) -> list:
+def predict(content: Union[str, list], model, model_conf: dict, alternative_version: bool = False, **kwargs) -> list:
     '''Gets predictions of a model on a content
 
     Args:
         content (Union[str, list]): New content to be predicted
         model (ModelClass): Model to use
         model_conf (dict): Model configurations
+    Kwargs:
+        alternative_version (bool): If an alternative version must be used. Should be faster with low nb of inputs.
+                                    Only available for Keras models.
     Returns:
         list: a list of strings (resp. tuples) in case of mono-label (resp. multi-labels) classification predictions
     '''
     if isinstance(content, str):
         content = [content]
         
     # Get preprocessor
@@ -298,27 +301,31 @@
         preprocess_str = 'no_preprocess'
     preprocessor = preprocess.get_preprocessor(preprocess_str)
 
     # Preprocess
     content = preprocessor(content)
 
     # Get prediction (some models need an iterable)
-    predictions = model.predict(content)
+    predictions = model.predict(content, alternative_version=alternative_version)
 
     # Return predictions with inverse transform when relevant
     return model.inverse_transform(predictions)
 
 
-def predict_with_proba(content: Union[str, list], model, model_conf: dict) -> Union[Tuple[List[str], List[float]], Tuple[List[tuple], List[tuple]]]:
+def predict_with_proba(content: Union[str, list], model, model_conf: dict, alternative_version: bool = False,
+                       **kwargs) -> Union[Tuple[List[str], List[float]], Tuple[List[tuple], List[tuple]]]:
     '''Gets predictions of a model on a content, with probabilities
 
     Args:
         content (Union[str, list]): New content to be predicted
         model (ModelClass): Model to use
         model_conf (dict): Model configurations
+    Kwargs:
+        alternative_version (bool): If an alternative version must be used. Should be faster with low nb of inputs.
+                                    Only available for Keras models.
     Returns:
         MONO-LABEL CLASSIFICATION:
             List[str]: predictions
             List[float]: probabilities
         MULTI-LABELS CLASSIFICATION:
             List[tuple]: predictions
             List[tuple]: probabilities
@@ -335,22 +342,21 @@
 
     # Preprocess
     content = preprocessor(content)
 
     # Get prediction (some models need an iterable)
     # predictions is a ndarray of shape (n_samples, n_classes)
     # probas is a ndarray of shape (n_samples, n_classes)
-    predictions, probas = model.predict_with_proba(content)
+    predictions, probas = model.predict_with_proba(content, alternative_version=alternative_version)
 
     # Rework format :
     if model.multi_label:
         model_labels = np.array(model.list_classes)
         all_preds = [tuple(np.compress(content_pred, model_labels)) for content_pred in predictions]
         all_probs = [tuple(np.compress(content_pred, content_prob)) for content_pred, content_prob in zip(predictions, probas)]
-
     else:
         all_preds = model.inverse_transform(predictions)
         all_probs = probas.max(axis=1)
 
     # Return prediction & proba
     return all_preds, all_probs
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/monitoring/__init__.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/monitoring/mlflow_logger.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/monitoring/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/monitoring/model_explainer.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/monitoring/model_explainer.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/preprocessing/__init__.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/preprocessing/preprocess.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name/utils.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name/utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/EDA.ipynb` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/EDA.ipynb`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/ds.jpg` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/ds.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel.jpg` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel2.jpg` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/kernel2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/negative.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/negative.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/positive.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-exploration/EDA/images/positive.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/post-checkout` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/post-checkout`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-commit` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-commit`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-push` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/git_hooks/pre-push`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-ressources/nlp.jpg` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-ressources/nlp.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/1_preprocess_data.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/1_preprocess_data.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/2_training.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/2_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         x_col (str | int): Name of the model's input column - x
         y_col (list<str|int>): Name of the model's target column(s) - y
     Kwargs:
         min_rows (int): Minimal number of occurrences for a class to be considered by the model
             Corresponding entries are removed from both training & validation dataset - mono-label only
         filename_valid (str): Name of the validation dataset (actually a path relative to {{package_name}}-data)
             If None, we do not use a validation dataset.
-                -> for keras models (i.e. Neural Networks), we'll use a portion of the training dataset as the validation.
+                -> for Keras models (i.e. Neural Networks), we'll use a portion of the training dataset as the validation.
         level_save (str): Save level
             LOW: statistics + configurations + logger keras - /!\\ the model won't be reusable /!\\ -
             MEDIUM: LOW + hdf5 + pkl + plots
             HIGH: MEDIUM + predictions
         sep (str): Separator to use with the .csv files
         encoding (str): Encoding to use with the .csv files
         model (ModelClass): A model to be fitted. This should only be used for testing purposes.
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/3_predict.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/3_predict.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/4_demonstrator.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/4_demonstrator.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_create_samples.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_create_samples.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_get_embedding_dict.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_get_embedding_dict.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_merge_files.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_merge_files.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_reload_model.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_reload_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     This is done be reusing 'standalone' files.
 
     Args:
         model_dir (str): Name of the model to reload (not a path, just the directory name)
     Kwargs:
         config_file (str): Name of the configuration file
         sklearn_pipeline_file (str): Standalone sklearn pipeline file name (pipeline models)
-        weights_file (str): Neural Network weights file name (keras models)
+        weights_file (str): Neural Network weights file name (Keras models)
         tokenizer_file (str): Tokenizer file name (models with embeddings)
         tfidf_file (str): TFIDF file name (models with tfidf)
         hf_model_dir (str): HuggingFace model folder
         hf_tokenizer_dir (str): HuggingFace tokenizer folder
         aggregation_function_path (str): aggregation_function file name (model aggregation)
     Raises:
         FileNotFoundError: If model can't be found
@@ -167,15 +167,15 @@
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     # model_X should be the model's directory name: e.g. model_tfidf_svm_2019_12_05-12_57_18
     parser.add_argument('-m', '--model_dir', required=True, help="Name of the model to reload (not a path, just the directory name)")
     parser.add_argument('-c', '--config_file', default='configurations.json', help="Name of the configuration file")
     parser.add_argument('--sklearn_pipeline_file', default='sklearn_pipeline_standalone.pkl', help="Standalone sklearn pipeline file name (pipeline models)")
-    parser.add_argument('-w', '--weights_file', default='best.hdf5', help="Neural Network weights file name (keras models)")
+    parser.add_argument('-w', '--weights_file', default='best.hdf5', help="Neural Network weights file name (Keras models)")
     parser.add_argument('--tokenizer_file', default='embedding_tokenizer.pkl', help="Tokenizer file name (models with embeddings)")
     parser.add_argument('--tfidf_file', default='tfidf_standalone.pkl', help="TFIDF file name (models with tfidf)")
     parser.add_argument('--hf_model_dir', default='hf_model', help="HuggingFace model folder name")
     parser.add_argument('--hf_tokenizer_dir', default='hf_tokenizer', help="HuggingFace tokenizer folder name")
     parser.add_argument('--aggregation_function_file', default='aggregation_function.pkl', help="aggregation_function_file file name (models aggregation)")
     args = parser.parse_args()
     main(model_dir=args.model_dir, config_file=args.config_file, weights_file=args.weights_file,
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_split_train_valid_test.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_split_train_valid_test.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_sweetviz_report.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-scripts/utils/0_sweetviz_report.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/Tutorial_fr.ipynb` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/Tutorial_fr.ipynb`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_1.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_2.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/images/jules_verne_2.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/model_author.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/model_author.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/utils_tutorial_fr.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/fr/jules_verne/utils_tutorial_fr.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/Tutorial.ipynb` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/demonstrator.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/demonstrator.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/lstm_choice.jpg` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/lstm_choice.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1_path.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model1_path.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model2.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/model2.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/predictions.png` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/images/predictions.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/package_name-tutorials/main/utils_main_tutorial.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/package_name-tutorials/main/utils_main_tutorial.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/requirements.txt` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/requirements.txt`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/setup.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/setup.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_dataset.csv` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_dataset.csv`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_dataset2.csv` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_dataset2.csv`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_mlflow_logger.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_aggregation.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_aggregation.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         else:
             return np.array([self.dict_predictions[x] for x in x_test])
 
     def predict_proba(self, x_test, **kwargs):
         return np.array([self.dict_predictions_proba[x] for x in x_test])
 
 # Predictions for the mock mono_label models
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 dict_predictions_1 = {"ceci est un test": '0', "pas cela": '0', "cela non plus": '1', "ici test": '0', "là, rien!": '1'}
 dict_predictions_2 = {"ceci est un test": '1', "pas cela": '1', "cela non plus": '0', "ici test": '0', "là, rien!": '1'}
 dict_predictions_3 = {"ceci est un test": '1', "pas cela": '1', "cela non plus": '2', "ici test": '1', "là, rien!": '4'}
 dict_predictions_4 = {"ceci est un test": '2', "pas cela": '2', "cela non plus": '3', "ici test": '3', "là, rien!": '1'}
 dict_predictions_5 = {"ceci est un test": '3', "pas cela": '2', "cela non plus": '4', "ici test": '3', "là, rien!": '1'}
 list_dict_predictions = [dict_predictions_1, dict_predictions_2, dict_predictions_3, dict_predictions_4, dict_predictions_5]
 
@@ -89,14 +90,15 @@
                             "cela non plus": np.array([0.3, 0.25, 0.45]), "ici test": np.array([0.4, 0.1, 0.5]), "là, rien!": np.array([0.25, 0.4, 0.35])}
 dict_predictions_proba_5 = {"ceci est un test": np.array([0.1, 0.3, 0.5, 0.1]), "pas cela": np.array([0.1, 0.5, 0.3, 0.1]),
                             "cela non plus": np.array([0.1, 0.3, 0.1, 0.5]), "ici test": np.array([0.1, 0.3, 0.5, 0.1]), "là, rien!": np.array([0.5, 0.3, 0.1, 0.1])}
 
 x_test = np.array(["ceci est un test", "pas cela", "cela non plus", "ici test", "là, rien!"])
 
 # Definition of the targets for the mono_label cases
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 target_predict_mono_majority_vote_dict = {"ceci est un test":'1', "pas cela":'1', "cela non plus":'1', "ici test":'0', "là, rien!":'1'}
 target_get_predictions_mono = np.array([[list_dict_predictions[i][key] for i in range(len(list_dict_predictions))] for key in x_test])
 target_get_proba_mono = np.array([[[0.7, 0.3, 0.0, 0.0, 0.0],
   [0.3, 0.7, 0.0, 0.0, 0.0],
   [0.0, 0.4, 0.25, 0.0, 0.35],
   [0.0, 0.1, 0.5, 0.4, 0.0],
   [0.0, 0.1, 0.3, 0.5, 0.1]],
@@ -153,22 +155,24 @@
                                                 "ici test": [1, 1, 0, 1, 0], "là, rien!": [0, 1, 0, 0, 1]}
 target_predict_mono_vote_labels_dict = {"ceci est un test": [0, 0, 0, 0, 0], "pas cela": [0, 0, 0, 0, 0,], "cela non plus": [0, 0, 0, 0, 0],
                                                 "ici test": [0, 0, 0, 0, 0], "là, rien!": [0, 1, 0, 0, 0]}
 target_predict_mono_all_predictions = np.array([target_predict_mono_all_predictions_dict[x] for x in x_test])
 target_predict_mono_vote_labels = np.array([target_predict_mono_vote_labels_dict[x] for x in x_test])
 
 # Instanciation of the mock mono_label models
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 mock_model_mono_1 = MockModel(dict_predictions_1, dict_predictions_proba_1, 'model_mono_1', False, ['0', '1'])
 mock_model_mono_2 = MockModel(dict_predictions_2, dict_predictions_proba_2, 'model_mono_2', False, ['1', '0'])
 mock_model_mono_3 = MockModel(dict_predictions_3, dict_predictions_proba_3, 'model_mono_3', False, ['1', '2', '4'])
 mock_model_mono_4 = MockModel(dict_predictions_4, dict_predictions_proba_4, 'model_mono_4', False, ['2', '1', '3'])
 mock_model_mono_5 = MockModel(dict_predictions_5, dict_predictions_proba_5, 'model_mono_5', False, ['1', '2', '3', '4'])
 list_models_mono = [mock_model_mono_1, mock_model_mono_2, mock_model_mono_3, mock_model_mono_4, mock_model_mono_5]
 
 # Instanciation of the mock multi_label models
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 mock_model_multi_1 = MockModel(dict_predictions_multi_1, dict_predictions_proba_1, 'model_multi_1', True, ['0', '1'])
 mock_model_multi_2 = MockModel(dict_predictions_multi_2, dict_predictions_proba_2, 'model_multi_2', True, ['1', '0'])
 mock_model_multi_3 = MockModel(dict_predictions_multi_3, dict_predictions_proba_3, 'model_multi_3', True, ['1', '2', '4'])
 mock_model_multi_4 = MockModel(dict_predictions_multi_4, dict_predictions_proba_4, 'model_multi_4', True, ['2', '1', '3'])
 list_models_multi = [mock_model_multi_1, mock_model_multi_2, mock_model_multi_3, mock_model_multi_4]
 
 # Definitions for a mixture of mono/multi-labels models
@@ -632,14 +636,19 @@
             possible_classes = {vote[0] for vote in votes if vote[1]==votes[0][1]}
             return [prediction for prediction in predictions if prediction in possible_classes][0]
 
         # Function including all the checks we have to perform
         def test_predict(model, x_test, target_predict, target_probas):
             preds = model.predict(x_test)
             probas = model.predict(x_test, return_proba=True)
+            preds_alt = model.predict(x_test, alternative_version=True)
+            probas_alt = model.predict(x_test, return_proba=True, alternative_version=True)
+            # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+            # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+            np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
             self.assertEqual(preds.shape, target_predict.shape)
             self.assertEqual(probas.shape, target_probas.shape)
             # Check the predictions
             if model.multi_label:
                 for truth, pred in zip(target_predict, preds):
                     for value_true, value_pred in zip(truth, pred):
                         self.assertEqual(value_true, value_pred)
@@ -691,79 +700,95 @@
         '''Test of {{package_name}}.models_training.model_aggregation.ModelAggregation._predict_probas_sub_models'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         model = ModelAggregation(model_dir=model_dir, list_models=list_models_mono)
         probas = model._predict_probas_sub_models(x_test)
+        probas_alt = model._predict_probas_sub_models(x_test, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertTrue(isinstance(probas, np.ndarray))
         self.assertEqual(target_get_proba_mono.shape, probas.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_get_proba_mono[i], probas[i]):
                 for truth_value, pred_value in zip(truth, pred):
                     self.assertAlmostEqual(truth_value, pred_value)
         remove_dir_model(model, model_dir)
 
         # Model needs to be fitted
         model = ModelAggregation(model_dir=model_dir)
         with self.assertRaises(AttributeError):
             model._predict_probas_sub_models('test')
+        with self.assertRaises(AttributeError):
+            model._predict_probas_sub_models('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test08_model_aggregation_predict_sub_models(self):
         '''Test of {{package_name}}.models_training.model_aggregation.ModelAggregation._predict_sub_models'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # mono_label
         model = ModelAggregation(model_dir=model_dir, list_models=list_models_mono)
         preds = model._predict_sub_models(x_test)
+        preds_alt = model._predict_sub_models(x_test, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertTrue(isinstance(preds, np.ndarray))
         self.assertEqual(target_get_predictions_mono.shape, preds.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_get_predictions_mono[i], preds[i]):
                 self.assertEqual(truth, pred)
         remove_dir_model(model, model_dir)
 
         # multi_label
         model = ModelAggregation(model_dir=model_dir, list_models=list_models_multi, aggregation_function='all_predictions', multi_label=True)
         preds = model._predict_sub_models(x_test)
+        preds_alt = model._predict_sub_models(x_test, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertTrue(isinstance(preds, np.ndarray))
         self.assertEqual(target_get_predictions_multi.shape, preds.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_get_predictions_multi[i], preds[i]):
                 for truth_value, pred_value in zip(truth, pred):
                     self.assertEqual(truth_value, pred_value)
         remove_dir_model(model, model_dir)
 
         # Model needs to be fitted
         model = ModelAggregation(model_dir=model_dir)
         with self.assertRaises(AttributeError):
             model._predict_sub_models('test')
+        with self.assertRaises(AttributeError):
+            model._predict_sub_models('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test09_model_aggregation_predict_proba(self):
         '''Test of {{package_name}}.models_training.model_aggregation.ModelAggregation.predict_proba'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         model = ModelAggregation(model_dir=model_dir, list_models=list_models_mono)
         probas = model.predict_proba(x_test)
+        probas_alt = model.predict_proba(x_test, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(target_predict_mono_proba.shape, probas.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_predict_mono_proba[i], probas[i]):
                 self.assertAlmostEqual(truth, pred)
         remove_dir_model(model, model_dir)
 
         # Model needs to be fitted
         model = ModelAggregation(model_dir=model_dir)
         with self.assertRaises(AttributeError):
             model.predict_proba('test')
+        with self.assertRaises(AttributeError):
+            model.predict_proba('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test10_model_aggregation_predict_full_list_classes(self):
         '''Test of {{package_name}}.models_training.model_aggregation.ModelAggregation._predict_full_list_classes'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
@@ -779,21 +804,27 @@
                                     {'test_1':np.array([0.2, 0.8, 0.0]), 'test_2':np.array([0.9, 0.0, 0.1]), 'test_3':np.array([0.2, 0.1, 0.7])},
                                     'model_mono',
                                     False,
                                     ['1', '2', '4'])
 
         # mono_label, no return_proba
         preds = model._predict_full_list_classes(mock_model_mono, np.array(['test_1', 'test_2', 'test_3']), return_proba=False)
+        preds_alt = model._predict_full_list_classes(mock_model_mono, np.array(['test_1', 'test_2', 'test_3']), return_proba=False, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_mono = np.array(['2', '1', '4'])
         self.assertEqual(target_mono.shape, preds.shape)
         for truth, pred in zip(target_mono, preds):
             self.assertEqual(truth, pred)
 
         # mono_label, return_proba
         preds = model._predict_full_list_classes(mock_model_mono, np.array(['test_1', 'test_2', 'test_3']), return_proba=True)
+        preds_alt = model._predict_full_list_classes(mock_model_mono, np.array(['test_1', 'test_2', 'test_3']), return_proba=True, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_mono_return_proba = np.array([[0.0, 0.2, 0.8, 0.0, 0.0, 0.0], [0.0, 0.9, 0.0, 0.0, 0.1, 0.0], [0.0, 0.2, 0.1, 0.0, 0.7, 0.0]])
         self.assertEqual(target_mono_return_proba.shape, preds.shape)
         for truth, pred in zip(target_mono_return_proba, preds):
             for truth_value, pred_value in zip(truth, pred):
                 self.assertAlmostEqual(truth_value, pred_value)
 
         remove_dir(model_dir)
@@ -810,22 +841,28 @@
                                     {'test_1':np.array([0.2, 0.8, 0.0]), 'test_2':np.array([0.9, 0.0, 0.1]), 'test_3':np.array([0.2, 0.1, 0.7])},
                                     'model_mono',
                                     True,
                                     ['1', '2', '4'])
 
         # multi_label, no return_proba
         preds = model._predict_full_list_classes(mock_model_multi, np.array(['test_1', 'test_2', 'test_3']), return_proba=False)
+        preds_alt = model._predict_full_list_classes(mock_model_multi, np.array(['test_1', 'test_2', 'test_3']), return_proba=False, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_multi = np.array([[0, 1, 1, 0, 0, 0], [0, 1, 0, 0, 1, 0], [0, 0, 0, 0, 0, 0]])
         self.assertEqual(target_multi.shape, preds.shape)
         for truth, pred in zip(target_multi, preds):
             for truth_value, pred_value in zip(truth, pred):
                 self.assertEqual(truth_value, pred_value)
 
         # multi_label, return_proba
         preds = model._predict_full_list_classes(mock_model_multi, np.array(['test_1', 'test_2', 'test_3']), return_proba=True)
+        preds_alt = model._predict_full_list_classes(mock_model_multi, np.array(['test_1', 'test_2', 'test_3']), return_proba=True, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_mono_return_proba = np.array([[0.0, 0.2, 0.8, 0.0, 0.0, 0.0], [0.0, 0.9, 0.0, 0.0, 0.1, 0.0], [0.0, 0.2, 0.1, 0.0, 0.7, 0.0]])
         self.assertEqual(target_mono_return_proba.shape, preds.shape)
         for truth, pred in zip(target_mono_return_proba, preds):
             for truth_value, pred_value in zip(truth, pred):
                 self.assertAlmostEqual(truth_value, pred_value)
 
         remove_dir(model_dir)
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_class.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_class.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_cnn.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,53 +164,57 @@
         # Mono-label
         model = ModelEmbeddingCnn(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                   max_sequence_length=10, max_words=100,
                                   padding='pre', truncating='post',
                                   embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), 3))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingCnn(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                   max_sequence_length=10, max_words=100,
                                   padding='pre', truncating='post',
                                   embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), 3))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Multi-labels
         model = ModelEmbeddingCnn(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                   max_sequence_length=10, max_words=100,
                                   padding='pre', truncating='post',
                                   embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingCnn(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                   max_sequence_length=10, max_words=100,
                                   padding='pre', truncating='post',
                                   embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelEmbeddingCnn(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                       max_sequence_length=10, max_words=100,
                                       padding='pre', truncating='post',
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,53 +163,57 @@
         # Mono-label
         model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                    max_sequence_length=10, max_words=100,
                                    padding='pre', truncating='post',
                                    embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), 3))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                    max_sequence_length=10, max_words=100,
                                    padding='pre', truncating='post',
                                    embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), 3))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Multi-labels
         model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                    max_sequence_length=10, max_words=100,
                                    padding='pre', truncating='post',
                                    embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                    max_sequence_length=10, max_words=100,
                                    padding='pre', truncating='post',
                                    embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                        max_sequence_length=10, max_words=100,
                                        padding='pre', truncating='post',
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_attention.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,53 +162,57 @@
         # Mono-label
         model = ModelEmbeddingLstmAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                             max_sequence_length=10, max_words=100,
                                             padding='pre', truncating='post',
                                             embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), 3))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstmAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                             max_sequence_length=10, max_words=100,
                                             padding='pre', truncating='post',
                                             embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), 3))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Multi-labels
         model = ModelEmbeddingLstmAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                             max_sequence_length=10, max_words=100,
                                             padding='pre', truncating='post',
                                             embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstmAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                             max_sequence_length=10, max_words=100,
                                             padding='pre', truncating='post',
                                             embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelEmbeddingLstmAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                                 max_sequence_length=10, max_words=100,
                                                 padding='pre', truncating='post',
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_gru.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_gru.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,53 +163,57 @@
         # Mono-label
         model = ModelEmbeddingLstmGru(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                          max_sequence_length=10, max_words=100,
                                          padding='pre', truncating='post',
                                          embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), 3))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstmGru(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                          max_sequence_length=10, max_words=100,
                                          padding='pre', truncating='post',
                                          embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), 3))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Multi-labels
         model = ModelEmbeddingLstmGru(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                          max_sequence_length=10, max_words=100,
                                          padding='pre', truncating='post',
                                          embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstmGru(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                          max_sequence_length=10, max_words=100,
                                          padding='pre', truncating='post',
                                          embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelEmbeddingLstmGru(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                              max_sequence_length=10, max_words=100,
                                              padding='pre', truncating='post',
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_structured_attention.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_embedding_lstm_structured_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,53 +176,57 @@
         # Mono-label
         model = ModelEmbeddingLstmStructuredAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                                       max_sequence_length=10, max_words=100,
                                                       padding='pre', truncating='post',
                                                       embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), 3))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstmStructuredAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                                       max_sequence_length=10, max_words=100,
                                                       padding='pre', truncating='post',
                                                       embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), 3))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Multi-labels
         model = ModelEmbeddingLstmStructuredAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                                       max_sequence_length=10, max_words=100,
                                                       padding='pre', truncating='post',
                                                       embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelEmbeddingLstmStructuredAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                                       max_sequence_length=10, max_words=100,
                                                       padding='pre', truncating='post',
                                                       embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi[cols])
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelEmbeddingLstmStructuredAttention(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                                           max_sequence_length=10, max_words=100,
                                                           padding='pre', truncating='post',
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_explainer.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_explainer.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_huggingface.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -663,15 +663,36 @@
         f1_1 =  2 * precision_1 * recall_1 / (precision_1 + recall_1)
         f1 = (f1_0 * weight_0) + (f1_1 * weight_1)  # weighted f1
         self.assertAlmostEqual(metrics['weighted_f1'], f1)
 
         # Clean
         remove_dir(model_dir)
 
-    def test13_model_huggingface_save(self):
+    def test13_model_plot_metrics_and_loss(self):
+        '''Test of the method _plot_metrics_and_loss of {{package_name}}.models_training.model_huggingface.ModelHuggingFace'''
+        model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
+        remove_dir(model_dir)
+
+        # Nominal case
+        model = ModelHuggingFace(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
+
+        list_metrics = ['loss', 'accuracy', 'weighted_f1', 'weighted_precision', 'weighted_recall']
+        fit_history_train = [{f'train_metrics_{metric}':[0.1, 0.2, 0.3, 0.5, 0.4]} for metric in list_metrics]
+        fit_history_val = [{f'eval_{metric}':[0.05, 0.1, 0.2, 0.4, 0.4]} for metric in list_metrics]
+        fit_history = fit_history_train+fit_history_val
+
+        model._plot_metrics_and_loss(fit_history)
+        plots_path = os.path.join(model.model_dir, 'plots')
+        for filename in ['accuracy', 'loss', 'weighted_f1_score', 'weighted_precision', 'weighted_recall']:
+            self.assertTrue(os.path.exists(os.path.join(plots_path, f"{filename}.jpeg")))
+
+        # Clean
+        remove_dir(model_dir)
+
+    def test14_model_huggingface_save(self):
         '''Test of the method save of {{package_name}}.models_training.model_huggingface.ModelHuggingFace'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Nominal case
         model = ModelHuggingFace(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
@@ -705,15 +726,15 @@
         self.assertTrue('trainer_params' in configs.keys())
         self.assertTrue('_get_model' in configs.keys())
         self.assertTrue('_get_tokenizer' in configs.keys())
 
         # Clean
         remove_dir(model_dir)
 
-    def test14_model_huggingface_init_new_instance_from_configs(self):
+    def test15_model_huggingface_init_new_instance_from_configs(self):
         '''Test of the method _init_new_instance_from_configs of {{package_name}}.models_training.models_tensorflow.model_huggingface.ModelHuggingFace'''
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Nominal case
         model = ModelHuggingFace(model_dir=model_dir)
         model.save(json_data={'test': 8})
@@ -776,15 +797,15 @@
         self.assertEqual(set(model.transformer_params), set(new_model.transformer_params))
         self.assertEqual(model.transformer_params['evaluation_strategy'], new_model.transformer_params['evaluation_strategy'])
         self.assertAlmostEqual(model.transformer_params['weight_decay'], new_model.transformer_params['weight_decay'])
         self.assertEqual(model.transformer_params['load_best_model_at_end'], new_model.transformer_params['load_best_model_at_end'])
         remove_dir(model_dir)
         remove_dir(new_model.model_dir)
 
-    def test15_model_huggingface_load_standalone_files(self):
+    def test16_model_huggingface_load_standalone_files(self):
         '''Test of the method _load_standalone_files of {{package_name}}.models_training.models_tensorflow.model_huggingface.ModelHuggingFace'''
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Nominal case with default_model_dir
         model = ModelHuggingFace(model_dir=model_dir, epochs=2)
         x_train = ['coucou', 'coucou_2', 'coucou_3']
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_keras.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,47 +448,73 @@
         cols = ['test1', 'test2', 'test3']
 
         # Mono-label
         model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                    max_sequence_length=10, max_words=100,
                                    embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_mono)
+        #
         preds = model.predict(x_train, return_proba=False)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train),))
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
         preds = model.predict('test', return_proba=False)
+        preds_alt = model.predict('test', return_proba=False, alternative_version=True)
         self.assertEqual(preds, model.predict(['test'], return_proba=False)[0])
-        proba = model.predict(x_train, return_proba=True)
-        self.assertEqual(proba.shape, (len(x_train), 3))
-        proba = model.predict('test', return_proba=True)
-        self.assertEqual([elem for elem in proba], [elem for elem in model.predict(['test'], return_proba=True)[0]])
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
+        probas = model.predict(x_train, return_proba=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
+        self.assertEqual(probas.shape, (len(x_train), 3))
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
+        #
+        probas = model.predict('test', return_proba=True)
+        probas_alt = model.predict('test', return_proba=True, alternative_version=True)
+        self.assertEqual([elem for elem in probas], [elem for elem in model.predict(['test'], return_proba=True)[0]])
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         remove_dir(model_dir)
 
         # Multi-labels
         model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True,
                                    max_sequence_length=10, max_words=100,
                                    embedding_name='fake_embedding.pkl')
         model.fit(x_train, y_train_multi)
+        #
         preds = model.predict(x_train, return_proba=False)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
         preds = model.predict('test', return_proba=False)
+        preds_alt = model.predict('test', return_proba=False, alternative_version=True)
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict(['test'], return_proba=False)[0]])
-        proba = model.predict(x_train, return_proba=True)
-        self.assertEqual(proba.shape, (len(x_train), len(cols)))
-        proba = model.predict('test', return_proba=True)
-        self.assertEqual([elem for elem in proba], [elem for elem in model.predict(['test'], return_proba=True)[0]])
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
+        probas = model.predict(x_train, return_proba=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
+        self.assertEqual(probas.shape, (len(x_train), len(cols)))
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
+        #
+        probas = model.predict('test', return_proba=True)
+        probas_alt = model.predict('test', return_proba=True, alternative_version=True)
+        self.assertEqual([elem for elem in probas], [elem for elem in model.predict(['test'], return_proba=True)[0]])
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelEmbeddingLstm(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False,
                                        max_sequence_length=10, max_words=100,
                                        embedding_name='fake_embedding.pkl')
             model.predict('test')
         remove_dir(model_dir)
 
+    # TODO: add test predict_proba
+
     def test04_model_keras_get_embedding_matrix(self):
         '''Test of the method _get_embedding_matrix of {{package_name}}.models_training.models_tensorflow.model_keras.ModelKeras'''
 
         # Create model
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
         model = ModelKeras(model_dir=model_dir, embedding_name='fake_embedding.pkl')
@@ -611,15 +637,41 @@
         # Nominal case
         model = ModelKeras(model_dir=model_dir, embedding_name='fake_embedding.pkl')
         self.assertEqual(model._get_learning_rate_scheduler(), None)
 
         # Clean
         remove_dir(model_dir)
 
-    def test08_model_keras_save(self):
+    def test08_model_keras_plot_metrics_and_loss(self):
+        '''Test of the method _plot_metrics_and_loss of {{package_name}}.models_training.models_tensorflow.model_keras.ModelKeras'''
+
+        model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
+        remove_dir(model_dir)
+
+        # Nominal case
+        model = ModelKeras(model_dir=model_dir, embedding_name='fake_embedding.pkl')
+
+        class FitHistory(object):
+
+            def __init__(self):
+                self.history = {}
+                for metric in ['acc', 'loss', 'categorical_accuracy', 'f1', 'precision', 'recall']:
+                    self.history[metric] = [0.1, 0.2, 0.3, 0.5, 0.4]
+                    self.history[f'val_{metric}'] = [0.05, 0.1, 0.2, 0.4, 0.4]
+
+        fit_history = FitHistory()
+        model._plot_metrics_and_loss(fit_history)
+        plots_path = os.path.join(model.model_dir, 'plots')
+        for filename in ['accuracy', 'loss', 'categorical_accuracy', 'f1_score', 'precision', 'recall']:
+            self.assertTrue(os.path.exists(os.path.join(plots_path, f"{filename}.jpeg")))
+
+        # Clean
+        remove_dir(model_dir)
+
+    def test09_model_keras_save(self):
         '''Test of the method save of {{package_name}}.models_training.models_tensorflow.model_keras.ModelKeras'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Nominal case
         model = ModelKeras(model_dir=model_dir, embedding_name='fake_embedding.pkl')
@@ -689,15 +741,15 @@
         self.assertTrue('_get_model' in configs.keys())
         self.assertTrue('_get_learning_rate_scheduler' in configs.keys())
         self.assertTrue('custom_objects' in configs.keys())
 
         # Clean
         remove_dir(model_dir)
 
-    def test09_model_keras_hook_post_load_model_pkl(self):
+    def test10_model_keras_hook_post_load_model_pkl(self):
         '''Test of the method _hook_post_load_model_pkl of {{package_name}}.models_training.models_tensorflow.model_keras.ModelKeras'''
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
         new_model_dir = os.path.join(os.getcwd(), 'model_test_987654321')
         remove_dir(new_model_dir)
 
         old_hdf5_path = os.path.join(model_dir, 'best.hdf5')
@@ -723,15 +775,15 @@
         self.assertTrue(new_model.model is None)
         with self.assertRaises(FileNotFoundError):
             new_model._hook_post_load_model_pkl()
 
         remove_dir(new_model_dir)
         remove_dir(model_dir)
 
-    def test10_model_keras_init_new_instance_from_configs(self):
+    def test11_model_keras_init_new_instance_from_configs(self):
         '''Test of the method _init_new_instance_from_configs of {{package_name}}.models_training.models_tensorflow.model_keras.ModelKeras'''
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
 
         # Nominal case
         model = ModelKeras(model_dir=model_dir)
@@ -781,15 +833,15 @@
         self.assertEqual(set(model.keras_params), set(new_model.keras_params))
         self.assertEqual(model.keras_params['coucou'], new_model.keras_params['coucou'])
         self.assertAlmostEqual(model.keras_params['coucou2'], new_model.keras_params['coucou2'])
         self.assertEqual(model.keras_params['coucou3'], new_model.keras_params['coucou3'])
         remove_dir(model_dir)
         remove_dir(new_model.model_dir)
     
-    def test11_model_keras_load_standalone_files(self):
+    def test12_model_keras_load_standalone_files(self):
         '''Test of the method _load_standalone_files of {{package_name}}.models_training.models_tensorflow.model_keras.ModelKeras'''
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
         new_model_dir = os.path.join(os.getcwd(), 'model_test_987654321')
         remove_dir(new_model_dir)
 
         old_hdf5_path = os.path.join(model_dir, 'best.hdf5')
@@ -844,15 +896,15 @@
             new_model._load_standalone_files()
         with self.assertRaises(FileNotFoundError):
             new_model._load_standalone_files(hdf5_path=old_hdf5_path)
 
         remove_dir(model_dir)
         remove_dir(new_model.model_dir)
 
-    def test12_model_keras_reload_weights(self):
+    def test13_model_keras_reload_weights(self):
         '''Test of the method _reload_weights of {{package_name}}.models_training.models_tensorflow.model_keras.ModelKeras'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
         new_model_dir = os.path.join(os.getcwd(), 'model_test_987654321')
         remove_dir(new_model_dir)
         old_hdf5_path = os.path.join(model_dir, 'best.hdf5')
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_pipeline.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_pipeline.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_dense.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,44 +96,48 @@
         y_test_multi = y_train_multi.copy()
         cols = ['test1', 'test2', 'test3']
 
         # Mono-label
         model = ModelTfidfDense(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono)
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), 3))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelTfidfDense(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono)
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), 3))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Multi-labels
         model = ModelTfidfDense(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True)
         model.fit(x_train, y_train_multi[cols])
         preds = model.predict_proba(x_train)
+        preds_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
         preds = model.predict_proba('test')
         self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'])[0]])
         remove_dir(model_dir)
 
         #
         model = ModelTfidfDense(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True)
         model.fit(x_train, y_train_multi[cols])
-        preds = model.predict_proba(x_train, experimental_version=True)
+        preds = model.predict_proba(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(cols)))
-        preds = model.predict_proba('test', experimental_version=True)
-        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], experimental_version=True)[0]])
+        preds = model.predict_proba('test', alternative_version=True)
+        self.assertEqual([elem for elem in preds], [elem for elem in model.predict_proba(['test'], alternative_version=True)[0]])
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelTfidfDense(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
             model.predict_proba('test')
         remove_dir(model_dir)
```

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_gbt.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_gbt.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_lgbm.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_lgbm.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_sgdc.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_sgdc.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_svm.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_model_tfidf_svm.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_preprocess.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_utils.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_nlp/nlp_project/tests/test_utils_models.py` & `gabarit-1.3.2/gabarit/template_nlp/nlp_project/tests/test_utils_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -313,27 +313,32 @@
         model_name = 'test_model3_name'
         model = model_tfidf_svm.ModelTfidfSvm(model_dir=model_dir, model_name=model_name)
         model.fit(x_train, y_train_mono)
         model.save()
         model, model_conf = utils_models.load_model('test_model3')
         self.assertEqual(utils_models.predict('Ceci est un test', model, model_conf), ['test'])
         self.assertEqual(utils_models.predict('Test "deux" !', model, model_conf), ['deux'])
+        self.assertEqual(utils_models.predict('Ceci est un test', model, model_conf, alternative_version=True), ['test'])
+        self.assertEqual(utils_models.predict('Test "deux" !', model, model_conf, alternative_version=True), ['deux'])
         remove_dir(model_dir)
 
         # Nominal case - multi-labels
         model_dir = os.path.join(utils.get_models_path(), 'test_model3')
         remove_dir(model_dir)
         model_name = 'test_model3_name'
         model = model_tfidf_svm.ModelTfidfSvm(model_dir=model_dir, model_name=model_name, multi_label=True)
         model.fit(x_train, y_train_multi)
         model.save()
         model, model_conf = utils_models.load_model('test_model3')
         self.assertEqual(utils_models.predict('Ceci est un test', model, model_conf), [('test',)])
         self.assertEqual(utils_models.predict('Toto "deux" !', model, model_conf), [('toto',)])
         self.assertEqual(utils_models.predict(['Ceci est un test', 'Toto test "deux" !'], model, model_conf), [('test',), ('test', 'toto')])
+        self.assertEqual(utils_models.predict('Ceci est un test', model, model_conf, alternative_version=True), [('test',)])
+        self.assertEqual(utils_models.predict('Toto "deux" !', model, model_conf, alternative_version=True), [('toto',)])
+        self.assertEqual(utils_models.predict(['Ceci est un test', 'Toto test "deux" !'], model, model_conf, alternative_version=True), [('test',), ('test', 'toto')])
         remove_dir(model_dir)
 
     def test10_predict_with_proba(self):
         '''Test of the function {{package_name}}.models_training.utils_models.predict_with_proba'''
         # Data
         x_train_base = ['Ceci est un test', 'Ceci est un test', 'Ceci est un test', 'Test "deux" !', 'Toto "deux" !', 'Test "deux" !', 'deux'] * 10
         y_train_mono = ['test', 'test', 'test', 'deux', 'deux', 'deux', 'deux'] * 10
@@ -345,39 +350,59 @@
         model_dir = os.path.join(utils.get_models_path(), 'test_model4')
         remove_dir(model_dir)
         model_name = 'test_model4_name'
         model = model_tfidf_svm.ModelTfidfSvm(model_dir=model_dir, model_name=model_name)
         model.fit(x_train, y_train_mono)
         model.save()
         model, model_conf = utils_models.load_model('test_model4')
+        #
         pred, proba = utils_models.predict_with_proba('Ceci est un test', model, model_conf)
+        pred_alt, proba_alt = utils_models.predict_with_proba('Ceci est un test', model, model_conf, alternative_version=True)
         self.assertEqual(pred, ['test'])
         self.assertEqual(proba, [1.0]) # 1.0 because svm
+        self.assertEqual(pred_alt, ['test'])
+        self.assertEqual(proba_alt, [1.0]) # 1.0 because svm
+        #
         pred, proba = utils_models.predict_with_proba('Test "deux" !', model, model_conf)
+        pred_alt, proba_alt = utils_models.predict_with_proba('Test "deux" !', model, model_conf, alternative_version=True)
         self.assertEqual(pred, ['deux'])
         self.assertEqual(proba, [1.0]) # 1.0 because svm
+        self.assertEqual(pred_alt, ['deux'])
+        self.assertEqual(proba_alt, [1.0]) # 1.0 because svm
         remove_dir(model_dir)
 
         # Nominal case - multi-labels
         model_dir = os.path.join(utils.get_models_path(), 'test_model4')
         remove_dir(model_dir)
         model_name = 'test_model4_name'
         model = model_tfidf_svm.ModelTfidfSvm(model_dir=model_dir, model_name=model_name, multi_label=True)
         model.fit(x_train, y_train_multi)
         model.save()
         model, model_conf = utils_models.load_model('test_model4')
+        #
         pred, proba = utils_models.predict_with_proba('Ceci est un test', model, model_conf)
+        pred_alt, proba_alt = utils_models.predict_with_proba('Ceci est un test', model, model_conf, alternative_version=True)
         self.assertEqual(pred, [('test',)])
         self.assertEqual(proba, [(1.0,)]) # 1.0 because svm
+        self.assertEqual(pred_alt, [('test',)])
+        self.assertEqual(proba_alt, [(1.0,)]) # 1.0 because svm
+        #
         pred, proba = utils_models.predict_with_proba('Toto "deux" !', model, model_conf)
+        pred_alt, proba_alt = utils_models.predict_with_proba('Toto "deux" !', model, model_conf, alternative_version=True)
         self.assertEqual(pred, [('toto',)])
         self.assertEqual(proba, [(1.0,)]) # 1.0 because svm
+        self.assertEqual(pred_alt, [('toto',)])
+        self.assertEqual(proba_alt, [(1.0,)]) # 1.0 because svm
+        #
         pred, proba = utils_models.predict_with_proba(['Ceci est un test', 'Toto test "deux" !'], model, model_conf)
+        pred_alt, proba_alt = utils_models.predict_with_proba(['Ceci est un test', 'Toto test "deux" !'], model, model_conf, alternative_version=True)
         self.assertEqual(pred, [('test',), ('test', 'toto')])
         self.assertEqual(proba, [(1.0,), (1.0, 1.0)]) # 1.0 because svm
+        self.assertEqual(pred_alt, [('test',), ('test', 'toto')])
+        self.assertEqual(proba_alt, [(1.0,), (1.0, 1.0)]) # 1.0 because svm
         remove_dir(model_dir)
 
     def test11_search_hp_cv(self):
         '''Test of the function {{package_name}}.models_training.utils_models.search_hp_cv'''
         # Definition of the variables for the nominal case
         x_train = ['Ceci est un test', 'Ceci est un test', 'Ceci est un test', 'Test "deux" !', 'Toto "deux" !', 'Test "deux" !', 'deux'] * 10
         y_train_mono = ['test', 'test', 'test', 'deux', 'deux', 'deux', 'deux'] * 10
```

### Comparing `gabarit-1.3.1/gabarit/template_num/generate_num_project.py` & `gabarit-1.3.2/gabarit/template_num/generate_num_project.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/Makefile` & `gabarit-1.3.2/gabarit/template_num/num_project/Makefile`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/README.md` & `gabarit-1.3.2/gabarit/template_num/num_project/README.md`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/nose_setup_coverage.cfg` & `gabarit-1.3.2/gabarit/template_num/num_project/nose_setup_coverage.cfg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/model_aggregation_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/model_aggregation_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,91 +251,103 @@
         if not self.trained:
             self.nb_fit = 1
 
         # Update attributes
         self.trained, self.list_classes, self.dict_classes = self._check_trained()
 
     @utils.trained_needed
-    def predict(self, x_test, return_proba: bool = False, **kwargs) -> np.ndarray:
+    def predict(self, x_test, return_proba: bool = False, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Prediction
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
             return_proba (bool): If the function should return the probabilities instead of the classes
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: array of shape = [n_samples]
         '''
         # We decide whether to rely on each model's probas or their predictions
         if return_proba:
-            return self.predict_proba(x_test)
+            return self.predict_proba(x_test, alternative_version=alternative_version)
         else:
             # Get what we want (probas or preds) and use the aggregation function
             if self.using_proba:
-                preds_or_probas = self._predict_probas_sub_models(x_test, **kwargs)
+                preds_or_probas = self._predict_probas_sub_models(x_test, alternative_version=alternative_version, **kwargs)
             else:
-                preds_or_probas = self._predict_sub_models(x_test, **kwargs)
+                preds_or_probas = self._predict_sub_models(x_test, alternative_version=alternative_version, **kwargs)
             return np.array([self.aggregation_function(array, list_classes=self.list_classes) for array in preds_or_probas])  # type: ignore
 
     @utils.trained_needed
-    def predict_proba(self, x_test, **kwargs) -> np.ndarray:
+    def predict_proba(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Predicts the probabilities on the test set
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: array of shape = [n_samples, n_classes]
         '''
-        probas_sub_models = self._predict_probas_sub_models(x_test, **kwargs)
+        probas_sub_models = self._predict_probas_sub_models(x_test, alternative_version=alternative_version, **kwargs)
         # The probas of all models are averaged
         return np.sum(probas_sub_models, axis=1) / probas_sub_models.shape[1]
     
     @utils.trained_needed
-    def _predict_sub_models(self, x_test, **kwargs) -> np.ndarray:
+    def _predict_sub_models(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Recover the predictions of each model being aggregated
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: not multi_label : array of shape = [n_samples, nb_model]
                         multi_label : array of shape = [n_samples, nb_model, n_classes]
         '''
         if self.multi_label:
-            array_predict = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=False) for sub_model in self.sub_models])
+            array_predict = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=False, alternative_version=alternative_version)
+                                      for sub_model in self.sub_models])
             array_predict = np.transpose(array_predict, (1, 0, 2))
         else:
-            array_predict = np.array([sub_model['model'].predict(x_test) for sub_model in self.sub_models])
+            array_predict = np.array([sub_model['model'].predict(x_test, alternative_version=alternative_version) for sub_model in self.sub_models])
             array_predict = np.transpose(array_predict, (1, 0))
         return array_predict
 
     @utils.trained_needed
-    def _predict_probas_sub_models(self, x_test, **kwargs) -> np.ndarray:
+    def _predict_probas_sub_models(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Recover the probabilities of each model being aggregated
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: array of shape = [n_samples, nb_model, nb_classes]
         '''
-        array_probas = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=True) for sub_model in self.sub_models])
+        array_probas = np.array([self._predict_full_list_classes(sub_model['model'], x_test, return_proba=True, alternative_version=alternative_version)
+                                 for sub_model in self.sub_models])
         array_probas = np.transpose(array_probas, (1, 0, 2))
         return array_probas
 
-    def _predict_full_list_classes(self, model: Type[ModelClass], x_test, return_proba: bool = False) -> np.ndarray:
+    def _predict_full_list_classes(self, model: Type[ModelClass], x_test, return_proba: bool = False, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''For multi_label: adds missing columns in the prediction of model (class missing in their list_classes)
         Or, if return_proba, adds a proba of zero to the missing classes in their list_classes
 
         Args:
             model (ModelClass): Model to use
             x_test (?): Array-like or sparse matrix of shape = [n_samples, n_features]
             return_proba (bool): If the function should return the probabilities instead of the classes
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             np.ndarray: The array with the missing columns added
         '''
         # Get predictions or probas
-        preds_or_probas = model.predict(x_test, return_proba=return_proba) # type: ignore
+        preds_or_probas = model.predict(x_test, return_proba=return_proba, alternative_version=alternative_version) # type: ignore
 
         # Manage each cases. Reorder predictions or probas according to aggregation model list_classes
         # Multi label, proba = True
         # Multi label, proba = False
         # Mono label, proba = True
         if model.multi_label or return_proba:
             df_all = pd.DataFrame(np.zeros((len(preds_or_probas), len(self.list_classes))), columns=self.list_classes)  # type: ignore
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/model_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/model_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,25 +74,25 @@
         self.list_classes = None
         self.dict_classes = None
 
         # Other options
         self.level_save = level_save
 
     @utils.trained_needed
-    def predict_with_proba(self, x_test: pd.DataFrame) -> Tuple[np.ndarray, np.ndarray]:
+    def predict_with_proba(self, x_test: pd.DataFrame, **kwargs) -> Tuple[np.ndarray, np.ndarray]:
         '''Predictions on test with probabilities
 
         Args:
             x_test (pd.DataFrame): DataFrame with the test data to be predicted
         Returns:
             predicted_class (np.ndarray): The predicted classes, shape = [n_samples, n_classes] if multi-labels, shape = [n_samples, 1] otherwise
             predicted_proba (np.ndarray): The predicted probabilities for each class, shape = [n_samples, n_classes]
         '''
         # Process
-        predicted_proba = self.predict(x_test, return_proba=True)
+        predicted_proba = self.predict(x_test, return_proba=True, **kwargs)
         predicted_class = self.get_classes_from_proba(predicted_proba)
         return predicted_class, predicted_proba
 
     @utils.trained_needed
     def get_predict_position(self, x_test: pd.DataFrame, y_true) -> np.ndarray:
         '''Gets the order of predictions of y_true.
         Positions start at 1 (not 0)
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/model_xgboost_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/model_xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_gbt_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_gbt_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_knn_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_lgbm_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_logistic_regression_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_rf_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_rf_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_ridge_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_ridge_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_sgd_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_svm_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_sklearn/model_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/model_dense_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/classifiers/models_tensorflow/model_dense_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/model_class.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/model_class.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/model_keras.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/model_keras.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         Kwargs:
             batch_size (int): Batch size
             epochs (int): Number of epochs
             validation_split (float): Percentage for the validation set split
                 Only used if no input validation set when fitting
             patience (int): Early stopping patience
-            keras_params (dict): Parameters used by keras models.
+            keras_params (dict): Parameters used by Keras models.
                 e.g. learning_rate, nb_lstm_units, etc...
                 The purpose of this dictionary is for the user to use it as they wants in the _get_model function
                 This parameter was initially added in order to do an hyperparameters search
         '''
         # TODO: learning rate should be an attribute !
         # Init.
         super().__init__(**kwargs)
@@ -300,22 +300,22 @@
             )
 
         # Set trained
         self.trained = True
         self.nb_fit += 1
 
     @utils.trained_needed
-    def predict(self, x_test: pd.DataFrame, return_proba: bool = False, experimental_version: bool = False, **kwargs) -> np.ndarray:
+    def predict(self, x_test: pd.DataFrame, return_proba: bool = False, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Predictions on test set
 
         Args:
             x_test (pd.DataFrame): DataFrame with the test data to be predicted
         Kwargs:
             return_proba (bool): If the function should return the probabilities instead of the classes
-            experimental_version (bool): If an experimental (but faster) version must be used
+            alternative_version (bool): If an alternative predict version must be used. Should be faster with low nb of inputs.
         Raises:
             ValueError: If the model is not classifier and return_proba=True
             ValueError: If the model is neither a classifier nor a regressor
         Returns:
             (np.ndarray): Array
                 # If not return_proba, shape = [n_samples,] or [n_samples, n_classes]
                 # Else, shape = [n_samples, n_classes]
@@ -326,112 +326,122 @@
 
         # We check input format
         x_test, _ = self._check_input_format(x_test)
 
         # Predict depends on model type
         if self.model_type == 'classifier':
             return self._predict_classifier(x_test, return_proba=return_proba,
-                                            experimental_version=experimental_version)
+                                            alternative_version=alternative_version)
         elif self.model_type == 'regressor':
-            return self._predict_regressor(x_test, experimental_version=experimental_version)
+            return self._predict_regressor(x_test, alternative_version=alternative_version)
         else:
             raise ValueError(f"The model type ({self.model_type}) must be 'classifier' or 'regressor'")
 
     @utils.trained_needed
     def _predict_classifier(self, x_test: pd.DataFrame, return_proba: bool = False,
-                            experimental_version: bool = False) -> np.ndarray:
+                            alternative_version: bool = False) -> np.ndarray:
         '''Predictions on test
         Args:
             x_test (pd.DataFrame): DataFrame with the test data to be predicted
         Kwargs:
             return_proba (boolean): If the function should return the probabilities instead of the classes
-            experimental_version (bool): If an experimental (but faster) version must be used
+            alternative_version (bool): If an alternative predict version must be used. Should be faster with low nb of inputs.
         Raises:
             ValueError: If the model is not of classifier type
         Returns:
             (np.ndarray): Array
                 # If not return_proba, shape = [n_samples,] or [n_samples, n_classes]
                 # Else, shape = [n_samples, n_classes]
         '''
         if self.model_type != 'classifier':
             raise ValueError(f"Models of type {self.model_type} do not implement the method predict_classifier")
 
         # Getting the predictions
-        if experimental_version:
-            predicted_proba = self.experimental_predict_proba(x_test)
+        if alternative_version:
+            predicted_proba = self._alternative_predict_proba(x_test)
         else:
             predicted_proba = self.model.predict(x_test, batch_size=128, verbose=1)  # type: ignore
 
         # We return the probabilities if wanted
         if return_proba:
             return predicted_proba
 
         # Finally, we get the classes predictions
         return self.get_classes_from_proba(predicted_proba)  # type: ignore
 
     @utils.trained_needed
-    def _predict_regressor(self, x_test, experimental_version: bool = False) -> np.ndarray:
+    def _predict_regressor(self, x_test, alternative_version: bool = False) -> np.ndarray:
         '''Predictions on test
         Args:
             x_test (pd.DataFrame): DataFrame with the test data to be predicted
         Kwargs:
-            experimental_version (bool): If an experimental (but faster) version must be used
+            alternative_version (bool): If an alternative predict version must be used. Should be faster with low nb of inputs.
         Raises:
             ValueError: If the model is not of regressor type
         Returns:
             (np.ndarray): Array, shape = [n_samples]
         '''
         if self.model_type != 'regressor':
             raise ValueError(f"Models of type {self.model_type} do not implement the method predict_regressor")
 
         # Getting the predictions
-        if experimental_version:
-            predictions = self.experimental_predict_proba(x_test)
+        if alternative_version:
+            predictions = self._alternative_predict_proba(x_test)
         else:
             predictions = self.model.predict(x_test, batch_size=128, verbose=1)  # type: ignore
 
         # Finally, we get the final format
         # TODO : should certainly be changed for multi-output
         # TODO : create an equivalent of get_classes_from_proba for regression ?
         return np.array([pred[0] for pred in predictions])
 
     @utils.trained_needed
-    def predict_proba(self, x_test: pd.DataFrame, **kwargs) -> np.ndarray:
+    def predict_proba(self, x_test: pd.DataFrame, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Predicts the probabilities on the test set
 
         Args:
             x_test (pd.DataFrame): Array-like, shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative predict version must be used. Should be faster with low nb of inputs.
         Raises:
             ValueError: If model not classifier
         Returns:
             (np.ndarray): Array, shape = [n_samples, n_classes]
         '''
         if self.model_type != 'classifier':
             raise ValueError(f"Models of type {self.model_type} do not implement the method predict_proba")
 
         # We check input format
         x_test, _ = self._check_input_format(x_test)
 
         # We use predict again
-        return self.predict(x_test, return_proba=True)
+        return self.predict(x_test, return_proba=True, alternative_version=alternative_version)
 
     @utils.trained_needed
-    def experimental_predict_proba(self, x_test: pd.DataFrame) -> np.ndarray:
-        '''Predictions on test set - simple pass forward - experimental
+    def _alternative_predict_proba(self, x_test: pd.DataFrame) -> np.ndarray:
+        '''Predicts probabilities on the test dataset - Alternative version
+        Should be faster with low nb of inputs.
 
         Args:
             x_test (pd.DataFrame): Array-like, shape = [n_samples]
         Returns:
             (np.ndarray): Array, shape = [n_samples, n_classes]
         '''
-        @tf.function
-        def serve(x):
-            return self.model(x, training=False)
+        return self._serve(x_test).numpy()
+
+    @tf.function
+    def _serve(self, x: pd.DataFrame):
+        '''Improves predict function using tf.function (cf. https://www.tensorflow.org/guide/function)
 
-        return serve(x_test).numpy()
+        Args:
+            x (pd.DataFrame): input data
+        Returns:
+            tf.tensor: model's output
+        '''
+        return self.model(x, training=False)
 
     def _get_model(self) -> Model:
         '''Gets a model structure - returns the instance model instead if already defined
 
         Returns:
             (Model): a Keras model
         '''
@@ -555,15 +565,15 @@
                 plt.plot(fit_history.history[metric])
                 plt.plot(fit_history.history[f'val_{metric}'])
                 plt.title(f"Model {title}")
                 plt.ylabel(title)
                 plt.xlabel('Epoch')
                 plt.legend(['Train', 'Validation'], loc='upper left')
                 # Save
-                filename == f"{filename}.jpeg"
+                filename = f"{filename}.jpeg"
                 plt.savefig(os.path.join(plots_path, filename))
 
                 # Close figures
                 plt.close('all')
 
     def _save_model_png(self, model) -> None:
         '''Tries to save the structure of the model in png format
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/model_pipeline.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/model_aggregation_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/model_aggregation_regressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,51 +190,55 @@
         # Set nb_fit to 1 if not already trained
         if not self.trained:
             self.nb_fit = 1
 
         self.trained = self._check_trained()
 
     @utils.trained_needed
-    def predict(self, x_test, return_proba: bool = False, **kwargs) -> np.ndarray:
+    def predict(self, x_test, return_proba: bool = False, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Prediction
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
             return_proba (bool): If the function should return the probabilities instead of the classes (Keras compatibility)
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             (np.ndarray): Array of shape = [n_samples]
         Raises:
             ValueError: If return_proba=True
         '''
         if return_proba:
             raise ValueError(f"Models of the type {self.model_type} can't handle probabilities")
-        preds = self._predict_sub_models(x_test, **kwargs)
+        preds = self._predict_sub_models(x_test, alternative_version=alternative_version, **kwargs)
         return np.array([self.aggregation_function(array) for array in preds]) # type: ignore
 
     @utils.trained_needed
     def predict_proba(self, x_test, **kwargs) -> None:
         '''Predicts the probabilities on the test set - raise ValueError
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
         Raises:
             ValueError: Models of type regressor do not implement the method predict_proba
         '''
         raise ValueError(f"Models of type regressor do not implement the method predict_proba")
 
     @utils.trained_needed
-    def _predict_sub_models(self, x_test, **kwargs) -> np.ndarray:
+    def _predict_sub_models(self, x_test, alternative_version: bool = False, **kwargs) -> np.ndarray:
         '''Recover the predictions of each model being aggregated
 
         Args:
             x_test (?): array-like or sparse matrix of shape = [n_samples, n_features]
+        Kwargs:
+            alternative_version (bool): If an alternative version must be used for Keras models. Should be faster with low nb of inputs.
         Returns:
             (np.ndarray): array of shape = [n_samples, nb_model]
         '''
-        array_predict = np.array([sub_model['model'].predict(x_test) for sub_model in self.sub_models])
+        array_predict = np.array([sub_model['model'].predict(x_test, alternative_version=alternative_version) for sub_model in self.sub_models])
         array_predict = np.transpose(array_predict, (1, 0))
         return array_predict
 
     def save(self, json_data: Union[dict, None] = None) -> None:
         '''Saves the model
 
         Kwargs:
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/model_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/model_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/model_xgboost_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/model_xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_bayesian_ridge_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_bayesian_ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_elasticnet_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_elasticnet_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_gbt_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_gbt_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_kernel_ridge_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_kernel_ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_knn_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_knn_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_lgbm_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_pls_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_pls_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_rf_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_rf_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_sgd_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_sgd_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_svr_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_sklearn/model_svr_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/model_dense_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/regressors/models_tensorflow/model_dense_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/utils_deep_keras.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/utils_deep_keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-## Utils - tools-functions for deep_learning keras models
+## Utils - tools-functions for deep_learning Keras models
 # Copyright (C) <2018-2022>  <Agence Data Services, DSI Pôle Emploi>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/models_training/utils_models.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/models_training/utils_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -344,20 +344,23 @@
     preprocessed_x = preprocess_pipeline.transform(df[columns_in])
     # Reconstruct dataframe & return
     preprocessed_df = pd.DataFrame(preprocessed_x)
     preprocessed_df = preprocess.retrieve_columns_from_pipeline(preprocessed_df, preprocess_pipeline)
     return preprocessed_df
 
 
-def predict(content: pd.DataFrame, model, **kwargs) -> list:
+def predict(content: pd.DataFrame, model, alternative_version: bool = False, **kwargs) -> list:
     '''Gets predictions of a model on a dataset
 
     Args:
         content (pd.DataFrame): New dataset to be predicted
         model (ModelClass): Model to use
+    Kwargs:
+        alternative_version (bool): If an alternative version must be used. Should be faster with low nb of inputs.
+                                    Only available for Keras models.
     Returns:
         REGRESSION :
             float: prediction
         MONO-LABEL CLASSIFICATION:
             str: prediction
         MULTI-LABELS CLASSIFICATION:
             tuple: predictions
@@ -368,29 +371,33 @@
     if model.preprocess_pipeline is not None:
         df_prep = apply_pipeline(content, model.preprocess_pipeline)
     else:
         df_prep = content.copy()
         logger.warning("No preprocessing pipeline found - we consider no preprocessing, but it should not be so !")
 
     # Get predictions
-    predictions = model.predict(df_prep)
+    predictions = model.predict(df_prep, alternative_version=alternative_version)
 
     # Inverse transform (needed for classification)
     predictions = model.inverse_transform(predictions)
 
     # Return
     return predictions
 
 
-def predict_with_proba(content: pd.DataFrame, model) -> Union[Tuple[List[str], List[float]], Tuple[List[tuple], List[tuple]]]:
+def predict_with_proba(content: pd.DataFrame, model, alternative_version: bool = False,
+                       **kwargs) -> Union[Tuple[List[str], List[float]], Tuple[List[tuple], List[tuple]]]:
     '''Gets probabilities predictions of a model on a dataset
 
     Args:
         content (pd.DataFrame): New dataset to be predicted
         model (ModelClass): Model to use
+    Kwargs:
+        alternative_version (bool): If an alternative version must be used. Should be faster with low nb of inputs.
+                                    Only available for Keras models.
     Raises:
         ValueError: If the model type is not classifier
     Returns:
         MONO-LABEL CLASSIFICATION:
             List[str]: predictions
             List[float]: probabilities
         MULTI-LABELS CLASSIFICATION:
@@ -405,26 +412,26 @@
     if model.preprocess_pipeline is not None:
         df_prep = apply_pipeline(content, model.preprocess_pipeline)
     else:
         df_prep = content.copy()
         logger.warning("No preprocessing pipeline found - we consider no preprocessing, but it should not be so !")
 
     # Get predictions
-    predictions, probas = model.predict_with_proba(df_prep)
+    predictions, probas = model.predict_with_proba(df_prep, alternative_version=alternative_version)
 
     # Rework format
     if not model.multi_label:
-        prediction = model.inverse_transform(predictions)
-        proba = list(probas.max(axis=1))
+        predictions = model.inverse_transform(predictions)
+        probas = list(probas.max(axis=1))
     else:
-        prediction = [tuple(np.array(model.list_classes).compress(indicators)) for indicators in predictions]
-        proba = [tuple(np.array(probas[i]).compress(indicators)) for i, indicators in enumerate(predictions)]
+        probas = [tuple(np.array(probas[i]).compress(indicators)) for i, indicators in enumerate(predictions)]
+        predictions = [tuple(np.array(model.list_classes).compress(indicators)) for indicators in predictions]
 
-    # Return prediction & proba
-    return prediction, proba
+    # Return predictions & probas
+    return predictions, probas
 
 
 def search_hp_cv(model_cls, model_params: dict, hp_params: dict, scoring_fn: Union[str, Callable],
                  kwargs_fit: dict, n_splits: int = 5):
     '''Searches for hyperparameters - works only with classifiers !
 
     Args:
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/monitoring/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/monitoring/mlflow_logger.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/monitoring/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/monitoring/model_explainer.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/monitoring/model_explainer.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/__init__.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/column_preprocessors.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/column_preprocessors.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/outlier_detection.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/preprocessing/preprocess.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name/utils.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name/utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-exploration/EDA/EDA.ipynb` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-exploration/EDA/EDA.ipynb`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/post-checkout` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/post-checkout`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-commit` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-commit`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-push` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/git_hooks/pre-push`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-ressources/robot.jpg` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-ressources/robot.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/1_preprocess_data.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/1_preprocess_data.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/2_apply_existing_pipeline.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/2_apply_existing_pipeline.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/3_training_classification.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/3_training_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         y_col (list<str|int>): Name of the model's target column(s) - y
     Kwargs:
         excluded_cols (list<str|int>): List of columns to NOT use as model's input (no need to include target columns)
         min_rows (int): Minimal number of occurrences for a class to be considered by the model
             Corresponding entries are removed from both training & validation dataset - mono-label only
         filename_valid (str): Name of the validation dataset (actually a path relative to {{package_name}}-data)
             If None, we do not use a validation dataset.
-                -> for keras models (i.e. Neural Networks), we'll use a portion of the training dataset as the validation.
+                -> for Keras models (i.e. Neural Networks), we'll use a portion of the training dataset as the validation.
         level_save (str): Save level
             LOW: statistics + configurations + logger keras - /!\\ the model won't be reusable /!\\ -
             MEDIUM: LOW + hdf5 + pkl + plots
             HIGH: MEDIUM + predictions
         sep (str): Separator to use with the .csv files
         encoding (str): Encoding to use with the .csv files
         model (ModelClass): A model to be fitted. This should only be used for testing purposes.
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/3_training_regression.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/3_training_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     Args:
         filename (str): Name of the training dataset (actually a path relative to {{package_name}}-data)
         y_col (str | int): Name of the model's target column - y
     Kwargs:
         excluded_cols (list<str|int>): List of columns to NOT use as model's input (no need to include target columns)
         filename_valid (str): Name of the validation dataset (actually a path relative to {{package_name}}-data)
             If None, we do not use a validation dataset.
-                -> for keras models (i.e. Neural Networks), we'll use a portion of the training dataset as the validation.
+                -> for Keras models (i.e. Neural Networks), we'll use a portion of the training dataset as the validation.
         level_save (str): Save level
             LOW: statistics + configurations + logger keras - /!\\ the model won't be reusable /!\\ -
             MEDIUM: LOW + hdf5 + pkl + plots
             HIGH: MEDIUM + predictions
         sep (str): Separator to use with the .csv files
         encoding (str): Encoding to use with the .csv files
         model (ModelClass): A model to be fitted. This should only be used for testing purposes.
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/4_predict.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/4_predict.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/5_demonstrator.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/5_demonstrator.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_create_samples.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_create_samples.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_fairness_report.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_fairness_report.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_merge_files.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_merge_files.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_reload_model.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_reload_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     This is done be reusing 'standalone' files.
 
     Args:
         model_dir (str): Name of the model to reload (not a path, just the directory name)
     Kwargs:
         config_file (str): Name of the configuration file
         sklearn_pipeline_file (str): Standalone sklearn pipeline file name (pipeline models)
-        weights_file (str): Neural Network weights file name (keras models)
+        weights_file (str): Neural Network weights file name (Keras models)
         xgboost_file (str): Standalone XGBoost file name (xgboost models)
         preprocess_pipeline_file (str): Name of the preprocessing pipeline file (all models)
         aggregation_function_path (str): aggregation_function file name (model aggregation)
     Raises:
         FileNotFoundError: If model can't be found
         FileNotFoundError: If model's configuration does not exist
         ValueError: If the model's type is invalid
@@ -184,15 +184,15 @@
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     # model_X should be the model's directory name: e.g. model_preprocess_pipeline_svm_2019_12_05-12_57_18
     parser.add_argument('-m', '--model_dir', required=True, help="Name of the model to reload (not a path, just the directory name)")
     parser.add_argument('-c', '--config_file', default='configurations.json', help="Name of the configuration file")
     parser.add_argument('--sklearn_pipeline_file', default='sklearn_pipeline_standalone.pkl', help="Standalone sklearn pipeline file name (pipeline models)")
-    parser.add_argument('-w', '--weights_file', default='best.hdf5', help="Neural Network weights file name (keras models)")
+    parser.add_argument('-w', '--weights_file', default='best.hdf5', help="Neural Network weights file name (Keras models)")
     parser.add_argument('--xgboost_file', default='xbgoost_standalone.model', help="Standalone XGBoost file name (xgboost models)")
     parser.add_argument('-p', '--preprocess_pipeline_file', default='preprocess_pipeline.pkl', help="Name of the preprocessing pipeline file (all models)")
     parser.add_argument('--aggregation_function_file', default='aggregation_function.pkl', help="aggregation_function_file file name (models aggregation)")
     args = parser.parse_args()
     main(model_dir=args.model_dir, config_file=args.config_file,
          sklearn_pipeline_file=args.sklearn_pipeline_file, weights_file=args.weights_file,
          xgboost_file=args.xgboost_file, preprocess_pipeline_file=args.preprocess_pipeline_file,
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_split_train_valid_test.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_split_train_valid_test.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-scripts/utils/0_sweetviz_report.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-scripts/utils/0_sweetviz_report.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/answers.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/answers.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/utils.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/verify.py` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_exercices/verify.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/package_name-tutorials/tutorial_num.ipynb` & `gabarit-1.3.2/gabarit/template_num/num_project/package_name-tutorials/tutorial_num.ipynb`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/requirements.txt` & `gabarit-1.3.2/gabarit/template_num/num_project/requirements.txt`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/setup.py` & `gabarit-1.3.2/gabarit/template_num/num_project/setup.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_column_preprocessors.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_column_preprocessors.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_dataset.csv` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_dataset.csv`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_dataset2.csv` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_dataset2.csv`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_mlflow_logger.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_aggregation_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_aggregation_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         else:
             return np.array([self.dict_predictions[tuple(x)] for x in x_test])
 
     def predict_proba(self, x_test, **kwargs):
         return np.array([self.dict_predictions_proba[tuple(x)] for x in x_test])
 
 # Predictions for the mock mono_label models
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 dict_predictions_1 = {(1, 2): '0', (1, 3): '0', (2, 1): '1', (2, 2): '0', (3, 1): '1'}
 dict_predictions_2 = {(1, 2): '1', (1, 3): '1', (2, 1): '0', (2, 2): '0', (3, 1): '1'}
 dict_predictions_3 = {(1, 2): '1', (1, 3): '1', (2, 1): '2', (2, 2): '1', (3, 1): '4'}
 dict_predictions_4 = {(1, 2): '2', (1, 3): '2', (2, 1): '3', (2, 2): '3', (3, 1): '1'}
 dict_predictions_5 = {(1, 2): '3', (1, 3): '2', (2, 1): '4', (2, 2): '3', (3, 1): '1'}
 list_dict_predictions = [dict_predictions_1, dict_predictions_2, dict_predictions_3, dict_predictions_4, dict_predictions_5] 
 
@@ -97,14 +98,15 @@
                             (2, 1): np.array([0.3, 0.25, 0.45]), (2, 2): np.array([0.4, 0.1, 0.5]), (3, 1): np.array([0.25, 0.4, 0.35])}
 dict_predictions_proba_5 = {(1, 2): np.array([0.1, 0.3, 0.5, 0.1]), (1, 3): np.array([0.1, 0.5, 0.3, 0.1]), 
                             (2, 1): np.array([0.1, 0.3, 0.1, 0.5]), (2, 2): np.array([0.1, 0.3, 0.5, 0.1]), (3, 1): np.array([0.5, 0.3, 0.1, 0.1])}
 
 x_test = np.array([(1, 2), (1, 3), (2, 1), (2, 2), (3, 1)])
 
 # Definition of the targets for the mono_label cases
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 target_predict_mono_majority_vote_dict = {(1, 2):'1', (1, 3):'1', (2, 1):'1', (2, 2):'0', (3, 1):'1'}
 target_get_predictions_mono = np.array([[list_dict_predictions[i][tuple(key)] for i in range(len(list_dict_predictions))] for key in x_test])
 target_get_proba_mono = np.array([[[0.7, 0.3, 0.0, 0.0, 0.0],
   [0.3, 0.7, 0.0, 0.0, 0.0],
   [0.0, 0.4, 0.25, 0.0, 0.35],
   [0.0, 0.1, 0.5, 0.4, 0.0],
   [0.0, 0.1, 0.3, 0.5, 0.1]],
@@ -161,22 +163,24 @@
                                                 (2, 2): [1, 1, 0, 1, 0], (3, 1): [0, 1, 0, 0, 1]}
 target_predict_mono_vote_labels_dict = {(1, 2): [0, 0, 0, 0, 0], (1, 3): [0, 0, 0, 0, 0,], (2, 1): [0, 0, 0, 0, 0], 
                                                 (2, 2): [0, 0, 0, 0, 0], (3, 1): [0, 1, 0, 0, 0]}
 target_predict_mono_all_predictions = np.array([target_predict_mono_all_predictions_dict[tuple(x)] for x in x_test])
 target_predict_mono_vote_labels = np.array([target_predict_mono_vote_labels_dict[tuple(x)] for x in x_test])
 
 # Instanciation of the mock mono_label models
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 mock_model_mono_1 = MockModel(dict_predictions_1, dict_predictions_proba_1, 'model_mono_1', False, ['0', '1'])
 mock_model_mono_2 = MockModel(dict_predictions_2, dict_predictions_proba_2, 'model_mono_2', False, ['1', '0'])
 mock_model_mono_3 = MockModel(dict_predictions_3, dict_predictions_proba_3, 'model_mono_3', False, ['1', '2', '4'])
 mock_model_mono_4 = MockModel(dict_predictions_4, dict_predictions_proba_4, 'model_mono_4', False, ['2', '1', '3'])
 mock_model_mono_5 = MockModel(dict_predictions_5, dict_predictions_proba_5, 'model_mono_5', False, ['1', '2', '3', '4'])
 list_models_mono = [mock_model_mono_1, mock_model_mono_2, mock_model_mono_3, mock_model_mono_4, mock_model_mono_5]
 
 # Instanciation of the mock multi_label models
+# TODO: to be changed, cf. https://github.com/OSS-Pole-Emploi/gabarit/issues/160
 mock_model_multi_1 = MockModel(dict_predictions_multi_1, dict_predictions_proba_1, 'model_multi_1', True, ['0', '1'])
 mock_model_multi_2 = MockModel(dict_predictions_multi_2, dict_predictions_proba_2, 'model_multi_2', True, ['1', '0'])
 mock_model_multi_3 = MockModel(dict_predictions_multi_3, dict_predictions_proba_3, 'model_multi_3', True, ['1', '2', '4'])
 mock_model_multi_4 = MockModel(dict_predictions_multi_4, dict_predictions_proba_4, 'model_multi_4', True, ['2', '1', '3'])
 list_models_multi = [mock_model_multi_1, mock_model_multi_2, mock_model_multi_3, mock_model_multi_4]
 
 # Definitions for a mixture of mono/multi-labels models
@@ -629,14 +633,19 @@
             possible_classes = {vote[0] for vote in votes if vote[1]==votes[0][1]}
             return [prediction for prediction in predictions if prediction in possible_classes][0]
 
         # Function including all the checks we have to perform
         def test_predict(model, x_test, target_predict, target_probas):
             preds = model.predict(x_test)
             probas = model.predict(x_test, return_proba=True)
+            preds_alt = model.predict(x_test, alternative_version=True)
+            probas_alt = model.predict(x_test, return_proba=True, alternative_version=True)
+            # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+            # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+            np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
             self.assertEqual(preds.shape, target_predict.shape)
             self.assertEqual(probas.shape, target_probas.shape)
             # Check the predictions
             if model.multi_label:
                 for truth, pred in zip(target_predict, preds):
                     for value_true, value_pred in zip(truth, pred):
                         self.assertEqual(value_true, value_pred)
@@ -688,79 +697,95 @@
         '''Test of {{package_name}}.models_training.model_aggregation_classifier.ModelAggregationClassifier._predict_probas_sub_models'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         model = ModelAggregationClassifier(model_dir=model_dir, list_models=list_models_mono)
         probas = model._predict_probas_sub_models(x_test)
+        probas_alt = model._predict_probas_sub_models(x_test, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertTrue(isinstance(probas, np.ndarray))
         self.assertEqual(target_get_proba_mono.shape, probas.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_get_proba_mono[i], probas[i]):
                 for truth_value, pred_value in zip(truth, pred):
                     self.assertAlmostEqual(truth_value, pred_value)
         remove_dir_model(model, model_dir)
 
         # Model needs to be fitted
         model = ModelAggregationClassifier(model_dir=model_dir)
         with self.assertRaises(AttributeError):
             model._predict_probas_sub_models('test')
+        with self.assertRaises(AttributeError):
+            model._predict_probas_sub_models('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test08_model_aggregation_classifier__predict_sub_models(self):
         '''Test of {{package_name}}.models_training.model_aggregation_classifier.ModelAggregationClassifier._predict_sub_models'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # mono_label
         model = ModelAggregationClassifier(model_dir=model_dir, list_models=list_models_mono)
         preds = model._predict_sub_models(x_test)
+        preds_alt = model._predict_sub_models(x_test, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertTrue(isinstance(preds, np.ndarray))
         self.assertEqual(target_get_predictions_mono.shape, preds.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_get_predictions_mono[i], preds[i]):
                 self.assertEqual(truth, pred)
         remove_dir_model(model, model_dir)
 
         # multi_label
         model = ModelAggregationClassifier(model_dir=model_dir, list_models=list_models_multi, aggregation_function='all_predictions', multi_label=True)
         preds = model._predict_sub_models(x_test)
+        preds_alt = model._predict_sub_models(x_test, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertTrue(isinstance(preds, np.ndarray))
         self.assertEqual(target_get_predictions_multi.shape, preds.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_get_predictions_multi[i], preds[i]):
                 for truth_value, pred_value in zip(truth, pred):
                     self.assertEqual(truth_value, pred_value)
         remove_dir_model(model, model_dir)
 
         # Model needs to be fitted
         model = ModelAggregationClassifier(model_dir=model_dir)
         with self.assertRaises(AttributeError):
             model._predict_sub_models('test')
+        with self.assertRaises(AttributeError):
+            model._predict_sub_models('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test09_model_aggregation_classifier_predict_proba(self):
         '''Test of {{package_name}}.models_training.model_aggregation_classifier.ModelAggregationClassifier.predict_proba'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         model = ModelAggregationClassifier(model_dir=model_dir, list_models=list_models_mono)
         probas = model.predict_proba(x_test)
+        probas_alt = model.predict_proba(x_test, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(target_predict_mono_proba.shape, probas.shape)
         for i in range(len(x_test)):
             for truth, pred in zip(target_predict_mono_proba[i], probas[i]):
                 self.assertAlmostEqual(truth, pred)
         remove_dir_model(model, model_dir)
 
         # Model needs to be fitted
         model = ModelAggregationClassifier(model_dir=model_dir)
         with self.assertRaises(AttributeError):
             model.predict_proba('test')
+        with self.assertRaises(AttributeError):
+            model.predict_proba('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test10_model_aggregation_classifier_predict_full_list_classes(self):
         '''Test of {{package_name}}.models_training.model_aggregation_classifier.ModelAggregationClassifier._predict_full_list_classes'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
@@ -776,21 +801,27 @@
                                     {(1, 2):np.array([0.2, 0.8, 0.0]), (1, 3):np.array([0.9, 0.0, 0.1]), (2, 1):np.array([0.2, 0.1, 0.7])}, 
                                     'model_mono', 
                                     False, 
                                     ['1', '2', '4'])
 
         # mono_label, no return_proba
         preds = model._predict_full_list_classes(mock_model_mono, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=False)
+        preds_alt = model._predict_full_list_classes(mock_model_mono, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=False, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_mono = np.array(['2', '1', '4'])
         self.assertEqual(target_mono.shape, preds.shape)
         for truth, pred in zip(target_mono, preds):
             self.assertEqual(truth, pred)
 
         # mono_label, return_proba
         preds = model._predict_full_list_classes(mock_model_mono, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=True)
+        preds_alt = model._predict_full_list_classes(mock_model_mono, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=True, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_mono_return_proba = np.array([[0.0, 0.2, 0.8, 0.0, 0.0, 0.0], [0.0, 0.9, 0.0, 0.0, 0.1, 0.0], [0.0, 0.2, 0.1, 0.0, 0.7, 0.0]])
         self.assertEqual(target_mono_return_proba.shape, preds.shape)
         for truth, pred in zip(target_mono_return_proba, preds):
             for truth_value, pred_value in zip(truth, pred):
                 self.assertAlmostEqual(truth_value, pred_value)
 
         remove_dir(model_dir)
@@ -807,22 +838,28 @@
                                     {(1, 2):np.array([0.2, 0.8, 0.0]), (1, 3):np.array([0.9, 0.0, 0.1]), (2, 1):np.array([0.2, 0.1, 0.7])}, 
                                     'model_mono', 
                                     True, 
                                     ['1', '2', '4'])
 
         # multi_label, no return_proba
         preds = model._predict_full_list_classes(mock_model_multi, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=False)
+        preds_alt = model._predict_full_list_classes(mock_model_multi, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=False, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_multi = np.array([[0, 1, 1, 0, 0, 0], [0, 1, 0, 0, 1, 0], [0, 0, 0, 0, 0, 0]])
         self.assertEqual(target_multi.shape, preds.shape)
         for truth, pred in zip(target_multi, preds):
             for truth_value, pred_value in zip(truth, pred):
                 self.assertEqual(truth_value, pred_value)
 
         # multi_label, return_proba
         preds = model._predict_full_list_classes(mock_model_multi, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=True)
+        preds_alt = model._predict_full_list_classes(mock_model_multi, np.array([(1, 2), (1, 3), (2, 1)]), return_proba=True, alternative_version=True)
+        # TODO: the folowing test should be included once issue 160 is fixed (https://github.com/OSS-Pole-Emploi/gabarit/issues/160)
+        # np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         target_mono_return_proba = np.array([[0.0, 0.2, 0.8, 0.0, 0.0, 0.0], [0.0, 0.9, 0.0, 0.0, 0.1, 0.0], [0.0, 0.2, 0.1, 0.0, 0.7, 0.0]])
         self.assertEqual(target_mono_return_proba.shape, preds.shape)
         for truth, pred in zip(target_mono_return_proba, preds):
             for truth_value, pred_value in zip(truth, pred):
                 self.assertAlmostEqual(truth_value, pred_value)
 
         remove_dir(model_dir)
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_aggregation_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_aggregation_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,14 +367,16 @@
         '''Test of {{package_name}}.models_training.model_aggregation_regressor.ModelAggregationRegressor.predict'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         def test_method(model, x_test, target_predict):
             preds = model.predict(x_test)
+            preds_alt = model.predict(x_test, alternative_version=True)
+            np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
             self.assertEqual(preds.shape, target_predict.shape)
             for i in range(len(preds)):
                 self.assertAlmostEqual(preds[i], target_predict[i], places=4)
 
         # median_predict
         model = ModelAggregationRegressor(model_dir=model_dir, list_models=list_mock_model, aggregation_function='median_predict')
         test_method(model, x_test, target_predict=mock_target_median)
@@ -402,22 +404,26 @@
         y_train = pd.Series([1, 1, 1, 2, 3, 3, 3] * 10)
 
         # Model needs to be fitted
         gbt, sgd, _, _ = self.create_models()
         model = ModelAggregationRegressor(model_dir=model_dir, list_models=[gbt, sgd])
         with self.assertRaises(AttributeError):
             model.predict(x_train)
+        with self.assertRaises(AttributeError):
+            model.predict(x_train, alternative_version=True)
         remove_dir_model(model, model_dir)
 
         # No return_proba
         gbt, sgd, _, _ = self.create_models()
         model = ModelAggregationRegressor(model_dir=model_dir, list_models=[gbt, sgd])
         model.fit(x_train, y_train)
         with self.assertRaises(ValueError):
             model.predict(x_train, return_proba=True)
+        with self.assertRaises(ValueError):
+            model.predict(x_train, return_proba=True, alternative_version=True)
         remove_dir_model(model, model_dir)
 
     def test07_model_aggregation_regressor_predict_proba(self):
         '''Test of {{package_name}}.models_training.model_aggregation_regressor.ModelAggregationRegressor.predict_proba'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
@@ -426,35 +432,41 @@
         y_train = pd.Series([1, 1, 1, 2, 3, 3, 3] * 10)
 
         gbt, sgd, _, _ = self.create_models()
         model = ModelAggregationRegressor(model_dir=model_dir, list_models=[gbt, sgd])
         model.fit(x_train, y_train)
         with self.assertRaises(ValueError):
             model.predict_proba(x_train)
+        with self.assertRaises(ValueError):
+            model.predict_proba(x_train, alternative_version=True)
         remove_dir_model(model, model_dir)
 
     def test08_model_aggregation_regressor_get_predictions(self):
         '''Test of {{package_name}}.models_training.model_aggregation_regressor.ModelAggregationRegressor._predict_sub_models'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         model = ModelAggregationRegressor(model_dir=model_dir, list_models=list_mock_model)
         preds = model._predict_sub_models(x_test)
+        preds_alt = model._predict_sub_models(x_test, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertTrue(isinstance(preds, np.ndarray))
         self.assertEqual(target_get_predictions.shape, preds.shape)
         for i in range(target_get_predictions.shape[0]):
             for j in range(target_get_predictions.shape[1]):
                 self.assertAlmostEqual(target_get_predictions[i][j], preds[i][j])
         remove_dir(model_dir)
 
         # Model needs to be fitted
         model = ModelAggregationRegressor(model_dir=model_dir)
         with self.assertRaises(AttributeError):
             model._predict_sub_models('test')
+        with self.assertRaises(AttributeError):
+            model._predict_sub_models('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test09_median_predict(self):
         '''Test of {{package_name}}.models_training.model_aggregation_regressor.median_predict'''
 
         # 3 models int
         preds = np.array([3, 4, 4])
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_bayesian_ridge_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_bayesian_ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_class.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_class.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_dense_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_dense_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,69 +110,77 @@
         x_col = ['col_1', 'col_2']
         y_col_mono = ['toto']
         y_col_multi = ['y1', 'y2', 'y3']
 
         # Classification - Mono-label - Mono-Class
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_2)
+        #
         preds = model.predict(x_train, return_proba=False)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train),))
+        #
         probas = model.predict(x_train, return_proba=True)
-        self.assertEqual(probas.shape, (len(x_train), 2))  # 2 classes
-        preds = model.predict(x_train, return_proba=False, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train),))
-        probas = model.predict(x_train, return_proba=True, experimental_version=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), 2))  # 2 classes
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         probas_inv = model.predict(x_train_inv, return_proba=True)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Mono-label - Multi-Classes
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_3)
+        #
         preds = model.predict(x_train, return_proba=False)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train),))
+        #
         probas = model.predict(x_train, return_proba=True)
-        self.assertEqual(probas.shape, (len(x_train), 3))  # 3 classes
-        preds = model.predict(x_train, return_proba=False, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train),))
-        probas = model.predict(x_train, return_proba=True, experimental_version=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), 3))  # 3 classes
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         probas_inv = model.predict(x_train_inv, return_proba=True)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Multi-labels
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True)
         model.fit(x_train, y_train_multi)
+        #
         preds = model.predict(x_train)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train), len(y_col_multi)))
+        #
         probas = model.predict(x_train, return_proba=True)
-        self.assertEqual(probas.shape, (len(x_train), len(y_col_multi)))
-        preds = model.predict(x_train, return_proba=False, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train), len(y_col_multi)))
-        probas = model.predict(x_train, return_proba=True, experimental_version=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), len(y_col_multi)))
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         probas_inv = model.predict(x_train_inv, return_proba=True)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Model needs to be fitted
+        model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         with self.assertRaises(AttributeError):
-            model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
             model.predict(x_train)
+        with self.assertRaises(AttributeError):
+            model.predict(x_train, alternative_version=True)
         remove_dir(model_dir)
 
     def test03_model_dense_classifier_predict_proba(self):
         '''Test of the method predict_proba of {{package_name}}.models_training.classifiers.models_tensorflow.model_dense_classifier.ModelDenseClassifier'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
@@ -186,48 +194,59 @@
         x_col = ['col_1', 'col_2']
         y_col_mono = ['toto']
         y_col_multi = ['y1', 'y2', 'y3']
 
         # Classification - Mono-label - Mono-Class
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_2)
+        #
         probas = model.predict_proba(x_train)
+        probas_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), 2))  # 2 classes
         self.assertTrue(isinstance(probas[0][0], (np.floating, float)))
         # Test inversed columns order
         probas_inv = model.predict_proba(x_train_inv)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Mono-label - Multi-Classes
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_3)
+        #
         probas = model.predict_proba(x_train)
+        probas_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), 3))  # 3 classes
         self.assertTrue(isinstance(probas[0][0], (np.floating, float)))
         # Test inversed columns order
         probas_inv = model.predict_proba(x_train_inv)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Multi-labels
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True)
         model.fit(x_train, y_train_multi)
+        #
         probas = model.predict_proba(x_train)
+        probas_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), len(y_col_multi)))  # 3 labels
         self.assertTrue(isinstance(probas[0][0], (np.floating, float)))
         # Test inversed columns order
         probas_inv = model.predict_proba(x_train_inv)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Model needs to be fitted
+        model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         with self.assertRaises(AttributeError):
-            model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
             model.predict_proba('test')
+        with self.assertRaises(AttributeError):
+            model.predict_proba('test', alternative_version=True)
         remove_dir(model_dir)
 
     def test04_model_dense_classifier_get_predict_position(self):
         '''Test of the method {{package_name}}.models_training.classifiers.models_tensorflow.model_dense_classifier.ModelDenseClassifier.get_predict_position'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_dense_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_dense_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,31 +105,35 @@
         y_train_regressor = pd.Series([-3, -2, -8, 0, 5, 6, 5] * 10)
         x_col = ['col_1', 'col_2']
         y_col_mono = ['toto']
 
         # Regressor
         model = ModelDenseRegressor(x_col=x_col, y_col=y_col_mono, model_dir=model_dir, batch_size=8, epochs=2)
         model.fit(x_train, y_train_regressor)
+        #
         preds = model.predict(x_train, return_proba=False)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
         self.assertEqual(preds.shape, (len(x_train),))
+        #
         with self.assertRaises(ValueError):
             probas = model.predict(x_train, return_proba=True)
-        preds = model.predict(x_train, return_proba=False, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train),))
         with self.assertRaises(ValueError):
-            probas = model.predict(x_train, return_proba=True, experimental_version=True)
+            probas = model.predict(x_train, return_proba=True, alternative_version=True)
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         remove_dir(model_dir)
 
         # Model needs to be fitted
+        model = ModelDenseRegressor(x_col=x_col, y_col=y_col_mono, model_dir=model_dir, batch_size=8, epochs=2)
         with self.assertRaises(AttributeError):
-            model = ModelDenseRegressor(x_col=x_col, y_col=y_col_mono, model_dir=model_dir, batch_size=8, epochs=2)
             model.predict(x_train)
+        with self.assertRaises(AttributeError):
+            model.predict(x_train, alternative_version=True)
         remove_dir(model_dir)
 
     def test03_model_dense_regressor_get_model(self):
         '''Test of the method {{package_name}}.models_training.regressors.models_tensorflow.model_dense_regressor.ModelDenseRegressor._get_model'''
 
         # Set vars
         x_col = ['col_1', 'col_2']
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_elasticnet_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_elasticnet_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_explainer.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_explainer.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_gbt_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_gbt_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_gbt_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_gbt_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_keras.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_keras.py`

 * *Files 6% similar despite different names*

```diff
@@ -463,76 +463,84 @@
         x_col = ['col_1', 'col_2']
         y_col_mono = ['toto']
         y_col_multi = ['y1', 'y2', 'y3']
 
         # Classification - Mono-label - Mono-Class
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_2)
+        #
         preds = model.predict(x_train, return_proba=False)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train),))
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
         probas = model.predict(x_train, return_proba=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
         self.assertEqual(probas.shape, (len(x_train), 2))  # 2 classes
-        preds = model.predict(x_train, return_proba=False, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train),))
-        probas = model.predict(x_train, return_proba=True, experimental_version=True)
-        self.assertEqual(probas.shape, (len(x_train), 2))  # 2 classes
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         probas_inv = model.predict(x_train_inv, return_proba=True)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Mono-label - Multi-Classes
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_3)
+        #
         preds = model.predict(x_train, return_proba=False)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train),))
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
         probas = model.predict(x_train, return_proba=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
         self.assertEqual(probas.shape, (len(x_train), 3))  # 3 classes
-        preds = model.predict(x_train, return_proba=False, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train),))
-        probas = model.predict(x_train, return_proba=True, experimental_version=True)
-        self.assertEqual(probas.shape, (len(x_train), 3))  # 3 classes
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         probas_inv = model.predict(x_train_inv, return_proba=True)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Multi-labels
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True)
         model.fit(x_train, y_train_multi)
+        #
         preds = model.predict(x_train)
+        preds_alt = model.predict(x_train, return_proba=False, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train), len(y_col_multi)))
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
         probas = model.predict(x_train, return_proba=True)
+        probas_alt = model.predict(x_train, return_proba=True, alternative_version=True)
         self.assertEqual(probas.shape, (len(x_train), len(y_col_multi)))
-        preds = model.predict(x_train, return_proba=False, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train), len(y_col_multi)))
-        probas = model.predict(x_train, return_proba=True, experimental_version=True)
-        self.assertEqual(probas.shape, (len(x_train), len(y_col_multi)))
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         probas_inv = model.predict(x_train_inv, return_proba=True)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Regressor
         model = ModelDenseRegressor(model_dir=model_dir, batch_size=8, epochs=2)
         model.fit(x_train, y_train_regressor)
+        #
         preds = model.predict(x_train)
+        preds_alt = model.predict(x_train, alternative_version=True)
         self.assertEqual(preds.shape, (len(x_train),))
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        #
         with self.assertRaises(ValueError):
             probas = model.predict(x_train, return_proba=True)
-        preds = model.predict(x_train, experimental_version=True)
-        self.assertEqual(preds.shape, (len(x_train),))
         with self.assertRaises(ValueError):
-            probas = model.predict(x_train, return_proba=True, experimental_version=True)
+            probas = model.predict(x_train, return_proba=True, alternative_version=True)
         # Test inversed columns order
         preds_inv = model.predict(x_train_inv, return_proba=False)
         np.testing.assert_almost_equal(preds, preds_inv, decimal=5)
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
@@ -557,48 +565,56 @@
         y_col_mono = ['toto']
         y_col_multi = ['y1', 'y2', 'y3']
 
         # Classification - Mono-label - Mono-Class
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_2)
         probas = model.predict_proba(x_train)
+        probas_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), 2))  # 2 classes
         self.assertTrue(isinstance(probas[0][0], (np.floating, float)))
         # Test inversed columns order
         probas_inv = model.predict_proba(x_train_inv)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Mono-label - Multi-Classes
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
         model.fit(x_train, y_train_mono_3)
         probas = model.predict_proba(x_train)
+        probas_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), 3))  # 3 classes
         self.assertTrue(isinstance(probas[0][0], (np.floating, float)))
         # Test inversed columns order
         probas_inv = model.predict_proba(x_train_inv)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Classification - Multi-labels
         model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=True)
         model.fit(x_train, y_train_multi)
         probas = model.predict_proba(x_train)
+        probas_alt = model.predict_proba(x_train, alternative_version=True)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
         self.assertEqual(probas.shape, (len(x_train), len(y_col_multi)))  # 3 labels
         self.assertTrue(isinstance(probas[0][0], (np.floating, float)))
         # Test inversed columns order
         probas_inv = model.predict_proba(x_train_inv)
         np.testing.assert_almost_equal(probas, probas_inv, decimal=5)
         remove_dir(model_dir)
 
         # Regressor
         model = ModelDenseRegressor(model_dir=model_dir, batch_size=8, epochs=2)
         model.fit(x_train, y_train_regressor)
         with self.assertRaises(ValueError):
             proba = model.predict_proba(x_train)
+        with self.assertRaises(ValueError):
+            proba = model.predict_proba(x_train, alternative_version=True)
         remove_dir(model_dir)
 
         # Model needs to be fitted
         with self.assertRaises(AttributeError):
             model = ModelDenseClassifier(model_dir=model_dir, batch_size=8, epochs=2, multi_label=False)
             model.predict_proba('test')
         remove_dir(model_dir)
@@ -646,15 +662,43 @@
         # Nominal case
         model = ModelKeras(model_dir=model_dir)
         self.assertEqual(model._get_learning_rate_scheduler(), None)
 
         # Clean
         remove_dir(model_dir)
 
-    def test07_model_keras_save(self):
+    def test07_model_keras_plot_metrics_and_loss(self):
+        '''Test of the method _plot_metrics_and_loss of {{package_name}}.models_training.model_keras.ModelKeras'''
+
+        model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
+        remove_dir(model_dir)
+
+        # Nominal case
+        model = ModelKeras(model_dir=model_dir)
+
+        class FitHistory(object):
+
+            def __init__(self):
+                self.history = {}
+                for metric in ['acc', 'loss', 'categorical_accuracy', 'f1', 'precision', 'recall','mean_absolute_error',
+                               'mae', 'mean_squared_error', 'mse', 'root_mean_squared_error', 'rmse']:
+                    self.history[metric] = [0.1, 0.2, 0.3, 0.5, 0.4]
+                    self.history[f'val_{metric}'] = [0.05, 0.1, 0.2, 0.4, 0.4]
+
+        fit_history = FitHistory()
+        model._plot_metrics_and_loss(fit_history)
+        plots_path = os.path.join(model.model_dir, 'plots')
+        for filename in ['accuracy', 'loss', 'categorical_accuracy', 'f1_score', 'precision', 'recall', 'mae',
+                         'mse', 'rmse']:
+            self.assertTrue(os.path.exists(os.path.join(plots_path, f"{filename}.jpeg")))
+
+        # Clean
+        remove_dir(model_dir)
+
+    def test08_model_keras_save(self):
         '''Test of the method save of {{package_name}}.models_training.model_keras.ModelKeras'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Nominal case
         model = ModelKeras(model_dir=model_dir)
@@ -735,15 +779,15 @@
         self.assertTrue('_get_learning_rate_scheduler' in configs.keys())
         self.assertTrue('custom_objects' in configs.keys())
         self.assertTrue('list_classes' not in configs.keys())  # not in because we do not use the Classifier mixin
         self.assertTrue('dict_classes' not in configs.keys())  # not in because we do not use the Classifier mixin
         self.assertTrue('multi_label' not in configs.keys())  # not in because we do not use the Classifier mixin
         remove_dir(model_dir)
 
-    def test08_model_keras_reload_model(self):
+    def test09_model_keras_reload_model(self):
         '''Test of the method reload_model of {{package_name}}.models_training.model_keras.ModelKeras'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Set vars
         x_train = pd.DataFrame({'col_1': [-5, -1, 0, -2, 2, -6, 3] * 10, 'col_2': [2, -1, -8, 2, 3, 12, 2] * 10})
```

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_kernel_ridge_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_kernel_ridge_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_knn_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_knn_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_knn_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_lgbm_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_lgbm_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_logistic_regression_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_pipeline.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_pipeline.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_pls_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_pls_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_rf_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_rf_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_rf_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_rf_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_ridge_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_ridge_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_sgd_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_sgd_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_sgd_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_svm_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_svr_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_svr_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_xgboost_classifier.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_model_xgboost_regressor.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_model_xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_outlier_detection.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_outlier_detection.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_preprocess.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_utils.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_num/num_project/tests/test_utils_models.py` & `gabarit-1.3.2/gabarit/template_num/num_project/tests/test_utils_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -510,14 +510,16 @@
         model.fit(x_train_1, y_train_classification)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
         self.assertEqual(utils_models.predict(x_test_1, model), y_test_classification)
         self.assertEqual(utils_models.predict(x_test_1_solo, model), y_test_1_classification_solo)
+        self.assertEqual(utils_models.predict(x_test_1, model, alternative_version=True), y_test_classification)
+        self.assertEqual(utils_models.predict(x_test_1_solo, model, alternative_version=True), y_test_1_classification_solo)
         remove_dir(model_dir)
 
         ################
         # RF Classification - mono-label - 2
 
         # Creation fake model
         remove_dir(model_dir)
@@ -525,14 +527,16 @@
         model.fit(x_train_2, y_train_classification)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
         self.assertEqual(utils_models.predict(x_test_2, model), y_test_classification)
         self.assertEqual(utils_models.predict(x_test_2_solo, model), y_test_2_classification_solo)
+        self.assertEqual(utils_models.predict(x_test_2, model, alternative_version=True), y_test_classification)
+        self.assertEqual(utils_models.predict(x_test_2_solo, model, alternative_version=True), y_test_2_classification_solo)
         remove_dir(model_dir)
 
         ################
         # RF Classification - multi-labels - 1
 
         # Creation fake model
         remove_dir(model_dir)
@@ -540,14 +544,16 @@
         model.fit(x_train_1, y_train_classification_multi)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
         self.assertEqual(utils_models.predict(x_test_1, model), y_test_classification_multi)
         self.assertEqual(utils_models.predict(x_test_1_solo, model), y_test_1_classification_multi_solo)
+        self.assertEqual(utils_models.predict(x_test_1, model, alternative_version=True), y_test_classification_multi)
+        self.assertEqual(utils_models.predict(x_test_1_solo, model, alternative_version=True), y_test_1_classification_multi_solo)
         remove_dir(model_dir)
 
         ################
         # RF Classification - multi-labels - 2
 
         # Creation fake model
         remove_dir(model_dir)
@@ -555,14 +561,16 @@
         model.fit(x_train_2, y_train_classification_multi)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
         self.assertEqual(utils_models.predict(x_test_2, model), y_test_classification_multi)
         self.assertEqual(utils_models.predict(x_test_2_solo, model), y_test_2_classification_multi_solo)
+        self.assertEqual(utils_models.predict(x_test_2, model, alternative_version=True), y_test_classification_multi)
+        self.assertEqual(utils_models.predict(x_test_2_solo, model, alternative_version=True), y_test_2_classification_multi_solo)
         remove_dir(model_dir)
 
         ################
         # RF Regression - 1
 
         # Creation fake model
         remove_dir(model_dir)
@@ -571,14 +579,15 @@
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
         # Check just the type, regression is complicated...
         self.assertEqual(type(utils_models.predict(x_test_1, model)), list)
         self.assertTrue(isinstance(utils_models.predict(x_test_1_solo, model), list))
+        np.testing.assert_almost_equal(utils_models.predict(x_test_1, model), utils_models.predict(x_test_1, model, alternative_version=True))
         remove_dir(model_dir)
 
         ################
         # RF Regression - 2
 
         # Creation fake model
         remove_dir(model_dir)
@@ -587,14 +596,15 @@
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
         # Check just the type, regression is complicated...
         self.assertEqual(type(utils_models.predict(x_test_2, model)), list)
         self.assertTrue(isinstance(utils_models.predict(x_test_2_solo, model), list))
+        np.testing.assert_almost_equal(utils_models.predict(x_test_2, model), utils_models.predict(x_test_2, model, alternative_version=True))
         remove_dir(model_dir)
 
 
     def test11_predict_with_proba(self):
         '''Test of the function {{package_name}}.models_training.utils_models.predict_with_proba'''
 
         # Data for training
@@ -623,94 +633,110 @@
         remove_dir(model_dir)
         model = model_rf_classifier.ModelRFClassifier(model_dir=model_dir, model_name=model_name)
         model.fit(x_train_1, y_train_classification)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
-        pred, proba = utils_models.predict_with_proba(x_test_1, model)
-        self.assertEqual(pred, y_test_classification)
-        self.assertEqual(len(proba), len(y_test_classification))
-        self.assertEqual(sum([round(p) for p in proba]), len(y_test_classification))
-        pred, proba = utils_models.predict_with_proba(x_test_1_solo, model)
-        self.assertEqual(pred, y_test_1_classification_solo)
-        self.assertTrue(proba[0] >= 0.5)
+        #
+        preds, probas = utils_models.predict_with_proba(x_test_1, model)
+        preds_alt, probas_alt = utils_models.predict_with_proba(x_test_1, model, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
+        self.assertEqual(preds, y_test_classification)
+        self.assertEqual(len(probas), len(y_test_classification))
+        self.assertEqual(sum([round(p) for p in probas]), len(y_test_classification))
+        #
+        preds, probas = utils_models.predict_with_proba(x_test_1_solo, model)
+        self.assertEqual(preds, y_test_1_classification_solo)
+        self.assertTrue(probas[0] >= 0.5)
         remove_dir(model_dir)
 
         ################
         # RF Classification - mono-label - 2
 
         # Creation fake model
         remove_dir(model_dir)
         model = model_rf_classifier.ModelRFClassifier(model_dir=model_dir, model_name=model_name)
         model.fit(x_train_2, y_train_classification)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
-        pred, proba = utils_models.predict_with_proba(x_test_2, model)
-        self.assertEqual(pred, y_test_classification)
-        self.assertEqual(len(proba), len(y_test_classification))
-        self.assertEqual(sum([round(p) for p in proba]), len(y_test_classification))
-        pred, proba = utils_models.predict_with_proba(x_test_2_solo, model)
-        self.assertEqual(pred, y_test_2_classification_solo)
-        self.assertTrue(proba[0] >= 0.5)
+        preds, probas = utils_models.predict_with_proba(x_test_2, model)
+        preds_alt, probas_alt = utils_models.predict_with_proba(x_test_2, model, alternative_version=True)
+        np.testing.assert_almost_equal(preds, preds_alt, decimal=5)
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
+        self.assertEqual(preds, y_test_classification)
+        self.assertEqual(len(probas), len(y_test_classification))
+        self.assertEqual(sum([round(p) for p in probas]), len(y_test_classification))
+        preds, probas = utils_models.predict_with_proba(x_test_2_solo, model)
+        self.assertEqual(preds, y_test_2_classification_solo)
+        self.assertTrue(probas[0] >= 0.5)
         remove_dir(model_dir)
 
         ################
         # RF Classification - multi-labels - 1
 
         # Creation fake model
         remove_dir(model_dir)
         model = model_rf_classifier.ModelRFClassifier(model_dir=model_dir, model_name=model_name, multi_label=True)
         model.fit(x_train_1, y_train_classification_multi)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
-        pred, proba = utils_models.predict_with_proba(x_test_1, model)
-        self.assertEqual(pred, y_test_classification_multi)
-        self.assertEqual(len(proba), len(y_test_classification_multi))
-        self.assertEqual(sum([round(p[0]) for p in proba]), sum([len(_) for _ in y_test_classification_multi]))
-        pred, proba = utils_models.predict_with_proba(x_test_1_solo, model)
-        self.assertEqual(pred, y_test_1_classification_multi_solo)
-        self.assertTrue(proba[0][0] >= 0.5)
+        preds, probas = utils_models.predict_with_proba(x_test_1, model)
+        preds_alt, probas_alt = utils_models.predict_with_proba(x_test_1, model, alternative_version=True)
+        self.assertEqual(preds, preds_alt)  # List of tuples of strings
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
+        self.assertEqual(preds, y_test_classification_multi)
+        self.assertEqual(len(probas), len(y_test_classification_multi))
+        self.assertEqual(sum([round(p[0]) for p in probas]), sum([len(_) for _ in y_test_classification_multi]))
+        preds, probas = utils_models.predict_with_proba(x_test_1_solo, model)
+        self.assertEqual(preds, y_test_1_classification_multi_solo)
+        self.assertTrue(probas[0][0] >= 0.5)
         remove_dir(model_dir)
 
         ################
         # RF Classification - multi-labels - 2
 
         # Creation fake model
         remove_dir(model_dir)
         model = model_rf_classifier.ModelRFClassifier(model_dir=model_dir, model_name=model_name, multi_label=True)
         model.fit(x_train_2, y_train_classification_multi)
         model.save()
 
         # Nominal case
         model, model_conf = utils_models.load_model(model_dir='test_model')
-        pred, proba = utils_models.predict_with_proba(x_test_2, model)
-        self.assertEqual(pred, y_test_classification_multi)
-        self.assertEqual(len(proba), len(y_test_classification_multi))
-        self.assertEqual(sum([round(p[0]) for p in proba]), sum([len(_) for _ in y_test_classification_multi]))
-        pred, proba = utils_models.predict_with_proba(x_test_2_solo, model)
-        self.assertEqual(pred, y_test_2_classification_multi_solo)
-        self.assertTrue(proba[0][0] >= 0.5)
+        preds, probas = utils_models.predict_with_proba(x_test_2, model)
+        preds_alt, probas_alt = utils_models.predict_with_proba(x_test_2, model, alternative_version=True)
+        self.assertEqual(preds, preds_alt)  # List of tuples of strings
+        np.testing.assert_almost_equal(probas, probas_alt, decimal=5)
+        self.assertEqual(preds, y_test_classification_multi)
+        self.assertEqual(len(probas), len(y_test_classification_multi))
+        self.assertEqual(sum([round(p[0]) for p in probas]), sum([len(_) for _ in y_test_classification_multi]))
+        preds, probas = utils_models.predict_with_proba(x_test_2_solo, model)
+        self.assertEqual(preds, y_test_2_classification_multi_solo)
+        self.assertTrue(probas[0][0] >= 0.5)
         remove_dir(model_dir)
 
         ################
         # RF Regression
 
         # Creation fake model
         remove_dir(model_dir)
         model = model_rf_regressor.ModelRFRegressor(model_dir=model_dir, model_name=model_name)
         model.fit(x_train_1, y_train_regression)
         model.save()
 
         with self.assertRaises(ValueError):
             pred, proba = utils_models.predict_with_proba(x_test_1, model)
+        with self.assertRaises(ValueError):
+            pred, proba = utils_models.predict_with_proba(x_test_1, model, alternative_version=True)
 
         remove_dir(model_dir)
 
 
     def test12_search_hp_cv(self):
         '''Test of the function {{package_name}}.models_training.utils_models.search_hp_cv'''
         # Definition of the variables for the nominal case
```

### Comparing `gabarit-1.3.1/gabarit/template_vision/default_config.ini` & `gabarit-1.3.2/gabarit/template_vision/default_config.ini`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/generate_vision_project.py` & `gabarit-1.3.2/gabarit/template_vision/generate_vision_project.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/Makefile` & `gabarit-1.3.2/gabarit/template_vision/vision_project/Makefile`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/README.md` & `gabarit-1.3.2/gabarit/template_vision/vision_project/README.md`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/nose_setup_coverage.cfg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/nose_setup_coverage.cfg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/__init__.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/__init__.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/__init__.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_classifier.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_cnn_classifier.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_cnn_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_transfer_learning_classifier.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/classifiers/model_transfer_learning_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/model_class.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/model_class.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/model_keras.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/model_keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 /!\\ OOM errors can happen really quickly (depends on the dataset size)
                 /!\\ Data augmentation impossible if `in_memory` is set to True
             data_augmentation_params (dict): Dictionnary of parameters to be used with the data augmentation
                 cf. https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/image/ImageDataGenerator
                 /!\\ Not used if `in_memory` is set to True
             nb_train_generator_images_to_save (int): If > 0, save some input generated images
                 If helps with to understand what goes in your NN
-            keras_params (dict): Parameters used by keras models.
+            keras_params (dict): Parameters used by Keras models.
                 e.g. learning_rate, nb_lstm_units, etc...
                 The purpose of this dictionary is for the user to use it as they wants in the _get_model function
                 This parameter was initially added in order to do an hyperparameters search
         Raises:
             ValueError: If `in_memory` is set to True and `data_augmentation_params` is not empty
         '''
         # TODO: learning rate should be an attribute !
@@ -726,15 +726,15 @@
                 plt.plot(fit_history.history[metric])
                 plt.plot(fit_history.history[f'val_{metric}'])
                 plt.title(f"Model {title}")
                 plt.ylabel(title)
                 plt.xlabel('Epoch')
                 plt.legend(['Train', 'Validation'], loc='upper left')
                 # Save
-                filename == f"{filename}.jpeg"
+                filename = f"{filename}.jpeg"
                 plt.savefig(os.path.join(plots_path, filename))
 
                 # Close figures
                 plt.close('all')
 
     def _save_model_png(self, model) -> None:
         '''Tries to save the structure of the model in png format
```

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/__init__.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_detectron_faster_rcnn.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_detectron_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_keras_faster_rcnn.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_keras_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_object_detector.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/model_object_detector.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_faster_rcnn.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_object_detectors.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/object_detectors/utils_object_detectors.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/utils_deep_keras.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/utils_deep_keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-## Utils - tools-functions for deep_learning keras models
+## Utils - tools-functions for deep_learning Keras models
 # Copyright (C) <2018-2022>  <Agence Data Services, DSI Pôle Emploi>
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/models_training/utils_models.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/models_training/utils_models.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/monitoring/__init__.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/monitoring/mlflow_logger.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/monitoring/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/monitoring/model_explainer.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/monitoring/model_explainer.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/preprocessing/__init__.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/preprocessing/manage_white_borders.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/preprocessing/manage_white_borders.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/preprocessing/preprocess.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name/utils.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name/utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/post-checkout` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/post-checkout`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-commit` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-commit`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-push` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/git_hooks/pre-push`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-ressources/robot.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-ressources/robot.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/1_preprocess_data.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/1_preprocess_data.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/2_training_classifier.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/2_training_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/2_training_object_detector.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/2_training_object_detector.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/3_predict.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/3_predict.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/4_demonstrator.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/4_demonstrator.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/utils/0_create_samples.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/utils/0_create_samples.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/utils/0_reload_model.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/utils/0_reload_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     The idea here is to reload a model that was trained on another package version.
     This is done be reusing 'standalone' files.
 
     Args:
         model_dir (str): Name of the model to reload (not a path, just the directory name)
     Kwargs:
         config_file (str): Name of the configuration file
-        weights_file (str): Neural Network weights file name (keras models)
+        weights_file (str): Neural Network weights file name (Keras models)
         detectron_file (str): Detectron best model file name (detectron models)
-        preprocess_input_file (str): Model's internal preprocessing file (keras models)
+        preprocess_input_file (str): Model's internal preprocessing file (Keras models)
     Raises:
         FileNotFoundError: If model can't be found
         FileNotFoundError: If model's configuration does not exist
         ValueError: If the model's type is invalid
     '''
     logger.info(f"Reloading a model ...")
 
@@ -134,13 +134,13 @@
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     # model_X should be the model's directory name: e.g. model_preprocess_pipeline_svm_2019_12_05-12_57_18
     parser.add_argument('-m', '--model_dir', required=True, help="Name of the model to reload (not a path, just the directory name)")
     parser.add_argument('-c', '--config_file', default='configurations.json', help="Name of the configuration file")
-    parser.add_argument('-w', '--weights_file', default='best.hdf5', help="Neural Network weights file name (keras models)")
+    parser.add_argument('-w', '--weights_file', default='best.hdf5', help="Neural Network weights file name (Keras models)")
     parser.add_argument('-d', '--detectron_file', default='best.pth', help="Detectron best model file name (detectron models)")
-    parser.add_argument('-p', '--preprocess_input_file', default='preprocess_input.pkl', help="Model's internal preprocessing file (keras models)")
+    parser.add_argument('-p', '--preprocess_input_file', default='preprocess_input.pkl', help="Model's internal preprocessing file (Keras models)")
     args = parser.parse_args()
     main(model_dir=args.model_dir, config_file=args.config_file, weights_file=args.weights_file,
          detectron_file=args.detectron_file, preprocess_input_file=args.preprocess_input_file)
```

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-scripts/utils/0_split_train_valid_test.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-scripts/utils/0_split_train_valid_test.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/answers.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/answers.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/utils.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/verify.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_exercices/verify.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_vision.ipynb` & `gabarit-1.3.2/gabarit/template_vision/vision_project/package_name-tutorials/tutorial_vision.ipynb`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/requirements.txt` & `gabarit-1.3.2/gabarit/template_vision/vision_project/requirements.txt`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/setup.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/setup.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/apple_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/apple_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/apple.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/apple.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_1/subfolder/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/birman_Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/bombay_Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_2/shiba_shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/birman/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/bombay/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3/shiba/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/birman/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/bombay/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/bad_test_data_3_v2/shiba/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1/subfolder/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_diff_sep/subfolder/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_no_class/subfolder/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_1_with_preprocess/subfolder/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/birman_Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/bombay_Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2/shiba_shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Birman4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/Bombay3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_no_class/shiba34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/birman_Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/bombay_Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_2_with_preprocess/shiba_shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/birman/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/bombay/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3/shiba/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_1.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_1.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_2.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_2.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_36.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_36.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_4.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/birman/Birman_4.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_1.png` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_1.png`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_10.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_10.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_19.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_19.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_3.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/bombay/Bombay_3.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_15.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_15.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_30.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_30.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_31.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_31.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_34.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/package_name-data/test_data_3_with_preprocess/shiba/shiba_inu_34.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/mixed_22.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/error_fruits/mixed_22.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fake_metrics.json` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fake_metrics.json`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/apple_76.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/apple_76.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/banana_76.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/banana_76.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/mixed_22.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/mixed_22.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/orange_77.jpg` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_data_object_detection/fruits/orange_77.jpg`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_data/test_map.json` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_data/test_map.json`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_manage_white_borders.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_manage_white_borders.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_mlflow_logger.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_class.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_class.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_classifier.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_cnn_classifier.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_cnn_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_detectron_faster_rcnn.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_detectron_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_explainer.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_explainer.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_keras.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,15 +844,41 @@
         # Nominal case
         model = ModelKeras(model_dir=model_dir)
         self.assertEqual(model._get_learning_rate_scheduler(), None)
 
         # Clean
         remove_dir(model_dir)
 
-    def test09_model_keras_save(self):
+    def test09_model_keras_plot_metrics_and_loss(self):
+        '''Test of the method _plot_metrics_and_loss of {{package_name}}.models_training.model_keras.ModelKeras'''
+
+        model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
+        remove_dir(model_dir)
+
+        # Nominal case
+        model = ModelKeras(model_dir=model_dir, embedding_name='fake_embedding.pkl')
+
+        class FitHistory(object):
+
+            def __init__(self):
+                self.history = {}
+                for metric in ['acc', 'loss', 'categorical_accuracy', 'f1', 'precision', 'recall']:
+                    self.history[metric] = [0.1, 0.2, 0.3, 0.5, 0.4]
+                    self.history[f'val_{metric}'] = [0.05, 0.1, 0.2, 0.4, 0.4]
+
+        fit_history = FitHistory()
+        model._plot_metrics_and_loss(fit_history)
+        plots_path = os.path.join(model.model_dir, 'plots')
+        for filename in ['accuracy', 'loss', 'categorical_accuracy', 'f1_score', 'precision', 'recall']:
+            self.assertTrue(os.path.exists(os.path.join(plots_path, f"{filename}.jpeg")))
+
+        # Clean
+        remove_dir(model_dir)
+
+    def test10_model_keras_save(self):
         '''Test of the method save of {{package_name}}.models_training.model_keras.ModelKeras'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Nominal case
         model = ModelKeras(model_dir=model_dir)
@@ -937,15 +963,15 @@
         self.assertTrue('_get_model' in configs.keys())
         self.assertTrue('_get_learning_rate_scheduler' in configs.keys())
         self.assertTrue('custom_objects' in configs.keys())
         self.assertTrue('list_classes' not in configs.keys()) # not in because we do not use the Classifier mixin
         self.assertTrue('dict_classes' not in configs.keys()) # not in because we do not use the Classifier mixin
         remove_dir(model_dir)
 
-    def test10_model_keras_reload_model(self):
+    def test11_model_keras_reload_model(self):
         '''Test of the method reload_model of {{package_name}}.models_training.model_keras.ModelKeras'''
 
         model_dir = os.path.join(os.getcwd(), 'model_test_123456789')
         remove_dir(model_dir)
 
         # Set vars
         data_path = os.path.join(os.getcwd(), 'test_data', '{{package_name}}-data', 'test_data_1')
```

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_keras_faster_rcnn.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_keras_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_object_detector.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_object_detector.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_model_transfer_learning_classifier.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_model_transfer_learning_classifier.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_preprocess.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils_faster_rcnn.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils_models.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils_models.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit/template_vision/vision_project/tests/test_utils_object_detector.py` & `gabarit-1.3.2/gabarit/template_vision/vision_project/tests/test_utils_object_detector.py`

 * *Files identical despite different names*

### Comparing `gabarit-1.3.1/gabarit.egg-info/PKG-INFO` & `gabarit-1.3.2/gabarit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gabarit
-Version: 1.3.1
+Version: 1.3.2
 Summary: Kickstart your AI project as code
 Home-page: https://github.com/OSS-Pole-Emploi/gabarit
 Author: Agence Data Services PE Nantes
 Author-email: contactadsaiframeworks.00619@pole-emploi.fr
 License: AGPL-3.0
 Description: [![pypi badge](https://img.shields.io/pypi/v/gabarit.svg)](https://pypi.python.org/pypi/gabarit)
         ![NLP tests](https://github.com/OSS-Pole-Emploi/gabarit/actions/workflows/nlp_build_tests.yaml/badge.svg)
```

### Comparing `gabarit-1.3.1/gabarit.egg-info/SOURCES.txt` & `gabarit-1.3.2/gabarit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 gabarit.egg-info/top_level.txt
 gabarit/template_api/__init__.py
 gabarit/template_api/generate_api_project.py
 gabarit/template_api/api_project/.coveragerc
 gabarit/template_api/api_project/.dockerignore
 gabarit/template_api/api_project/.env
 gabarit/template_api/api_project/.gitignore
-gabarit/template_api/api_project/Dockerfile.svc
+gabarit/template_api/api_project/Dockerfile
 gabarit/template_api/api_project/README.md
 gabarit/template_api/api_project/launch.sh
 gabarit/template_api/api_project/makefile
 gabarit/template_api/api_project/pyproject.toml
 gabarit/template_api/api_project/setup.py
 gabarit/template_api/api_project/package_name/__init__.py
 gabarit/template_api/api_project/package_name/application.py
```

### Comparing `gabarit-1.3.1/setup.py` & `gabarit-1.3.2/setup.py`

 * *Files identical despite different names*

