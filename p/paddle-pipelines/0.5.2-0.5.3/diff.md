# Comparing `tmp/paddle-pipelines-0.5.2.tar.gz` & `tmp/paddle-pipelines-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddle-pipelines-0.5.2.tar", last modified: Thu Mar 23 11:03:26 2023, max compression
+gzip compressed data, was "paddle-pipelines-0.5.3.tar", last modified: Tue Jun 20 08:09:18 2023, max compression
```

## Comparing `paddle-pipelines-0.5.2.tar` & `paddle-pipelines-0.5.3.tar`

### file list

```diff
@@ -1,115 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.358709 paddle-pipelines-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (122)    16386 2023-03-23 11:03:26.358709 paddle-pipelines-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13833 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.346709 paddle-pipelines-0.5.2/paddle_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    16386 2023-03-23 11:03:26.000000 paddle-pipelines-0.5.2/paddle_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-03-23 11:03:26.000000 paddle-pipelines-0.5.2/paddle_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-23 11:03:26.000000 paddle-pipelines-0.5.2/paddle_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-03-23 11:03:26.000000 paddle-pipelines-0.5.2/paddle_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-23 11:03:26.000000 paddle-pipelines-0.5.2/paddle_pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.346709 paddle-pipelines-0.5.2/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/data_handler/
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/data_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3183 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/data_handler/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/data_handler/inputs.py
--rw-r--r--   0 runner    (1001) docker     (122)    15154 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/data_handler/predictions.py
--rw-r--r--   0 runner    (1001) docker     (122)    47483 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/data_handler/processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/data_handler/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/document_stores/
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30608 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/base.py
--rw-r--r--   0 runner    (1001) docker     (122)   116235 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (122)    32569 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (122)    26355 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/filter_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    32844 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/milvus2.py
--rw-r--r--   0 runner    (1001) docker     (122)    33468 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)    21187 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/document_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/nodes/
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/answer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/answer_extractor_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     8377 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/qa_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/qa_filter_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     8349 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/nodes/document/
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8693 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/document/document_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (122)     5244 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/document/document_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/nodes/file_classifier/
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_classifier/file_type.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8650 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/docx.py
--rw-r--r--   0 runner    (1001) docker     (122)     6317 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     2930 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/markdown.py
--rw-r--r--   0 runner    (1001) docker     (122)    11991 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/file_converter/txt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/nodes/models/
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4660 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/models/neural_search_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.350709 paddle-pipelines-0.5.2/pipelines/nodes/other/
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/other/docs2answers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/other/join_answers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5121 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/other/join_docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4329 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/other/route_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/nodes/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/preprocessor/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    18511 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/preprocessor/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/nodes/question_generator/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/question_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11664 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/question_generator/question_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/nodes/ranker/
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/ranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5539 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/ranker/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     9997 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/ranker/ernie_ranker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/nodes/reader/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/reader/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    44701 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/reader/ernie_dureader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/nodes/retriever/
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9088 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/retriever/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16240 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/retriever/dense.py
--rw-r--r--   0 runner    (1001) docker     (122)     9142 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/retriever/embedder.py
--rw-r--r--   0 runner    (1001) docker     (122)    10969 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/retriever/multimodal_retriever.py
--rw-r--r--   0 runner    (1001) docker     (122)    17969 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/retriever/sparse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/senta.py
--rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/senta_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/senta_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/nodes/text_to_image_generator/
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/text_to_image_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11053 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/nodes/text_to_image_generator/text_to_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43147 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/pipelines/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6606 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/pipelines/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    16061 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/pipelines/standard_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (122)     8978 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/pipelines/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    52194 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/pipelines/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1431 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6593 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/doc_store.py
--rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/export_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     9099 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5303 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/pipelines/utils/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-23 11:03:26.000000 paddle-pipelines-0.5.2/pipelines/version.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-23 11:03:26.358709 paddle-pipelines-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 11:03:26.354709 paddle-pipelines-0.5.2/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6026 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/utils/offline_ann.py
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-03-23 11:01:49.000000 paddle-pipelines-0.5.2/utils/offline_ann_mm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.814542 paddle-pipelines-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    16386 2023-06-20 08:09:18.814542 paddle-pipelines-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13833 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.802542 paddle-pipelines-0.5.3/paddle_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16386 2023-06-20 08:09:18.000000 paddle-pipelines-0.5.3/paddle_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-06-20 08:09:18.000000 paddle-pipelines-0.5.3/paddle_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 08:09:18.000000 paddle-pipelines-0.5.3/paddle_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-20 08:09:18.000000 paddle-pipelines-0.5.3/paddle_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-20 08:09:18.000000 paddle-pipelines-0.5.3/paddle_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.802542 paddle-pipelines-0.5.3/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     6206 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.802542 paddle-pipelines-0.5.3/pipelines/agents/
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6807 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/agent_step.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20536 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.802542 paddle-pipelines-0.5.3/pipelines/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/memory/conversation_memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/memory/no_memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/agents/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.802542 paddle-pipelines-0.5.3/pipelines/data_handler/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/data_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3183 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/data_handler/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/data_handler/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15154 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/data_handler/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47483 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/data_handler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/data_handler/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/document_stores/
+-rw-r--r--   0 runner    (1001) docker     (122)     1790 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30608 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)   119497 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32565 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26355 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/filter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32840 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/milvus2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33468 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21187 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/document_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7359 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/answer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/answer_extractor_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8377 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/qa_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/qa_filter_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8349 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/document/
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8693 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/document/document_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5244 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/document/document_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/file_classifier/
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_classifier/file_type.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8650 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/docx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6317 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2930 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11597 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/file_converter/txt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/llm/
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/llm/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4879 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/llm/ernie_bot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/llm/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/llm/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4660 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/models/neural_search_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/other/
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/other/docs2answers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/other/join_answers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5121 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/other/join_docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4329 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/other/route_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/preprocessor/
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/preprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/preprocessor/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19459 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/preprocessor/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8311 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/preprocessor/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.806542 paddle-pipelines-0.5.3/pipelines/nodes/prompt/
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/
+-rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4036 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/ernie_bot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3633 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12252 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/invocation_layer/open_ai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/prompt_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28686 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/prompt_node.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22779 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36796 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/prompt/shapers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/question_generator/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/question_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11664 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/question_generator/question_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/ranker/
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/ranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5539 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/ranker/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9997 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/ranker/ernie_ranker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/reader/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/reader/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44701 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/reader/ernie_dureader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/retriever/
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9071 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/retriever/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16469 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/retriever/dense.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9142 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/retriever/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10969 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/retriever/multimodal_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17969 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/retriever/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15710 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/retriever/web.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/search_engine/
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/search_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/search_engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10210 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/search_engine/providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/search_engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4775 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/search_engine/web.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/senta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2521 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/senta_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25923 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/senta_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/nodes/text_to_image_generator/
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/text_to_image_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11053 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/nodes/text_to_image_generator/text_to_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.810542 paddle-pipelines-0.5.3/pipelines/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43182 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6606 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/pipelines/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19114 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/pipelines/standard_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8978 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/pipelines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52194 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.814542 paddle-pipelines-0.5.3/pipelines/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1431 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6593 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/doc_store.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/export_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9225 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5303 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/pipelines/utils/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-20 08:09:18.000000 paddle-pipelines-0.5.3/pipelines/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 08:09:18.814542 paddle-pipelines-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:09:18.814542 paddle-pipelines-0.5.3/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6026 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/utils/offline_ann.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-06-20 08:07:39.000000 paddle-pipelines-0.5.3/utils/offline_ann_mm.py
```

### Comparing `paddle-pipelines-0.5.2/PKG-INFO` & `paddle-pipelines-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddle-pipelines
-Version: 0.5.2
+Version: 0.5.3
 Summary: Paddle-Pipelines: An End to End Natural Language Proceessing Development Kit Based on PaddleNLP
 Home-page: https://github.com/PaddlePaddle/PaddleNLP
 Author: PaddlePaddle Speech and Language Team
 Author-email: paddlenlp@baidu.com
 License: Apache 2.0
 Description: ## PaddleNLP Pipelines：NLP流水线系统
