# Comparing `tmp/giskard-2.0.0b5.tar.gz` & `tmp/giskard-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.0.0b5.tar", last modified: Mon Jun 12 13:00:47 2023, max compression
+gzip compressed data, was "giskard-2.0.0b6.tar", last modified: Mon Jun 12 17:18:25 2023, max compression
```

## Comparing `giskard-2.0.0b5.tar` & `giskard-2.0.0b6.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.358250 giskard-2.0.0b5/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 13:00:47.358371 giskard-2.0.0b5/PKG-INFO
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-12 12:56:38.000000 giskard-2.0.0b5/README.md
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.317499 giskard-2.0.0b5/giskard/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1737 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/cli.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/cli_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.327101 giskard-2.0.0b5/giskard/client/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/client/dtos.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/client/giskard_client.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/client/io_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/client/project.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b5/giskard/client/python_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.327664 giskard-2.0.0b5/giskard/commands/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15997 2023-06-12 12:48:22.000000 giskard-2.0.0b5/giskard/commands/cli_server.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7206 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/commands/cli_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.328786 giskard-2.0.0b5/giskard/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/core/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/core.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/dataset_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/errors.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/model_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/suite.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/validation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.328961 giskard-2.0.0b5/giskard/datasets/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/datasets/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.329125 giskard-2.0.0b5/giskard/datasets/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.330569 giskard-2.0.0b5/giskard/datasets/metadata/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/datasets/metadata/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.330938 giskard-2.0.0b5/giskard/demo/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3059 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/demo/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/demo/titanic.csv
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.331483 giskard-2.0.0b5/giskard/ml_worker/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.332498 giskard-2.0.0b5/giskard/ml_worker/bridge/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/service_messages.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.332862 giskard-2.0.0b5/giskard/ml_worker/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/core/log_listener.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/core/savable.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.333385 giskard-2.0.0b5/giskard/ml_worker/exceptions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/exceptions/giskard_exception.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.333757 giskard-2.0.0b5/giskard/ml_worker/generated/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.333980 giskard-2.0.0b5/giskard/ml_worker/server/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/server/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/server/ml_worker_service.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.335008 giskard-2.0.0b5/giskard/ml_worker/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b5/giskard/ml_worker/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.335639 giskard-2.0.0b5/giskard/ml_worker/testing/functions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/functions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/functions/slicing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/functions/transformation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.336881 giskard-2.0.0b5/giskard/ml_worker/testing/registry/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/giskard_test.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/slicing_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/transformation_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/udf_repository.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/test_result.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.337784 giskard-2.0.0b5/giskard/ml_worker/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/ml_worker/utils/file_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/ml_worker/utils/logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/utils/network.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/utils/request_interceptor.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.338661 giskard-2.0.0b5/giskard/models/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/_precooked.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.338878 giskard-2.0.0b5/giskard/models/automodel/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9181 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/automodel/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339069 giskard-2.0.0b5/giskard/models/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339469 giskard-2.0.0b5/giskard/models/cache/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/cache/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/cache/cache.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339655 giskard-2.0.0b5/giskard/models/catboost/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/catboost/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339954 giskard-2.0.0b5/giskard/models/function/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/function/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340146 giskard-2.0.0b5/giskard/models/huggingface/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/huggingface/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340336 giskard-2.0.0b5/giskard/models/langchain/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/langchain/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/model_explanation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340499 giskard-2.0.0b5/giskard/models/pytorch/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/pytorch/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340671 giskard-2.0.0b5/giskard/models/sklearn/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/sklearn/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340916 giskard-2.0.0b5/giskard/models/tensorflow/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/tensorflow/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/path_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.342390 giskard-2.0.0b5/giskard/scanner/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.342951 giskard-2.0.0b5/giskard/scanner/calibration/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/calibration/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.343264 giskard-2.0.0b5/giskard/scanner/common/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/common/examples.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/common/loss_based_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.343416 giskard-2.0.0b5/giskard/scanner/data_leakage/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/issues.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.343713 giskard-2.0.0b5/giskard/scanner/llm/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/llm/toxicity_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/llm/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/logger.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.344341 giskard-2.0.0b5/giskard/scanner/performance/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/performance/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/performance/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/performance/metrics.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/result.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.346629 giskard-2.0.0b5/giskard/scanner/robustness/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/robustness/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/scanner.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.346897 giskard-2.0.0b5/giskard/scanner/stochasticity/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.348157 giskard-2.0.0b5/giskard/scanner/templates/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-12 12:50:19.000000 giskard-2.0.0b5/giskard/scanner/templates/_code_snippet.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.349478 giskard-2.0.0b5/giskard/scanner/templates/_issues/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/data_leakage.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/default.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/llm_toxicity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/overconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/performance.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/robustness.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/stochasticity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/underconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues_table.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_main_content.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_tab_header.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-12 11:29:06.000000 giskard-2.0.0b5/giskard/scanner/templates/base.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/scan_results.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.350200 giskard-2.0.0b5/giskard/scanner/templates/static/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/templates/static/external.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/static/style.css
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.350561 giskard-2.0.0b5/giskard/scanner/visualization/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/visualization/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/visualization/custom_jinja.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/settings.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.352420 giskard-2.0.0b5/giskard/slicing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/base.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/category_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/opt_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/slicing/slice.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/slicing/stop_words.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/slicing/text_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/slicing/tree_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.352599 giskard-2.0.0b5/giskard/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.353674 giskard-2.0.0b5/giskard/testing/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/testing/tests/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.354320 giskard-2.0.0b5/giskard/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6009 2023-06-12 11:29:06.000000 giskard-2.0.0b5/giskard/utils/analytics_collector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/utils/display.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/utils/environment_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.319990 giskard-2.0.0b5/giskard.egg-info/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/PKG-INFO
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/SOURCES.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/dependency_links.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/entry_points.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/requires.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/top_level.txt
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7425 2023-06-12 12:53:45.000000 giskard-2.0.0b5/pyproject.toml
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-12 13:00:47.358686 giskard-2.0.0b5/setup.cfg
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-07 15:34:18.000000 giskard-2.0.0b5/setup.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.357905 giskard-2.0.0b5/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_custom_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_data_drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_data_processing_pipeline.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_dataset.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b5/tests/test_logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_metamorphic_direction.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_metamorphic_invariance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_model_auto_inference.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b5/tests/test_model_explanation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b5/tests/test_model_postprocess.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_programmatic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_project_uploads.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_statistical.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_upload.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-12 11:29:06.000000 giskard-2.0.0b5/tests/test_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.227971 giskard-2.0.0b6/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 17:18:25.228067 giskard-2.0.0b6/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-12 14:14:57.000000 giskard-2.0.0b6/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.197521 giskard-2.0.0b6/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1836 2023-06-12 16:43:55.000000 giskard-2.0.0b6/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.199303 giskard-2.0.0b6/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b6/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.199886 giskard-2.0.0b6/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15997 2023-06-12 16:24:17.000000 giskard-2.0.0b6/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7206 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.201028 giskard-2.0.0b6/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.201186 giskard-2.0.0b6/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.201341 giskard-2.0.0b6/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26225 2023-06-12 16:43:48.000000 giskard-2.0.0b6/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.202617 giskard-2.0.0b6/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.202990 giskard-2.0.0b6/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3059 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/demo/titanic.csv
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.203603 giskard-2.0.0b6/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.204477 giskard-2.0.0b6/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.204837 giskard-2.0.0b6/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.205360 giskard-2.0.0b6/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.205717 giskard-2.0.0b6/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.205982 giskard-2.0.0b6/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.206906 giskard-2.0.0b6/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b6/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.207517 giskard-2.0.0b6/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.208655 giskard-2.0.0b6/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.209397 giskard-2.0.0b6/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.209915 giskard-2.0.0b6/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210047 giskard-2.0.0b6/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9234 2023-06-12 16:43:52.000000 giskard-2.0.0b6/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210260 giskard-2.0.0b6/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210585 giskard-2.0.0b6/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210714 giskard-2.0.0b6/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210953 giskard-2.0.0b6/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211080 giskard-2.0.0b6/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211211 giskard-2.0.0b6/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211339 giskard-2.0.0b6/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211472 giskard-2.0.0b6/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211599 giskard-2.0.0b6/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.212712 giskard-2.0.0b6/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213295 giskard-2.0.0b6/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213547 giskard-2.0.0b6/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213683 giskard-2.0.0b6/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213978 giskard-2.0.0b6/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.214587 giskard-2.0.0b6/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.216854 giskard-2.0.0b6/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.217063 giskard-2.0.0b6/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.218262 giskard-2.0.0b6/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-12 14:14:57.000000 giskard-2.0.0b6/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.219360 giskard-2.0.0b6/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-12 11:29:06.000000 giskard-2.0.0b6/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.219990 giskard-2.0.0b6/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.220442 giskard-2.0.0b6/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.222370 giskard-2.0.0b6/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.222600 giskard-2.0.0b6/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.223472 giskard-2.0.0b6/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.224172 giskard-2.0.0b6/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7152 2023-06-12 16:45:35.000000 giskard-2.0.0b6/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.198359 giskard-2.0.0b6/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7425 2023-06-12 16:48:36.000000 giskard-2.0.0b6/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-12 17:18:25.228306 giskard-2.0.0b6/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-07 15:34:18.000000 giskard-2.0.0b6/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.227763 giskard-2.0.0b6/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b6/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b6/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b6/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-12 16:46:51.000000 giskard-2.0.0b6/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-12 11:29:06.000000 giskard-2.0.0b6/tests/test_utils.py
```

### Comparing `giskard-2.0.0b5/PKG-INFO` & `giskard-2.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b5 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b6 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b5/README.md` & `giskard-2.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/__init__.py` & `giskard-2.0.0b6/giskard/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,42 +15,45 @@
 from giskard.ml_worker.testing.registry.transformation_function import transformation_function
 from giskard.ml_worker.testing.test_result import TestResult
 from giskard.ml_worker.utils.logging import configure_logging
 from giskard.models.automodel import Model
 from . import demo
 from .ml_worker.utils.network import check_latest_giskard_version
 from .scanner import scan
