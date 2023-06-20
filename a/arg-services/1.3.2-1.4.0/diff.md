# Comparing `tmp/arg_services-1.3.2.tar.gz` & `tmp/arg_services-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arg_services-1.3.2.tar", max compression
+gzip compressed data, was "arg_services-1.4.0.tar", max compression
```

## Comparing `arg_services-1.3.2.tar` & `arg_services-1.4.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1067 2023-06-12 07:55:34.199488 arg_services-1.3.2/LICENSE
--rw-r--r--   0        0        0      657 2023-06-12 07:55:34.199488 arg_services-1.3.2/README.md
--rw-r--r--   0        0        0      675 2023-06-12 07:56:06.627819 arg_services-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     7288 2023-06-12 07:56:05.543807 arg_services-1.3.2/src/arg_services/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.523806 arg_services-1.3.2/src/arg_services/cbr/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.527807 arg_services-1.3.2/src/arg_services/cbr/v1beta/__init__.py
--rw-r--r--   0        0        0     7099 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.py
--rw-r--r--   0        0        0    12424 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
--rw-r--r--   0        0        0     2783 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
--rw-r--r--   0        0        0     3416 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.py
--rw-r--r--   0        0        0     3094 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
--rw-r--r--   0        0        0     2519 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.py
--rw-r--r--   0        0        0     2515 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
--rw-r--r--   0        0        0     8286 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.py
--rw-r--r--   0        0        0    15179 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
--rw-r--r--   0        0        0     4628 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
--rw-r--r--   0        0        0     1252 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.535807 arg_services-1.3.2/src/arg_services/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.539807 arg_services-1.3.2/src/arg_services/graph/v1/__init__.py
--rw-r--r--   0        0        0    11861 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.py
--rw-r--r--   0        0        0    33449 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2_grpc.py
--rw-r--r--   0        0        0      151 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.527807 arg_services-1.3.2/src/arg_services/mining/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.527807 arg_services-1.3.2/src/arg_services/mining/v1beta/__init__.py
--rw-r--r--   0        0        0     5028 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     6692 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     4625 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     1237 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     6102 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     8973 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     4721 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1298 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     4150 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.py
--rw-r--r--   0        0        0     3932 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
--rw-r--r--   0        0        0     3092 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
--rw-r--r--   0        0        0     3812 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     4057 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     2896 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      856 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0     2930 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.py
--rw-r--r--   0        0        0     2419 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.pyi
--rw-r--r--   0        0        0     2834 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.py
--rw-r--r--   0        0        0      821 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.531807 arg_services-1.3.2/src/arg_services/mining_explanation/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.535807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/__init__.py
--rw-r--r--   0        0        0     3371 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     3359 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     3044 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0      916 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     4502 2023-06-12 07:56:05.511806 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     5167 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     3110 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0      961 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     3857 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     3980 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     3112 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0      960 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.531807 arg_services-1.3.2/src/arg_services/nlp/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.531807 arg_services-1.3.2/src/arg_services/nlp/v1/__init__.py
--rw-r--r--   0        0        0     9005 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.py
--rw-r--r--   0        0        0    27846 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.pyi
--rw-r--r--   0        0        0     6344 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.519806 arg_services-1.3.2/src/google/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 07:56:05.519806 arg_services-1.3.2/src/google/api/__init__.py
--rw-r--r--   0        0        0     1813 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2631 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2.py
--rw-r--r--   0        0        0    18295 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-06-12 07:56:05.515807 arg_services-1.3.2/src/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 arg_services-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-20 11:45:57.926421 arg_services-1.4.0/LICENSE
+-rw-r--r--   0        0        0      657 2023-06-20 11:45:57.926421 arg_services-1.4.0/README.md
+-rw-r--r--   0        0        0      675 2023-06-20 11:46:36.038418 arg_services-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7288 2023-06-20 11:46:35.286418 arg_services-1.4.0/src/arg_services/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.278418 arg_services-1.4.0/src/arg_services/cbr/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.282418 arg_services-1.4.0/src/arg_services/cbr/v1beta/__init__.py
+-rw-r--r--   0        0        0     7099 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2.py
+-rw-r--r--   0        0        0    12424 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
+-rw-r--r--   0        0        0     2783 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3416 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2.py
+-rw-r--r--   0        0        0     3094 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2519 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/model_pb2.py
+-rw-r--r--   0        0        0     2515 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/model_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8286 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2.py
+-rw-r--r--   0        0        0    15179 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
+-rw-r--r--   0        0        0     4628 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
+-rw-r--r--   0        0        0     1252 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.274418 arg_services-1.4.0/src/arg_services/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.274418 arg_services-1.4.0/src/arg_services/graph/v1/__init__.py
+-rw-r--r--   0        0        0    11861 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/graph/v1/graph_pb2.py
+-rw-r--r--   0        0        0    33449 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/graph/v1/graph_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-20 11:46:35.258418 arg_services-1.4.0/src/arg_services/graph/v1/graph_pb2_grpc.py
+-rw-r--r--   0        0        0      151 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/graph/v1/graph_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.270418 arg_services-1.4.0/src/arg_services/mining/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.270418 arg_services-1.4.0/src/arg_services/mining/v1beta/__init__.py
+-rw-r--r--   0        0        0     5028 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     6692 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     4625 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     1237 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4950 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     6905 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     2894 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0      857 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4150 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2.py
+-rw-r--r--   0        0        0     3932 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
+-rw-r--r--   0        0        0     3092 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3812 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     4057 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     2896 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      856 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2930 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2.py
+-rw-r--r--   0        0        0     2419 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2.pyi
+-rw-r--r--   0        0        0     2834 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py
+-rw-r--r--   0        0        0      821 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.278418 arg_services-1.4.0/src/arg_services/mining_explanation/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.278418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/__init__.py
+-rw-r--r--   0        0        0     3371 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     3359 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     3044 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0      916 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4502 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     5167 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     3110 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0      961 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3857 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     3980 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     3112 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0      960 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.270418 arg_services-1.4.0/src/arg_services/nlp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.274418 arg_services-1.4.0/src/arg_services/nlp/v1/__init__.py
+-rw-r--r--   0        0        0     9005 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2.py
+-rw-r--r--   0        0        0    27846 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2.pyi
+-rw-r--r--   0        0        0     6344 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.282418 arg_services-1.4.0/src/google/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 11:46:35.282418 arg_services-1.4.0/src/google/api/__init__.py
+-rw-r--r--   0        0        0     1813 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2631 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18295 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-06-20 11:46:35.262418 arg_services-1.4.0/src/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 arg_services-1.4.0/PKG-INFO
```

### Comparing `arg_services-1.3.2/LICENSE` & `arg_services-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/README.md` & `arg_services-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/pyproject.toml` & `arg_services-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arg-services"
-version = "1.3.2"
+version = "1.4.0"
 description = "gRPC definitions for microservice-based argumentation machines"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arg-services-python"
 include = ["src/**/*"]