```

### Comparing `paddle-pipelines-0.5.2/README.md` & `paddle-pipelines-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/paddle_pipelines.egg-info/PKG-INFO` & `paddle-pipelines-0.5.3/paddle_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddle-pipelines
-Version: 0.5.2
+Version: 0.5.3
 Summary: Paddle-Pipelines: An End to End Natural Language Proceessing Development Kit Based on PaddleNLP
 Home-page: https://github.com/PaddlePaddle/PaddleNLP
 Author: PaddlePaddle Speech and Language Team
 Author-email: paddlenlp@baidu.com
 License: Apache 2.0
 Description: ## PaddleNLP Pipelines：NLP流水线系统
```

### Comparing `paddle-pipelines-0.5.2/pipelines/__init__.py` & `paddle-pipelines-0.5.3/pipelines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 logging.basicConfig(
     format="%(levelname)s - %(name)s -  %(message)s", datefmt="%m/%d/%Y %H:%M:%S", level=logging.WARNING
 )
 logging.getLogger("pipelines").setLevel(logging.INFO)
 
 import pandas as pd
 
-from pipelines import pipelines, utils
+from pipelines import utils
 from pipelines.nodes import BaseComponent
 from pipelines.pipelines import Pipeline
 from pipelines.pipelines.standard_pipelines import (
     BaseStandardPipeline,
     DocPipeline,
     ExtractiveQAPipeline,
     QAGenerationPipeline,
```

### Comparing `paddle-pipelines-0.5.2/pipelines/data_handler/__init__.py` & `paddle-pipelines-0.5.3/pipelines/data_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/data_handler/dataset.py` & `paddle-pipelines-0.5.3/pipelines/data_handler/dataset.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/data_handler/inputs.py` & `paddle-pipelines-0.5.3/pipelines/data_handler/inputs.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/data_handler/predictions.py` & `paddle-pipelines-0.5.3/pipelines/data_handler/predictions.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/data_handler/processor.py` & `paddle-pipelines-0.5.3/pipelines/data_handler/processor.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/data_handler/samples.py` & `paddle-pipelines-0.5.3/pipelines/data_handler/samples.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/__init__.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 OpenDistroElasticsearchDocumentStore = safe_import(
     "pipelines.document_stores.elasticsearch", "OpenDistroElasticsearchDocumentStore", "elasticsearch"
 )
 OpenSearchDocumentStore = safe_import(
     "pipelines.document_stores.elasticsearch", "OpenSearchDocumentStore", "elasticsearch"
 )
 
+BaiduElasticsearchDocumentStore = safe_import(
+    "pipelines.document_stores.elasticsearch", "BaiduElasticsearchDocumentStore", "elasticsearch"
+)
+
 FAISSDocumentStore = safe_import("pipelines.document_stores.faiss", "FAISSDocumentStore", "faiss")
 
 MilvusDocumentStore = safe_import("pipelines.document_stores.milvus2", "Milvus2DocumentStore", "milvus")
 
 from pipelines.document_stores.utils import (
     es_index_to_document_store,
     eval_data_from_json,
```

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/base.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/base.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/elasticsearch.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/elasticsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         index: str = "document",
         label_index: str = "label",
         search_fields: Union[str, list] = "content",
         content_field: str = "content",
         name_field: str = "name",
         embedding_field: str = "embedding",
         embedding_dim: int = 768,
+        vector_type: str = "dense_vector",
         custom_mapping: Optional[dict] = None,
         excluded_meta_data: Optional[list] = None,
         analyzer: str = "standard",
         scheme: str = "http",
         ca_certs: Optional[str] = None,
         verify_certs: bool = True,
         recreate_index: bool = False,
@@ -98,15 +99,15 @@
         :param api_key: Secret value of the API key (altenative authentication mode to the above http_auth)
         :param aws4auth: Authentication for usage with aws elasticsearch (can be generated with the requests-aws4auth package)
         :param index: Name of index in elasticsearch to use for storing the documents that we want to search. If not existing yet, we will create one.
         :param label_index: Name of index in elasticsearch to use for storing labels. If not existing yet, we will create one.
         :param search_fields: Name of fields used by ElasticsearchRetriever to find matches in the docs to our incoming query (using elastic's multi_match query), e.g. ["title", "full_text"]
         :param content_field: Name of field that might contain the answer and will therefore be passed to the Reader Model (e.g. "full_text").
                            If no Reader is used (e.g. in FAQ-Style QA) the plain content of this field will just be returned.
-        :param name_field: Name of field that contains the title of the the doc
+        :param name_field: Name of field that contains the title of the doc
         :param embedding_field: Name of field containing an embedding vector (Only needed when using a dense retriever (e.g. DensePassageRetriever, EmbeddingRetriever) on top)
         :param embedding_dim: Dimensionality of embedding vector (Only needed when using a dense retriever (e.g. DensePassageRetriever, EmbeddingRetriever) on top)
         :param custom_mapping: If you want to use your own custom mapping for creating a new index in Elasticsearch, you can supply it here as a dictionary.
         :param analyzer: Specify the default analyzer from one of the built-ins when creating a new Elasticsearch Index.
                          Elasticsearch also has built-in analyzers for different languages (e.g. impacting tokenization). More info at:
                          https://www.elastic.co/guide/en/elasticsearch/reference/7.9/analysis-analyzers.html
         :param excluded_meta_data: Name of fields in Elasticsearch that should not be returned (e.g. [field_one, field_two]).
@@ -181,14 +182,15 @@
             create_index=create_index,
             duplicate_documents=duplicate_documents,
             refresh_type=refresh_type,
             similarity=similarity,
             timeout=timeout,
             return_embedding=return_embedding,
             index_type=index_type,
+            vector_type=vector_type,
             scroll=scroll,
             skip_missing_embeddings=skip_missing_embeddings,
             synonyms=synonyms,
             synonym_type=synonym_type,
             use_system_proxy=use_system_proxy,
         )
 
@@ -225,20 +227,17 @@
         self.custom_mapping = custom_mapping
         self.synonyms = synonyms
         self.synonym_type = synonym_type
         self.index: str = index
         self.label_index: str = label_index
         self.scroll = scroll
         self.skip_missing_embeddings: bool = skip_missing_embeddings
-        if similarity in ["cosine", "dot_product", "l2"]:
-            self.similarity = similarity
-        else:
-            raise Exception(
-                f"Invalid value {similarity} for similarity in ElasticSearchDocumentStore constructor. Choose between 'cosine', 'l2' and 'dot_product'"
-            )
+        self.vector_type = vector_type
+
+        self.similarity_check(similarity)
         if index_type in ["flat", "hnsw"]:
             self.index_type = index_type
         else:
             raise Exception("Invalid value for index_type in constructor. Choose between 'flat' and 'hnsw'")
         if index_type == "hnsw" and type(self) == ElasticsearchDocumentStore:
             raise Exception(
                 "The HNSW algorithm for approximate nearest neighbours calculation is currently not available in the ElasticSearchDocumentStore. "
@@ -252,14 +251,22 @@
         elif create_index:
             self._create_document_index(index)
             self._create_label_index(label_index)
 
         self.duplicate_documents = duplicate_documents
         self.refresh_type = refresh_type
 
+    def similarity_check(self, similarity):
+        if similarity in ["cosine", "dot_product", "l2"]:
+            self.similarity = similarity
+        else:
+            raise Exception(
+                f"Invalid value {similarity} for similarity in ElasticSearchDocumentStore constructor. Choose between 'cosine', 'l2' and 'dot_product'"
+            )
+
     @classmethod
     def _init_elastic_client(
         cls,
         host: Union[str, List[str]],
         port: Union[int, List[int]],
         username: str,
         password: str,
@@ -374,22 +381,22 @@
                             f"This error might occur if you are trying to use pipelines 1.0 and above with an existing elasticsearch index created with a previous version of pipelines."
                             f"In this case deleting the index with `curl -X DELETE \"{self.pipeline_config['params']['host']}:{self.pipeline_config['params']['port']}/{index_name}\"` will fix your environment. "
                             f"Note, that all data stored in the index will be lost!"
                         )
             if self.embedding_field:
                 if (
                     self.embedding_field in mapping["properties"]
-                    and mapping["properties"][self.embedding_field]["type"] != "dense_vector"
+                    and mapping["properties"][self.embedding_field]["type"] != self.vector_type
                 ):
                     raise Exception(
                         f"The '{index_name}' index in Elasticsearch already has a field called '{self.embedding_field}'"
                         f" with the type '{mapping['properties'][self.embedding_field]['type']}'. Please update the "
                         f"document_store to use a different name for the embedding_field parameter."
                     )
-                mapping["properties"][self.embedding_field] = {"type": "dense_vector", "dims": self.embedding_dim}
+                mapping["properties"][self.embedding_field] = {"type": self.vector_type, "dims": self.embedding_dim}
                 self.client.indices.put_mapping(index=index_name, body=mapping, headers=headers)
             return
 
         if self.custom_mapping:
             mapping = self.custom_mapping
         else:
             mapping = {
@@ -431,15 +438,15 @@
 
             else:
                 for field in self.search_fields:
                     mapping["mappings"]["properties"].update({field: {"type": "text"}})
 
             if self.embedding_field:
                 mapping["mappings"]["properties"][self.embedding_field] = {
-                    "type": "dense_vector",
+                    "type": self.vector_type,
                     "dims": self.embedding_dim,
                 }
 
         try:
             self.client.indices.create(index=index_name, body=mapping, headers=headers)
         except RequestError as e:
             # With multiple workers we need to avoid race conditions, where:
@@ -1401,15 +1408,15 @@
         index: Optional[str] = None,
         filters: Optional[Dict[str, Union[Dict, List, str, int, float, bool]]] = None,
         update_existing_embeddings: bool = True,
         batch_size: int = 10_000,
         headers: Optional[Dict[str, str]] = None,
     ):
         """
-        Updates the embeddings in the the document store using the encoding model specified in the retriever.
+        Updates the embeddings in the document store using the encoding model specified in the retriever.
         This can be useful if want to add or change the embeddings for your documents (e.g. after changing the retriever config).
 
         :param retriever: Retriever to use to update the embeddings.
         :param index: Index name to update
         :param update_existing_embeddings: Whether to update existing embeddings of the documents. If set to False,
                                            only documents without embeddings are processed. This mode can be used for
                                            incremental updating of embeddings, wherein, only newly indexed documents
@@ -1680,15 +1687,15 @@
         :param api_key: Secret value of the API key (altenative authentication mode to the above http_auth)
         :param aws4auth: Authentication for usage with aws elasticsearch (can be generated with the requests-aws4auth package)
         :param index: Name of index in elasticsearch to use for storing the documents that we want to search. If not existing yet, we will create one.
         :param label_index: Name of index in elasticsearch to use for storing labels. If not existing yet, we will create one.
         :param search_fields: Name of fields used by ElasticsearchRetriever to find matches in the docs to our incoming query (using elastic's multi_match query), e.g. ["title", "full_text"]
         :param content_field: Name of field that might contain the answer and will therefore be passed to the Reader Model (e.g. "full_text").
                            If no Reader is used (e.g. in FAQ-Style QA) the plain content of this field will just be returned.
-        :param name_field: Name of field that contains the title of the the doc
+        :param name_field: Name of field that contains the title of the doc
         :param embedding_field: Name of field containing an embedding vector (Only needed when using a dense retriever (e.g. DensePassageRetriever, EmbeddingRetriever) on top)
                                 Note, that in OpenSearch the similarity type for efficient approximate vector similarity calculations is tied to the embedding field's data type which cannot be changed after creation.
         :param embedding_dim: Dimensionality of embedding vector (Only needed when using a dense retriever (e.g. DensePassageRetriever, EmbeddingRetriever) on top)
         :param custom_mapping: If you want to use your own custom mapping for creating a new index in Elasticsearch, you can supply it here as a dictionary.
         :param analyzer: Specify the default analyzer from one of the built-ins when creating a new Elasticsearch Index.
                          Elasticsearch also has built-in analyzers for different languages (e.g. impacting tokenization). More info at:
                          https://www.elastic.co/guide/en/elasticsearch/reference/7.9/analysis-analyzers.html
@@ -2147,7 +2154,72 @@
             "See https://opensearch.org/faq/ for details. "
             "We recommend using the OpenSearchDocumentStore instead."
         )
         super(OpenDistroElasticsearchDocumentStore, self).__init__(host=host, similarity=similarity, **kwargs)
 
     def _prepare_hosts(self, host, port):
         return host
+
+
+class BaiduElasticsearchDocumentStore(ElasticsearchDocumentStore):
+    def similarity_check(self, similarity):
+        if similarity in ["cosine", "dot_prod", "l2", "l1"]:
+            self.similarity = similarity
+        else:
+            raise Exception(
+                f"Invalid value {similarity} for similarity in BaiduElasticSearchDocumentStore constructor. Choose between 'cosine', 'l1', 'l2' and 'dot_prod'"
+            )
+
+    def _get_vector_similarity_query(self, query_emb: np.ndarray, top_k: int):
+        """
+        Generate Elasticsearch query for vector similarity.
+        """
+        # To handle scenarios where embeddings may be missing
+        script_score_query: dict = {"match_all": {}}
+        if self.skip_missing_embeddings:
+            script_score_query = {
+                "bool": {"filter": {"bool": {"must": [{"exists": {"field": self.embedding_field}}]}}}
+            }
+
+        query = {
+            "script_score": {
+                "query": script_score_query,
+                "script": {
+                    # offset score to ensure a positive range as required by Elasticsearch
+                    "source": "bpack_knn_script",
+                    "lang": "knn",
+                    "params": {"space": self.similarity, "field": "embedding", "vector": query_emb.tolist()},
+                },
+            }
+        }
+        return query
+
+    def _create_label_index(self, index_name: str, headers: Optional[Dict[str, str]] = None):
+        if self.client.indices.exists(index=index_name, headers=headers):
+            return
+        mapping = {
+            "mappings": {
+                "properties": {
+                    "query": {"type": "text"},
+                    "answer": {"type": "text"},  # light-weight but less search options than full object
+                    "document": {"type": "text"},
+                    "is_correct_answer": {"type": "boolean"},
+                    "is_correct_document": {"type": "boolean"},
+                    "origin": {"type": "keyword"},  # e.g. user-feedback or gold-label
+                    "document_id": {"type": "keyword"},
+                    "no_answer": {"type": "boolean"},
+                    "pipeline_id": {"type": "keyword"},
+                    "created_at": {"type": "date", "format": "yyyy-MM-dd HH:mm:ss||yyyy-MM-dd||epoch_millis"},
+                    "updated_at": {"type": "date", "format": "yyyy-MM-dd HH:mm:ss||yyyy-MM-dd||epoch_millis"}
+                    # TODO add pipeline_hash and pipeline_name once we migrated the REST API to pipelines
+                }
+            }
+        }
+        try:
+            self.client.indices.create(index=index_name, body=mapping, headers=headers)
+        except RequestError as e:
+            # With multiple workers we need to avoid race conditions, where:
+            # - there's no index in the beginning
+            # - both want to create one
+            # - one fails as the other one already created it
+            if not self.client.indices.exists(index=index_name, headers=headers):
+                raise e
```

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/faiss.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/faiss.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         retriever: "BaseRetriever",
         index: Optional[str] = None,
         update_existing_embeddings: bool = True,
         filters: Optional[Dict[str, Any]] = None,  # TODO: Adapt type once we allow extended filters in FAISSDocStore
         batch_size: int = 10000,
     ):
         """
-        Updates the embeddings in the the document store using the encoding model specified in the retriever.
+        Updates the embeddings in the document store using the encoding model specified in the retriever.
         This can be useful if want to add or change the embeddings for your documents (e.g. after changing the retriever config).
 
         :param retriever: Retriever to use to get embeddings for text
         :param index: Index name for which embeddings are to be updated. If set to None, the default self.index is used.
         :param update_existing_embeddings: Whether to update existing embeddings of the documents. If set to False,
                                            only documents without embeddings are processed. This mode can be used for
                                            incremental updating of embeddings, wherein, only newly indexed documents
```

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/filter_utils.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/filter_utils.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/milvus2.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/milvus2.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         retriever: "BaseRetriever",
         index: Optional[str] = None,
         batch_size: int = 10_000,
         update_existing_embeddings: bool = True,
         filters: Optional[Dict[str, Any]] = None,  # TODO: Adapt type once we allow extended filters in Milvus2DocStore
     ):
         """
-        Updates the embeddings in the the document store using the encoding model specified in the retriever.
+        Updates the embeddings in the document store using the encoding model specified in the retriever.
         This can be useful if want to add or change the embeddings for your documents (e.g. after changing the retriever config).
 
         :param retriever: Retriever to use to get embeddings for text
         :param index: (SQL) index name for storing the docs and metadata
         :param batch_size: When working with large number of documents, batching can help reduce memory footprint.
         :param update_existing_embeddings: Whether to update existing embeddings of the documents. If set to False,
                                            only documents without embeddings are processed. This mode can be used for
```

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/sql.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/sql.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/document_stores/utils.py` & `paddle-pipelines-0.5.3/pipelines/document_stores/utils.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/errors.py` & `paddle-pipelines-0.5.3/pipelines/errors.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,24 +27,35 @@
     DocxToTextConverter,
     ImageToTextConverter,
     MarkdownConverter,
     PDFToTextConverter,
     PDFToTextOCRConverter,
     TextConverter,
 )