+from .utils.analytics_collector import analytics
 
 configure_logging()
 if sys.version_info >= (3, 8):
     from importlib import metadata as importlib_metadata
 else:
     import importlib_metadata
 
+
 def get_version() -> str:
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
         return "unknown"
 
 
 __version__: str = get_version()
 
 check_latest_giskard_version()
+analytics.track("Initialized giskard library")
 
 __all__ = [
-    'SingleTestResult',
-    'Project',
-    'Dataset',
-    'GiskardClient',
-    'test',
-    'Model',
-    'Suite',
-    'slicing_function',
-    'transformation_function',
-    'SuiteInput',
-    'SlicingFunction',
-    'scan',
-    'TestResult',
-    'GiskardTest',
-    "demo"
-]
+    "SingleTestResult",
+    "Project",
+    "Dataset",
+    "GiskardClient",
+    "test",
+    "Model",
+    "Suite",
+    "slicing_function",
+    "transformation_function",
+    "SuiteInput",
+    "SlicingFunction",
+    "scan",
+    "TestResult",
+    "GiskardTest",
+    "demo",
+]
```

### Comparing `giskard-2.0.0b5/giskard/cli.py` & `giskard-2.0.0b6/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/cli_utils.py` & `giskard-2.0.0b6/giskard/cli_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/client/giskard_client.py` & `giskard-2.0.0b6/giskard/client/giskard_client.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/client/io_utils.py` & `giskard-2.0.0b6/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/client/project.py` & `giskard-2.0.0b6/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/client/python_utils.py` & `giskard-2.0.0b6/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/commands/cli_server.py` & `giskard-2.0.0b6/giskard/commands/cli_server.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/commands/cli_worker.py` & `giskard-2.0.0b6/giskard/commands/cli_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/core/core.py` & `giskard-2.0.0b6/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/core/dataset_validation.py` & `giskard-2.0.0b6/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/core/errors.py` & `giskard-2.0.0b6/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/core/model_validation.py` & `giskard-2.0.0b6/giskard/core/model_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/core/suite.py` & `giskard-2.0.0b6/giskard/core/suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/core/validation.py` & `giskard-2.0.0b6/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/datasets/__init__.py` & `giskard-2.0.0b6/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/datasets/base/__init__.py` & `giskard-2.0.0b6/giskard/datasets/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             validate_column_categorization(self)
             validate_numeric_columns(self)
 
         self.number_of_rows = len(self.df.index)
         self.category_features = {
             column: list(map(lambda x: str(x), self.df[column].dropna().unique()))
             for column, column_type in self.column_types.items()
-            if column_type == 'category'
+            if column_type == "category"
         }
 
         self.data_processor = DataProcessor()
 
         logger.info("Your 'pandas.DataFrame' is successfully wrapped by Giskard's 'Dataset' wrapper class.")
 
     def add_slicing_function(self, slicing_function: SlicingFunction):