```

### Comparing `arg_services-1.3.2/src/arg_services/__init__.py` & `arg_services-1.4.0/src/arg_services/__init__.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.py` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from arg_services.cbr.v1beta import model_pb2 as arg__services_dot_cbr_dot_v1beta_dot_model__pb2
 from arg_services.cbr.v1beta import retrieval_pb2 as arg__services_dot_cbr_dot_v1beta_dot_retrieval__pb2
 from arg_services.nlp.v1 import nlp_pb2 as arg__services_dot_nlp_dot_v1_dot_nlp__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(arg_services/cbr/v1beta/adaptation.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\'arg_services/cbr/v1beta/retrieval.proto\x1a\x1d\x61rg_services/nlp/v1/nlp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xae\x03\n\x0c\x41\x64\x61ptRequest\x12\x46\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\x30.arg_services.cbr.v1beta.AdaptRequest.CasesEntryR\x05\x63\x61ses\x12=\n\x05query\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05query\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12@\n\tdirection\x18\x06 \x01(\x0e\x32\".arg_services.cbr.v1beta.DirectionR\tdirection\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x65\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x41\n\x05value\x18\x02 \x01(\x0b\x32+.arg_services.cbr.v1beta.AdaptedCaseRequestR\x05value:\x02\x38\x01\"\xf1\x01\n\rAdaptResponse\x12G\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x31.arg_services.cbr.v1beta.AdaptResponse.CasesEntryR\x05\x63\x61ses\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x66\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x42\n\x05value\x18\x02 \x01(\x0b\x32,.arg_services.cbr.v1beta.AdaptedCaseResponseR\x05value:\x02\x38\x01\"\xdc\x01\n\x12\x41\x64\x61ptedCaseRequest\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12\x33\n\x05rules\x18\x02 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x05rules\x12H\n\x07mapping\x18\x03 \x01(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingH\x00R\x07mapping\x88\x01\x01\x42\n\n\x08_mapping\"\x9a\x04\n\x13\x41\x64\x61ptedCaseResponse\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12O\n\x12\x65xtracted_concepts\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x65xtractedConcepts\x12O\n\x12\x64iscarded_concepts\x18\x03 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x64iscardedConcepts\x12\x42\n\rapplied_rules\x18\x04 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0c\x61ppliedRules\x12\x46\n\x0f\x64iscarded_rules\x18\x05 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0e\x64iscardedRules\x12\x46\n\x0fgenerated_rules\x18\x07 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0egeneratedRules\x12P\n\x0frule_candidates\x18\x06 \x03(\x0b\x32\'.arg_services.cbr.v1beta.RuleCandidatesR\x0eruleCandidates\"z\n\x04Rule\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target\"e\n\x07\x43oncept\x12\x14\n\x05lemma\x18\x01 \x01(\tR\x05lemma\x12.\n\x03pos\x18\x02 \x01(\x0e\x32\x1c.arg_services.cbr.v1beta.PosR\x03pos\x12\x14\n\x05score\x18\x03 \x01(\x01R\x05score\"\x84\x01\n\x0eRuleCandidates\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target*z\n\tDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x44IRECTION_GENERALIZATION\x10\x01\x12\x1c\n\x18\x44IRECTION_SPECIALIZATION\x10\x02\x12\x16\n\x12\x44IRECTION_COMBINED\x10\x03*Y\n\x03Pos\x12\x13\n\x0fPOS_UNSPECIFIED\x10\x00\x12\x0c\n\x08POS_NOUN\x10\x01\x12\x0c\n\x08POS_VERB\x10\x02\x12\x11\n\rPOS_ADJECTIVE\x10\x03\x12\x0e\n\nPOS_ADVERB\x10\x04\x32\x89\x01\n\x11\x41\x64\x61ptationService\x12t\n\x05\x41\x64\x61pt\x12%.arg_services.cbr.v1beta.AdaptRequest\x1a&.arg_services.cbr.v1beta.AdaptResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/cbr/v1beta/adaptB\xa8\x01\n\x1b\x63om.arg_services.cbr.v1betaB\x0f\x41\x64\x61ptationProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(arg_services/cbr/v1beta/adaptation.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\'arg_services/cbr/v1beta/retrieval.proto\x1a\x1d\x61rg_services/nlp/v1/nlp.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xae\x03\n\x0c\x41\x64\x61ptRequest\x12\x46\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\x30.arg_services.cbr.v1beta.AdaptRequest.CasesEntryR\x05\x63\x61ses\x12=\n\x05query\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05query\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12@\n\tdirection\x18\x06 \x01(\x0e\x32\".arg_services.cbr.v1beta.DirectionR\tdirection\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x65\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x41\n\x05value\x18\x02 \x01(\x0b\x32+.arg_services.cbr.v1beta.AdaptedCaseRequestR\x05value:\x02\x38\x01\"\xf1\x01\n\rAdaptResponse\x12G\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x31.arg_services.cbr.v1beta.AdaptResponse.CasesEntryR\x05\x63\x61ses\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x66\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x42\n\x05value\x18\x02 \x01(\x0b\x32,.arg_services.cbr.v1beta.AdaptedCaseResponseR\x05value:\x02\x38\x01\"\xdc\x01\n\x12\x41\x64\x61ptedCaseRequest\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12\x33\n\x05rules\x18\x02 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x05rules\x12H\n\x07mapping\x18\x03 \x01(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingH\x00R\x07mapping\x88\x01\x01\x42\n\n\x08_mapping\"\x9a\x04\n\x13\x41\x64\x61ptedCaseResponse\x12;\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x04\x63\x61se\x12O\n\x12\x65xtracted_concepts\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x65xtractedConcepts\x12O\n\x12\x64iscarded_concepts\x18\x03 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x11\x64iscardedConcepts\x12\x42\n\rapplied_rules\x18\x04 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0c\x61ppliedRules\x12\x46\n\x0f\x64iscarded_rules\x18\x05 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0e\x64iscardedRules\x12\x46\n\x0fgenerated_rules\x18\x07 \x03(\x0b\x32\x1d.arg_services.cbr.v1beta.RuleR\x0egeneratedRules\x12P\n\x0frule_candidates\x18\x06 \x03(\x0b\x32\'.arg_services.cbr.v1beta.RuleCandidatesR\x0eruleCandidates\"z\n\x04Rule\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target\"e\n\x07\x43oncept\x12\x14\n\x05lemma\x18\x01 \x01(\tR\x05lemma\x12.\n\x03pos\x18\x02 \x01(\x0e\x32\x1c.arg_services.cbr.v1beta.PosR\x03pos\x12\x14\n\x05score\x18\x03 \x01(\x01R\x05score\"\x84\x01\n\x0eRuleCandidates\x12\x38\n\x06source\x18\x01 \x01(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06source\x12\x38\n\x06target\x18\x02 \x03(\x0b\x32 .arg_services.cbr.v1beta.ConceptR\x06target*z\n\tDirection\x12\x19\n\x15\x44IRECTION_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x44IRECTION_GENERALIZATION\x10\x01\x12\x1c\n\x18\x44IRECTION_SPECIALIZATION\x10\x02\x12\x16\n\x12\x44IRECTION_COMBINED\x10\x03*Y\n\x03Pos\x12\x13\n\x0fPOS_UNSPECIFIED\x10\x00\x12\x0c\n\x08POS_NOUN\x10\x01\x12\x0c\n\x08POS_VERB\x10\x02\x12\x11\n\rPOS_ADJECTIVE\x10\x03\x12\x0e\n\nPOS_ADVERB\x10\x04\x32\x89\x01\n\x11\x41\x64\x61ptationService\x12t\n\x05\x41\x64\x61pt\x12%.arg_services.cbr.v1beta.AdaptRequest\x1a&.arg_services.cbr.v1beta.AdaptResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/cbr/v1beta/adaptB\xa8\x01\n\x1b\x63om.arg_services.cbr.v1betaB\x0f\x41\x64\x61ptationProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.adaptation_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2.pyi` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.py` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from arg_services.cbr.v1beta import model_pb2 as arg__services_dot_cbr_dot_v1beta_dot_model__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&arg_services/cbr/v1beta/casebase.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xc8\x01\n\x0f\x43\x61sebaseRequest\x12\x41\n\x07include\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x07include\x12\x41\n\x07\x65xclude\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x07\x65xclude\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xc1\x01\n\x10\x43\x61sebaseResponse\x12J\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x34.arg_services.cbr.v1beta.CasebaseResponse.CasesEntryR\x05\x63\x61ses\x1a\x61\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12=\n\x05value\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05value:\x02\x38\x01\x32\x94\x01\n\x0f\x43\x61sebaseService\x12\x80\x01\n\x08\x43\x61sebase\x12(.arg_services.cbr.v1beta.CasebaseRequest\x1a).arg_services.cbr.v1beta.CasebaseResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/cbr/v1beta/casebaseB\xa6\x01\n\x1b\x63om.arg_services.cbr.v1betaB\rCasebaseProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&arg_services/cbr/v1beta/casebase.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xc8\x01\n\x0f\x43\x61sebaseRequest\x12\x41\n\x07include\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x07include\x12\x41\n\x07\x65xclude\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x07\x65xclude\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xc1\x01\n\x10\x43\x61sebaseResponse\x12J\n\x05\x63\x61ses\x18\x01 \x03(\x0b\x32\x34.arg_services.cbr.v1beta.CasebaseResponse.CasesEntryR\x05\x63\x61ses\x1a\x61\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12=\n\x05value\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05value:\x02\x38\x01\x32\x94\x01\n\x0f\x43\x61sebaseService\x12\x80\x01\n\x08\x43\x61sebase\x12(.arg_services.cbr.v1beta.CasebaseRequest\x1a).arg_services.cbr.v1beta.CasebaseResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/cbr/v1beta/casebaseB\xa6\x01\n\x1b\x63om.arg_services.cbr.v1betaB\rCasebaseProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.casebase_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2.pyi` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.py` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/model_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/model_pb2.pyi` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.py` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from arg_services.cbr.v1beta import model_pb2 as arg__services_dot_cbr_dot_v1beta_dot_model__pb2
 from arg_services.nlp.v1 import nlp_pb2 as arg__services_dot_nlp_dot_v1_dot_nlp__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'arg_services/cbr/v1beta/retrieval.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\x1d\x61rg_services/nlp/v1/nlp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xa2\x06\n\x0fRetrieveRequest\x12P\n\x0f\x63\x61sebase_filter\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x0e\x63\x61sebaseFilter\x12I\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\x33.arg_services.cbr.v1beta.RetrieveRequest.CasesEntryR\x05\x63\x61ses\x12\x41\n\x07queries\x18\x03 \x03(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x07queries\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12\x14\n\x05limit\x18\x06 \x01(\x05R\x05limit\x12-\n\x12semantic_retrieval\x18\x07 \x01(\x08R\x11semanticRetrieval\x12\x31\n\x14structural_retrieval\x18\x08 \x01(\x08R\x13structuralRetrieval\x12V\n\x11mapping_algorithm\x18\t \x01(\x0e\x32).arg_services.cbr.v1beta.MappingAlgorithmR\x10mappingAlgorithm\x12:\n\x19mapping_algorithm_variant\x18\n \x01(\x05R\x17mappingAlgorithmVariant\x12P\n\x0fscheme_handling\x18\x0b \x01(\x0e\x32\'.arg_services.cbr.v1beta.SchemeHandlingR\x0eschemeHandling\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x61\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12=\n\x05value\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05value:\x02\x38\x01\"\x94\x01\n\x10RetrieveResponse\x12O\n\x0fquery_responses\x18\x01 \x03(\x0b\x32&.arg_services.cbr.v1beta.QueryResponseR\x0equeryResponses\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x93\x02\n\rQueryResponse\x12Q\n\x10semantic_ranking\x18\x01 \x03(\x0b\x32&.arg_services.cbr.v1beta.RetrievedCaseR\x0fsemanticRanking\x12U\n\x12structural_ranking\x18\x02 \x03(\x0b\x32&.arg_services.cbr.v1beta.RetrievedCaseR\x11structuralRanking\x12X\n\x12structural_mapping\x18\x03 \x03(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingR\x11structuralMapping\"~\n\rRetrievedCase\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1e\n\nsimilarity\x18\x02 \x01(\x01R\nsimilarity\x12=\n\x05graph\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05graph\"\x9b\x01\n\x10RetrievedMapping\x12:\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32&.arg_services.cbr.v1beta.RetrievedCaseR\x04\x63\x61se\x12K\n\rnode_mappings\x18\x02 \x03(\x0b\x32&.arg_services.cbr.v1beta.MappedElementR\x0cnodeMappings\"c\n\rMappedElement\x12\x19\n\x08query_id\x18\x01 \x01(\tR\x07queryId\x12\x17\n\x07\x63\x61se_id\x18\x02 \x01(\tR\x06\x63\x61seId\x12\x1e\n\nsimilarity\x18\x03 \x01(\x01R\nsimilarity\"\x89\x04\n\x13SimilaritiesRequest\x12=\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05\x63\x61ses\x12=\n\x05query\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05query\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12\x1e\n\nstructural\x18\x07 \x01(\x08R\nstructural\x12V\n\x11mapping_algorithm\x18\t \x01(\x0e\x32).arg_services.cbr.v1beta.MappingAlgorithmR\x10mappingAlgorithm\x12:\n\x19mapping_algorithm_variant\x18\n \x01(\x05R\x17mappingAlgorithmVariant\x12P\n\x0fscheme_handling\x18\x0b \x01(\x0e\x32\'.arg_services.cbr.v1beta.SchemeHandlingR\x0eschemeHandling\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x98\x01\n\x14SimilaritiesResponse\x12O\n\x0csimilarities\x18\x01 \x03(\x0b\x32+.arg_services.cbr.v1beta.SimilarityResponseR\x0csimilarities\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xd4\x01\n\x12SimilarityResponse\x12/\n\x13semantic_similarity\x18\x01 \x01(\x01R\x12semanticSimilarity\x12\x33\n\x15structural_similarity\x18\x02 \x01(\x01R\x14structuralSimilarity\x12X\n\x12structural_mapping\x18\x03 \x03(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingR\x11structuralMapping*\x93\x01\n\x10MappingAlgorithm\x12!\n\x1dMAPPING_ALGORITHM_UNSPECIFIED\x10\x00\x12\x1b\n\x17MAPPING_ALGORITHM_ASTAR\x10\x01\x12\x1c\n\x18MAPPING_ALGORITHM_GREEDY\x10\x02\x12!\n\x1dMAPPING_ALGORITHM_ISOMORPHISM\x10\x03*k\n\x0eSchemeHandling\x12\x1f\n\x1bSCHEME_HANDLING_UNSPECIFIED\x10\x00\x12\x1a\n\x16SCHEME_HANDLING_BINARY\x10\x01\x12\x1c\n\x18SCHEME_HANDLING_TAXONOMY\x10\x02\x32\x9f\x02\n\x10RetrievalService\x12|\n\x08Retrieve\x12(.arg_services.cbr.v1beta.RetrieveRequest\x1a).arg_services.cbr.v1beta.RetrieveResponse\"\x1b\x82\xd3\xe4\x93\x02\x15:\x01*\"\x10/crb/v1/retrieve\x12\x8c\x01\n\x0cSimilarities\x12,.arg_services.cbr.v1beta.SimilaritiesRequest\x1a-.arg_services.cbr.v1beta.SimilaritiesResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/crb/v1/similaritiesB\xa7\x01\n\x1b\x63om.arg_services.cbr.v1betaB\x0eRetrievalProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'arg_services/cbr/v1beta/retrieval.proto\x12\x17\x61rg_services.cbr.v1beta\x1a#arg_services/cbr/v1beta/model.proto\x1a\x1d\x61rg_services/nlp/v1/nlp.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xa2\x06\n\x0fRetrieveRequest\x12P\n\x0f\x63\x61sebase_filter\x18\x01 \x01(\x0b\x32\'.arg_services.cbr.v1beta.CasebaseFilterR\x0e\x63\x61sebaseFilter\x12I\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\x33.arg_services.cbr.v1beta.RetrieveRequest.CasesEntryR\x05\x63\x61ses\x12\x41\n\x07queries\x18\x03 \x03(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x07queries\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12\x14\n\x05limit\x18\x06 \x01(\x05R\x05limit\x12-\n\x12semantic_retrieval\x18\x07 \x01(\x08R\x11semanticRetrieval\x12\x31\n\x14structural_retrieval\x18\x08 \x01(\x08R\x13structuralRetrieval\x12V\n\x11mapping_algorithm\x18\t \x01(\x0e\x32).arg_services.cbr.v1beta.MappingAlgorithmR\x10mappingAlgorithm\x12:\n\x19mapping_algorithm_variant\x18\n \x01(\x05R\x17mappingAlgorithmVariant\x12P\n\x0fscheme_handling\x18\x0b \x01(\x0e\x32\'.arg_services.cbr.v1beta.SchemeHandlingR\x0eschemeHandling\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\x61\n\nCasesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12=\n\x05value\x18\x02 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05value:\x02\x38\x01\"\x94\x01\n\x10RetrieveResponse\x12O\n\x0fquery_responses\x18\x01 \x03(\x0b\x32&.arg_services.cbr.v1beta.QueryResponseR\x0equeryResponses\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x93\x02\n\rQueryResponse\x12Q\n\x10semantic_ranking\x18\x01 \x03(\x0b\x32&.arg_services.cbr.v1beta.RetrievedCaseR\x0fsemanticRanking\x12U\n\x12structural_ranking\x18\x02 \x03(\x0b\x32&.arg_services.cbr.v1beta.RetrievedCaseR\x11structuralRanking\x12X\n\x12structural_mapping\x18\x03 \x03(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingR\x11structuralMapping\"~\n\rRetrievedCase\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1e\n\nsimilarity\x18\x02 \x01(\x01R\nsimilarity\x12=\n\x05graph\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05graph\"\x9b\x01\n\x10RetrievedMapping\x12:\n\x04\x63\x61se\x18\x01 \x01(\x0b\x32&.arg_services.cbr.v1beta.RetrievedCaseR\x04\x63\x61se\x12K\n\rnode_mappings\x18\x02 \x03(\x0b\x32&.arg_services.cbr.v1beta.MappedElementR\x0cnodeMappings\"c\n\rMappedElement\x12\x19\n\x08query_id\x18\x01 \x01(\tR\x07queryId\x12\x17\n\x07\x63\x61se_id\x18\x02 \x01(\tR\x06\x63\x61seId\x12\x1e\n\nsimilarity\x18\x03 \x01(\x01R\nsimilarity\"\x89\x04\n\x13SimilaritiesRequest\x12=\n\x05\x63\x61ses\x18\x02 \x03(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05\x63\x61ses\x12=\n\x05query\x18\x03 \x01(\x0b\x32\'.arg_services.cbr.v1beta.AnnotatedGraphR\x05query\x12=\n\nnlp_config\x18\x05 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\tnlpConfig\x12\x1e\n\nstructural\x18\x07 \x01(\x08R\nstructural\x12V\n\x11mapping_algorithm\x18\t \x01(\x0e\x32).arg_services.cbr.v1beta.MappingAlgorithmR\x10mappingAlgorithm\x12:\n\x19mapping_algorithm_variant\x18\n \x01(\x05R\x17mappingAlgorithmVariant\x12P\n\x0fscheme_handling\x18\x0b \x01(\x0e\x32\'.arg_services.cbr.v1beta.SchemeHandlingR\x0eschemeHandling\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x98\x01\n\x14SimilaritiesResponse\x12O\n\x0csimilarities\x18\x01 \x03(\x0b\x32+.arg_services.cbr.v1beta.SimilarityResponseR\x0csimilarities\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xd4\x01\n\x12SimilarityResponse\x12/\n\x13semantic_similarity\x18\x01 \x01(\x01R\x12semanticSimilarity\x12\x33\n\x15structural_similarity\x18\x02 \x01(\x01R\x14structuralSimilarity\x12X\n\x12structural_mapping\x18\x03 \x03(\x0b\x32).arg_services.cbr.v1beta.RetrievedMappingR\x11structuralMapping*\x93\x01\n\x10MappingAlgorithm\x12!\n\x1dMAPPING_ALGORITHM_UNSPECIFIED\x10\x00\x12\x1b\n\x17MAPPING_ALGORITHM_ASTAR\x10\x01\x12\x1c\n\x18MAPPING_ALGORITHM_GREEDY\x10\x02\x12!\n\x1dMAPPING_ALGORITHM_ISOMORPHISM\x10\x03*k\n\x0eSchemeHandling\x12\x1f\n\x1bSCHEME_HANDLING_UNSPECIFIED\x10\x00\x12\x1a\n\x16SCHEME_HANDLING_BINARY\x10\x01\x12\x1c\n\x18SCHEME_HANDLING_TAXONOMY\x10\x02\x32\x9f\x02\n\x10RetrievalService\x12|\n\x08Retrieve\x12(.arg_services.cbr.v1beta.RetrieveRequest\x1a).arg_services.cbr.v1beta.RetrieveResponse\"\x1b\x82\xd3\xe4\x93\x02\x15:\x01*\"\x10/crb/v1/retrieve\x12\x8c\x01\n\x0cSimilarities\x12,.arg_services.cbr.v1beta.SimilaritiesRequest\x1a-.arg_services.cbr.v1beta.SimilaritiesResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/crb/v1/similaritiesB\xa7\x01\n\x1b\x63om.arg_services.cbr.v1betaB\x0eRetrievalProtoP\x01\xa2\x02\x03\x41\x43X\xaa\x02\x16\x41rgServices.Cbr.V1beta\xca\x02\x16\x41rgServices\\Cbr\\V1beta\xe2\x02\"ArgServices\\Cbr\\V1beta\\GPBMetadata\xea\x02\x18\x41rgServices::Cbr::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.cbr.v1beta.retrieval_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2.pyi` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.py` & `arg_services-1.4.0/src/arg_services/graph/v1/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/graph/v1/graph_pb2.pyi` & `arg_services-1.4.0/src/arg_services/graph/v1/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$arg_services/mining/v1beta/adu.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"Z\n\x13SegmentationRequest\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x88\x01\n\x14SegmentationResponse\x12?\n\x08segments\x18\x01 \x03(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"E\n\x07Segment\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12\x14\n\x05start\x18\x02 \x01(\x04R\x05start\x12\x10\n\x03\x65nd\x18\x03 \x01(\x04R\x03\x65nd\"\xe2\x01\n\x15\x43lassificationRequest\x12[\n\x08segments\x18\x01 \x03(\x0b\x32?.arg_services.mining.v1beta.ClassificationRequest.SegmentsEntryR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a;\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"~\n\x16\x43lassificationResponse\x12\x33\n\x04\x61\x64us\x18\x01 \x03(\x0b\x32\x1f.arg_services.mining.v1beta.AduR\x04\x61\x64us\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"_\n\x03\x41\x64u\x12\x1d\n\nsegment_id\x18\x01 \x01(\tR\tsegmentId\x12\x39\n\x06tokens\x18\x02 \x03(\x0b\x32!.arg_services.mining.v1beta.TokenR\x06tokens\"[\n\x05Token\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12$\n\rargumentative\x18\x02 \x01(\x08R\rargumentative\x12\x18\n\x07keyword\x18\x03 \x01(\x08R\x07keyword2\xd4\x02\n\nAduService\x12\x9d\x01\n\x0cSegmentation\x12/.arg_services.mining.v1beta.SegmentationRequest\x1a\x30.arg_services.mining.v1beta.SegmentationResponse\"*\x82\xd3\xe4\x93\x02$:\x01*\"\x1f/mining/v1beta/adu/segmentation\x12\xa5\x01\n\x0e\x43lassification\x12\x31.arg_services.mining.v1beta.ClassificationRequest\x1a\x32.arg_services.mining.v1beta.ClassificationResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/mining/v1beta/adu/classificationB\xb0\x01\n\x1e\x63om.arg_services.mining.v1betaB\x08\x41\x64uProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$arg_services/mining/v1beta/adu.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"Z\n\x13SegmentationRequest\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x88\x01\n\x14SegmentationResponse\x12?\n\x08segments\x18\x01 \x03(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"E\n\x07Segment\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12\x14\n\x05start\x18\x02 \x01(\x04R\x05start\x12\x10\n\x03\x65nd\x18\x03 \x01(\x04R\x03\x65nd\"\xe2\x01\n\x15\x43lassificationRequest\x12[\n\x08segments\x18\x01 \x03(\x0b\x32?.arg_services.mining.v1beta.ClassificationRequest.SegmentsEntryR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a;\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"~\n\x16\x43lassificationResponse\x12\x33\n\x04\x61\x64us\x18\x01 \x03(\x0b\x32\x1f.arg_services.mining.v1beta.AduR\x04\x61\x64us\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"_\n\x03\x41\x64u\x12\x1d\n\nsegment_id\x18\x01 \x01(\tR\tsegmentId\x12\x39\n\x06tokens\x18\x02 \x03(\x0b\x32!.arg_services.mining.v1beta.TokenR\x06tokens\"[\n\x05Token\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12$\n\rargumentative\x18\x02 \x01(\x08R\rargumentative\x12\x18\n\x07keyword\x18\x03 \x01(\x08R\x07keyword2\xd4\x02\n\nAduService\x12\x9d\x01\n\x0cSegmentation\x12/.arg_services.mining.v1beta.SegmentationRequest\x1a\x30.arg_services.mining.v1beta.SegmentationResponse\"*\x82\xd3\xe4\x93\x02$:\x01*\"\x1f/mining/v1beta/adu/segmentation\x12\xa5\x01\n\x0e\x43lassification\x12\x31.arg_services.mining.v1beta.ClassificationRequest\x1a\x32.arg_services.mining.v1beta.ClassificationResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/mining/v1beta/adu/classificationB\xb0\x01\n\x1e\x63om.arg_services.mining.v1betaB\x08\x41\x64uProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.adu_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,42 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.mining.v1beta import adu_pb2 as arg__services_dot_mining_dot_v1beta_dot_adu__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+arg_services/mining/v1beta/entailment.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a$arg_services/mining/v1beta/adu.proto\x1a\x1cgoogle/api/annotations.proto\"\x90\x01\n\x11\x45ntailmentRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x18\n\x07premise\x18\x02 \x01(\tR\x07premise\x12\x14\n\x05\x63laim\x18\x03 \x01(\tR\x05\x63laim\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xee\x01\n\x12\x45ntailmentResponse\x12S\n\x0f\x65ntailment_type\x18\x01 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x0e\x65ntailmentType\x12R\n\x0bpredictions\x18\x02 \x03(\x0b\x32\x30.arg_services.mining.v1beta.EntailmentPredictionR\x0bpredictions\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x9d\x02\n\x12\x45ntailmentsRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12X\n\x08segments\x18\x02 \x03(\x0b\x32<.arg_services.mining.v1beta.EntailmentsRequest.SegmentsEntryR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a`\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x8e\x01\n\x13\x45ntailmentsResponse\x12\x46\n\x07results\x18\x01 \x03(\x0b\x32,.arg_services.mining.v1beta.EntailmentResultR\x07results\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xae\x01\n\x10\x45ntailmentResult\x12\x46\n\nentailment\x18\x01 \x01(\x0b\x32&.arg_services.mining.v1beta.EntailmentR\nentailment\x12R\n\x0bpredictions\x18\x02 \x03(\x0b\x32\x30.arg_services.mining.v1beta.EntailmentPredictionR\x0bpredictions\"\x86\x01\n\nEntailment\x12\x1d\n\npremise_id\x18\x01 \x01(\tR\tpremiseId\x12\x19\n\x08\x63laim_id\x18\x02 \x01(\tR\x07\x63laimId\x12>\n\x04type\x18\x03 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type\"x\n\x14\x45ntailmentPrediction\x12 \n\x0bprobability\x18\x01 \x01(\x01R\x0bprobability\x12>\n\x04type\x18\x02 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type*\x91\x01\n\x0e\x45ntailmentType\x12\x1f\n\x1b\x45NTAILMENT_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x45NTAILMENT_TYPE_ENTAILMENT\x10\x01\x12!\n\x1d\x45NTAILMENT_TYPE_CONTRADICTION\x10\x02\x12\x1b\n\x17\x45NTAILMENT_TYPE_NEUTRAL\x10\x03\x32\xbf\x02\n\x11\x45ntailmentService\x12\x91\x01\n\nEntailment\x12-.arg_services.mining.v1beta.EntailmentRequest\x1a..arg_services.mining.v1beta.EntailmentResponse\"$\x82\xd3\xe4\x93\x02\x1e:\x01*\"\x19/mining/v1beta/entailment\x12\x95\x01\n\x0b\x45ntailments\x12..arg_services.mining.v1beta.EntailmentsRequest\x1a/.arg_services.mining.v1beta.EntailmentsResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/mining/v1beta/entailmentsB\xb7\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0f\x45ntailmentProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+arg_services/mining/v1beta/entailment.proto\x12\x1a\x61rg_services.mining.v1beta\x1a$arg_services/mining/v1beta/adu.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xd0\x02\n\x12\x45ntailmentsRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12L\n\x04\x61\x64us\x18\x02 \x03(\x0b\x32\x38.arg_services.mining.v1beta.EntailmentsRequest.AdusEntryR\x04\x61\x64us\x12\x41\n\x05query\x18\x03 \x03(\x0b\x32+.arg_services.mining.v1beta.EntailmentQueryR\x05query\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\\\n\tAdusEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x90\x01\n\x13\x45ntailmentsResponse\x12H\n\x0b\x65ntailments\x18\x01 \x03(\x0b\x32&.arg_services.mining.v1beta.EntailmentR\x0b\x65ntailments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"K\n\x0f\x45ntailmentQuery\x12\x1d\n\npremise_id\x18\x01 \x01(\tR\tpremiseId\x12\x19\n\x08\x63laim_id\x18\x02 \x01(\tR\x07\x63laimId\"\xda\x01\n\nEntailment\x12>\n\x04type\x18\x01 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type\x12R\n\x0bpredictions\x18\x02 \x03(\x0b\x32\x30.arg_services.mining.v1beta.EntailmentPredictionR\x0bpredictions\x12\x1d\n\npremise_id\x18\x03 \x01(\tR\tpremiseId\x12\x19\n\x08\x63laim_id\x18\x04 \x01(\tR\x07\x63laimId\"x\n\x14\x45ntailmentPrediction\x12 \n\x0bprobability\x18\x01 \x01(\x01R\x0bprobability\x12>\n\x04type\x18\x02 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type*\x91\x01\n\x0e\x45ntailmentType\x12\x1f\n\x1b\x45NTAILMENT_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x45NTAILMENT_TYPE_ENTAILMENT\x10\x01\x12!\n\x1d\x45NTAILMENT_TYPE_CONTRADICTION\x10\x02\x12\x1b\n\x17\x45NTAILMENT_TYPE_NEUTRAL\x10\x03\x32\xab\x01\n\x11\x45ntailmentService\x12\x95\x01\n\x0b\x45ntailments\x12..arg_services.mining.v1beta.EntailmentsRequest\x1a/.arg_services.mining.v1beta.EntailmentsResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/mining/v1beta/entailmentsB\xb7\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0f\x45ntailmentProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.entailment_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\036com.arg_services.mining.v1betaB\017EntailmentProtoP\001\242\002\003AMX\252\002\031ArgServices.Mining.V1beta\312\002\031ArgServices\\Mining\\V1beta\342\002%ArgServices\\Mining\\V1beta\\GPBMetadata\352\002\033ArgServices::Mining::V1beta'
-  _ENTAILMENTSREQUEST_SEGMENTSENTRY._options = None
-  _ENTAILMENTSREQUEST_SEGMENTSENTRY._serialized_options = b'8\001'
-  _ENTAILMENTSERVICE.methods_by_name['Entailment']._options = None
-  _ENTAILMENTSERVICE.methods_by_name['Entailment']._serialized_options = b'\202\323\344\223\002\036:\001*\"\031/mining/v1beta/entailment'
+  _ENTAILMENTSREQUEST_ADUSENTRY._options = None
+  _ENTAILMENTSREQUEST_ADUSENTRY._serialized_options = b'8\001'
   _ENTAILMENTSERVICE.methods_by_name['Entailments']._options = None
   _ENTAILMENTSERVICE.methods_by_name['Entailments']._serialized_options = b'\202\323\344\223\002\037:\001*\"\032/mining/v1beta/entailments'
-  _globals['_ENTAILMENTTYPE']._serialized_start=1431
-  _globals['_ENTAILMENTTYPE']._serialized_end=1576
-  _globals['_ENTAILMENTREQUEST']._serialized_start=174
-  _globals['_ENTAILMENTREQUEST']._serialized_end=318
-  _globals['_ENTAILMENTRESPONSE']._serialized_start=321
-  _globals['_ENTAILMENTRESPONSE']._serialized_end=559
-  _globals['_ENTAILMENTSREQUEST']._serialized_start=562
-  _globals['_ENTAILMENTSREQUEST']._serialized_end=847
-  _globals['_ENTAILMENTSREQUEST_SEGMENTSENTRY']._serialized_start=751
-  _globals['_ENTAILMENTSREQUEST_SEGMENTSENTRY']._serialized_end=847
-  _globals['_ENTAILMENTSRESPONSE']._serialized_start=850
-  _globals['_ENTAILMENTSRESPONSE']._serialized_end=992
-  _globals['_ENTAILMENTRESULT']._serialized_start=995
-  _globals['_ENTAILMENTRESULT']._serialized_end=1169
-  _globals['_ENTAILMENT']._serialized_start=1172
-  _globals['_ENTAILMENT']._serialized_end=1306
-  _globals['_ENTAILMENTPREDICTION']._serialized_start=1308
-  _globals['_ENTAILMENTPREDICTION']._serialized_end=1428
-  _globals['_ENTAILMENTSERVICE']._serialized_start=1579
-  _globals['_ENTAILMENTSERVICE']._serialized_end=1898
+  _globals['_ENTAILMENTTYPE']._serialized_start=1080
+  _globals['_ENTAILMENTTYPE']._serialized_end=1225
+  _globals['_ENTAILMENTSREQUEST']._serialized_start=174
+  _globals['_ENTAILMENTSREQUEST']._serialized_end=510
+  _globals['_ENTAILMENTSREQUEST_ADUSENTRY']._serialized_start=418
+  _globals['_ENTAILMENTSREQUEST_ADUSENTRY']._serialized_end=510
+  _globals['_ENTAILMENTSRESPONSE']._serialized_start=513
+  _globals['_ENTAILMENTSRESPONSE']._serialized_end=657
+  _globals['_ENTAILMENTQUERY']._serialized_start=659
+  _globals['_ENTAILMENTQUERY']._serialized_end=734
+  _globals['_ENTAILMENT']._serialized_start=737
+  _globals['_ENTAILMENT']._serialized_end=955
+  _globals['_ENTAILMENTPREDICTION']._serialized_start=957
+  _globals['_ENTAILMENTPREDICTION']._serialized_end=1077
+  _globals['_ENTAILMENTSERVICE']._serialized_start=1228
+  _globals['_ENTAILMENTSERVICE']._serialized_end=1399
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -36,71 +36,19 @@
 ENTAILMENT_TYPE_UNSPECIFIED: EntailmentType.ValueType  # 0
 ENTAILMENT_TYPE_ENTAILMENT: EntailmentType.ValueType  # 1
 ENTAILMENT_TYPE_CONTRADICTION: EntailmentType.ValueType  # 2
 ENTAILMENT_TYPE_NEUTRAL: EntailmentType.ValueType  # 3
 global___EntailmentType = EntailmentType
 
 @typing_extensions.final
-class EntailmentRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    LANGUAGE_FIELD_NUMBER: builtins.int
-    PREMISE_FIELD_NUMBER: builtins.int
-    CLAIM_FIELD_NUMBER: builtins.int
-    EXTRAS_FIELD_NUMBER: builtins.int
-    language: builtins.str
-    premise: builtins.str
-    claim: builtins.str
-    @property
-    def extras(self) -> google.protobuf.struct_pb2.Struct:
-        """Implementation-specific information can be encoded here"""
-    def __init__(
-        self,
-        *,
-        language: builtins.str = ...,
-        premise: builtins.str = ...,
-        claim: builtins.str = ...,
-        extras: google.protobuf.struct_pb2.Struct | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["claim", b"claim", "extras", b"extras", "language", b"language", "premise", b"premise"]) -> None: ...
-
-global___EntailmentRequest = EntailmentRequest
-
-@typing_extensions.final
-class EntailmentResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    ENTAILMENT_TYPE_FIELD_NUMBER: builtins.int
-    PREDICTIONS_FIELD_NUMBER: builtins.int
-    EXTRAS_FIELD_NUMBER: builtins.int
-    entailment_type: global___EntailmentType.ValueType
-    @property
-    def predictions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntailmentPrediction]: ...
-    @property
-    def extras(self) -> google.protobuf.struct_pb2.Struct:
-        """Implementation-specific information can be encoded here"""
-    def __init__(
-        self,
-        *,
-        entailment_type: global___EntailmentType.ValueType = ...,
-        predictions: collections.abc.Iterable[global___EntailmentPrediction] | None = ...,
-        extras: google.protobuf.struct_pb2.Struct | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["entailment_type", b"entailment_type", "extras", b"extras", "predictions", b"predictions"]) -> None: ...
-
-global___EntailmentResponse = EntailmentResponse
-
-@typing_extensions.final
 class EntailmentsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
-    class SegmentsEntry(google.protobuf.message.Message):
+    class AdusEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> arg_services.mining.v1beta.adu_pb2.Segment: ...
@@ -110,95 +58,100 @@
             key: builtins.str = ...,
             value: arg_services.mining.v1beta.adu_pb2.Segment | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     LANGUAGE_FIELD_NUMBER: builtins.int
-    SEGMENTS_FIELD_NUMBER: builtins.int
+    ADUS_FIELD_NUMBER: builtins.int
+    QUERY_FIELD_NUMBER: builtins.int
     EXTRAS_FIELD_NUMBER: builtins.int
     language: builtins.str
     @property
-    def segments(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, arg_services.mining.v1beta.adu_pb2.Segment]: ...
+    def adus(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, arg_services.mining.v1beta.adu_pb2.Segment]: ...
+    @property
+    def query(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntailmentQuery]: ...
     @property
     def extras(self) -> google.protobuf.struct_pb2.Struct:
         """Implementation-specific information can be encoded here"""
     def __init__(
         self,
         *,
         language: builtins.str = ...,
-        segments: collections.abc.Mapping[builtins.str, arg_services.mining.v1beta.adu_pb2.Segment] | None = ...,
+        adus: collections.abc.Mapping[builtins.str, arg_services.mining.v1beta.adu_pb2.Segment] | None = ...,
+        query: collections.abc.Iterable[global___EntailmentQuery] | None = ...,
         extras: google.protobuf.struct_pb2.Struct | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["extras", b"extras", "language", b"language", "segments", b"segments"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["adus", b"adus", "extras", b"extras", "language", b"language", "query", b"query"]) -> None: ...
 
 global___EntailmentsRequest = EntailmentsRequest
 
 @typing_extensions.final
 class EntailmentsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    RESULTS_FIELD_NUMBER: builtins.int
+    ENTAILMENTS_FIELD_NUMBER: builtins.int
     EXTRAS_FIELD_NUMBER: builtins.int
     @property
-    def results(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntailmentResult]: ...
+    def entailments(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Entailment]: ...
     @property
     def extras(self) -> google.protobuf.struct_pb2.Struct:
         """Implementation-specific information can be encoded here"""
     def __init__(
         self,
         *,
-        results: collections.abc.Iterable[global___EntailmentResult] | None = ...,
+        entailments: collections.abc.Iterable[global___Entailment] | None = ...,
         extras: google.protobuf.struct_pb2.Struct | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["extras", b"extras", "results", b"results"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["entailments", b"entailments", "extras", b"extras"]) -> None: ...
 
 global___EntailmentsResponse = EntailmentsResponse
 
 @typing_extensions.final
-class EntailmentResult(google.protobuf.message.Message):
+class EntailmentQuery(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ENTAILMENT_FIELD_NUMBER: builtins.int
-    PREDICTIONS_FIELD_NUMBER: builtins.int
-    @property
-    def entailment(self) -> global___Entailment: ...
-    @property
-    def predictions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntailmentPrediction]: ...
+    PREMISE_ID_FIELD_NUMBER: builtins.int
+    CLAIM_ID_FIELD_NUMBER: builtins.int
+    premise_id: builtins.str
+    claim_id: builtins.str
     def __init__(
         self,
         *,
-        entailment: global___Entailment | None = ...,
-        predictions: collections.abc.Iterable[global___EntailmentPrediction] | None = ...,
+        premise_id: builtins.str = ...,
+        claim_id: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["entailment", b"entailment"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["entailment", b"entailment", "predictions", b"predictions"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["claim_id", b"claim_id", "premise_id", b"premise_id"]) -> None: ...
 
-global___EntailmentResult = EntailmentResult
+global___EntailmentQuery = EntailmentQuery
 
 @typing_extensions.final
 class Entailment(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    TYPE_FIELD_NUMBER: builtins.int
+    PREDICTIONS_FIELD_NUMBER: builtins.int
     PREMISE_ID_FIELD_NUMBER: builtins.int
     CLAIM_ID_FIELD_NUMBER: builtins.int
-    TYPE_FIELD_NUMBER: builtins.int
+    type: global___EntailmentType.ValueType
+    @property
+    def predictions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntailmentPrediction]: ...
     premise_id: builtins.str
     claim_id: builtins.str
-    type: global___EntailmentType.ValueType
     def __init__(
         self,
         *,
+        type: global___EntailmentType.ValueType = ...,
+        predictions: collections.abc.Iterable[global___EntailmentPrediction] | None = ...,
         premise_id: builtins.str = ...,
         claim_id: builtins.str = ...,
-        type: global___EntailmentType.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["claim_id", b"claim_id", "premise_id", b"premise_id", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["claim_id", b"claim_id", "predictions", b"predictions", "premise_id", b"premise_id", "type", b"type"]) -> None: ...
 
 global___Entailment = Entailment
 
 @typing_extensions.final
 class EntailmentPrediction(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,49 +10,33 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.Entailment = channel.unary_unary(
-                '/arg_services.mining.v1beta.EntailmentService/Entailment',
-                request_serializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentRequest.SerializeToString,
-                response_deserializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentResponse.FromString,
-                )
         self.Entailments = channel.unary_unary(
                 '/arg_services.mining.v1beta.EntailmentService/Entailments',
                 request_serializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentsRequest.SerializeToString,
                 response_deserializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentsResponse.FromString,
                 )
 
 
 class EntailmentServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def Entailment(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def Entailments(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_EntailmentServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'Entailment': grpc.unary_unary_rpc_method_handler(
-                    servicer.Entailment,
-                    request_deserializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentRequest.FromString,
-                    response_serializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentResponse.SerializeToString,
-            ),
             'Entailments': grpc.unary_unary_rpc_method_handler(
                     servicer.Entailments,
                     request_deserializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentsRequest.FromString,
                     response_serializer=arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -61,31 +45,14 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class EntailmentService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Entailment(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/arg_services.mining.v1beta.EntailmentService/Entailment',
-            arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentRequest.SerializeToString,
-            arg__services_dot_mining_dot_v1beta_dot_entailment__pb2.EntailmentResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def Entailments(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,21 @@
 """
 import abc
 import arg_services.mining.v1beta.entailment_pb2
 import grpc
 
 class EntailmentServiceStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
-    Entailment: grpc.UnaryUnaryMultiCallable[
-        arg_services.mining.v1beta.entailment_pb2.EntailmentRequest,
-        arg_services.mining.v1beta.entailment_pb2.EntailmentResponse,
-    ]
     Entailments: grpc.UnaryUnaryMultiCallable[
         arg_services.mining.v1beta.entailment_pb2.EntailmentsRequest,
         arg_services.mining.v1beta.entailment_pb2.EntailmentsResponse,
     ]
 
 class EntailmentServiceServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def Entailment(
-        self,
-        request: arg_services.mining.v1beta.entailment_pb2.EntailmentRequest,
-        context: grpc.ServicerContext,
-    ) -> arg_services.mining.v1beta.entailment_pb2.EntailmentResponse: ...
-    @abc.abstractmethod
     def Entailments(
         self,
         request: arg_services.mining.v1beta.entailment_pb2.EntailmentsRequest,
         context: grpc.ServicerContext,
     ) -> arg_services.mining.v1beta.entailment_pb2.EntailmentsResponse: ...
 
 def add_EntailmentServiceServicer_to_server(servicer: EntailmentServiceServicer, server: grpc.Server) -> None: ...
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from arg_services.graph.v1 import graph_pb2 as arg__services_dot_graph_dot_v1_dot_graph__pb2
 from arg_services.mining.v1beta import adu_pb2 as arg__services_dot_mining_dot_v1beta_dot_adu__pb2
 from arg_services.mining.v1beta import entailment_pb2 as arg__services_dot_mining_dot_v1beta_dot_entailment__pb2
-from arg_services.graph.v1 import graph_pb2 as arg__services_dot_graph_dot_v1_dot_graph__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3arg_services/mining/v1beta/graph_construction.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a$arg_services/mining/v1beta/adu.proto\x1a+arg_services/mining/v1beta/entailment.proto\x1a!arg_services/graph/v1/graph.proto\x1a\x1cgoogle/api/annotations.proto\"\x89\x03\n\x18GraphConstructionRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12R\n\x04\x61\x64us\x18\x02 \x03(\x0b\x32>.arg_services.mining.v1beta.GraphConstructionRequest.AdusEntryR\x04\x61\x64us\x12$\n\x0emajor_claim_id\x18\x03 \x01(\tR\x0cmajorClaimId\x12H\n\x0b\x65ntailments\x18\x04 \x03(\x0b\x32&.arg_services.mining.v1beta.EntailmentR\x0b\x65ntailments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\\\n\tAdusEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x80\x01\n\x19GraphConstructionResponse\x12\x32\n\x05graph\x18\x01 \x01(\x0b\x32\x1c.arg_services.graph.v1.GraphR\x05graph\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras2\xcb\x01\n\x18GraphConstructionService\x12\xae\x01\n\x11GraphConstruction\x12\x34.arg_services.mining.v1beta.GraphConstructionRequest\x1a\x35.arg_services.mining.v1beta.GraphConstructionResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/mining/v1beta/graph_constructionB\xbe\x01\n\x1e\x63om.arg_services.mining.v1betaB\x16GraphConstructionProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3arg_services/mining/v1beta/graph_construction.proto\x12\x1a\x61rg_services.mining.v1beta\x1a!arg_services/graph/v1/graph.proto\x1a$arg_services/mining/v1beta/adu.proto\x1a+arg_services/mining/v1beta/entailment.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x89\x03\n\x18GraphConstructionRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12R\n\x04\x61\x64us\x18\x02 \x03(\x0b\x32>.arg_services.mining.v1beta.GraphConstructionRequest.AdusEntryR\x04\x61\x64us\x12$\n\x0emajor_claim_id\x18\x03 \x01(\tR\x0cmajorClaimId\x12H\n\x0b\x65ntailments\x18\x04 \x03(\x0b\x32&.arg_services.mining.v1beta.EntailmentR\x0b\x65ntailments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a\\\n\tAdusEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x80\x01\n\x19GraphConstructionResponse\x12\x32\n\x05graph\x18\x01 \x01(\x0b\x32\x1c.arg_services.graph.v1.GraphR\x05graph\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras2\xcb\x01\n\x18GraphConstructionService\x12\xae\x01\n\x11GraphConstruction\x12\x34.arg_services.mining.v1beta.GraphConstructionRequest\x1a\x35.arg_services.mining.v1beta.GraphConstructionResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/mining/v1beta/graph_constructionB\xbe\x01\n\x1e\x63om.arg_services.mining.v1betaB\x16GraphConstructionProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.graph_construction_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.mining.v1beta import adu_pb2 as arg__services_dot_mining_dot_v1beta_dot_adu__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,arg_services/mining/v1beta/major_claim.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a$arg_services/mining/v1beta/adu.proto\x1a\x1cgoogle/api/annotations.proto\"\xb1\x02\n\x11MajorClaimRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12W\n\x08segments\x18\x02 \x03(\x0b\x32;.arg_services.mining.v1beta.MajorClaimRequest.SegmentsEntryR\x08segments\x12\x14\n\x05limit\x18\x04 \x01(\x04R\x05limit\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a`\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x8d\x01\n\x12MajorClaimResponse\x12\x46\n\x07ranking\x18\x01 \x03(\x0b\x32,.arg_services.mining.v1beta.MajorClaimResultR\x07ranking\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"D\n\x10MajorClaimResult\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12 \n\x0bprobability\x18\x02 \x01(\x01R\x0bprobability2\xa8\x01\n\x11MajorClaimService\x12\x92\x01\n\nMajorClaim\x12-.arg_services.mining.v1beta.MajorClaimRequest\x1a..arg_services.mining.v1beta.MajorClaimResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/mining/v1beta/major_claimB\xb7\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0fMajorClaimProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,arg_services/mining/v1beta/major_claim.proto\x12\x1a\x61rg_services.mining.v1beta\x1a$arg_services/mining/v1beta/adu.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xb1\x02\n\x11MajorClaimRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12W\n\x08segments\x18\x02 \x03(\x0b\x32;.arg_services.mining.v1beta.MajorClaimRequest.SegmentsEntryR\x08segments\x12\x14\n\x05limit\x18\x04 \x01(\x04R\x05limit\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\x1a`\n\rSegmentsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.arg_services.mining.v1beta.SegmentR\x05value:\x02\x38\x01\"\x8d\x01\n\x12MajorClaimResponse\x12\x46\n\x07ranking\x18\x01 \x03(\x0b\x32,.arg_services.mining.v1beta.MajorClaimResultR\x07ranking\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"D\n\x10MajorClaimResult\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12 \n\x0bprobability\x18\x02 \x01(\x01R\x0bprobability2\xa8\x01\n\x11MajorClaimService\x12\x92\x01\n\nMajorClaim\x12-.arg_services.mining.v1beta.MajorClaimRequest\x1a..arg_services.mining.v1beta.MajorClaimResponse\"%\x82\xd3\xe4\x93\x02\x1f:\x01*\"\x1a/mining/v1beta/major_claimB\xb7\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0fMajorClaimProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.major_claim_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.graph.v1 import graph_pb2 as arg__services_dot_graph_dot_v1_dot_graph__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'arg_services/mining/v1beta/mining.proto\x12\x1a\x61rg_services.mining.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a!arg_services/graph/v1/graph.proto\x1a\x1cgoogle/api/annotations.proto\"[\n\x12RunPipelineRequest\x12\x14\n\x05texts\x18\x01 \x03(\tR\x05texts\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"|\n\x13RunPipelineResponse\x12\x34\n\x06graphs\x18\x01 \x03(\x0b\x32\x1c.arg_services.graph.v1.GraphR\x06graphs\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras2\xa8\x01\n\rMiningService\x12\x96\x01\n\x0bRunPipeline\x12..arg_services.mining.v1beta.RunPipelineRequest\x1a/.arg_services.mining.v1beta.RunPipelineResponse\"&\x82\xd3\xe4\x93\x02 :\x01*\"\x1b/mining/v1beta/run_pipelineB\xb3\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0bMiningProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'arg_services/mining/v1beta/mining.proto\x12\x1a\x61rg_services.mining.v1beta\x1a!arg_services/graph/v1/graph.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"[\n\x12RunPipelineRequest\x12\x14\n\x05texts\x18\x01 \x03(\tR\x05texts\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"|\n\x13RunPipelineResponse\x12\x34\n\x06graphs\x18\x01 \x03(\x0b\x32\x1c.arg_services.graph.v1.GraphR\x06graphs\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras2\xa8\x01\n\rMiningService\x12\x96\x01\n\x0bRunPipeline\x12..arg_services.mining.v1beta.RunPipelineRequest\x1a/.arg_services.mining.v1beta.RunPipelineResponse\"&\x82\xd3\xe4\x93\x02 :\x01*\"\x1b/mining/v1beta/run_pipelineB\xb3\x01\n\x1e\x63om.arg_services.mining.v1betaB\x0bMiningProtoP\x01\xa2\x02\x03\x41MX\xaa\x02\x19\x41rgServices.Mining.V1beta\xca\x02\x19\x41rgServices\\Mining\\V1beta\xe2\x02%ArgServices\\Mining\\V1beta\\GPBMetadata\xea\x02\x1b\x41rgServices::Mining::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining.v1beta.mining_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.py` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0arg_services/mining_explanation/v1beta/adu.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\x80\x01\n\x15\x43lassificationRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x1a\n\x08segments\x18\x02 \x03(\tR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x96\x01\n\x16\x43lassificationResponse\x12K\n\x08segments\x18\x01 \x03(\x0b\x32/.arg_services.mining_explanation.v1beta.SegmentR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"L\n\x07Segment\x12\'\n\x0fkeyword_markers\x18\x01 \x03(\x08R\x0ekeywordMarkers\x12\x18\n\x07\x63lauses\x18\x02 \x03(\tR\x07\x63lauses2\xe3\x01\n\x15\x41\x64uExplanationService\x12\xc9\x01\n\x0e\x43lassification\x12=.arg_services.mining_explanation.v1beta.ClassificationRequest\x1a>.arg_services.mining_explanation.v1beta.ClassificationResponse\"8\x82\xd3\xe4\x93\x02\x32:\x01*\"-/mining_explanation/v1beta/adu/classificationB\xe8\x01\n*com.arg_services.mining_explanation.v1betaB\x08\x41\x64uProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0arg_services/mining_explanation/v1beta/adu.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x80\x01\n\x15\x43lassificationRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x1a\n\x08segments\x18\x02 \x03(\tR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x96\x01\n\x16\x43lassificationResponse\x12K\n\x08segments\x18\x01 \x03(\x0b\x32/.arg_services.mining_explanation.v1beta.SegmentR\x08segments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"L\n\x07Segment\x12\'\n\x0fkeyword_markers\x18\x01 \x03(\x08R\x0ekeywordMarkers\x12\x18\n\x07\x63lauses\x18\x02 \x03(\tR\x07\x63lauses2\xe3\x01\n\x15\x41\x64uExplanationService\x12\xc9\x01\n\x0e\x43lassification\x12=.arg_services.mining_explanation.v1beta.ClassificationRequest\x1a>.arg_services.mining_explanation.v1beta.ClassificationResponse\"8\x82\xd3\xe4\x93\x02\x32:\x01*\"-/mining_explanation/v1beta/adu/classificationB\xe8\x01\n*com.arg_services.mining_explanation.v1betaB\x08\x41\x64uProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.adu_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.py` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from arg_services.mining.v1beta import entailment_pb2 as arg__services_dot_mining_dot_v1beta_dot_entailment__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7arg_services/mining_explanation/v1beta/entailment.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a+arg_services/mining/v1beta/entailment.proto\x1a\x1cgoogle/api/annotations.proto\"\xb7\x01\n\x12\x45ntailmentsRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12T\n\x0b\x65ntailments\x18\x02 \x03(\x0b\x32\x32.arg_services.mining_explanation.v1beta.EntailmentR\x0b\x65ntailments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x9a\x01\n\x13\x45ntailmentsResponse\x12R\n\x07results\x18\x01 \x03(\x0b\x32\x38.arg_services.mining_explanation.v1beta.EntailmentResultR\x07results\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"|\n\nEntailment\x12\x18\n\x07premise\x18\x01 \x01(\tR\x07premise\x12\x14\n\x05\x63laim\x18\x02 \x01(\tR\x05\x63laim\x12>\n\x04type\x18\x03 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type\"\x95\x02\n\x10\x45ntailmentResult\x12n\n\x0csimilarities\x18\x01 \x03(\x0b\x32J.arg_services.mining_explanation.v1beta.EntailmentResult.SimilaritiesEntryR\x0csimilarities\x12)\n\x10keywords_premise\x18\x02 \x03(\x08R\x0fkeywordsPremise\x12%\n\x0ekeywords_claim\x18\x03 \x03(\x08R\rkeywordsClaim\x1a?\n\x11SimilaritiesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x01R\x05value:\x02\x38\x01\x32\xda\x01\n\x1c\x45ntailmentExplanationService\x12\xb9\x01\n\x0b\x45ntailments\x12:.arg_services.mining_explanation.v1beta.EntailmentsRequest\x1a;.arg_services.mining_explanation.v1beta.EntailmentsResponse\"1\x82\xd3\xe4\x93\x02+:\x01*\"&/mining_explanation/v1beta/entailmentsB\xef\x01\n*com.arg_services.mining_explanation.v1betaB\x0f\x45ntailmentProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7arg_services/mining_explanation/v1beta/entailment.proto\x12&arg_services.mining_explanation.v1beta\x1a+arg_services/mining/v1beta/entailment.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xb7\x01\n\x12\x45ntailmentsRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12T\n\x0b\x65ntailments\x18\x02 \x03(\x0b\x32\x32.arg_services.mining_explanation.v1beta.EntailmentR\x0b\x65ntailments\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x9a\x01\n\x13\x45ntailmentsResponse\x12R\n\x07results\x18\x01 \x03(\x0b\x32\x38.arg_services.mining_explanation.v1beta.EntailmentResultR\x07results\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"|\n\nEntailment\x12\x18\n\x07premise\x18\x01 \x01(\tR\x07premise\x12\x14\n\x05\x63laim\x18\x02 \x01(\tR\x05\x63laim\x12>\n\x04type\x18\x03 \x01(\x0e\x32*.arg_services.mining.v1beta.EntailmentTypeR\x04type\"\x95\x02\n\x10\x45ntailmentResult\x12n\n\x0csimilarities\x18\x01 \x03(\x0b\x32J.arg_services.mining_explanation.v1beta.EntailmentResult.SimilaritiesEntryR\x0csimilarities\x12)\n\x10keywords_premise\x18\x02 \x03(\x08R\x0fkeywordsPremise\x12%\n\x0ekeywords_claim\x18\x03 \x03(\x08R\rkeywordsClaim\x1a?\n\x11SimilaritiesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x01R\x05value:\x02\x38\x01\x32\xda\x01\n\x1c\x45ntailmentExplanationService\x12\xb9\x01\n\x0b\x45ntailments\x12:.arg_services.mining_explanation.v1beta.EntailmentsRequest\x1a;.arg_services.mining_explanation.v1beta.EntailmentsResponse\"1\x82\xd3\xe4\x93\x02+:\x01*\"&/mining_explanation/v1beta/entailmentsB\xef\x01\n*com.arg_services.mining_explanation.v1betaB\x0f\x45ntailmentProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.entailment_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8arg_services/mining_explanation/v1beta/major_claim.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\x83\x01\n\x11MajorClaimRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12!\n\x0cmajor_claims\x18\x02 \x03(\tR\x0bmajorClaims\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xa2\x01\n\x12MajorClaimResponse\x12[\n\x0cmajor_claims\x18\x01 \x03(\x0b\x32\x38.arg_services.mining_explanation.v1beta.MajorClaimResultR\x0bmajorClaims\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xdf\x01\n\x10MajorClaimResult\x12n\n\x0csimilarities\x18\x01 \x03(\x0b\x32J.arg_services.mining_explanation.v1beta.MajorClaimResult.SimilaritiesEntryR\x0csimilarities\x12\x1a\n\x08keywords\x18\x02 \x03(\x08R\x08keywords\x1a?\n\x11SimilaritiesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x01R\x05value:\x02\x38\x01\x32\xc0\x01\n\x1cMajorClaimExplanationService\x12\x9f\x01\n\nMajorClaim\x12\x39.arg_services.mining_explanation.v1beta.MajorClaimRequest\x1a:.arg_services.mining_explanation.v1beta.MajorClaimResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/nlp/v1/vectorsB\xef\x01\n*com.arg_services.mining_explanation.v1betaB\x0fMajorClaimProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8arg_services/mining_explanation/v1beta/major_claim.proto\x12&arg_services.mining_explanation.v1beta\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x83\x01\n\x11MajorClaimRequest\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12!\n\x0cmajor_claims\x18\x02 \x03(\tR\x0bmajorClaims\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xa2\x01\n\x12MajorClaimResponse\x12[\n\x0cmajor_claims\x18\x01 \x03(\x0b\x32\x38.arg_services.mining_explanation.v1beta.MajorClaimResultR\x0bmajorClaims\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xdf\x01\n\x10MajorClaimResult\x12n\n\x0csimilarities\x18\x01 \x03(\x0b\x32J.arg_services.mining_explanation.v1beta.MajorClaimResult.SimilaritiesEntryR\x0csimilarities\x12\x1a\n\x08keywords\x18\x02 \x03(\x08R\x08keywords\x1a?\n\x11SimilaritiesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x01R\x05value:\x02\x38\x01\x32\xc0\x01\n\x1cMajorClaimExplanationService\x12\x9f\x01\n\nMajorClaim\x12\x39.arg_services.mining_explanation.v1beta.MajorClaimRequest\x1a:.arg_services.mining_explanation.v1beta.MajorClaimResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/nlp/v1/vectorsB\xef\x01\n*com.arg_services.mining_explanation.v1betaB\x0fMajorClaimProtoP\x01\xa2\x02\x03\x41MX\xaa\x02$ArgServices.MiningExplanation.V1beta\xca\x02$ArgServices\\MiningExplanation\\V1beta\xe2\x02\x30\x41rgServices\\MiningExplanation\\V1beta\\GPBMetadata\xea\x02&ArgServices::MiningExplanation::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.mining_explanation.v1beta.major_claim_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.py` & `arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x61rg_services/nlp/v1/nlp.proto\x12\x13\x61rg_services.nlp.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\"\xec\x01\n\tNlpConfig\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x1f\n\x0bspacy_model\x18\x02 \x01(\tR\nspacyModel\x12N\n\x10\x65mbedding_models\x18\x03 \x03(\x0b\x32#.arg_services.nlp.v1.EmbeddingModelR\x0f\x65mbeddingModels\x12R\n\x11similarity_method\x18\x04 \x01(\x0e\x32%.arg_services.nlp.v1.SimilarityMethodR\x10similarityMethod\"\xbf\x01\n\x13SimilaritiesRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12?\n\x0btext_tuples\x18\x02 \x03(\x0b\x32\x1e.arg_services.nlp.v1.TextTupleR\ntextTuples\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"k\n\x14SimilaritiesResponse\x12\"\n\x0csimilarities\x18\x01 \x03(\x01R\x0csimilarities\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"7\n\tTextTuple\x12\x14\n\x05text1\x18\x01 \x01(\tR\x05text1\x12\x14\n\x05text2\x18\x02 \x01(\tR\x05text2\"!\n\x07Strings\x12\x16\n\x06values\x18\x01 \x03(\tR\x06values\"\xc5\x03\n\rDocBinRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12\x41\n\nattributes\x18\x03 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x01R\nattributes\x88\x01\x01\x12\x43\n\renabled_pipes\x18\x04 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\x0c\x65nabledPipes\x12\x45\n\x0e\x64isabled_pipes\x18\x05 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\rdisabledPipes\x12N\n\x10\x65mbedding_levels\x18\x06 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtrasB\x07\n\x05pipesB\r\n\x0b_attributes\"Y\n\x0e\x44ocBinResponse\x12\x16\n\x06\x64ocbin\x18\x01 \x01(\x0cR\x06\x64ocbin\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xdf\x01\n\x0eVectorsRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12N\n\x10\x65mbedding_levels\x18\x03 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x81\x01\n\x0fVectorsResponse\x12=\n\x07vectors\x18\x01 \x03(\x0b\x32#.arg_services.nlp.v1.VectorResponseR\x07vectors\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xea\x01\n\x0eVectorResponse\x12\x37\n\x08\x64ocument\x18\x01 \x01(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x08\x64ocument\x12\x33\n\x06tokens\x18\x02 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x06tokens\x12\x39\n\tsentences\x18\x03 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\tsentences\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\" \n\x06Vector\x12\x16\n\x06vector\x18\x01 \x03(\x01R\x06vector\"\xd8\x01\n\x0e\x45mbeddingModel\x12\x41\n\nmodel_type\x18\x01 \x01(\x0e\x32\".arg_services.nlp.v1.EmbeddingTypeR\tmodelType\x12\x1d\n\nmodel_name\x18\x02 \x01(\tR\tmodelName\x12\x41\n\x0cpooling_type\x18\x03 \x01(\x0e\x32\x1c.arg_services.nlp.v1.PoolingH\x00R\x0bpoolingType\x12\x16\n\x05pmean\x18\x04 \x01(\x01H\x00R\x05pmeanB\t\n\x07pooling*\xe0\x02\n\x10SimilarityMethod\x12!\n\x1dSIMILARITY_METHOD_UNSPECIFIED\x10\x00\x12\x1c\n\x18SIMILARITY_METHOD_COSINE\x10\x01\x12%\n!SIMILARITY_METHOD_DYNAMAX_JACCARD\x10\x02\x12%\n!SIMILARITY_METHOD_MAXPOOL_JACCARD\x10\x03\x12\"\n\x1eSIMILARITY_METHOD_DYNAMAX_DICE\x10\x04\x12$\n SIMILARITY_METHOD_DYNAMAX_OTSUKA\x10\x05\x12\x19\n\x15SIMILARITY_METHOD_WMD\x10\x06\x12\x1a\n\x16SIMILARITY_METHOD_EDIT\x10\x07\x12\x1d\n\x19SIMILARITY_METHOD_JACCARD\x10\x08\x12\x1d\n\x19SIMILARITY_METHOD_ANGULAR\x10\t*\x8a\x01\n\x0e\x45mbeddingLevel\x12\x1f\n\x1b\x45MBEDDING_LEVEL_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45MBEDDING_LEVEL_DOCUMENT\x10\x01\x12\x1a\n\x16\x45MBEDDING_LEVEL_TOKENS\x10\x02\x12\x1d\n\x19\x45MBEDDING_LEVEL_SENTENCES\x10\x03*\xc6\x01\n\x07Pooling\x12\x17\n\x13POOLING_UNSPECIFIED\x10\x00\x12\x10\n\x0cPOOLING_MEAN\x10\x01\x12\x0f\n\x0bPOOLING_MAX\x10\x02\x12\x0f\n\x0bPOOLING_MIN\x10\x03\x12\x0f\n\x0bPOOLING_SUM\x10\x04\x12\x11\n\rPOOLING_FIRST\x10\x05\x12\x10\n\x0cPOOLING_LAST\x10\x06\x12\x12\n\x0ePOOLING_MEDIAN\x10\x07\x12\x11\n\rPOOLING_GMEAN\x10\x08\x12\x11\n\rPOOLING_HMEAN\x10\t*\xd2\x01\n\rEmbeddingType\x12\x1e\n\x1a\x45MBEDDING_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x45MBEDDING_TYPE_SPACY\x10\x01\x12\x1f\n\x1b\x45MBEDDING_TYPE_TRANSFORMERS\x10\x02\x12(\n$EMBEDDING_TYPE_SENTENCE_TRANSFORMERS\x10\x03\x12!\n\x1d\x45MBEDDING_TYPE_TENSORFLOW_HUB\x10\x04\x12\x19\n\x15\x45MBEDDING_TYPE_OPENAI\x10\x05\x32\xf3\x02\n\nNlpService\x12p\n\x07Vectors\x12#.arg_services.nlp.v1.VectorsRequest\x1a$.arg_services.nlp.v1.VectorsResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/nlp/v1/vectors\x12\x84\x01\n\x0cSimilarities\x12(.arg_services.nlp.v1.SimilaritiesRequest\x1a).arg_services.nlp.v1.SimilaritiesResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/nlp/v1/similarities\x12l\n\x06\x44ocBin\x12\".arg_services.nlp.v1.DocBinRequest\x1a#.arg_services.nlp.v1.DocBinResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/nlp/v1/docbinB\x8d\x01\n\x17\x63om.arg_services.nlp.v1B\x08NlpProtoP\x01\xa2\x02\x03\x41NX\xaa\x02\x12\x41rgServices.Nlp.V1\xca\x02\x12\x41rgServices\\Nlp\\V1\xe2\x02\x1e\x41rgServices\\Nlp\\V1\\GPBMetadata\xea\x02\x14\x41rgServices::Nlp::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x61rg_services/nlp/v1/nlp.proto\x12\x13\x61rg_services.nlp.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xec\x01\n\tNlpConfig\x12\x1a\n\x08language\x18\x01 \x01(\tR\x08language\x12\x1f\n\x0bspacy_model\x18\x02 \x01(\tR\nspacyModel\x12N\n\x10\x65mbedding_models\x18\x03 \x03(\x0b\x32#.arg_services.nlp.v1.EmbeddingModelR\x0f\x65mbeddingModels\x12R\n\x11similarity_method\x18\x04 \x01(\x0e\x32%.arg_services.nlp.v1.SimilarityMethodR\x10similarityMethod\"\xbf\x01\n\x13SimilaritiesRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12?\n\x0btext_tuples\x18\x02 \x03(\x0b\x32\x1e.arg_services.nlp.v1.TextTupleR\ntextTuples\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"k\n\x14SimilaritiesResponse\x12\"\n\x0csimilarities\x18\x01 \x03(\x01R\x0csimilarities\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"7\n\tTextTuple\x12\x14\n\x05text1\x18\x01 \x01(\tR\x05text1\x12\x14\n\x05text2\x18\x02 \x01(\tR\x05text2\"!\n\x07Strings\x12\x16\n\x06values\x18\x01 \x03(\tR\x06values\"\xc5\x03\n\rDocBinRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12\x41\n\nattributes\x18\x03 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x01R\nattributes\x88\x01\x01\x12\x43\n\renabled_pipes\x18\x04 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\x0c\x65nabledPipes\x12\x45\n\x0e\x64isabled_pipes\x18\x05 \x01(\x0b\x32\x1c.arg_services.nlp.v1.StringsH\x00R\rdisabledPipes\x12N\n\x10\x65mbedding_levels\x18\x06 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtrasB\x07\n\x05pipesB\r\n\x0b_attributes\"Y\n\x0e\x44ocBinResponse\x12\x16\n\x06\x64ocbin\x18\x01 \x01(\x0cR\x06\x64ocbin\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xdf\x01\n\x0eVectorsRequest\x12\x36\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.arg_services.nlp.v1.NlpConfigR\x06\x63onfig\x12\x14\n\x05texts\x18\x02 \x03(\tR\x05texts\x12N\n\x10\x65mbedding_levels\x18\x03 \x03(\x0e\x32#.arg_services.nlp.v1.EmbeddingLevelR\x0f\x65mbeddingLevels\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x81\x01\n\x0fVectorsResponse\x12=\n\x07vectors\x18\x01 \x03(\x0b\x32#.arg_services.nlp.v1.VectorResponseR\x07vectors\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xea\x01\n\x0eVectorResponse\x12\x37\n\x08\x64ocument\x18\x01 \x01(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x08\x64ocument\x12\x33\n\x06tokens\x18\x02 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\x06tokens\x12\x39\n\tsentences\x18\x03 \x03(\x0b\x32\x1b.arg_services.nlp.v1.VectorR\tsentences\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\" \n\x06Vector\x12\x16\n\x06vector\x18\x01 \x03(\x01R\x06vector\"\xd8\x01\n\x0e\x45mbeddingModel\x12\x41\n\nmodel_type\x18\x01 \x01(\x0e\x32\".arg_services.nlp.v1.EmbeddingTypeR\tmodelType\x12\x1d\n\nmodel_name\x18\x02 \x01(\tR\tmodelName\x12\x41\n\x0cpooling_type\x18\x03 \x01(\x0e\x32\x1c.arg_services.nlp.v1.PoolingH\x00R\x0bpoolingType\x12\x16\n\x05pmean\x18\x04 \x01(\x01H\x00R\x05pmeanB\t\n\x07pooling*\xe0\x02\n\x10SimilarityMethod\x12!\n\x1dSIMILARITY_METHOD_UNSPECIFIED\x10\x00\x12\x1c\n\x18SIMILARITY_METHOD_COSINE\x10\x01\x12%\n!SIMILARITY_METHOD_DYNAMAX_JACCARD\x10\x02\x12%\n!SIMILARITY_METHOD_MAXPOOL_JACCARD\x10\x03\x12\"\n\x1eSIMILARITY_METHOD_DYNAMAX_DICE\x10\x04\x12$\n SIMILARITY_METHOD_DYNAMAX_OTSUKA\x10\x05\x12\x19\n\x15SIMILARITY_METHOD_WMD\x10\x06\x12\x1a\n\x16SIMILARITY_METHOD_EDIT\x10\x07\x12\x1d\n\x19SIMILARITY_METHOD_JACCARD\x10\x08\x12\x1d\n\x19SIMILARITY_METHOD_ANGULAR\x10\t*\x8a\x01\n\x0e\x45mbeddingLevel\x12\x1f\n\x1b\x45MBEDDING_LEVEL_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45MBEDDING_LEVEL_DOCUMENT\x10\x01\x12\x1a\n\x16\x45MBEDDING_LEVEL_TOKENS\x10\x02\x12\x1d\n\x19\x45MBEDDING_LEVEL_SENTENCES\x10\x03*\xc6\x01\n\x07Pooling\x12\x17\n\x13POOLING_UNSPECIFIED\x10\x00\x12\x10\n\x0cPOOLING_MEAN\x10\x01\x12\x0f\n\x0bPOOLING_MAX\x10\x02\x12\x0f\n\x0bPOOLING_MIN\x10\x03\x12\x0f\n\x0bPOOLING_SUM\x10\x04\x12\x11\n\rPOOLING_FIRST\x10\x05\x12\x10\n\x0cPOOLING_LAST\x10\x06\x12\x12\n\x0ePOOLING_MEDIAN\x10\x07\x12\x11\n\rPOOLING_GMEAN\x10\x08\x12\x11\n\rPOOLING_HMEAN\x10\t*\xd2\x01\n\rEmbeddingType\x12\x1e\n\x1a\x45MBEDDING_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x45MBEDDING_TYPE_SPACY\x10\x01\x12\x1f\n\x1b\x45MBEDDING_TYPE_TRANSFORMERS\x10\x02\x12(\n$EMBEDDING_TYPE_SENTENCE_TRANSFORMERS\x10\x03\x12!\n\x1d\x45MBEDDING_TYPE_TENSORFLOW_HUB\x10\x04\x12\x19\n\x15\x45MBEDDING_TYPE_OPENAI\x10\x05\x32\xf3\x02\n\nNlpService\x12p\n\x07Vectors\x12#.arg_services.nlp.v1.VectorsRequest\x1a$.arg_services.nlp.v1.VectorsResponse\"\x1a\x82\xd3\xe4\x93\x02\x14:\x01*\"\x0f/nlp/v1/vectors\x12\x84\x01\n\x0cSimilarities\x12(.arg_services.nlp.v1.SimilaritiesRequest\x1a).arg_services.nlp.v1.SimilaritiesResponse\"\x1f\x82\xd3\xe4\x93\x02\x19:\x01*\"\x14/nlp/v1/similarities\x12l\n\x06\x44ocBin\x12\".arg_services.nlp.v1.DocBinRequest\x1a#.arg_services.nlp.v1.DocBinResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/nlp/v1/docbinB\x8d\x01\n\x17\x63om.arg_services.nlp.v1B\x08NlpProtoP\x01\xa2\x02\x03\x41NX\xaa\x02\x12\x41rgServices.Nlp.V1\xca\x02\x12\x41rgServices\\Nlp\\V1\xe2\x02\x1e\x41rgServices\\Nlp\\V1\\GPBMetadata\xea\x02\x14\x41rgServices::Nlp::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.nlp.v1.nlp_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2.pyi` & `arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.py` & `arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi` & `arg_services-1.4.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/google/api/annotations_pb2.py` & `arg_services-1.4.0/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/google/api/annotations_pb2.pyi` & `arg_services-1.4.0/src/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/google/api/annotations_pb2_grpc.pyi` & `arg_services-1.4.0/src/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/google/api/http_pb2.py` & `arg_services-1.4.0/src/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/google/api/http_pb2.pyi` & `arg_services-1.4.0/src/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/src/google/api/http_pb2_grpc.pyi` & `arg_services-1.4.0/src/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.3.2/PKG-INFO` & `arg_services-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arg-services
-Version: 1.3.2
+Version: 1.4.0
 Summary: gRPC definitions for microservice-based argumentation machines
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