+from pipelines.nodes.llm import ChatGLMBot
+from pipelines.nodes.llm.ernie_bot import ErnieBot
+from pipelines.nodes.llm.history import TruncatedConversationHistory
+from pipelines.nodes.llm.prompt_template import PromptTemplate
 from pipelines.nodes.other import JoinDocuments
-from pipelines.nodes.preprocessor import BasePreProcessor, PreProcessor
+from pipelines.nodes.preprocessor import (
+    BasePreProcessor,
+    CharacterTextSplitter,
+    PreProcessor,
+    RecursiveCharacterTextSplitter,
+)
+from pipelines.nodes.prompt import PromptModel, PromptNode, Shaper
 from pipelines.nodes.question_generator import QuestionGenerator
 from pipelines.nodes.ranker import BaseRanker, ErnieRanker
 from pipelines.nodes.reader import BaseReader, ErnieReader
 from pipelines.nodes.retriever import (
     BaseRetriever,
     BM25Retriever,
     DensePassageRetriever,
     MultiModalRetriever,
+    WebRetriever,
 )
 from pipelines.nodes.sentiment_analysis import (
     SentaProcessor,
     SentaVisualization,
     UIESenta,
 )
 from pipelines.nodes.text_to_image_generator import ErnieTextToImageGenerator
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/answer_extractor.py` & `paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/answer_extractor.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/answer_extractor_preprocessor.py` & `paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/answer_extractor_preprocessor.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/qa_filter.py` & `paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/qa_filter.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/answer_extractor/qa_filter_postprocessor.py` & `paddle-pipelines-0.5.3/pipelines/nodes/answer_extractor/qa_filter_postprocessor.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/base.py` & `paddle-pipelines-0.5.3/pipelines/nodes/base.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/document/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/document/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/document/document_intelligence.py` & `paddle-pipelines-0.5.3/pipelines/nodes/document/document_intelligence.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/document/document_preprocessor.py` & `paddle-pipelines-0.5.3/pipelines/nodes/document/document_preprocessor.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_classifier/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_classifier/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_classifier/file_type.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_classifier/file_type.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_converter/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_converter/base.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_converter/base.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_converter/docx.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_converter/docx.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_converter/image.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_converter/image.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_converter/markdown.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_converter/markdown.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_converter/pdf.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_converter/pdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 logger = logging.getLogger(__name__)
 
 
 class PDFToTextConverter(BaseConverter):
     def __init__(
         self,
         remove_numeric_tables: bool = False,
+        language: str = "en",
         valid_languages: Optional[List[str]] = None,
     ):
         """
         :param remove_numeric_tables: This option uses heuristics to remove numeric rows from the tables.
                                       The tabular structures in documents might be noise for the reader model if it
                                       does not have table parsing capability for finding answers. However, tables
                                       may also have long strings that could possible candidate for searching answers.
@@ -51,22 +52,23 @@
                                 not one of the valid languages, then it might likely be encoding error resulting
                                 in garbled text.
         """
         # save init parameters to enable export of component config as YAML
         self.set_config(remove_numeric_tables=remove_numeric_tables, valid_languages=valid_languages)
 
         super().__init__(remove_numeric_tables=remove_numeric_tables, valid_languages=valid_languages)