@@ -220,15 +220,15 @@
         self.data_processor.add_step(transformation_function)
         return self
 
     @cached_property
     def row_hashes(self):
         return pandas.Series(
             map(
-                lambda row: xxh3_128_hexdigest(f"{', '.join(map(lambda x: repr(x), row))}".encode('utf-8')),
+                lambda row: xxh3_128_hexdigest(f"{', '.join(map(lambda x: repr(x), row))}".encode("utf-8")),
                 self.df.values,
             ),
             index=self.df.index,
         )
 
     @configured_validate_arguments
     def slice(
@@ -259,17 +259,18 @@
         Notes:
             Raises TypeError: If `slicing_function` is not a callable or a `SlicingFunction` object.
         """
         if inspect.isfunction(slicing_function):
             slicing_function = SlicingFunction(slicing_function, row_level=row_level, cell_level=cell_level)
 
         if slicing_function.cell_level and column_name is not None:
-            slicing_function = slicing_function(column_name=column_name,
-                                                **{key: value for key, value in slicing_function.params.items() if
-                                                   key != 'column_name'})
+            slicing_function = slicing_function(
+                column_name=column_name,
+                **{key: value for key, value in slicing_function.params.items() if key != "column_name"},
+            )
 
         return self.data_processor.add_step(slicing_function).apply(self, apply_only_last=True)
 
     @configured_validate_arguments
     def transform(
         self,
         transformation_function: Union[TransformationFunction, TransformationFunctionType],
@@ -300,58 +301,59 @@
 
         if inspect.isfunction(transformation_function):
             transformation_function = TransformationFunction(
                 transformation_function, row_level=row_level, cell_level=cell_level
             )
 
         if transformation_function.cell_level and column_name is not None:
-            transformation_function = transformation_function(column_name=column_name,
-                                                              **{key: value for key, value in
-                                                                 transformation_function.params.items() if
-                                                                 key != 'column_name'})
+            transformation_function = transformation_function(
+                column_name=column_name,
+                **{key: value for key, value in transformation_function.params.items() if key != "column_name"},
+            )
 
         assert (
-            not transformation_function.cell_level or 'column_name' in transformation_function.params
+            not transformation_function.cell_level or "column_name" in transformation_function.params
         ), "column_name should be provided for TransformationFunction at cell level"
         return self.data_processor.add_step(transformation_function).apply(self, apply_only_last=True)
 
     def process(self):
         """
         Process the dataset by applying all the transformation and slicing functions in the defined order.
 
         Returns:
             The processed dataset after applying all the transformation and slicing functions.
         """
         return self.data_processor.apply(self)
 
-    def _infer_column_types(self, column_types: Optional[Dict[str, str]], cat_columns: Optional[List[str]],
-                            validation: bool = True):
+    def _infer_column_types(
+        self, column_types: Optional[Dict[str, str]], cat_columns: Optional[List[str]], validation: bool = True
+    ):
         """
-       This function infers the column types of a given DataFrame based on the number of unique values and column data types. It takes into account the provided column types and categorical columns. The inferred types can be 'text', 'numeric', or 'category'. The function also applies a logarithmic rule to determine the category threshold.
+        This function infers the column types of a given DataFrame based on the number of unique values and column data types. It takes into account the provided column types and categorical columns. The inferred types can be 'text', 'numeric', or 'category'. The function also applies a logarithmic rule to determine the category threshold.
 
-       Here's a summary of the function's logic:
+        Here's a summary of the function's logic:
 
-       1. If no column types are provided, initialize an empty dictionary.
-       2. Determine the columns in the DataFrame, excluding the target column if it exists.
-       3. If categorical columns are specified, prioritize them over the provided column types and mark them as 'category'.
-       4. Check for any unknown columns in the provided column types and remove them from the dictionary.
-       5. If there are no missing columns, remove the target column (if present) from the column types dictionary.
-       6. Calculate the number of unique values in each missing column.
-       7. For each missing column:
-
-          - If the number of unique values is less than or equal to the category threshold, categorize it as 'category'.
-          - Otherwise, attempt to convert the column to numeric using `pd.to_numeric` and categorize it as 'numeric'.
-          - If the column does not have the expected numeric data type and validation is enabled, issue a warning message.
-          - If conversion to numeric raises a ValueError, categorize the column as 'text'.
-       8. Return the column types dictionary.
+        1. If no column types are provided, initialize an empty dictionary.
+        2. Determine the columns in the DataFrame, excluding the target column if it exists.
+        3. If categorical columns are specified, prioritize them over the provided column types and mark them as 'category'.
+        4. Check for any unknown columns in the provided column types and remove them from the dictionary.
+        5. If there are no missing columns, remove the target column (if present) from the column types dictionary.
+        6. Calculate the number of unique values in each missing column.
+        7. For each missing column:
+
+           - If the number of unique values is less than or equal to the category threshold, categorize it as 'category'.
+           - Otherwise, attempt to convert the column to numeric using `pd.to_numeric` and categorize it as 'numeric'.
+           - If the column does not have the expected numeric data type and validation is enabled, issue a warning message.
+           - If conversion to numeric raises a ValueError, categorize the column as 'text'.
+        8. Return the column types dictionary.
 
-       The logarithmic rule is used to calculate the category threshold. The formula is: `category_threshold = round(np.log10(len(self.df))) if len(self.df) >= 100 else 2`. This means that if the length of the DataFrame is greater than or equal to 100, the category threshold is set to the rounded value of the base-10 logarithm of the DataFrame length. Otherwise, the category threshold is set to 2. The logarithmic rule helps in dynamically adjusting the category threshold based on the size of the DataFrame.
+        The logarithmic rule is used to calculate the category threshold. The formula is: `category_threshold = round(np.log10(len(self.df))) if len(self.df) >= 100 else 2`. This means that if the length of the DataFrame is greater than or equal to 100, the category threshold is set to the rounded value of the base-10 logarithm of the DataFrame length. Otherwise, the category threshold is set to 2. The logarithmic rule helps in dynamically adjusting the category threshold based on the size of the DataFrame.
 
-       Returns:
-          dict: A dictionary that maps column names to their inferred types, one of 'text', 'numeric', or 'category'.
+        Returns:
+           dict: A dictionary that maps column names to their inferred types, one of 'text', 'numeric', or 'category'.
         """
         if not column_types:
             column_types = {}
         df_columns = set([col for col in self.columns if col != self.target]) if self.target else set(self.columns)
 
         # priority of cat_columns over column_types (for categorical columns)
         if cat_columns:
@@ -453,15 +455,15 @@
 
     @staticmethod
     def cast_column_to_dtypes(df, column_dtypes):
         current_types = df.dtypes.apply(lambda x: x.name).to_dict()
         logger.info(f"Casting dataframe columns from {current_types} to {column_dtypes}")
         if column_dtypes:
             try:
-                df = df.astype(column_dtypes, errors='ignore')
+                df = df.astype(column_dtypes, errors="ignore")
             except Exception as e:
                 raise ValueError("Failed to apply column types to dataset") from e
         return df
 
     @classmethod
     def load(cls, local_path: str):
         with open(local_path, "rb") as ds_stream:
```

### Comparing `giskard-2.0.0b5/giskard/datasets/metadata/indexing.py` & `giskard-2.0.0b6/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/datasets/metadata/registry.py` & `giskard-2.0.0b6/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.0.0b6/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/demo/__init__.py` & `giskard-2.0.0b6/giskard/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/demo/titanic.csv` & `giskard-2.0.0b6/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.0.0b6/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/bridge/ml_worker_bridge.py` & `giskard-2.0.0b6/giskard/ml_worker/bridge/ml_worker_bridge.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/core/log_listener.py` & `giskard-2.0.0b6/giskard/ml_worker/core/log_listener.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/core/savable.py` & `giskard-2.0.0b6/giskard/ml_worker/core/savable.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/ml_worker.py` & `giskard-2.0.0b6/giskard/ml_worker/ml_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/server/ml_worker_service.py` & `giskard-2.0.0b6/giskard/ml_worker/server/ml_worker_service.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/functions/slicing.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/functions/transformation.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators_utils.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/registry/giskard_test.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/registry/registry.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/registry/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/registry/slicing_function.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/registry/transformation_function.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/registry/udf_repository.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/registry/udf_repository.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/test_result.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/test_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/testing/utils.py` & `giskard-2.0.0b6/giskard/ml_worker/testing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b6/giskard/ml_worker/utils/logging.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/utils/network.py` & `giskard-2.0.0b6/giskard/ml_worker/utils/network.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/ml_worker/utils/request_interceptor.py` & `giskard-2.0.0b6/giskard/ml_worker/utils/request_interceptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/__init__.py` & `giskard-2.0.0b6/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/_precooked.py` & `giskard-2.0.0b6/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/automodel/__init__.py` & `giskard-2.0.0b6/giskard/models/automodel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,85 +1,85 @@
+import logging
 from abc import ABC
 from typing import Callable, Optional, Iterable, Any
 
 import pandas as pd
-import logging
 
 from giskard.core.core import ModelType
 from giskard.models import infer_giskard_cls
 from giskard.models.base import CloudpickleBasedModel
 from giskard.models.function import PredictionFunctionModel
 
 logger = logging.getLogger(__name__)
 
 
 class Model(CloudpickleBasedModel, ABC):
     """
-   A wrapper class that automatically infers the ML library of the ``model`` argument and provides suitable
-   serialization methods (provided by ``save_model`` and ``load_model`` methods).
+    A wrapper class that automatically infers the ML library of the ``model`` argument and provides suitable
+    serialization methods (provided by ``save_model`` and ``load_model`` methods).
 
-   Pre-defined serialization and prediction methods cover the ``sklearn``, ``catboost``, ``pytorch``, ``tensorflow``,
-   ``huggingface`` and ``langchain`` libraries. If none of these libraries are detected, ``cloudpickle`` is used as the
-   default serialization method, and the user is prompted to provide their own prediction method.
-
-   Two ways to wrap your model:
-
-   1. Wrap a prediction function that contains all your data preprocessing steps. It takes as input the raw pandas
-      dataframe and returns the probabilities for each classification label or predictions for your regression task.
-      Make sure that:
-
-      - ``prediction_function`` encapsulates all the data preprocessing steps (categorical encoding, numerical scaling,
-        etc.).
-      - ``prediction_function(df[feature_names])`` does not return an error message.
-
-   2. Wrap a model object. This is recommended if your model is not
-      serializable by ``cloudpickle`` (e.g., TensorFlow models). This requires:
-
-      - Mandatory: Overriding the ``model_predict`` method, which should take as input the raw pandas dataframe and
-        return the probabilities for each classification label (classification), predictions (regression or text generation).
-      - Optional: If none of the pre-defined serialization methods apply, ``cloudpickle`` is used as the default
-        serialization method. If this fails, the user is asked to override the ``save_model`` and ``load_model``
-        methods to provide their own serialization of the model object.
-
-   Args:
-       model (Any):
-           Could be any function or ML model. The standard model output required for Giskard is:
-
-           * if classification: an array (nxm) of probabilities corresponding to n data entries
-             (rows of pandas.DataFrame)
-             and m classification_labels. In the case of binary classification, an array of (nx1) probabilities is
-             also accepted.
-             Make sure that the probability provided is for the second label provided in classification_labels.
-           * if regression or text_generation: an array of predictions corresponding to data entries
-             (rows of pandas.DataFrame) and outputs.
-       name (Optional[str]):
-            the name of the model.
-       model_type (ModelType):
-           The type of the model: regression, classification or text_generation.
-       data_preprocessing_function (Optional[Callable[[pd.DataFrame], Any]]):
-           A function that takes a pandas.DataFrame as raw input, applies preprocessing and returns any object
-           that could be directly fed to clf. You can also choose to include your preprocessing inside clf,
-           in which case no need to provide this argument.
-       model_postprocessing_function (Optional[Callable[[Any], Any]]):
-           A function that takes a clf output as input,
-           applies postprocessing and returns an object of the same type and shape as the clf output.
-       feature_names (Optional[Iterable[str]]):
-           list of feature names matching the column names in the data that correspond to the features which the model
-           trained on. By default, feature_names are all the Dataset columns except from target.
-       classification_threshold (float):
-           represents the classification model threshold, for binary
-           classification models.
-       classification_labels (Optional[Iterable[str]]):
-           that represents the classification labels, if model_type is
-           classification. Make sure the labels have the same order as the column output of clf.
-       **kwargs: Additional keyword arguments.
-
-   Returns:
-       Union[CloudpickleBasedModel, SKLearnModel, HuggingFaceModel,
-       CatboostModel, PyTorchModel, TensorFlowModel]: The wrapped Giskard model.
+    Pre-defined serialization and prediction methods cover the ``sklearn``, ``catboost``, ``pytorch``, ``tensorflow``,
+    ``huggingface`` and ``langchain`` libraries. If none of these libraries are detected, ``cloudpickle`` is used as the
+    default serialization method, and the user is prompted to provide their own prediction method.
+
+    Two ways to wrap your model:
+
+    1. Wrap a prediction function that contains all your data preprocessing steps. It takes as input the raw pandas
+       dataframe and returns the probabilities for each classification label or predictions for your regression task.
+       Make sure that:
+
+       - ``prediction_function`` encapsulates all the data preprocessing steps (categorical encoding, numerical scaling,
+         etc.).
+       - ``prediction_function(df[feature_names])`` does not return an error message.
+
+    2. Wrap a model object. This is recommended if your model is not
+       serializable by ``cloudpickle`` (e.g., TensorFlow models). This requires:
+
+       - Mandatory: Overriding the ``model_predict`` method, which should take as input the raw pandas dataframe and
+         return the probabilities for each classification label (classification), predictions (regression or text generation).
+       - Optional: If none of the pre-defined serialization methods apply, ``cloudpickle`` is used as the default
+         serialization method. If this fails, the user is asked to override the ``save_model`` and ``load_model``
+         methods to provide their own serialization of the model object.
+
+    Args:
+        model (Any):
+            Could be any function or ML model. The standard model output required for Giskard is:
+
+            * if classification: an array (nxm) of probabilities corresponding to n data entries
+              (rows of pandas.DataFrame)
+              and m classification_labels. In the case of binary classification, an array of (nx1) probabilities is
+              also accepted.
+              Make sure that the probability provided is for the second label provided in classification_labels.
+            * if regression or text_generation: an array of predictions corresponding to data entries
+              (rows of pandas.DataFrame) and outputs.
+        name (Optional[str]):
+             the name of the model.
+        model_type (ModelType):
+            The type of the model: regression, classification or text_generation.
+        data_preprocessing_function (Optional[Callable[[pd.DataFrame], Any]]):
+            A function that takes a pandas.DataFrame as raw input, applies preprocessing and returns any object
+            that could be directly fed to clf. You can also choose to include your preprocessing inside clf,
+            in which case no need to provide this argument.
+        model_postprocessing_function (Optional[Callable[[Any], Any]]):
+            A function that takes a clf output as input,
+            applies postprocessing and returns an object of the same type and shape as the clf output.
+        feature_names (Optional[Iterable[str]]):
+            list of feature names matching the column names in the data that correspond to the features which the model
+            trained on. By default, feature_names are all the Dataset columns except from target.
+        classification_threshold (float):
+            represents the classification model threshold, for binary
+            classification models.
+        classification_labels (Optional[Iterable[str]]):
+            that represents the classification labels, if model_type is
+            classification. Make sure the labels have the same order as the column output of clf.
+        **kwargs: Additional keyword arguments.
+
+    Returns:
+        Union[CloudpickleBasedModel, SKLearnModel, HuggingFaceModel,
+        CatboostModel, PyTorchModel, TensorFlowModel]: The wrapped Giskard model.
     """
 
     should_save_model_class = True
 
     def __new__(
         cls,
         model: Any,
@@ -113,15 +113,15 @@
                 "\nIf a prediction function is provided, we use cloudpickle to serialize it."
             )
         else:
             giskard_cls = infer_giskard_cls(model)
             # if the Model class is overriden (thus != Model) -> get the methods from the subclass
             # if the Model class is instantiated (thus == Model) -> get the methods from the inferred class
             # if giskard_cls == None -> get the methods from CloudpickleBasedModel
-            is_overriden = cls.__name__ != 'Model'  # TODO: Improve this
+            is_overriden = cls.__name__ != "Model"  # TODO: Improve this
             if is_overriden:
                 if not giskard_cls:
                     giskard_cls = CloudpickleBasedModel
                 # if save_model and load_model are overriden, replace them, if not, these equalities will be identities.
                 possibly_overriden_cls = cls
                 possibly_overriden_cls.save_model = giskard_cls.save_model
                 possibly_overriden_cls.load_model = giskard_cls.load_model
@@ -134,23 +134,23 @@
                     + " is successfully wrapped by Giskard's '"
                     + str(giskard_cls.__name__)
                     + "' wrapper class."
                 )
                 possibly_overriden_cls = giskard_cls
             else:  # possibly_overriden_cls = CloudpickleBasedModel
                 raise NotImplementedError(
-                    'We could not infer your model library. You have two options:'
-                    '\n- Pass a prediction_function to the Model class '
+                    "We could not infer your model library. You have two options:"
+                    "\n- Pass a prediction_function to the Model class "
                     '(we will try to serialize it with "cloudpickle").'
-                    '\n- Extend the Model class and override '
+                    "\n- Extend the Model class and override "
                     'the abstract "model_predict" method. Upon upload to the Giskard server, we will try to serialise'
                     'it with "cloudpickle", if that does not work, we will ask you to override the "save_model" and'
                     '"load_model" with your own serialization methods.'
-                    '\nWe recommend that you follow our documentation page: '
-                    'https://giskard.readthedocs.io/en/latest/getting-started/scan'
+                    "\nWe recommend that you follow our documentation page: "
+                    "https://giskard.readthedocs.io/en/latest/getting-started/scan"
                 )
 
             methods = dict(possibly_overriden_cls.__dict__)
             output_cls = type(possibly_overriden_cls.__name__, (giskard_cls,), methods)
 
             obj = output_cls(
                 model=model,
```

### Comparing `giskard-2.0.0b5/giskard/models/base/__init__.py` & `giskard-2.0.0b6/giskard/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/cache/__init__.py` & `giskard-2.0.0b6/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/cache/cache.py` & `giskard-2.0.0b6/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/catboost/__init__.py` & `giskard-2.0.0b6/giskard/models/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/function/__init__.py` & `giskard-2.0.0b6/giskard/models/function/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/huggingface/__init__.py` & `giskard-2.0.0b6/giskard/models/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/langchain/__init__.py` & `giskard-2.0.0b6/giskard/models/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/model_explanation.py` & `giskard-2.0.0b6/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/pytorch/__init__.py` & `giskard-2.0.0b6/giskard/models/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/sklearn/__init__.py` & `giskard-2.0.0b6/giskard/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/tensorflow/__init__.py` & `giskard-2.0.0b6/giskard/models/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/models/utils.py` & `giskard-2.0.0b6/giskard/models/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/path_utils.py` & `giskard-2.0.0b6/giskard/path_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/__init__.py` & `giskard-2.0.0b6/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/calibration/issues.py` & `giskard-2.0.0b6/giskard/scanner/calibration/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.0.0b6/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.0.0b6/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/common/examples.py` & `giskard-2.0.0b6/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/common/loss_based_detector.py` & `giskard-2.0.0b6/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.0.0b6/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/decorators.py` & `giskard-2.0.0b6/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/issues.py` & `giskard-2.0.0b6/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/llm/toxicity_detector.py` & `giskard-2.0.0b6/giskard/scanner/llm/toxicity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/llm/utils.py` & `giskard-2.0.0b6/giskard/scanner/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/performance/issues.py` & `giskard-2.0.0b6/giskard/scanner/performance/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/performance/metrics.py` & `giskard-2.0.0b6/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.0.0b6/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/registry.py` & `giskard-2.0.0b6/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/result.py` & `giskard-2.0.0b6/giskard/scanner/result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/robustness/base_detector.py` & `giskard-2.0.0b6/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/robustness/entity_swap.py` & `giskard-2.0.0b6/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.0.0b6/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/robustness/issues.py` & `giskard-2.0.0b6/giskard/scanner/robustness/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/robustness/nationalities.json` & `giskard-2.0.0b6/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.0.0b6/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/robustness/text_transformations.py` & `giskard-2.0.0b6/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/scanner.py` & `giskard-2.0.0b6/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.0.0b6/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_code_snippet.html` & `giskard-2.0.0b6/giskard/scanner/templates/_code_snippet.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/data_leakage.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/data_leakage.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/default.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/default.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/llm_toxicity.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/llm_toxicity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/overconfidence.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/overconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/performance.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/performance.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/robustness.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/robustness.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/stochasticity.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/stochasticity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues/underconfidence.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues/underconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_issues_table.html` & `giskard-2.0.0b6/giskard/scanner/templates/_issues_table.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_main_content.html` & `giskard-2.0.0b6/giskard/scanner/templates/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/_tab_header.html` & `giskard-2.0.0b6/giskard/scanner/templates/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/scan_results.html` & `giskard-2.0.0b6/giskard/scanner/templates/scan_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/static/external.js` & `giskard-2.0.0b6/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/static/internal.js` & `giskard-2.0.0b6/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/templates/static/style.css` & `giskard-2.0.0b6/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/scanner/visualization/custom_jinja.py` & `giskard-2.0.0b6/giskard/scanner/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/settings.py` & `giskard-2.0.0b6/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/base.py` & `giskard-2.0.0b6/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/bruteforce_slicer.py` & `giskard-2.0.0b6/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/category_slicer.py` & `giskard-2.0.0b6/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/multiscale_slicer.py` & `giskard-2.0.0b6/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/opt_slicer.py` & `giskard-2.0.0b6/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/slice.py` & `giskard-2.0.0b6/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/stop_words.py` & `giskard-2.0.0b6/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/text_slicer.py` & `giskard-2.0.0b6/giskard/slicing/text_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/tree_slicer.py` & `giskard-2.0.0b6/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/slicing/utils.py` & `giskard-2.0.0b6/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/testing/__init__.py` & `giskard-2.0.0b6/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/testing/tests/drift.py` & `giskard-2.0.0b6/giskard/testing/tests/drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/testing/tests/metamorphic.py` & `giskard-2.0.0b6/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/testing/tests/performance.py` & `giskard-2.0.0b6/giskard/testing/tests/performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/testing/tests/statistic.py` & `giskard-2.0.0b6/giskard/testing/tests/statistic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard/utils/analytics_collector.py` & `giskard-2.0.0b6/giskard/utils/analytics_collector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import getpass
 import hashlib
 import os
 import platform
+import sys
+import threading
+import traceback
 import uuid
 from functools import wraps
 from threading import Lock
 from typing import Dict, Optional
 
 import requests
 from mixpanel import Mixpanel
@@ -23,15 +26,15 @@
     @wraps(f)
     def inner_function(*args, **kwargs):
         try:
             if not settings.disable_analytics:
                 return f(*args, **kwargs)
         except BaseException as e:  # NOSONAR
             try:
-                analytics.track('tracking error', {'error': str(e)})
+                analytics.track("tracking error", {"error": str(e)})
             except BaseException:  # NOSONAR
                 pass
 
     return inner_function
 
 
 def anonymize(message):
@@ -73,14 +76,33 @@
         "dataset_rows": dataset.df.shape[0],
         "dataset_cols": dataset.df.shape[1],
         "dataset_column_types": column_types,
         "dataset_column_dtypes": column_dtypes,
     }
 
 
+def _report_error(e):
+    exc = traceback.TracebackException.from_exception(e)
+    is_giskard_error = False
+
+    for frame in exc.stack:
+        if not is_giskard_error and "giskard" in frame.filename:
+            is_giskard_error = True
+        frame.filename = os.path.relpath(frame.filename)
+    if is_giskard_error:
+        analytics.track(
+            "python error",
+            {
+                "exception": fullname(e),
+                "error message": str(e),
+                "stack": "".join(exc.format()),
+            },
+        )
+
+
 class GiskardAnalyticsCollector:
     lock = Lock()
     ip: Optional[str]
     dev_mp_project_key = "4cca5fabca54f6df41ea500e33076c99"
     prod_mp_project_key = "2c3efacc6c26ffb991a782b476b8c620"
     server_info: Optional[Dict] = None
     mp: Mixpanel
@@ -136,29 +158,30 @@
             self.mp.track(
                 distinct_id=self.distinct_user_id, event_name=event_name, properties=dict(merged_props), meta=meta
             )
 
     def initialize_giskard_version(self):
         if not self.giskard_version:
             import giskard
+
             self.giskard_version = giskard.get_version()
 
     def initialize_user_properties(self):
         if not self.ip:
             self.initialize_geo()
             self.mp.people_set(
                 self.distinct_user_id,
                 {
                     "$name": "",
                     "arch": platform.machine(),
                     "$os": platform.system(),
                     "os-full": platform.platform(aliased=True),
                 },
                 # only for aggregated stats: city, country, region. IP itself isn't stored
-                meta={'$ip': self.ip},
+                meta={"$ip": self.ip},
             )
 
     @staticmethod
     def machine_based_user_id():
         try:
             return anonymize(str(uuid.getnode()) + getpass.getuser())
         except BaseException:  # noqa NOSONAR
@@ -174,13 +197,32 @@
         IP address itself **isn't stored** by in the telemetry data, see:
         https://docs.mixpanel.com/docs/tracking/how-tos/effective-server#tracking-geolocation
         """
         with GiskardAnalyticsCollector.lock:
             if self.ip:
                 return
             try:
-                self.ip = requests.get('https://api64.ipify.org/?format=json').json().get('ip', 'unknown')
+                self.ip = requests.get("https://api64.ipify.org/?format=json").json().get("ip", "unknown")
             except:  # noqa NOSONAR
                 self.ip = "unknown"
 
 
+def add_exception_hook(original_hook=None):
+    def _exception_hook(type, value, traceback):
+        try:
+            _report_error(value)
+        except BaseException:  # noqa NOSONAR
+            pass
+
+        if original_hook:
+            return original_hook(type, value, traceback)
+        else:
+            return sys.__excepthook__(type, value, traceback)
+
+    return _exception_hook
+
+
+if not settings.disable_analytics:
+    sys.excepthook = add_exception_hook(sys.excepthook)
+    threading.excepthook = add_exception_hook(threading.excepthook)
+
 analytics = GiskardAnalyticsCollector()
```

### Comparing `giskard-2.0.0b5/giskard/utils/environment_detector.py` & `giskard-2.0.0b6/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard.egg-info/PKG-INFO` & `giskard-2.0.0b6/giskard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b5 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b6 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b5/giskard.egg-info/SOURCES.txt` & `giskard-2.0.0b6/giskard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/giskard.egg-info/requires.txt` & `giskard-2.0.0b6/giskard.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/pyproject.toml` & `giskard-2.0.0b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.0.0b5"
+version = "2.0.0b6"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [
     { name = "Giskard AI", email = "hello@giskard.ai" },
 ]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
```

### Comparing `giskard-2.0.0b5/setup.py` & `giskard-2.0.0b6/setup.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_custom_model.py` & `giskard-2.0.0b6/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_data_drift.py` & `giskard-2.0.0b6/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_data_processing_pipeline.py` & `giskard-2.0.0b6/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_dataset.py` & `giskard-2.0.0b6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_metamorphic_direction.py` & `giskard-2.0.0b6/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_metamorphic_invariance.py` & `giskard-2.0.0b6/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_model.py` & `giskard-2.0.0b6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_model_auto_inference.py` & `giskard-2.0.0b6/tests/test_model_auto_inference.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_model_explanation.py` & `giskard-2.0.0b6/tests/test_model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_model_postprocess.py` & `giskard-2.0.0b6/tests/test_model_postprocess.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_performance.py` & `giskard-2.0.0b6/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_programmatic.py` & `giskard-2.0.0b6/tests/test_programmatic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_project_uploads.py` & `giskard-2.0.0b6/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_statistical.py` & `giskard-2.0.0b6/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b5/tests/test_upload.py` & `giskard-2.0.0b6/tests/test_upload.py`

 * *Files identical despite different names*

