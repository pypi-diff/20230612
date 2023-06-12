# Comparing `tmp/arg_services-1.3.1.tar.gz` & `tmp/arg_services-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arg_services-1.3.1.tar", max compression
+gzip compressed data, was "arg_services-1.3.2.tar", max compression
```

## Comparing `arg_services-1.3.1.tar` & `arg_services-1.3.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1067 2023-04-21 09:06:53.310260 arg_services-1.3.1/LICENSE
--rw-r--r--   0        0        0      657 2023-04-21 09:06:53.310260 arg_services-1.3.1/README.md
--rw-r--r--   0        0        0      671 2023-04-21 09:07:30.726636 arg_services-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     7288 2023-04-21 09:07:29.786626 arg_services-1.3.1/src/arg_services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.770626 arg_services-1.3.1/src/arg_services/cbr/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.770626 arg_services-1.3.1/src/arg_services/cbr/v1beta/__init__.py
--rw-r--r--   0        0        0     7099 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.py
--rw-r--r--   0        0        0    12424 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
--rw-r--r--   0        0        0     2783 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
--rw-r--r--   0        0        0     3416 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.py
--rw-r--r--   0        0        0     3094 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
--rw-r--r--   0        0        0     2519 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.py
--rw-r--r--   0        0        0     2515 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
--rw-r--r--   0        0        0     8286 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.py
--rw-r--r--   0        0        0    15179 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
--rw-r--r--   0        0        0     4628 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
--rw-r--r--   0        0        0     1252 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.766626 arg_services-1.3.1/src/arg_services/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.770626 arg_services-1.3.1/src/arg_services/graph/v1/__init__.py
--rw-r--r--   0        0        0    11861 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.py
--rw-r--r--   0        0        0    33449 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2_grpc.py
--rw-r--r--   0        0        0      151 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.774626 arg_services-1.3.1/src/arg_services/mining/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.774626 arg_services-1.3.1/src/arg_services/mining/v1beta/__init__.py
--rw-r--r--   0        0        0     5028 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     6692 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     4625 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     1237 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     6102 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     8973 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     4721 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1298 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     4150 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.py
--rw-r--r--   0        0        0     3932 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
--rw-r--r--   0        0        0     3092 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
--rw-r--r--   0        0        0     3812 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     4057 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     2896 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      856 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0     2930 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.py
--rw-r--r--   0        0        0     2419 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.pyi
--rw-r--r--   0        0        0     2834 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.py
--rw-r--r--   0        0        0      821 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.774626 arg_services-1.3.1/src/arg_services/mining_explanation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.778626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/__init__.py
--rw-r--r--   0        0        0     3371 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     3359 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     3044 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0      916 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     4502 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     5167 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     3110 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     3857 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     3980 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     3112 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      960 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.778626 arg_services-1.3.1/src/arg_services/nlp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.782626 arg_services-1.3.1/src/arg_services/nlp/v1/__init__.py
--rw-r--r--   0        0        0     9005 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.py
--rw-r--r--   0        0        0    27846 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.pyi
--rw-r--r--   0        0        0     6344 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.782626 arg_services-1.3.1/src/google/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:07:29.782626 arg_services-1.3.1/src/google/api/__init__.py
--rw-r--r--   0        0        0     1813 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2631 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2.py
--rw-r--r--   0        0        0    18295 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-04-21 09:07:29.758626 arg_services-1.3.1/src/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 arg_services-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-12 07:55:34.199488 arg_services-1.3.2/LICENSE
+-rw-r--r--   0        0        0      657 2023-06-12 07:55:34.199488 arg_services-1.3.2/README.md
+-rw-r--r--   0        0        0      675 2023-06-12 07:56:06.627819 arg_services-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7288 2023-06-12 07:56:05.543807 arg_services-1.3.2/src/arg_services/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.523806 arg_services-1.3.2/src/arg_services/cbr/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.527807 arg_services-1.3.2/src/arg_services/cbr/v1beta/__init__.py
+-rw-r--r--   0        0        0     7099 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.py
+-rw-r--r--   0        0        0    12424 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
+-rw-r--r--   0        0        0     2783 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3416 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.py
+-rw-r--r--   0        0        0     3094 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2519 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.py
+-rw-r--r--   0        0        0     2515 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8286 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.py
+-rw-r--r--   0        0        0    15179 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
+-rw-r--r--   0        0        0     4628 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
+-rw-r--r--   0        0        0     1252 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.535807 arg_services-1.3.2/src/arg_services/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.539807 arg_services-1.3.2/src/arg_services/graph/v1/__init__.py
+-rw-r--r--   0        0        0    11861 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.py
+-rw-r--r--   0        0        0    33449 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2_grpc.py
+-rw-r--r--   0        0        0      151 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.527807 arg_services-1.3.2/src/arg_services/mining/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.527807 arg_services-1.3.2/src/arg_services/mining/v1beta/__init__.py
+-rw-r--r--   0        0        0     5028 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     6692 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     4625 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     1237 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6102 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     8973 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     4721 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0     1298 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4150 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.py
+-rw-r--r--   0        0        0     3932 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
+-rw-r--r--   0        0        0     3092 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3812 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     4057 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     2896 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      856 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2930 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.py
+-rw-r--r--   0        0        0     2419 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.pyi
+-rw-r--r--   0        0        0     2834 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.py
+-rw-r--r--   0        0        0      821 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.531807 arg_services-1.3.2/src/arg_services/mining_explanation/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.535807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/__init__.py
+-rw-r--r--   0        0        0     3371 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     3359 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     3044 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0      916 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4502 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     5167 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     3110 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3857 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     3980 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     3112 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      960 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.531807 arg_services-1.3.2/src/arg_services/nlp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.531807 arg_services-1.3.2/src/arg_services/nlp/v1/__init__.py
+-rw-r--r--   0        0        0     9005 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.py
+-rw-r--r--   0        0        0    27846 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.pyi
+-rw-r--r--   0        0        0     6344 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.519806 arg_services-1.3.2/src/google/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:56:05.519806 arg_services-1.3.2/src/google/api/__init__.py
+-rw-r--r--   0        0        0     1813 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2631 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18295 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 arg_services-1.3.2/PKG-INFO
```

### Comparing `arg_services-1.3.1/LICENSE` & `arg_services-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/README.md` & `arg_services-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/pyproject.toml` & `arg_services-1.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "arg-services"
-version = "1.3.1"
+version = "1.3.2"
 description = "gRPC definitions for microservice-based argumentation machines"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arg-services-python"
 include = ["src/**/*"]
 packages = [
     { include = "arg_services", from = "src" },
-    { include = "google", from = "src" },
+    { include = "google/api", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 grpcio = "^1.53.0"
 protobuf = "^4.22.1"
 grpcio-reflection = "^1.53.0"
```

### Comparing `arg_services-1.3.1/src/arg_services/__init__.py` & `arg_services-1.3.2/src/arg_services/__init__.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.py` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2.pyi` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.py` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2.pyi` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.py` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/model_pb2.pyi` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.py` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2.pyi` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.py` & `arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/graph/v1/graph_pb2.pyi` & `arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.py` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.py` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.py` & `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2.pyi` & `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.py` & `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi` & `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/google/api/annotations_pb2.py` & `arg_services-1.3.2/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/google/api/annotations_pb2.pyi` & `arg_services-1.3.2/src/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/google/api/annotations_pb2_grpc.pyi` & `arg_services-1.3.2/src/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/google/api/http_pb2.py` & `arg_services-1.3.2/src/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/google/api/http_pb2.pyi` & `arg_services-1.3.2/src/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/src/google/api/http_pb2_grpc.pyi` & `arg_services-1.3.2/src/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.1/PKG-INFO` & `arg_services-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arg-services
-Version: 1.3.1
+Version: 1.3.2
 Summary: gRPC definitions for microservice-based argumentation machines
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