+        self.language = language
 
     def convert(
         self,
         file_path: Path,
         meta: Optional[Dict[str, str]] = None,
         remove_numeric_tables: Optional[bool] = None,
         valid_languages: Optional[List[str]] = None,
-        encoding: Optional[str] = "Latin1",
+        language: Optional[str] = "en",
     ) -> List[Dict[str, Any]]:
         """
         Extract text from a .pdf file using the pdftotext library (https://www.xpdfreader.com/pdftotext-man.html)
 
         :param file_path: Path to the .pdf file you want to convert
         :param meta: Optional dictionary with metadata that shall be attached to all resulting documents.
                      Can be any custom keys and values.
@@ -76,69 +78,68 @@
                                       may also have long strings that could possible candidate for searching answers.
                                       The rows containing strings are thus retained in this option.
         :param valid_languages: validate languages from a list of languages specified in the ISO 639-1
                                 (https://en.wikipedia.org/wiki/ISO_639-1) format.
                                 This option can be used to add test for encoding errors. If the extracted text is
                                 not one of the valid languages, then it might likely be encoding error resulting
                                 in garbled text.
-        :param encoding: Encoding that will be passed as -enc parameter to pdftotext. "Latin 1" is the default encoding
-                         of pdftotext. While this works well on many PDFs, it might be needed to switch to "UTF-8" or
-                         others if your doc contains special characters (e.g. German Umlauts, Cyrillic characters ...).
-                         Note: With "UTF-8" we experienced cases, where a simple "fi" gets wrongly parsed as
-                         "xef\xac\x81c" (see test cases). That's why we keep "Latin 1" as default here.
-                         (See list of available encodings by running `pdftotext -listenc` in the terminal)
         """
 
