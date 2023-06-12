# Comparing `tmp/giskard-2.0.0b4.tar.gz` & `tmp/giskard-2.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.0.0b4.tar", last modified: Wed Jun  7 11:44:00 2023, max compression
+gzip compressed data, was "giskard-2.0.0b5.tar", last modified: Mon Jun 12 13:00:47 2023, max compression
```

## Comparing `giskard-2.0.0b4.tar` & `giskard-2.0.0b5.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.314212 giskard-2.0.0b4/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 11:44:00.314327 giskard-2.0.0b4/PKG-INFO
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8623 2023-06-07 11:37:58.000000 giskard-2.0.0b4/README.md
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.282557 giskard-2.0.0b4/giskard/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1779 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/cli.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/cli_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.284270 giskard-2.0.0b4/giskard/client/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/dtos.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/giskard_client.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/io_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/client/project.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b4/giskard/client/python_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.284823 giskard-2.0.0b4/giskard/commands/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15306 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/commands/cli_server.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7206 2023-06-07 11:36:36.000000 giskard-2.0.0b4/giskard/commands/cli_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.286234 giskard-2.0.0b4/giskard/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/core/core.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/dataset_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/errors.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/core/model_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/suite.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/core/validation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.286393 giskard-2.0.0b4/giskard/datasets/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.286533 giskard-2.0.0b4/giskard/datasets/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.287270 giskard-2.0.0b4/giskard/datasets/metadata/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.287570 giskard-2.0.0b4/giskard/demo/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2931 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/demo/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/demo/titanic.csv
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.287957 giskard-2.0.0b4/giskard/ml_worker/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.288795 giskard-2.0.0b4/giskard/ml_worker/bridge/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/bridge/service_messages.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.289261 giskard-2.0.0b4/giskard/ml_worker/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/core/log_listener.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/core/savable.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.289756 giskard-2.0.0b4/giskard/ml_worker/exceptions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/exceptions/giskard_exception.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.290178 giskard-2.0.0b4/giskard/ml_worker/generated/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.290465 giskard-2.0.0b4/giskard/ml_worker/server/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/server/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/server/ml_worker_service.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.291218 giskard-2.0.0b4/giskard/ml_worker/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b4/giskard/ml_worker/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.291691 giskard-2.0.0b4/giskard/ml_worker/testing/functions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/functions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/testing/functions/slicing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/testing/functions/transformation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.293043 giskard-2.0.0b4/giskard/ml_worker/testing/registry/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/giskard_test.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/slicing_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/transformation_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/registry/udf_repository.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/testing/test_result.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/testing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.294000 giskard-2.0.0b4/giskard/ml_worker/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b4/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/utils/file_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/utils/logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/ml_worker/utils/network.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/ml_worker/utils/request_interceptor.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.294793 giskard-2.0.0b4/giskard/models/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/_precooked.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.294967 giskard-2.0.0b4/giskard/models/automodel/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9181 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/automodel/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.295129 giskard-2.0.0b4/giskard/models/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34228 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.295814 giskard-2.0.0b4/giskard/models/cache/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/cache/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/cache/cache.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.295970 giskard-2.0.0b4/giskard/models/catboost/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/catboost/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296159 giskard-2.0.0b4/giskard/models/function/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/function/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296330 giskard-2.0.0b4/giskard/models/huggingface/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/huggingface/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296486 giskard-2.0.0b4/giskard/models/langchain/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/langchain/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/model_explanation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296667 giskard-2.0.0b4/giskard/models/pytorch/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/pytorch/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.296854 giskard-2.0.0b4/giskard/models/sklearn/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/sklearn/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.297012 giskard-2.0.0b4/giskard/models/tensorflow/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/models/tensorflow/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/models/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/path_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.298492 giskard-2.0.0b4/giskard/scanner/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.299185 giskard-2.0.0b4/giskard/scanner/calibration/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/calibration/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.299575 giskard-2.0.0b4/giskard/scanner/common/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/common/examples.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/common/loss_based_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.299773 giskard-2.0.0b4/giskard/scanner/data_leakage/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/issues.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.300115 giskard-2.0.0b4/giskard/scanner/llm/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/llm/toxicity_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/llm/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/logger.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.300786 giskard-2.0.0b4/giskard/scanner/performance/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/performance/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/performance/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/performance/metrics.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/result.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.302843 giskard-2.0.0b4/giskard/scanner/robustness/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/scanner.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.303115 giskard-2.0.0b4/giskard/scanner/stochasticity/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.304145 giskard-2.0.0b4/giskard/scanner/templates/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      785 2023-06-07 11:37:38.000000 giskard-2.0.0b4/giskard/scanner/templates/_code_snippet.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.305367 giskard-2.0.0b4/giskard/scanner/templates/_issues/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/data_leakage.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/default.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/llm_toxicity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/overconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/performance.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/robustness.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/stochasticity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues/underconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_issues_table.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_main_content.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/_tab_header.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      187 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/base.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/scanner/templates/scan_results.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.306121 giskard-2.0.0b4/giskard/scanner/templates/static/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/static/external.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/templates/static/style.css
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.306384 giskard-2.0.0b4/giskard/scanner/visualization/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/visualization/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/scanner/visualization/custom_jinja.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/settings.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.308207 giskard-2.0.0b4/giskard/slicing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/base.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/category_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/opt_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/slice.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/stop_words.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/text_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/tree_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/slicing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.308393 giskard-2.0.0b4/giskard/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.309943 giskard-2.0.0b4/giskard/testing/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/testing/tests/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.310747 giskard-2.0.0b4/giskard/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5534 2023-06-07 11:12:34.000000 giskard-2.0.0b4/giskard/utils/analytics_collector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/utils/display.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-06 19:53:55.000000 giskard-2.0.0b4/giskard/utils/environment_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.283454 giskard-2.0.0b4/giskard.egg-info/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9939 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/PKG-INFO
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/SOURCES.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/dependency_links.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/entry_points.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/requires.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        8 2023-06-07 11:44:00.000000 giskard-2.0.0b4/giskard.egg-info/top_level.txt
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7375 2023-06-07 11:37:59.000000 giskard-2.0.0b4/pyproject.toml
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-07 11:44:00.314630 giskard-2.0.0b4/setup.cfg
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-06 19:53:55.000000 giskard-2.0.0b4/setup.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 11:44:00.314027 giskard-2.0.0b4/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-07 11:12:34.000000 giskard-2.0.0b4/tests/test_custom_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_data_drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_data_processing_pipeline.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_dataset.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b4/tests/test_logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_metamorphic_direction.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_metamorphic_invariance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-07 11:12:34.000000 giskard-2.0.0b4/tests/test_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_model_auto_inference.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_model_explanation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_model_postprocess.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-07 11:12:34.000000 giskard-2.0.0b4/tests/test_performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-07 11:43:22.000000 giskard-2.0.0b4/tests/test_programmatic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_project_uploads.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_statistical.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_upload.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-06 19:53:55.000000 giskard-2.0.0b4/tests/test_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.358250 giskard-2.0.0b5/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 13:00:47.358371 giskard-2.0.0b5/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-12 12:56:38.000000 giskard-2.0.0b5/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.317499 giskard-2.0.0b5/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1737 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.327101 giskard-2.0.0b5/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b5/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.327664 giskard-2.0.0b5/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15997 2023-06-12 12:48:22.000000 giskard-2.0.0b5/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7206 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.328786 giskard-2.0.0b5/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.328961 giskard-2.0.0b5/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.329125 giskard-2.0.0b5/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26419 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.330569 giskard-2.0.0b5/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.330938 giskard-2.0.0b5/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3059 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/demo/titanic.csv
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.331483 giskard-2.0.0b5/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.332498 giskard-2.0.0b5/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.332862 giskard-2.0.0b5/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.333385 giskard-2.0.0b5/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.333757 giskard-2.0.0b5/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.333980 giskard-2.0.0b5/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.335008 giskard-2.0.0b5/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b5/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.335639 giskard-2.0.0b5/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.336881 giskard-2.0.0b5/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.337784 giskard-2.0.0b5/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b5/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.338661 giskard-2.0.0b5/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.338878 giskard-2.0.0b5/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9181 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339069 giskard-2.0.0b5/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339469 giskard-2.0.0b5/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339655 giskard-2.0.0b5/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.339954 giskard-2.0.0b5/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340146 giskard-2.0.0b5/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340336 giskard-2.0.0b5/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340499 giskard-2.0.0b5/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340671 giskard-2.0.0b5/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.340916 giskard-2.0.0b5/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.342390 giskard-2.0.0b5/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.342951 giskard-2.0.0b5/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.343264 giskard-2.0.0b5/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.343416 giskard-2.0.0b5/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.343713 giskard-2.0.0b5/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.344341 giskard-2.0.0b5/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.346629 giskard-2.0.0b5/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.346897 giskard-2.0.0b5/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.348157 giskard-2.0.0b5/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-12 12:50:19.000000 giskard-2.0.0b5/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.349478 giskard-2.0.0b5/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-12 11:29:06.000000 giskard-2.0.0b5/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.350200 giskard-2.0.0b5/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.350561 giskard-2.0.0b5/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.352420 giskard-2.0.0b5/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.352599 giskard-2.0.0b5/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.353674 giskard-2.0.0b5/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b5/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.354320 giskard-2.0.0b5/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-12 07:28:20.000000 giskard-2.0.0b5/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6009 2023-06-12 11:29:06.000000 giskard-2.0.0b5/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b5/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.319990 giskard-2.0.0b5/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-12 13:00:47.000000 giskard-2.0.0b5/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7425 2023-06-12 12:53:45.000000 giskard-2.0.0b5/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-12 13:00:47.358686 giskard-2.0.0b5/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-07 15:34:18.000000 giskard-2.0.0b5/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 13:00:47.357905 giskard-2.0.0b5/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b5/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b5/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b5/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-12 07:28:20.000000 giskard-2.0.0b5/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-12 11:29:06.000000 giskard-2.0.0b5/tests/test_utils.py
```

### Comparing `giskard-2.0.0b4/PKG-INFO` & `giskard-2.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
@@ -114,31 +114,32 @@
 
 ## Getting started
 
 <div id="installation">
 
 ### Installation
 ```sh
-pip install "giskard[server]==2.0.0b4"
+pip install "giskard[server]>=2.0.0b" -U
 
 giskard server start
 ```
 
 That's it. Access at http://localhost:19000
 </div>
 <div id="scan-your-model-to-detect-vulnerabilities">
 
 ### Scan your model to detect vulnerabilities
 
 After having wrapped your [model](https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset](https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can scan your model for vulnerabilities using:
 
 ```python
 import giskard
+from giskard import demo
 
-model, df = giskard.demo.titanic()
+model, df = demo.titanic()
 
 model = giskard.Model(model=model, model_type="classification")
 dataset = giskard.Dataset(
     df=df,
     target="Survived",
     cat_columns=["Pclass", "Sex", "SibSp", "Parch", "Embarked"],
 )
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b4 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b5 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
@@ -59,22 +59,22 @@
                                 [Scan Example]
 And of course, Giskard works with any model, any environment and integrates
 seamlessly with your favorite tools â¤µï¸
                  [https://github.com/Giskard-AI/giskard/blob/
       9f9f9994ab5deb503ed9c64e672982432a493cca/readme/tools.png?raw=true]
 
 ## Getting started
-### Installation ```sh pip install "giskard[server]==2.0.0b4" giskard server
+### Installation ```sh pip install "giskard[server]>=2.0.0b" -U giskard server
 start ``` That's it. Access at http://localhost:19000
 ### Scan your model to detect vulnerabilities After having wrapped your [model]
 (https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset]
 (https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can
-scan your model for vulnerabilities using: ```python import giskard model, df =
-giskard.demo.titanic() model = giskard.Model(model=model,
-model_type="classification") dataset = giskard.Dataset( df=df,
+scan your model for vulnerabilities using: ```python import giskard from
+giskard import demo model, df = demo.titanic() model = giskard.Model
+(model=model, model_type="classification") dataset = giskard.Dataset( df=df,
 target="Survived", cat_columns=["Pclass", "Sex", "SibSp", "Parch", "Embarked"],
 ) scan_results = giskard.scan(model, dataset) ``` Once the scan completes, you
 can display the results directly in your notebook: ```python display
 (scan_results) # in your notebook ```
 ### Automatically generate a test suite based on the scan results If the scan
 found potential issues in your model, you can automatically generate a test
 suite. Generating a test suite from your scan results will enable you to: -
```

### Comparing `giskard-2.0.0b4/README.md` & `giskard-2.0.0b5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,31 +85,32 @@
 
 ## Getting started
 
 <div id="installation">
 
 ### Installation
 ```sh
-pip install "giskard[server]==2.0.0b4"
+pip install "giskard[server]>=2.0.0b" -U
 
 giskard server start
 ```
 
 That's it. Access at http://localhost:19000
 </div>
 <div id="scan-your-model-to-detect-vulnerabilities">
 
 ### Scan your model to detect vulnerabilities
 
 After having wrapped your [model](https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset](https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can scan your model for vulnerabilities using:
 
 ```python
 import giskard
+from giskard import demo
 
-model, df = giskard.demo.titanic()
+model, df = demo.titanic()
 
 model = giskard.Model(model=model, model_type="classification")
 dataset = giskard.Dataset(
     df=df,
     target="Survived",
     cat_columns=["Pclass", "Sex", "SibSp", "Parch", "Embarked"],
 )
@@ -182,8 +183,8 @@
 <div id="like-what-were-doing">
 
 ## Like what we're doing?
 
 🌟 [Leave us a star](https://github.com/Giskard-AI/giskard), it helps the project to get discovered by others and keeps us motivated to build awesome open-source tools! 🌟
 
 ❤️ You can also [sponsor us](https://github.com/sponsors/Giskard-AI) on GitHub. With a monthly sponsor subscription, you can get a sponsor badge and get your bug reports prioritized. We also offer one-time sponsoring if you want us to get involved in a consulting project, run a workshop, or give a talk at your company.
-</div>
+</div>
```

#### html2text {}

```diff
@@ -41,22 +41,22 @@
                                 [Scan Example]
 And of course, Giskard works with any model, any environment and integrates
 seamlessly with your favorite tools â¤µï¸
                  [https://github.com/Giskard-AI/giskard/blob/
       9f9f9994ab5deb503ed9c64e672982432a493cca/readme/tools.png?raw=true]
 
 ## Getting started
-### Installation ```sh pip install "giskard[server]==2.0.0b4" giskard server
+### Installation ```sh pip install "giskard[server]>=2.0.0b" -U giskard server
 start ``` That's it. Access at http://localhost:19000
 ### Scan your model to detect vulnerabilities After having wrapped your [model]
 (https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset]
 (https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can
-scan your model for vulnerabilities using: ```python import giskard model, df =
-giskard.demo.titanic() model = giskard.Model(model=model,
-model_type="classification") dataset = giskard.Dataset( df=df,
+scan your model for vulnerabilities using: ```python import giskard from
+giskard import demo model, df = demo.titanic() model = giskard.Model
+(model=model, model_type="classification") dataset = giskard.Dataset( df=df,
 target="Survived", cat_columns=["Pclass", "Sex", "SibSp", "Parch", "Embarked"],
 ) scan_results = giskard.scan(model, dataset) ``` Once the scan completes, you
 can display the results directly in your notebook: ```python display
 (scan_results) # in your notebook ```
 ### Automatically generate a test suite based on the scan results If the scan
 found potential issues in your model, you can automatically generate a test
 suite. Generating a test suite from your scan results will enable you to: -
```

### Comparing `giskard-2.0.0b4/giskard/__init__.py` & `giskard-2.0.0b5/giskard/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from giskard.ml_worker.testing.registry.giskard_test import GiskardTest
 from giskard.ml_worker.testing.registry.slicing_function import SlicingFunction
 from giskard.ml_worker.testing.registry.slicing_function import slicing_function
 from giskard.ml_worker.testing.registry.transformation_function import transformation_function
 from giskard.ml_worker.testing.test_result import TestResult
 from giskard.ml_worker.utils.logging import configure_logging
 from giskard.models.automodel import Model
-from giskard.utils.analytics_collector import GiskardAnalyticsCollector
+from . import demo
 from .ml_worker.utils.network import check_latest_giskard_version
 from .scanner import scan
 
 configure_logging()
 if sys.version_info >= (3, 8):
     from importlib import metadata as importlib_metadata
 else:
@@ -48,8 +48,9 @@
     'slicing_function',
     'transformation_function',
     'SuiteInput',
     'SlicingFunction',
     'scan',
     'TestResult',
     'GiskardTest',
+    "demo"
 ]
```

### Comparing `giskard-2.0.0b4/giskard/cli.py` & `giskard-2.0.0b5/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/cli_utils.py` & `giskard-2.0.0b5/giskard/cli_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/client/giskard_client.py` & `giskard-2.0.0b5/giskard/client/giskard_client.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/client/io_utils.py` & `giskard-2.0.0b5/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/client/project.py` & `giskard-2.0.0b5/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/client/python_utils.py` & `giskard-2.0.0b5/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/commands/cli_server.py` & `giskard-2.0.0b5/giskard/commands/cli_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import os
-import re
 from pathlib import Path
 from typing import Optional
 from urllib.parse import urlparse
 
 import click
 import docker
 import requests
 import yaml
 from docker import DockerClient
 from docker.errors import NotFound, DockerException
 from docker.models.containers import Container
+from packaging import version
+from packaging.version import InvalidVersion, Version
 from tenacity import retry, wait_exponential
 
 import giskard
 from giskard.cli_utils import common_options
 from giskard.settings import settings
 from giskard.utils.analytics_collector import analytics
 
@@ -25,18 +26,21 @@
 IMAGE_NAME = "docker.io/giskardai/giskard"
 
 
 def create_docker_client() -> DockerClient:
     try:
         return docker.from_env()
     except DockerException as e:
-        logger.exception("""Failed to connect to Docker. Giskard requires Docker to be installed. If Docker is installed, please run it. Otherwise, please install it.
+        logger.exception(
+            """Failed to connect to Docker. Giskard requires Docker to be installed. If Docker is installed, please run it. Otherwise, please install it.
 For an easy installation of Docker you can execute:
 - sudo curl -fsSL https://get.docker.com -o get-docker.sh
-- sudo sh get-docker.sh""", e)
+- sudo sh get-docker.sh""",
+            e,
+        )
         exit(1)
 
 
 @click.group("server", help="Giskard UI management", context_settings={"show_default": True})
 def server() -> None:
     """
     Giskard UI management
@@ -45,26 +49,30 @@
 
 def update_options(fn):
     fn = click.option("--version", "version", is_flag=False, default="", help="Version to update to.")(fn)
     return fn
 
 
 def get_version(version=None):
-    if not version:
-        app_settings = _get_settings()
-        if not app_settings:
-            version = _fetch_latest_tag()
-            logger.info(f"Giskard Server not installed. Latest version is {version}")
-            _write_settings({"version": version})
-        else:
-            version = app_settings["version"]
-    else:
+    if version:
         current_settings = _get_settings() or {}
-        current_settings['version'] = version
+        current_settings["version"] = version
         _write_settings(current_settings)
+    else:
+        app_settings = _get_settings()
+        if app_settings:
+            version = app_settings["version"]
+        else:
+            version = giskard.get_version()
+            _write_settings({"version": version})
+            latest_version = _fetch_latest_tag()
+            message = f"Giskard Server not installed. Using version {version}."
+            if latest_version and version != latest_version:
+                message += f" Latest available version is {latest_version}. To use it pass a --version argument"
+            logger.info(message)
     return version
 
 
 def get_container_name(version=None):
     if not version:
         version = get_version()
     return f"giskard-server.{version}"
@@ -88,16 +96,16 @@
             return None
 
 
 def _start(attached=False, version=None):
     logger.info("Starting Giskard Server")
 
     settings = _get_settings() or {}
-    port = settings.get('port', 19000)
-    ml_worker_port = settings.get('ml_worker_port', 40051)
+    port = settings.get("port", 19000)
+    ml_worker_port = settings.get("ml_worker_port", 40051)
 
     version = get_version(version)
 
     _pull_image(version)
 
     home_volume = _get_home_volume()
 
@@ -105,15 +113,15 @@
 
     if not container:
         container = create_docker_client().containers.create(
             get_image_name(version),
             detach=not attached,
             name=get_container_name(version),
             ports={7860: port, 40051: ml_worker_port},
-            volumes={home_volume.name: {'bind': '/home/giskard/datadir', 'mode': 'rw'}},
+            volumes={home_volume.name: {"bind": "/home/giskard/datadir", "mode": "rw"}},
         )
     container.start()
     analytics.track("Giskard Server started", {"client version": giskard.__version__, "server version": version})
     logger.info(f"Giskard Server {version} started. You can access it at http://localhost:{port}")
 
 
 def _check_downloaded(version: str):
@@ -139,21 +147,27 @@
             )
             raise click.Abort()
 
 
 @retry(wait=wait_exponential(min=0.1, max=5, multiplier=0.1))
 def _fetch_latest_tag() -> str:
     """
-    Returns: the latest tag from the GitHub API. Format: vX.Y.Z
+    Returns: the latest tag from the Docker Hub API. Format: vX.Y.Z
     """
-    response = requests.get("https://api.github.com/repos/Giskard-AI/giskard/releases/latest")
+    response = requests.get("https://hub.docker.com/v2/namespaces/giskardai/repositories/giskard/tags?page_size=10")
     response.raise_for_status()
     json_response = response.json()
-    tag = json_response["tag_name"]
-    return tag.replace('v', '')
+    latest_tag = "latest"
+    latest = next(i for i in json_response["results"] if i["name"] == latest_tag)
+    latest_version_image = next(
+        i for i in json_response["results"] if ((i["name"] != latest_tag) and (i["digest"] == latest["digest"]))
+    )
+
+    tag = latest_version_image["name"]
+    return tag.replace("v", "")
 
 
 def _write_settings(settings):
     with open(giskard_settings_path, "w") as f:
         yaml.dump(settings, f)
 
 
@@ -176,44 +190,47 @@
 
     return home_volume
 
 
 def _expose(token):
     container = get_container()
     if container:
-        if container.status != 'running':
+        if container.status != "running":
             print("Error: Giskard server is not running. Please start it using `giskard server start`")
             raise click.Abort()
     else:
         raise click.Abort()
     print("Exposing Giskard Server to the internet...")
     from pyngrok import ngrok
     from pyngrok.conf import PyngrokConfig
+
     if token:
         ngrok.set_auth_token(token)
 
     http_tunnel = ngrok.connect(19000, "http", pyngrok_config=None if token else PyngrokConfig(region="us"))
     tcp_tunnel = ngrok.connect(40051, "tcp", pyngrok_config=None if token else PyngrokConfig(region="eu"))
 
     # Only split the last ':' in case the URL contains a port
     tcp_addr = urlparse(tcp_tunnel.public_url)
 
     analytics.track("Giskard Server exposed via ngrok", {"client version": giskard.__version__})
     print("Giskard Server is now exposed to the internet.")
     print("You can now upload objects to the Giskard Server using the following client: \n")
 
-    print(f"""token=...
+    print(
+        f"""token=...
 client = giskard.GiskardClient(\"{http_tunnel.public_url}\", token)
 
 # To run your model with the Giskard Server, execute these three lines on Google Colab:
 
 %env GSK_EXTERNAL_ML_WORKER_HOST={tcp_addr.hostname}
 %env GSK_EXTERNAL_ML_WORKER_PORT={tcp_addr.port}
 %env GSK_API_KEY=...
-!giskard worker start -d -u {http_tunnel.public_url}""")
+!giskard worker start -d -u {http_tunnel.public_url}"""
+    )
 
     ngrok_process = ngrok.get_ngrok_process()
     try:
         # Block until CTRL-C or some other terminating event
         ngrok_process.proc.wait()
     finally:
         print("Shutting down expose.")
@@ -246,15 +263,15 @@
 def stop():
     """\b
     Stop Giskard Server.
 
     Stops a running Giskard server. Does nothing if Giskard server is not running.
     """
     container = get_container()
-    if container.status != 'exited':
+    if container.status != "exited":
         logger.info("Stopping Giskard Server")
         container.stop()
         logger.info("Giskard Server stopped")
     else:
         logger.info(f"Giskard container {container.name} is not running")
 
 
@@ -265,15 +282,15 @@
 def restart(service, hard):
     """\b
     Restart Giskard Server.
 
     Stops any running Giskard server and starts it again.
     """
     container = get_container()
-    if container.status != 'running':
+    if container.status != "running":
         logger.info("Giskard server isn't running")
         _start()
     else:
         if hard:
             logger.info(f"Restarting {container.name} container")
             container.start()
             container.stop()
@@ -333,15 +350,15 @@
     out_dir = Path(local_dir)
     assert out_dir.is_dir(), "'output' should be an existing directory"
     bits, stat = get_container().get_archive("/home/giskard/datadir/run", encode_stream=True)
     from datetime import datetime
 
     now = datetime.now().strftime("%Y%m%d_%H%M%S_%f")
     out_file = out_dir / f"giskard-diagnose-{get_version().replace('.', '_')}-{now}.tar.gz"
-    with open(out_file, 'wb') as f:
+    with open(out_file, "wb") as f:
         for chunk in bits:
             f.write(chunk)
     analytics.track("Giskard Server diagnosis ran", {"client version": giskard.__version__})
     logger.info(f"Wrote diagnose info to {out_file}")
 
 
 @server.command("update")
@@ -351,28 +368,31 @@
     """\b
     Update Giskard Server. Uses the latest available version if not specified.
     """
     latest_version = _fetch_latest_tag()
     if not version:
         version = latest_version
 
-    installed_version = _get_settings().get('version')
+    installed_version = _get_settings().get("version")
     if installed_version == version:
         logger.info(f"Giskard server is already running version {version}")
         return
 
     logger.info(f"Updating Giskard Server {installed_version} -> {version}")
     _pull_image(version)
     _write_settings({**_get_settings(), **{"version": version}})
     analytics.track("Giskard Server updated", {"client version": giskard.__version__, "server version": version})
     logger.info(f"Giskard Server updated to {version}")
 
 
-def convert_version_to_number(version: str) -> int:
-    return int(''.join(re.findall(r'\d', version)))
+def read_version(version_str: str) -> Version:
+    try:
+        return version.parse(version_str)
+    except InvalidVersion:
+        return version.NegativeInfinity
 
 
 @server.command("status")
 @common_options
 def status():
     """\b
     Check if server container is running and status of each internal service
@@ -380,25 +400,25 @@
     app_settings = _get_settings()
     if not app_settings:
         logger.info("Giskard Server is not installed. Install using `giskard server start`")
         return
     else:
         version = app_settings["version"]
 
-    logger.info(f"Giskard Server {version} is installed.")
+    logger.info(f"Giskard Server version is set to {version}")
 
     latest = _fetch_latest_tag()
 
-    if convert_version_to_number(version) < convert_version_to_number(version):
+    if read_version(version) < read_version(latest):
         logger.info(f"A new version is available: {latest}")
 
     container = get_container()
     if container:
-        if container.status == 'running':
-            logger.info(F"Container {container.name} status:")
+        if container.status == "running":
+            logger.info(f"Container {container.name} status:")
             print(get_container().exec_run("supervisorctl -c /opt/giskard/supervisord.conf").output.decode())
         else:
             logger.info(f"Container {container.name} isn't running ({container.status})")
 
 
 @server.command("clean")
 @click.option("--data", "delete_data", is_flag=True, help="Delete user data (giskard-home volume)")
@@ -428,28 +448,28 @@
         client.images.get(image_name).remove(force=True)
         logger.info(f"Image {image_name} has been deleted")
     except NotFound:
         logger.info(f"Image {image_name} does not exist")
 
     if data_deletion_confirmed:
         try:
-            volume = client.volumes.get('giskard-home')
+            volume = client.volumes.get("giskard-home")
             volume.remove(force=True)
             logger.info("User data has been deleted in 'giskard-home' volume")
         except NotFound:
             logger.info("Volume 'giskard-home' does not exist")
 
 
 @server.command("expose")
 @click.option(
     "--token",
     "token",
     required=False,
     help="In case you have an ngrok account, you can use a token "
-         "generated from https://dashboard.ngrok.com/get-started/your-authtoken",
+    "generated from https://dashboard.ngrok.com/get-started/your-authtoken",
 )
 @common_options
 def expose(token):
     """\b
     Expose your local Giskard Server to the outside world using ngrok to use in notebooks like Google Colab
     """
     _expose(token)
```

### Comparing `giskard-2.0.0b4/giskard/commands/cli_worker.py` & `giskard-2.0.0b5/giskard/commands/cli_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/core/core.py` & `giskard-2.0.0b5/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/core/dataset_validation.py` & `giskard-2.0.0b5/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/core/errors.py` & `giskard-2.0.0b5/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/core/model_validation.py` & `giskard-2.0.0b5/giskard/core/model_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/core/suite.py` & `giskard-2.0.0b5/giskard/core/suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/core/validation.py` & `giskard-2.0.0b5/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/datasets/__init__.py` & `giskard-2.0.0b5/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/datasets/base/__init__.py` & `giskard-2.0.0b5/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/datasets/metadata/indexing.py` & `giskard-2.0.0b5/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/datasets/metadata/registry.py` & `giskard-2.0.0b5/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.0.0b5/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/demo/__init__.py` & `giskard-2.0.0b5/giskard/demo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import pandas as pd
-import numpy as np
 import os
+
+import numpy as np
+import pandas as pd
 from sklearn import model_selection
-from sklearn.linear_model import LogisticRegression
-from sklearn.preprocessing import OneHotEncoder, StandardScaler
-from sklearn.impute import SimpleImputer
-from sklearn.feature_extraction.text import TfidfVectorizer
-from sklearn.pipeline import Pipeline
 from sklearn.compose import ColumnTransformer
+from sklearn.feature_extraction.text import TfidfVectorizer
+from sklearn.impute import SimpleImputer
 from sklearn.linear_model import LinearRegression
+from sklearn.linear_model import LogisticRegression
+from sklearn.pipeline import Pipeline
+from sklearn.preprocessing import OneHotEncoder, StandardScaler
 
 
 def titanic_df():
     df = pd.read_csv(os.path.join(os.path.dirname(__file__), "titanic.csv"))
     df.drop(["Ticket", "Cabin"], axis=1, inplace=True)
     _classification_labels = {0: "no", 1: "yes"}
     df["Survived"] = df["Survived"].apply(lambda x: _classification_labels[x])
@@ -85,7 +86,17 @@
 def linear_pipeline():
     reg, _ = linear()
 
     def preprocessor(df):
         return df["x"].to_numpy().reshape(len(df["x"]), 1)
 
     return preprocessor, reg
+
+
+__all__ = [
+    "titanic_df",
+    "titanic",
+    "titanic_pipeline",
+    "linear_df",
+    "linear",
+    "linear_pipeline",
+]
```

### Comparing `giskard-2.0.0b4/giskard/demo/titanic.csv` & `giskard-2.0.0b5/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.0.0b5/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/bridge/ml_worker_bridge.py` & `giskard-2.0.0b5/giskard/ml_worker/bridge/ml_worker_bridge.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/core/log_listener.py` & `giskard-2.0.0b5/giskard/ml_worker/core/log_listener.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/core/savable.py` & `giskard-2.0.0b5/giskard/ml_worker/core/savable.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b5/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/ml_worker.py` & `giskard-2.0.0b5/giskard/ml_worker/ml_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/server/ml_worker_service.py` & `giskard-2.0.0b5/giskard/ml_worker/server/ml_worker_service.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/functions/slicing.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/functions/transformation.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/registry/decorators_utils.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/registry/giskard_test.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/registry/registry.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/registry/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/registry/slicing_function.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/registry/transformation_function.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/registry/udf_repository.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/registry/udf_repository.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/test_result.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/test_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/testing/utils.py` & `giskard-2.0.0b5/giskard/ml_worker/testing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b5/giskard/ml_worker/utils/logging.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/utils/network.py` & `giskard-2.0.0b5/giskard/ml_worker/utils/network.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/ml_worker/utils/request_interceptor.py` & `giskard-2.0.0b5/giskard/ml_worker/utils/request_interceptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/__init__.py` & `giskard-2.0.0b5/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/_precooked.py` & `giskard-2.0.0b5/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/automodel/__init__.py` & `giskard-2.0.0b5/giskard/models/automodel/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/base/__init__.py` & `giskard-2.0.0b5/giskard/models/base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,17 @@
         """
         Returns True if the model is of type regression, False otherwise.
         """
         return self.meta.model_type == SupportedModelTypes.REGRESSION
 
     @property
     def is_text_generation(self):
+        """
+        Returns True if the model is of type text generation, False otherwise.
+        """
         return self.meta.model_type == SupportedModelTypes.TEXT_GENERATION
 
     @classmethod
     def determine_model_class(cls, meta, local_dir):
         class_file = Path(local_dir) / MODEL_CLASS_PKL
         if class_file.exists():
             with open(class_file, "rb") as f:
```

### Comparing `giskard-2.0.0b4/giskard/models/cache/__init__.py` & `giskard-2.0.0b5/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/cache/cache.py` & `giskard-2.0.0b5/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/catboost/__init__.py` & `giskard-2.0.0b5/giskard/models/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/function/__init__.py` & `giskard-2.0.0b5/giskard/models/function/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/huggingface/__init__.py` & `giskard-2.0.0b5/giskard/models/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/langchain/__init__.py` & `giskard-2.0.0b5/giskard/models/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/model_explanation.py` & `giskard-2.0.0b5/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/pytorch/__init__.py` & `giskard-2.0.0b5/giskard/models/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/sklearn/__init__.py` & `giskard-2.0.0b5/giskard/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/tensorflow/__init__.py` & `giskard-2.0.0b5/giskard/models/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/models/utils.py` & `giskard-2.0.0b5/giskard/models/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/path_utils.py` & `giskard-2.0.0b5/giskard/path_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/__init__.py` & `giskard-2.0.0b5/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/calibration/issues.py` & `giskard-2.0.0b5/giskard/scanner/calibration/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.0.0b5/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.0.0b5/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/common/examples.py` & `giskard-2.0.0b5/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/common/loss_based_detector.py` & `giskard-2.0.0b5/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.0.0b5/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/decorators.py` & `giskard-2.0.0b5/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/issues.py` & `giskard-2.0.0b5/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/llm/toxicity_detector.py` & `giskard-2.0.0b5/giskard/scanner/llm/toxicity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/llm/utils.py` & `giskard-2.0.0b5/giskard/scanner/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/performance/issues.py` & `giskard-2.0.0b5/giskard/scanner/performance/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/performance/metrics.py` & `giskard-2.0.0b5/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.0.0b5/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/registry.py` & `giskard-2.0.0b5/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/result.py` & `giskard-2.0.0b5/giskard/scanner/result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/robustness/base_detector.py` & `giskard-2.0.0b5/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/robustness/entity_swap.py` & `giskard-2.0.0b5/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.0.0b5/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/robustness/issues.py` & `giskard-2.0.0b5/giskard/scanner/robustness/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/robustness/nationalities.json` & `giskard-2.0.0b5/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.0.0b5/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/robustness/text_transformations.py` & `giskard-2.0.0b5/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/scanner.py` & `giskard-2.0.0b5/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.0.0b5/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_code_snippet.html` & `giskard-2.0.0b5/giskard/scanner/templates/_code_snippet.html`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
     <div class="text-sm">
         <pre><code class="language-python rounded">{% raw %}from giskard import GiskardClient
 test_suite = results.generate_test_suite("My first test suite")
 
 # To start the Giskard server, run in your terminal within the Python
 # environment containing the dependencies of your model: 
-giskard server start --version 2.0.0b4
+giskard server start
 giskard worker start -u http://localhost:19000/
 
 # Then upload your test suite to the opened Giskard server
 client = GiskardClient("http://localhost:19000", "GISKARD_API_KEY")
 client.create_project("my_project_id", "my_project_name")
 test_suite.upload(client, "my_project_id"){% endraw %}
 </code></pre>
```

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/data_leakage.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/data_leakage.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/default.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/default.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/llm_toxicity.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/llm_toxicity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/overconfidence.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/overconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/performance.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/performance.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/robustness.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/robustness.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/stochasticity.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/stochasticity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues/underconfidence.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues/underconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_issues_table.html` & `giskard-2.0.0b5/giskard/scanner/templates/_issues_table.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_main_content.html` & `giskard-2.0.0b5/giskard/scanner/templates/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/_tab_header.html` & `giskard-2.0.0b5/giskard/scanner/templates/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/scan_results.html` & `giskard-2.0.0b5/giskard/scanner/templates/scan_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/static/external.js` & `giskard-2.0.0b5/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/static/internal.js` & `giskard-2.0.0b5/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/templates/static/style.css` & `giskard-2.0.0b5/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/scanner/visualization/custom_jinja.py` & `giskard-2.0.0b5/giskard/scanner/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/settings.py` & `giskard-2.0.0b5/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/base.py` & `giskard-2.0.0b5/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/bruteforce_slicer.py` & `giskard-2.0.0b5/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/category_slicer.py` & `giskard-2.0.0b5/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/multiscale_slicer.py` & `giskard-2.0.0b5/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/opt_slicer.py` & `giskard-2.0.0b5/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/slice.py` & `giskard-2.0.0b5/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/stop_words.py` & `giskard-2.0.0b5/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/text_slicer.py` & `giskard-2.0.0b5/giskard/slicing/text_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/tree_slicer.py` & `giskard-2.0.0b5/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/slicing/utils.py` & `giskard-2.0.0b5/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/testing/__init__.py` & `giskard-2.0.0b5/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/testing/tests/drift.py` & `giskard-2.0.0b5/giskard/testing/tests/drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/testing/tests/metamorphic.py` & `giskard-2.0.0b5/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/testing/tests/performance.py` & `giskard-2.0.0b5/giskard/testing/tests/performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/testing/tests/statistic.py` & `giskard-2.0.0b5/giskard/testing/tests/statistic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard/utils/analytics_collector.py` & `giskard-2.0.0b5/giskard/utils/analytics_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import getpass
 import hashlib
 import os
 import platform
 import uuid
 from functools import wraps
 from threading import Lock
 from typing import Dict, Optional
@@ -35,15 +36,15 @@
 
 def anonymize(message):
     if not message:
         return None
     if isinstance(message, list):
         return [anonymize(m) for m in message]
 
-    return hashlib.sha1(str(message).encode()).hexdigest()[:10]
+    return hashlib.sha1(str(message).encode()).hexdigest()[:16]
 
 
 def get_model_properties(model):
     from ..models.base import WrapperModel
 
     if model is None:
         return {}
@@ -114,58 +115,72 @@
             "Server license": server_info.get("instanceLicenseId"),
             "Giskard User": server_info.get("user"),
         }
 
     @threaded
     @analytics_method
     def track(self, event_name, properties=None, meta=None, force=False):
-        if not self.giskard_version:
-            import giskard
+        self.initialize_giskard_version()
+        self.initialize_user_properties()
 
-            self.giskard_version = giskard.get_version()
-        if not self.ip:
-            self.initialize_geo()
         if self.is_enabled or force:
             merged_props = {
                 "giskard_version": self.giskard_version,
                 "python_version": platform.python_version(),
-                "ip": self.ip,  # only for aggregated stats: city, country, region. IP itself isn't stored
-                "arch": platform.machine(),
-                "$os": platform.system(),
-                "os-full": platform.platform(aliased=True),
-                "environment": self.environment
+                "environment": self.environment,
             }
             if properties is not None:
                 merged_props = {**merged_props, **properties}
             if self.server_info is not None:
                 merged_props = {**merged_props, **self.server_info}
 
             self.mp.track(
                 distinct_id=self.distinct_user_id, event_name=event_name, properties=dict(merged_props), meta=meta
             )
 
+    def initialize_giskard_version(self):
+        if not self.giskard_version:
+            import giskard
+            self.giskard_version = giskard.get_version()
+
+    def initialize_user_properties(self):
+        if not self.ip:
+            self.initialize_geo()
+            self.mp.people_set(
+                self.distinct_user_id,
+                {
+                    "$name": "",
+                    "arch": platform.machine(),
+                    "$os": platform.system(),
+                    "os-full": platform.platform(aliased=True),
+                },
+                # only for aggregated stats: city, country, region. IP itself isn't stored
+                meta={'$ip': self.ip},
+            )
+
     @staticmethod
     def machine_based_user_id():
         try:
-            return anonymize(str(uuid.getnode()) + os.getlogin())
+            return anonymize(str(uuid.getnode()) + getpass.getuser())
         except BaseException:  # noqa NOSONAR
             # https://bugs.python.org/issue40821
             return "unknown"
 
     def initialize_geo(self):
         """
         Query a user's IP address to convert it to an aggregated telemetry:
             - city
             - region
             - country
-        IP address itself **isn't stored** by in the telemetry data
+        IP address itself **isn't stored** by in the telemetry data, see:
+        https://docs.mixpanel.com/docs/tracking/how-tos/effective-server#tracking-geolocation
         """
         with GiskardAnalyticsCollector.lock:
             if self.ip:
                 return
             try:
-                self.ip = requests.get('http://ip-api.com/json').json().get('query', 'unknown')  # noqa NOSONAR
+                self.ip = requests.get('https://api64.ipify.org/?format=json').json().get('ip', 'unknown')
             except:  # noqa NOSONAR
                 self.ip = "unknown"
 
 
 analytics = GiskardAnalyticsCollector()
```

### Comparing `giskard-2.0.0b4/giskard/utils/environment_detector.py` & `giskard-2.0.0b5/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard.egg-info/PKG-INFO` & `giskard-2.0.0b5/giskard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
@@ -114,31 +114,32 @@
 
 ## Getting started
 
 <div id="installation">
 
 ### Installation
 ```sh
-pip install "giskard[server]==2.0.0b4"
+pip install "giskard[server]>=2.0.0b" -U
 
 giskard server start
 ```
 
 That's it. Access at http://localhost:19000
 </div>
 <div id="scan-your-model-to-detect-vulnerabilities">
 
 ### Scan your model to detect vulnerabilities
 
 After having wrapped your [model](https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset](https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can scan your model for vulnerabilities using:
 
 ```python
 import giskard
+from giskard import demo
 
-model, df = giskard.demo.titanic()
+model, df = demo.titanic()
 
 model = giskard.Model(model=model, model_type="classification")
 dataset = giskard.Dataset(
     df=df,
     target="Survived",
     cat_columns=["Pclass", "Sex", "SibSp", "Parch", "Embarked"],
 )
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b4 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b5 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
@@ -59,22 +59,22 @@
                                 [Scan Example]
 And of course, Giskard works with any model, any environment and integrates
 seamlessly with your favorite tools â¤µï¸
                  [https://github.com/Giskard-AI/giskard/blob/
       9f9f9994ab5deb503ed9c64e672982432a493cca/readme/tools.png?raw=true]
 
 ## Getting started
-### Installation ```sh pip install "giskard[server]==2.0.0b4" giskard server
+### Installation ```sh pip install "giskard[server]>=2.0.0b" -U giskard server
 start ``` That's it. Access at http://localhost:19000
 ### Scan your model to detect vulnerabilities After having wrapped your [model]
 (https://docs.giskard.ai/en/latest/guides/wrap_model/index.html) & [dataset]
 (https://docs.giskard.ai/en/latest/guides/wrap_dataset/index.html), you can
-scan your model for vulnerabilities using: ```python import giskard model, df =
-giskard.demo.titanic() model = giskard.Model(model=model,
-model_type="classification") dataset = giskard.Dataset( df=df,
+scan your model for vulnerabilities using: ```python import giskard from
+giskard import demo model, df = demo.titanic() model = giskard.Model
+(model=model, model_type="classification") dataset = giskard.Dataset( df=df,
 target="Survived", cat_columns=["Pclass", "Sex", "SibSp", "Parch", "Embarked"],
 ) scan_results = giskard.scan(model, dataset) ``` Once the scan completes, you
 can display the results directly in your notebook: ```python display
 (scan_results) # in your notebook ```
 ### Automatically generate a test suite based on the scan results If the scan
 found potential issues in your model, you can automatically generate a test
 suite. Generating a test suite from your scan results will enable you to: -
```

### Comparing `giskard-2.0.0b4/giskard.egg-info/SOURCES.txt` & `giskard-2.0.0b5/giskard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/giskard.egg-info/requires.txt` & `giskard-2.0.0b5/giskard.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/pyproject.toml` & `giskard-2.0.0b5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 proto = "setup.py grpc"
 # add "-n auto" to the pytest command to parallelize the execution
 test.cmd = "pytest -c pyproject.toml tests --cov=giskard --cov-report=xml --disable-warnings"
 test.env = { GSK_DISABLE_ANALYTICS = "True"}
 # for some reason github runners don't work when calling 'pdm test -m "not slow"'
 test-fast.cmd = "pytest -n auto -m 'not slow' -c pyproject.toml tests --cov=giskard --cov-report=xml --disable-warnings"
 test-fast.env = { GSK_DISABLE_ANALYTICS = "True"}
-lint = "flake8 giskard tests"
+lint = "ruff giskard tests"
 doc = "python -m sphinx_autobuild docs docs/_build/html"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "typing-extensions>=4.5.0",
     "black>=23.3.0",
     "bandit>=1.7.4",
     "darglint>=1.8.1",
-    "flake8>=3.9.2",
     "jupyter>=1.0.0",
     "jupyterlab>=3.4.2",
     "pre-commit>=2.19.0",
     "pydocstyle>=6.1.1",
     "pylint>=2.13.9",
     "pyupgrade>=2.32.1",
     "safety>=1.10.3",
@@ -41,27 +40,28 @@
     "pip>=23.1.2",
     "langchain>=0.0.187",
     "nltk>=3.8.1",
     "xgboost>=1.7.5",
     "lightgbm>=3.3.5",
     "imbalanced-learn>=0.10.1",
     "pytest-xdist>=3.3.1",
+    "ruff>=0.0.271",
 ]
 proto = [
     "grpcio-tools>=1.46.3",
     "mypy-protobuf>=3.2.0",
     "mypy-extensions>=0.4.3",
 ]
 test = [
     "pytest-cov>=4.0.0",
     "pytest>=7.1.2",
     "catboost>=1.1.1",
     "requests-mock>=1.10.0",
     "tensorflow-hub>=0.12.0",
-    "transformers>=4.27.4",
+    "transformers>=4.27.4, <4.30",
     "torch>=2.0.0",
     "torchdata>=0.6.0",
     "torchtext>=0.15.1",
     "portalocker>=2.0.0",
     "scikit-learn==1.0.2",
     "tensorflow-macos>=2.8.0, <2.10; sys_platform == 'darwin' and platform_machine == 'arm64'",
     "tensorflow>=2.8.0, <2.10; sys_platform != 'darwin' or platform_machine != 'arm64'",
@@ -76,14 +76,15 @@
     "sphinx-autoapi>=2.1.0",
     "sphinx-rtd-theme>=1.2.0",
     "sphinx-tabs>=3.4.1",
     "sphinx-design>=0.4.1",
     "sphinx-copybutton>=0.5.2",
     "sphinx-click>=4.4.0",
     "nbsphinx>=0.9.2",
+    "sphinx-favicon>=1.0.1",
 ]
 
 [tool.setuptools.packages.find]
 include = ["giskard*"]
 exclude = ["docs*", "tests*"]
 
 [tool.setuptools.package-data]
@@ -103,15 +104,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.0.0b4"
+version = "2.0.0b5"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [
     { name = "Giskard AI", email = "hello@giskard.ai" },
 ]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
@@ -175,20 +176,23 @@
     "lockfile>=0.12.2",
     "protobuf<=3.20.3",
     "python-daemon>=2.2.2,<3",
     "pycryptodome>=3.6.1",
     "pyngrok>=6.0.0",
 ]
 
+[tool.ruff]
+line-length = 120
+ignore = ["E501"]
+
 [tool.black]
 # https://github.com/psf/black
 target-version = ['py38', 'py39', 'py310']
 line-length = 120
 color = true
-skip-string-normalization = true
 
 exclude = '''
 /(
     \.git
     | \.hg
     | \.mypy_cache
     | \.tox
```

### Comparing `giskard-2.0.0b4/setup.py` & `giskard-2.0.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_custom_model.py` & `giskard-2.0.0b5/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_data_drift.py` & `giskard-2.0.0b5/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_data_processing_pipeline.py` & `giskard-2.0.0b5/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_dataset.py` & `giskard-2.0.0b5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_metamorphic_direction.py` & `giskard-2.0.0b5/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_metamorphic_invariance.py` & `giskard-2.0.0b5/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_model.py` & `giskard-2.0.0b5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_model_auto_inference.py` & `giskard-2.0.0b5/tests/test_model_auto_inference.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_model_explanation.py` & `giskard-2.0.0b5/tests/test_model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_model_postprocess.py` & `giskard-2.0.0b5/tests/test_model_postprocess.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_performance.py` & `giskard-2.0.0b5/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_programmatic.py` & `giskard-2.0.0b5/tests/test_programmatic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_project_uploads.py` & `giskard-2.0.0b5/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_statistical.py` & `giskard-2.0.0b5/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b4/tests/test_upload.py` & `giskard-2.0.0b5/tests/test_upload.py`

 * *Files identical despite different names*