-        pages = self._read_pdf(file_path, layout=False, encoding=encoding)
+        pages = self._read_pdf(file_path, layout=False)
         if remove_numeric_tables is None:
             remove_numeric_tables = self.remove_numeric_tables
         if valid_languages is None:
             valid_languages = self.valid_languages
-
+        if language is None:
+            language = self.language
         cleaned_pages = []
         for page in pages:
             # pdftotext tool provides an option to retain the original physical layout of a PDF page. This behaviour
             # can be toggled by using the layout param.
             #  layout=True
             #      + table structures get retained better
             #      - multi-column pages(eg, research papers) gets extracted with text from multiple columns on same line
             #  layout=False
             #      + keeps strings in content stream order, hence multi column layout works well
             #      - cells of tables gets split across line
             #
             #  Here, as a "safe" default, layout is turned off.
             lines = page.splitlines()
+
             cleaned_lines = []
             for line in lines:
-                words = line.split()
+                if self.language == "chinese":
+                    words = list(line)
+                else:
+                    words = line.split()
                 digits = [word for word in words if any(i.isdigit() for i in word)]
 
                 # remove lines having > 40% of words as digits AND not ending with a period(.)
                 if remove_numeric_tables:
                     if words and len(digits) / len(words) > 0.4 and not line.strip().endswith("."):
                         logger.debug(f"Removing line '{line}' from {file_path}")
                         continue
                 cleaned_lines.append(line)
-            cleaned_pages.extend(cleaned_lines)
+
+            page = "\n".join(cleaned_lines)
+            cleaned_pages.append(page)
 
         if valid_languages:
             document_text = "".join(cleaned_pages)
             if not self.validate_language(document_text, valid_languages):
                 logger.warning(
                     f"The language for {file_path} is not one of {valid_languages}. The file may not have "
                     f"been decoded in the correct text format."
                 )
 
-        documents = []
-        for page in cleaned_pages:
-            document = {"content": page, "content_type": "text", "meta": meta}
-            documents.append(document)
-        return documents
+        text = "\f".join(cleaned_pages)
+        document = {"content": text, "content_type": "text", "meta": meta}
+        return [document]
 
-    def _read_pdf(self, file_path: Path, layout: bool, encoding: Optional[str] = "Latin1") -> List[str]:
+    def _read_pdf(self, file_path: Path, layout: bool) -> List[str]:
         """
         Extract pages from the pdf file at file_path.
 
         :param file_path: path of the pdf file
         :param layout: whether to retain the original physical layout for a page. If disabled, PDF pages are read in
                        the content stream order.
         """
@@ -205,17 +206,21 @@
                                 in garbled text.
         :param encoding: Select the file encoding (default is `utf-8`)
         """
         pages = []
         try:
             images = convert_from_path(file_path)
             for image in images:
-                temp_img = tempfile.NamedTemporaryFile(dir=os.path.dirname(os.path.realpath(__file__)), suffix=".jpeg")
+                temp_img = tempfile.NamedTemporaryFile(
+                    dir=os.path.dirname(os.path.realpath(__file__)), suffix=".jpeg", delete=False
+                )
                 image.save(temp_img.name)
                 pages.append(self.image_2_text.convert(temp_img.name)[0]["content"])
+                temp_img.close()
+                os.remove(temp_img.name)
         except Exception as exception:
             logger.error(f"File {file_path} has an error \n {exception}")
 
         raw_text = "\f".join(pages)
         document = {"content": raw_text, "meta": meta}
 
         return [document]
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/file_converter/txt.py` & `paddle-pipelines-0.5.3/pipelines/nodes/file_converter/txt.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/models/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/models/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/models/neural_search_model.py` & `paddle-pipelines-0.5.3/pipelines/nodes/models/neural_search_model.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/other/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/other/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/other/docs2answers.py` & `paddle-pipelines-0.5.3/pipelines/nodes/other/docs2answers.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/other/join_answers.py` & `paddle-pipelines-0.5.3/pipelines/nodes/other/join_answers.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/other/join_docs.py` & `paddle-pipelines-0.5.3/pipelines/nodes/other/join_docs.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/other/route_documents.py` & `paddle-pipelines-0.5.3/pipelines/nodes/other/route_documents.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/preprocessor/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/reader/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pipelines.nodes.preprocessor.base import BasePreProcessor
-from pipelines.nodes.preprocessor.preprocessor import PreProcessor
+from pipelines.nodes.reader.base import BaseReader
+from pipelines.nodes.reader.ernie_dureader import ErnieReader
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/preprocessor/base.py` & `paddle-pipelines-0.5.3/pipelines/nodes/preprocessor/base.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/preprocessor/preprocessor.py` & `paddle-pipelines-0.5.3/pipelines/nodes/preprocessor/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,26 +94,32 @@
             split_length=split_length,
             split_overlap=split_overlap,
             split_answers=split_answers,
             split_respect_sentence_boundary=split_respect_sentence_boundary,
         )
 
         try:
-            nltk.data.find("tokenizers/punkt")
+            if nltk:
+                nltk.data.find("tokenizers/punkt")
         except LookupError:
-            nltk.download("punkt")
+            try:
+                if nltk:
+                    nltk.download("punkt")
+            except FileExistsError as error:
+                logger.debug("NLTK punkt tokenizer seems to be already downloaded. Error message: %s", error)
+                pass
 
         self.clean_whitespace = clean_whitespace
         self.clean_header_footer = clean_header_footer
         self.clean_empty_lines = clean_empty_lines
         self.split_by = split_by
         self.split_length = split_length
         self.split_overlap = split_overlap
         self.split_respect_sentence_boundary = split_respect_sentence_boundary
-        self.language = iso639_to_nltk.get(language, language)
+        self.language = language
         self.print_log: Set[str] = set()
         self.split_answers = split_answers
 
     def process(
         self,
         documents: Union[dict, List[dict]],
         clean_whitespace: Optional[bool] = None,
@@ -256,62 +262,80 @@
                 "'split_respect_sentence_boundary=True' is only compatible with split_by='word'."
             )
 
         text = document["content"]
 
         if split_respect_sentence_boundary and split_by == "word":
             # split by words ensuring no sub sentence splits
-            sentences = nltk.tokenize.sent_tokenize(text, language=self.language)
+            if self.language == "chinese":
+                sentences = text
+            else:
+                language_name = iso639_to_nltk.get(self.language)
+                sentences = nltk.tokenize.sent_tokenize(text, language=language_name)
+
             word_count = 0
             list_splits = []
             current_slice: List[str] = []
             for sen in sentences:
-                current_word_count = len(sen.split(" "))
+                if self.language == "chinese":
+                    current_word_count = len(sen)
+                else:
+                    current_word_count = len(sen.split(" "))
                 if current_word_count > split_length:
                     long_sentence_message = "One or more sentence found with word count higher than the split length."
                     if long_sentence_message not in self.print_log:
                         self.print_log.add(long_sentence_message)
                         logger.warning(long_sentence_message)
                 if word_count + current_word_count > split_length:
                     list_splits.append(current_slice)
                     # Enable split_stride with split_by='word' while respecting sentence boundaries.
                     if split_overlap:
                         overlap = []
                         w_count = 0
                         for s in current_slice[::-1]:
-                            sen_len = len(s.split(" "))
+                            if self.language == "chinese":
+                                sen_len = len(s)
+                            else:
+                                sen_len = len(s.split(" "))
                             if w_count < split_overlap:
                                 overlap.append(s)
                                 w_count += sen_len
                             else:
                                 break
                         current_slice = list(reversed(overlap))
                         word_count = w_count
                     else:
                         current_slice = []
                         word_count = 0
                 current_slice.append(sen)
-                word_count += len(sen.split(" "))
+                if self.language == "chinese":
+                    word_count += len(sen)
+                else:
+                    word_count += len(sen.split(" "))
             if current_slice:
                 list_splits.append(current_slice)
 
             text_splits = []
             for sl in list_splits:
-                txt = " ".join(sl)
+                if self.language == "chinese":
+                    txt = "".join(sl)
+                else:
+                    txt = " ".join(sl)
                 if len(txt) > 0:
                     text_splits.append(txt)
         else:
             # create individual "elements" of passage, sentence, or word
             # Faq text need to split text by '\n' of a passage
             if split_answers and split_by == "passage":
                 text_splits = text.split("\n")
             elif split_by == "passage":
                 elements = text.split("\n\n")
             elif split_by == "sentence":
-                elements = nltk.tokenize.sent_tokenize(text, language=self.language)
+                language_name = iso639_to_nltk.get(self.language)
+                elements = nltk.tokenize.sent_tokenize(text, language=language_name)
             elif split_by == "word":
                 elements = text.split(" ")
             else:
                 raise NotImplementedError(
                     "PreProcessor only supports 'passage', 'sentence' or 'word' split_by options."
                 )
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/question_generator/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/question_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/question_generator/question_generator.py` & `paddle-pipelines-0.5.3/pipelines/nodes/question_generator/question_generator.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/ranker/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/ranker/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/ranker/base.py` & `paddle-pipelines-0.5.3/pipelines/nodes/ranker/base.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/ranker/ernie_ranker.py` & `paddle-pipelines-0.5.3/pipelines/nodes/ranker/ernie_ranker.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/reader/base.py` & `paddle-pipelines-0.5.3/pipelines/nodes/reader/base.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/reader/ernie_dureader.py` & `paddle-pipelines-0.5.3/pipelines/nodes/reader/ernie_dureader.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/retriever/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/retriever/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # flake8: noqa
 from pipelines.nodes.retriever.base import BaseRetriever
 from pipelines.nodes.retriever.dense import DensePassageRetriever
 from pipelines.nodes.retriever.multimodal_retriever import MultiModalRetriever
 from pipelines.nodes.retriever.sparse import BM25Retriever
+from pipelines.nodes.retriever.web import WebRetriever
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/retriever/base.py` & `paddle-pipelines-0.5.3/pipelines/nodes/retriever/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,18 +166,17 @@
         self,
         query: str,
         query_type: Optional[ContentTypes] = None,
         filters: Optional[dict] = None,
         top_k: Optional[int] = None,
         index: Optional[str] = None,
         headers: Optional[Dict[str, str]] = None,
+        **kwargs,
     ):
-        documents = self.retrieve(
-            query=query, query_type=query_type, filters=filters, top_k=top_k, index=index, headers=headers
-        )
+        documents = self.retrieve(query=query, filters=filters, top_k=top_k, index=index, headers=headers, **kwargs)
         document_ids = [doc.id for doc in documents]
         logger.debug(f"Retrieved documents with IDs: {document_ids}")
         output = {"documents": documents}
 
         return output, "output_1"
 
     def run_query_batch(
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/retriever/dense.py` & `paddle-pipelines-0.5.3/pipelines/nodes/retriever/dense.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 # limitations under the License.
 
 import logging
 import os
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
 import numpy as np
 import paddle
 from tqdm.auto import tqdm
 
 from paddlenlp import Taskflow
 from paddlenlp.transformers import AutoModel, AutoTokenizer
 from pipelines.document_stores import BaseDocumentStore
@@ -52,14 +57,15 @@
         max_seq_len_passage: int = 384,
         top_k: int = 10,
         use_gpu: bool = True,
         batch_size: int = 16,
         embed_title: bool = True,
         similarity_function: str = "dot_product",
         progress_bar: bool = True,
+        mode: Literal["snippets", "raw_documents", "preprocessed_documents"] = "preprocessed_documents",
     ):
         """
         Init the Retriever incl. the two encoder models from a local or remote model checkpoint.
 
         **Example:**
 
                 ```python
@@ -120,14 +126,15 @@
             logger.warning("Batch size is less than the number of devices. All gpus will not be utilized.")
 
         self.document_store = document_store
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.top_k = top_k
         self.embed_title = embed_title
+        self.mode = mode
 
         if document_store is None:
             logger.warning("DensePassageRetriever initialized without a document store. ")
         elif document_store.similarity != "dot_product":
             logger.warning(
                 f"You are using a Dense Passage Retriever model with the {document_store.similarity} function. "
                 "We recommend you use dot_product instead. "
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/retriever/embedder.py` & `paddle-pipelines-0.5.3/pipelines/nodes/retriever/embedder.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/retriever/multimodal_retriever.py` & `paddle-pipelines-0.5.3/pipelines/nodes/retriever/multimodal_retriever.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/retriever/sparse.py` & `paddle-pipelines-0.5.3/pipelines/nodes/retriever/sparse.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/senta.py` & `paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/senta.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/senta_preprocessor.py` & `paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/senta_preprocessor.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/sentiment_analysis/senta_visualization.py` & `paddle-pipelines-0.5.3/pipelines/nodes/sentiment_analysis/senta_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             )
 
     def plot_aspect_with_opinion(
         self, aspect_opinion, save_path, sentiment="all", image_type="wordcloud", with_line_chart="true", top_n=15
     ):
         """
         generate image with aspect and opinion, that is, combining apsect with opinion to display the more specifical opinions of aspect.
-        this method can help you at two aspects: 1. mining custom's overall impression of products/services; 2. analyzing the quality of some aspect and improve it futher.
+        this method can help you at two aspects: 1. mining custom's overall impression of products/services; 2. analyzing the quality of some aspect and improve it further.
         Args:
             aspect_opinion (dict[dict] or dict): when sentiment set be "all", a expected dict containing aspect, opinion and its frequency, the key is aspect and its value is a dict containing the aspect's opinion and frequency. when sentiment set be "positive" or "netative", a expected dict containing aspect with opinion and frequency, the key is aspect with opinion and its value is frequency.
             aspect_sentiment (dict[dict]): a dict containing aspect, sentiment and its frequency, the key is aspect and its value is a dict containing the aspect's sentiment and frequency.
             save_path (str): path that the image is saved to.
             sentiment (str): analyzing aspect with sentiment, Only "all", "positive" and "negative" are received. "positive" only analyzes positive aspects with opinions, "negative" only analyzes negative aspects with opinions, and "all" analyzes all apsects.
             image_type (str): Only wordcloud and histogram are supported, that is, you should set be in [wordcloud, histogram].
             with_line_chart (bool): Whether to plot line chart, Only work when image_type is set be histogram.
```

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/text_to_image_generator/__init__.py` & `paddle-pipelines-0.5.3/pipelines/nodes/text_to_image_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/nodes/text_to_image_generator/text_to_image_generator.py` & `paddle-pipelines-0.5.3/pipelines/nodes/text_to_image_generator/text_to_image_generator.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/pipelines/__init__.py` & `paddle-pipelines-0.5.3/pipelines/pipelines/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,9 @@
     BaseStandardPipeline,
     DocPipeline,
     ExtractiveQAPipeline,
     QAGenerationPipeline,
     SemanticSearchPipeline,
     SentaPipeline,
     TextToImagePipeline,
+    WebQAPipeline,
 )
```

### Comparing `paddle-pipelines-0.5.2/pipelines/pipelines/base.py` & `paddle-pipelines-0.5.3/pipelines/pipelines/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,16 +251,14 @@
         :param pipeline_name: if the YAML contains multiple pipelines, the pipeline_name to load must be set.
         :param overwrite_with_env_variables: Overwrite the YAML configuration with environment variables. For example,
                                              to change index name param for an ElasticsearchDocumentStore, an env
                                              variable 'MYDOCSTORE_PARAMS_INDEX=documents-2021' can be set. Note that an
                                              `_` sign must be used to specify nested hierarchical properties.
         """
         pipeline_config = read_pipeline_config_from_yaml(path)
-        print(pipeline_config)
-        print(pipeline_name)
         if pipeline_config["version"] != __version__:
             logger.warning(
                 f"YAML version ({pipeline_config['version']}) does not match with pipelines version ({__version__}). "
                 "Issues may occur during loading. "
                 "To fix this warning, save again this pipeline with the current pipelines version using Pipeline.save_to_yaml(), "
                 f"or downgrade to pipelines version {__version__}."
             )
@@ -362,14 +360,15 @@
         :param component: The component object to be set at the node.
         """
         self.graph.nodes[name]["component"] = component
 
     def run(  # type: ignore
         self,
         query: Optional[str] = None,
+        history: Optional[Dict[str, str]] = None,
         file_paths: Optional[List[str]] = None,
         labels: Optional[MultiLabel] = None,
         documents: Optional[List[Document]] = None,
         meta: Optional[dict] = None,
         params: Optional[dict] = None,
         debug: Optional[bool] = None,
     ):
@@ -411,14 +410,16 @@
 
         node_output = None
         queue = {
             self.root_node: {"root_node": self.root_node, "params": params}
         }  # ordered dict with "node_id" -> "input" mapping that acts as a FIFO queue
         if query:
             queue[self.root_node]["query"] = query
+        if history:
+            queue[self.root_node]["history"] = history
         if file_paths:
             queue[self.root_node]["file_paths"] = file_paths
         if labels:
             queue[self.root_node]["labels"] = labels
         if documents:
             queue[self.root_node]["documents"] = documents
         if meta:
@@ -471,14 +472,16 @@
                                     updated_input["file_paths"] = file_paths
                                 if labels:
                                     updated_input["labels"] = labels
                                 if documents:
                                     updated_input["documents"] = documents
                                 if meta:
                                     updated_input["meta"] = meta
+                                if history:
+                                    updated_input["history"] = history
                             else:
                                 existing_input["inputs"].append(node_output)
                                 updated_input = existing_input
                             queue[n] = updated_input
                         else:
                             queue[n] = node_output
                 i = 0
@@ -747,21 +750,17 @@
         """
         pipeline_definition = get_pipeline_definition(pipeline_config=pipeline_config, pipeline_name=pipeline_name)
         component_definitions = get_component_definitions(
             pipeline_config=pipeline_config, overwrite_with_env_variables=overwrite_with_env_variables
         )
 
         pipeline = cls()
-        print(pipeline_definition)
         components: dict = {}  # instances of component objects.
         for node in pipeline_definition["nodes"]:
-            print("node", node)
             name = node["name"]
-            if name == "QAFilterPostprocessor":
-                print("exit")
             component = cls._load_or_get_component(name=name, definitions=component_definitions, components=components)
             pipeline.add_node(component=component, name=name, inputs=node.get("inputs", []))
 
         return pipeline
 
     @classmethod
     def _load_or_get_component(cls, name: str, definitions: dict, components: dict):
```

### Comparing `paddle-pipelines-0.5.2/pipelines/pipelines/config.py` & `paddle-pipelines-0.5.3/pipelines/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/pipelines/standard_pipelines.py` & `paddle-pipelines-0.5.3/pipelines/pipelines/standard_pipelines.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 from abc import ABC
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from pipelines.document_stores import BaseDocumentStore
 from pipelines.nodes.answer_extractor import AnswerExtractor, QAFilter
 from pipelines.nodes.base import BaseComponent
+from pipelines.nodes.prompt import PromptNode, Shaper
 from pipelines.nodes.question_generator import QuestionGenerator
-from pipelines.nodes.ranker import BaseRanker
+from pipelines.nodes.ranker import BaseRanker, ErnieRanker
 from pipelines.nodes.reader import BaseReader
-from pipelines.nodes.retriever import BaseRetriever
+from pipelines.nodes.retriever import BaseRetriever, WebRetriever
 from pipelines.nodes.text_to_image_generator import ErnieTextToImageGenerator
 from pipelines.pipelines import Pipeline
-from pipelines.schema import Document
+from pipelines.schema import Answer, Document
 
 logger = logging.getLogger(__name__)
 
 
 class BaseStandardPipeline(ABC):
     """
     Base class for pre-made standard pipelines pipelines.
@@ -346,7 +347,59 @@
               All debug information can then be found in the dict returned
               by this method under the key "_debug"
         """
         output = self.pipeline.run(meta=meta, params=params, debug=debug)
         if "examples" in output:
             output.pop("examples")
         return output
+
+
+class WebQAPipeline(BaseStandardPipeline):
+    """
+    Pipeline for Generative Question Answering performed based on Documents returned from a web search engine.
+    """
+
+    def __init__(
+        self,
+        retriever: WebRetriever,
+        prompt_node: PromptNode,
+        sampler: Optional[BaseRanker] = None,
+        shaper: Optional[Shaper] = None,
+    ):
+        """
+        :param retriever: The WebRetriever used for retrieving documents from a web search engine.
+        :param prompt_node: The PromptNode used for generating the answer based on retrieved documents.
+        :param shaper: The Shaper used for transforming the documents and scores into a format that can be used by the PromptNode. Optional.
+        """
+        if not shaper:
+            shaper = Shaper(func="join_documents_and_scores", inputs={"documents": "documents"}, outputs=["documents"])
+        if not sampler and retriever.mode != "snippets":
+            # Documents returned by WebRetriever in mode "snippets" already have scores.
+            # For other modes, we need to add a sampler if none is provided to compute the scores.
+            # TODO(wugaosheng): Add topsampler into WebQAPipeline
+            sampler = ErnieRanker("rocketqa-zh-dureader-cross-encoder", top_k=2)
+
+        self.pipeline = Pipeline()
+        self.pipeline.add_node(component=retriever, name="Retriever", inputs=["Query"])
+        if sampler:
+            self.pipeline.add_node(component=sampler, name="Sampler", inputs=["Retriever"])
+            self.pipeline.add_node(component=shaper, name="Shaper", inputs=["Sampler"])
+        else:
+            self.pipeline.add_node(component=shaper, name="Shaper", inputs=["Retriever"])
+        self.pipeline.add_node(component=prompt_node, name="PromptNode", inputs=["Shaper"])
+        self.metrics_filter = {"Retriever": ["recall_single_hit"]}
+
+    def run(self, query: str, params: Optional[dict] = None, debug: Optional[bool] = None):
+        """
+        :param query: The search query string.
+        :param params: Params for the `Retriever`, `Sampler`, `Shaper`, and ``PromptNode. For instance,
+                       params={"Retriever": {"top_k": 3}, "Sampler": {"top_p": 0.8}}. See the API documentation of each node for available parameters and their descriptions.
+        :param debug: Whether the pipeline should instruct nodes to collect debug information
+                      about their execution. By default, these include the input parameters
+                      they received and the output they generated.
+                      YOu can then find all debug information in the dict thia method returns
+                      under the key "_debug".
+        """
+        output = self.pipeline.run(query=query, params=params, debug=debug)
+        # Extract the answer from the last line of the PromptNode's output
+        output["answers"] = [Answer(answer=output["results"][0].split("\n")[-1], type="generative")]
+        return output
```

### Comparing `paddle-pipelines-0.5.2/pipelines/pipelines/utils.py` & `paddle-pipelines-0.5.3/pipelines/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/schema.py` & `paddle-pipelines-0.5.3/pipelines/schema.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/__init__.py` & `paddle-pipelines-0.5.3/pipelines/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/cleaning.py` & `paddle-pipelines-0.5.3/pipelines/utils/cleaning.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/common_utils.py` & `paddle-pipelines-0.5.3/pipelines/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/doc_store.py` & `paddle-pipelines-0.5.3/pipelines/utils/doc_store.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/export_utils.py` & `paddle-pipelines-0.5.3/pipelines/utils/export_utils.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/import_utils.py` & `paddle-pipelines-0.5.3/pipelines/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/logger.py` & `paddle-pipelines-0.5.3/pipelines/utils/logger.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/preprocessing.py` & `paddle-pipelines-0.5.3/pipelines/utils/preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Callable, Dict, List, Optional
-
-import re
 import logging
+import re
 from pathlib import Path
+from typing import Callable, Dict, List, Optional
 
 from pipelines.nodes.file_converter import (
     BaseConverter,
     DocxToTextConverter,
+    ImageToTextConverter,
+    MarkdownConverter,
     PDFToTextConverter,
     TextConverter,
-    ImageToTextConverter,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def convert_files_to_dicts(
     dir_path: str,
@@ -43,15 +43,15 @@
     :param dir_path: path for the documents to be written to the DocumentStore
     :param clean_func: a custom cleaning function that gets applied to each doc (input: str, output:str)
     :param split_paragraphs: split text in paragraphs.
     :param split_answers: split text into two columns, including question column, answer column.
     :param encoding: character encoding to use when converting pdf documents.
     """
     file_paths = [p for p in Path(dir_path).glob("**/*")]
-    allowed_suffixes = [".pdf", ".txt", ".docx", ".png", ".jpg"]
+    allowed_suffixes = [".pdf", ".txt", ".docx", ".png", ".jpg", ".md"]
     suffix2converter: Dict[str, BaseConverter] = {}
 
     suffix2paths: Dict[str, List[Path]] = {}
     for path in file_paths:
         file_suffix = path.suffix.lower()
         if file_suffix in allowed_suffixes:
             if file_suffix not in suffix2paths:
@@ -69,14 +69,16 @@
             suffix2converter[file_suffix] = PDFToTextConverter()
         if file_suffix == ".txt":
             suffix2converter[file_suffix] = TextConverter()
         if file_suffix == ".docx":
             suffix2converter[file_suffix] = DocxToTextConverter()
         if file_suffix == ".png" or file_suffix == ".jpg":
             suffix2converter[file_suffix] = ImageToTextConverter()
+        if file_suffix == ".md":
+            suffix2converter[file_suffix] = MarkdownConverter()
 
     documents = []
     for suffix, paths in suffix2paths.items():
         for path in paths:
             if encoding is None and suffix == ".pdf":
                 encoding = "Latin1"
             logger.info("Converting {}".format(path))
```

### Comparing `paddle-pipelines-0.5.2/pipelines/utils/tokenization.py` & `paddle-pipelines-0.5.3/pipelines/utils/tokenization.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/setup.py` & `paddle-pipelines-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/utils/__init__.py` & `paddle-pipelines-0.5.3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/utils/offline_ann.py` & `paddle-pipelines-0.5.3/utils/offline_ann.py`

 * *Files identical despite different names*

### Comparing `paddle-pipelines-0.5.2/utils/offline_ann_mm.py` & `paddle-pipelines-0.5.3/utils/offline_ann_mm.py`

 * *Files identical despite different names*

