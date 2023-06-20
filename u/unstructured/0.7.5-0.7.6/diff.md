# Comparing `tmp/unstructured-0.7.5.tar.gz` & `tmp/unstructured-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.5.tar", last modified: Wed Jun 14 06:10:10 2023, max compression
+gzip compressed data, was "unstructured-0.7.6.tar", last modified: Fri Jun 16 15:25:02 2023, max compression
```

## Comparing `unstructured-0.7.5.tar` & `unstructured-0.7.6.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.747967 unstructured-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-14 06:09:58.000000 unstructured-0.7.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-14 06:09:58.000000 unstructured-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-14 06:10:10.747967 unstructured-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-06-14 06:09:58.000000 unstructured-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.723967 unstructured-0.7.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-14 06:10:10.751967 unstructured-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-14 06:09:58.000000 unstructured-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.723967 unstructured-0.7.5/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.731967 unstructured-0.7.5/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.731967 unstructured-0.7.5/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.731967 unstructured-0.7.5/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.735967 unstructured-0.7.5/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.735967 unstructured-0.7.5/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24579 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.735967 unstructured-0.7.5/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.743967 unstructured-0.7.5/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.747967 unstructured-0.7.5/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.747967 unstructured-0.7.5/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.920739 unstructured-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-16 15:24:53.000000 unstructured-0.7.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 15:24:53.000000 unstructured-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-06-16 15:25:02.920739 unstructured-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-06-16 15:24:53.000000 unstructured-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.908739 unstructured-0.7.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 15:24:53.000000 unstructured-0.7.6/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 15:25:02.924739 unstructured-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-16 15:24:53.000000 unstructured-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.908739 unstructured-0.7.6/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.908739 unstructured-0.7.6/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-16 15:24:53.000000 unstructured-0.7.6/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 15:24:53.000000 unstructured-0.7.6/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-16 15:24:53.000000 unstructured-0.7.6/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-16 15:24:53.000000 unstructured-0.7.6/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.908739 unstructured-0.7.6/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.908739 unstructured-0.7.6/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.912739 unstructured-0.7.6/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.912739 unstructured-0.7.6/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.912739 unstructured-0.7.6/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.912739 unstructured-0.7.6/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.912739 unstructured-0.7.6/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25155 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.912739 unstructured-0.7.6/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.920739 unstructured-0.7.6/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.920739 unstructured-0.7.6/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.920739 unstructured-0.7.6/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-16 15:24:53.000000 unstructured-0.7.6/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:25:02.908739 unstructured-0.7.6/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-06-16 15:25:02.000000 unstructured-0.7.6/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-16 15:25:02.000000 unstructured-0.7.6/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:25:02.000000 unstructured-0.7.6/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 15:25:02.000000 unstructured-0.7.6/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 15:25:02.000000 unstructured-0.7.6/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 15:25:02.000000 unstructured-0.7.6/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.5/LICENSE.md` & `unstructured-0.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/PKG-INFO` & `unstructured-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.5
+Version: 0.7.6
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -25,15 +25,15 @@
           [![Downloads](https://static.pepy.tech/badge/unstructured/month)](https://pepy.tech/project/unstructured)
         
         </div>
         
         <div>
           <p align="center">
           <a
-          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
+          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ">
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
         
@@ -106,16 +106,19 @@
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
+        | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
+        | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
+        | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
         
         
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.5 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.6 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -69,16 +69,19 @@
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
 Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
-Include Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes |
-None | | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Include Page Breaks | | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None
+| | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | | Word
+Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | Word Documents
+(`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
+(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.5/README.md` & `unstructured-0.7.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   [![Downloads](https://static.pepy.tech/badge/unstructured/month)](https://pepy.tech/project/unstructured)
 
 </div>
 
 <div>
   <p align="center">
   <a
-  href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
+  href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ">
     <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
   </a>
   <a href="https://www.linkedin.com/company/unstructuredio/">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
   </a>
 </div>
 
@@ -98,16 +98,19 @@
 | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
 | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
 | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
 | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
 | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
 | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
+| TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
 | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
 | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
+| Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
+| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
 | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
 
 
 
 ## :dizzy: Instructions for using the docker image
 
 The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
```

#### html2text {}

```diff
@@ -65,16 +65,19 @@
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
 Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
-Include Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes |
-None | | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Include Page Breaks | | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None
+| | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | | Word
+Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | Word Documents
+(`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
+(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.5/setup.py` & `unstructured-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.6/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.6/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/test_unstructured/test_utils.py` & `unstructured-0.7.6/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/cleaners/core.py` & `unstructured-0.7.6/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/cleaners/extract.py` & `unstructured-0.7.6/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/cleaners/translate.py` & `unstructured-0.7.6/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/documents/base.py` & `unstructured-0.7.6/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/documents/elements.py` & `unstructured-0.7.6/unstructured/documents/elements.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 import datetime
 import hashlib
+import inspect
 import os
 import pathlib
+import re
 from abc import ABC
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
+from functools import wraps
+from typing import Any, Callable, Dict, List, Optional, Tuple, TypedDict, Union, cast
 
 
 class NoID(ABC):
     """Class to indicate that an element do not have an ID."""
 
     pass
 
@@ -26,14 +29,22 @@
     date_modified: Optional[str] = None
     date_processed: Optional[str] = None
 
     def to_dict(self):
         return {key: value for key, value in self.__dict__.items() if value is not None}
 
 
+class RegexMetadata(TypedDict):
+    """Metadata that is extracted from a document element via regex."""
+
+    text: str
+    start: int
+    end: int
+
+
 @dataclass
 class ElementMetadata:
     data_source: Optional[DataSourceMetadata] = None
     filename: Optional[str] = None
     file_directory: Optional[str] = None
     date: Optional[str] = None
     filetype: Optional[str] = None
@@ -48,31 +59,39 @@
     url: Optional[str] = None
 
     # E-mail specific metadata fields
     sent_from: Optional[List[str]] = None
     sent_to: Optional[List[str]] = None
     subject: Optional[str] = None
 
+    # MSFT Word specific metadata fields
+    header_footer_type: Optional[str] = None
+
     # Text format metadata fields
     text_as_html: Optional[str] = None
 
+    # Metadata extracted via regex
+    regex_metadata: Optional[Dict[str, List[RegexMetadata]]] = None
+
     def __post_init__(self):
         if isinstance(self.filename, pathlib.Path):
             self.filename = str(self.filename)
 
         if self.filename is not None:
             file_directory, filename = os.path.split(self.filename)
             self.file_directory = file_directory or None
             self.filename = filename
 
     def to_dict(self):
-        dict = {key: value for key, value in self.__dict__.items() if value is not None}
+        _dict = {key: value for key, value in self.__dict__.items() if value is not None}
+        if "regex_metadata" in _dict and not _dict["regex_metadata"]:
+            _dict.pop("regex_metadata")
         if self.data_source:
-            dict["data_source"] = cast(DataSourceMetadata, self.data_source).to_dict()
-        return dict
+            _dict["data_source"] = cast(DataSourceMetadata, self.data_source).to_dict()
+        return _dict
 
     @classmethod
     def from_dict(cls, input_dict):
         return cls(**input_dict)
 
     def merge(self, other: ElementMetadata):
         for k in self.__dict__:
@@ -84,14 +103,66 @@
         """Converts the date field to a datetime object."""
         dt = None
         if self.date is not None:
             dt = datetime.datetime.fromisoformat(self.date)
         return dt
 
 
+def process_metadata():
+    """Decorator for processing metadata for document elements."""
+
+    def decorator(func: Callable):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            elements = func(*args, **kwargs)
+            sig = inspect.signature(func)
+            params = dict(**dict(zip(sig.parameters, args)), **kwargs)
+            for param in sig.parameters.values():
+                if param.name not in params and param.default is not param.empty:
+                    params[param.name] = param.default
+
+            regex_metadata: Dict["str", "str"] = params.get("regex_metadata", {})
+            elements = _add_regex_metadata(elements, regex_metadata)
+
+            return elements
+
+        return wrapper
+
+    return decorator
+
+
+def _add_regex_metadata(
+    elements: List[Element],
+    regex_metadata: Dict[str, str] = {},
+) -> List[Element]:
+    """Adds metadata based on a user provided regular expression.
+    The additional metadata will be added to the regex_metadata
+    attrbuted in the element metadata."""
+    for element in elements:
+        if isinstance(element, Text):
+            _regex_metadata: Dict["str", List[RegexMetadata]] = {}
+            for field_name, pattern in regex_metadata.items():
+                results: List[RegexMetadata] = []
+                for result in re.finditer(pattern, element.text):
+                    start, end = result.span()
+                    results.append(
+                        {
+                            "text": element.text[start:end],
+                            "start": start,
+                            "end": end,
+                        },
+                    )
+                if len(results) > 0:
+                    _regex_metadata[field_name] = results
+
+            element.metadata.regex_metadata = _regex_metadata
+
+    return elements
+
+
 class Element(ABC):
     """An element is a section of a page in the document."""
 
     def __init__(
         self,
         element_id: Union[str, NoID] = NoID(),
         coordinates: Optional[Tuple[Tuple[float, float], ...]] = None,
@@ -261,21 +332,39 @@
     """An element for capturing tables."""
 
     category = "Table"
 
     pass
 
 
+class Header(Text):
+    """An element for capturing document headers."""
+
+    category = "Header"
+
+    pass
+
+
+class Footer(Text):
+    """An element for capturing document footers."""
+
+    category = "Footer"
+
+    pass
+
+
 TYPE_TO_TEXT_ELEMENT_MAP: Dict[str, Any] = {
     "UncategorizedText": Text,
     "FigureCaption": FigureCaption,
     "Figure": FigureCaption,
     "Text": NarrativeText,
     "NarrativeText": NarrativeText,
     "ListItem": ListItem,
     "BulletedText": ListItem,
     "Title": Title,
     "Address": Address,
     "Image": Image,
     "PageBreak": PageBreak,
     "Table": Table,
+    "Header": Header,
+    "Footer": Footer,
 }
```

### Comparing `unstructured-0.7.5/unstructured/documents/email_elements.py` & `unstructured-0.7.6/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/documents/html.py` & `unstructured-0.7.6/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/documents/xml.py` & `unstructured-0.7.6/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/file_utils/encoding.py` & `unstructured-0.7.6/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/file_utils/exploration.py` & `unstructured-0.7.6/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.6/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/file_utils/filetype.py` & `unstructured-0.7.6/unstructured/file_utils/filetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
     # Plain Text Types
     EML = 40
     RTF = 41
     TXT = 42
     JSON = 43
     CSV = 44
+    TSV = 45
 
     # Markup Types
     HTML = 50
     XML = 51
     MD = 52
     EPUB = 53
     RST = 54
@@ -102,14 +103,15 @@
     "text/plain": FileType.TXT,
     "text/x-csv": FileType.CSV,
     "application/csv": FileType.CSV,
     "application/x-csv": FileType.CSV,
     "text/comma-separated-values": FileType.CSV,
     "text/x-comma-separated-values": FileType.CSV,
     "text/csv": FileType.CSV,
+    "text/tsv": FileType.TSV,
     "text/markdown": FileType.MD,
     "text/x-markdown": FileType.MD,
     "text/x-rst": FileType.RST,
     "application/epub": FileType.EPUB,
     "application/epub+zip": FileType.EPUB,
     "application/json": FileType.JSON,
     "application/rtf": FileType.RTF,
@@ -162,14 +164,15 @@
     ".ppt": FileType.PPT,
     ".rtf": FileType.RTF,
     ".json": FileType.JSON,
     ".epub": FileType.EPUB,
     ".msg": FileType.MSG,
     ".odt": FileType.ODT,
     ".csv": FileType.CSV,
+    ".tsv": FileType.TSV,
     # NOTE(robinson) - for now we are treating code files as plain text
     ".js": FileType.TXT,
     ".py": FileType.TXT,
     ".java": FileType.TXT,
     ".cpp": FileType.TXT,
     ".cc": FileType.TXT,
     ".cxx": FileType.TXT,
@@ -225,15 +228,19 @@
             import filetype as ft
 
             mime_type = ft.guess_mime(filename)
         if mime_type is None:
             return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
     elif file is not None:
-        extension = None
+        if hasattr(file, "name"):
+            _, extension = os.path.splitext(file.name)
+        else:
+            extension = ""
+        extension = extension.lower()
         # NOTE(robinson) - the python-magic docs recommend reading at least the first 2048 bytes
         # Increased to 4096 because otherwise .xlsx files get detected as a zip file
         # ref: https://github.com/ahupp/python-magic#usage
         if LIBMAGIC_AVAILABLE:
             mime_type = magic.from_buffer(file.read(4096), mime=True)
         else:
             import filetype as ft
@@ -247,76 +254,68 @@
             return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
     else:
         raise ValueError("No filename, file, nor file_filename were specified.")
 
     """Mime type special cases."""
     # third check (mime_type)
-    # NOTE(crag): for older versions of the OS libmagic package, such as is currently
-    # installed on the Unstructured docker image, .json files resolve to "text/plain"
-    # rather than "application/json". this corrects for that case.
-    if mime_type == "text/plain" and extension == ".json":
-        return FileType.JSON
 
     # NOTE(Crag): older magic lib does not differentiate between xls and doc
     if mime_type == "application/msword" and extension == ".xls":
         return FileType.XLS
 
     elif mime_type.endswith("xml"):
-        if extension and (extension == ".html" or extension == ".htm"):
+        if extension == ".html" or extension == ".htm":
             return FileType.HTML
         else:
             return FileType.XML
 
     elif mime_type in TXT_MIME_TYPES or mime_type.startswith("text"):
-        if extension and extension == ".eml":
-            return FileType.EML
-        elif extension and extension == ".md":
-            return FileType.MD
-        elif extension and extension == ".rst":
-            return FileType.RST
-        elif extension and extension == ".rtf":
-            return FileType.RTF
-        elif extension and extension == ".html":
-            return FileType.HTML
-
+        # NOTE(crag): for older versions of the OS libmagic package, such as is currently
+        # installed on the Unstructured docker image, .json files resolve to "text/plain"
+        # rather than "application/json". this corrects for that case.
         if _is_text_file_a_json(file=file, filename=filename, encoding=encoding):
             return FileType.JSON
 
         if _is_text_file_a_csv(file=file, filename=filename, encoding=encoding):
             return FileType.CSV
 
-        if file and not extension and _check_eml_from_buffer(file=file) is True:
+        if file and _check_eml_from_buffer(file=file) is True:
             return FileType.EML
 
+        if extension in [".eml", ".md", ".rtf", ".html", ".rst", ".tsv", ".json"]:
+            return EXT_TO_FILETYPE.get(extension)
+
         # Safety catch
         if mime_type in STR_TO_FILETYPE:
             return STR_TO_FILETYPE[mime_type]
 
         return FileType.TXT
 
     elif mime_type == "application/octet-stream":
-        if file and not extension:
+        if extension == ".docx":
+            return FileType.DOCX
+        elif file:
             return _detect_filetype_from_octet_stream(file=file)
         else:
             return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
     elif mime_type == "application/zip":
         filetype = FileType.UNK
-        if file and not extension:
+        if file:
             filetype = _detect_filetype_from_octet_stream(file=file)
         elif filename is not None:
             with open(filename, "rb") as f:
                 filetype = _detect_filetype_from_octet_stream(file=f)
 
         extension = extension if extension else ""
         if filetype == FileType.UNK:
-            return EXT_TO_FILETYPE.get(extension.lower(), FileType.ZIP)
+            return FileType.ZIP
         else:
-            return EXT_TO_FILETYPE.get(extension.lower(), filetype)
+            return EXT_TO_FILETYPE.get(extension, filetype)
 
     elif _is_code_mime_type(mime_type):
         # NOTE(robinson) - we'll treat all code files as plain text for now.
         # we can update this logic and add filetypes for specific languages
         # later if needed.
         return FileType.TXT
 
@@ -442,14 +441,15 @@
         filetype = FileType.JPG.name
     else:
         filetype = None
     elements = _add_element_metadata(
         elements,
         include_page_breaks=include_page_breaks,
         filetype=filetype,
+        initial_page_number=1,
     )
     return elements
 
 
 PROGRAMMING_LANGUAGES = [
     "javascript",
     "python",
```

### Comparing `unstructured-0.7.5/unstructured/file_utils/metadata.py` & `unstructured-0.7.6/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/azure.py` & `unstructured-0.7.6/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.6/unstructured/ingest/connector/biomed.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from dataclasses import dataclass
 from ftplib import FTP, error_perm
 from pathlib import Path
 from typing import List, Union
 
 import requests
 from bs4 import BeautifulSoup
+from requests.adapters import HTTPAdapter
+from urllib3.util import Retry
 
 from unstructured.ingest.interfaces import (
     BaseConnector,
     BaseConnectorConfig,
     BaseIngestDoc,
     StandardConnectorConfig,
 )
@@ -39,14 +41,17 @@
     id_, from_, until, format are API parameters."""
 
     path: str
     # OA Web Service API Options
     id_: str
     from_: str
     until: str
+    max_retries: int = 5
+    request_timeout: int = 45
+    decay: float = 0.3
 
     def validate_api_inputs(self):
         valid = False
 
         if self.from_:
             valid = validate_date_args(self.from_)
 
@@ -91,15 +96,17 @@
                 if "no such file or directory" in exc.args[0].lower():
                     raise ValueError(f"The path: {path} is not valid.")
                 elif "not a directory" in exc.args[0].lower():
                     self.is_file = True
                 elif "command successful" in response:
                     self.is_dir = True
                 else:
-                    raise ValueError("Something went wrong when validating the path: {path}.")
+                    raise ValueError(
+                        "Something went wrong when validating the path: {path}.",
+                    )
 
 
 @dataclass
 class BiomedIngestDoc(BaseIngestDoc):
     config: SimpleBiomedConfig
     file_meta: BiomedFileMeta
 
@@ -144,24 +151,30 @@
     def write_result(self):
         """Write the structured json result for this doc. result must be json serializable."""
         if self.standard_config.download_only:
             return
         output_filename = self._output_filename()
         output_filename.parent.mkdir(parents=True, exist_ok=True)
         with open(output_filename, "w") as output_f:
-            output_f.write(json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2))
+            output_f.write(
+                json.dumps(self.isd_elems_no_filename, ensure_ascii=False, indent=2),
+            )
         logger.info(f"Wrote {output_filename}")
 
 
 class BiomedConnector(BaseConnector):
     """Objects of this class support fetching documents from Biomedical literature FTP directory"""
 
     config: SimpleBiomedConfig
 
-    def __init__(self, standard_config: StandardConnectorConfig, config: SimpleBiomedConfig):
+    def __init__(
+        self,
+        standard_config: StandardConnectorConfig,
+        config: SimpleBiomedConfig,
+    ):
         super().__init__(standard_config, config)
         self.cleanup_files = (
             not self.standard_config.preserve_downloads and not self.standard_config.download_only
         )
 
     def _list_objects_api(self):
         def urls_to_metadata(urls):
@@ -194,15 +207,23 @@
         if self.config.from_:
             endpoint_url += f"&from={self.config.from_}"
 
         if self.config.until:
             endpoint_url += f"&until={self.config.until}"
 
         while endpoint_url:
-            response = requests.get(endpoint_url)
+            session = requests.Session()
+            retries = Retry(
+                total=self.config.max_retries,
+                backoff_factor=self.config.decay,
+            )
+            adapter = HTTPAdapter(max_retries=retries)
+            session.mount("http://", adapter)
+            session.mount("https://", adapter)
+            response = session.get(endpoint_url, timeout=self.config.request_timeout)
             soup = BeautifulSoup(response.content, features="lxml")
             urls = [link["href"] for link in soup.find_all("link")]
 
             if not urls:
                 return files
 
             endpoint_url = urls[-1] if "resumptiontoken" in urls[-1].lower() else None
```

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/discord.py` & `unstructured-0.7.6/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.6/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/git.py` & `unstructured-0.7.6/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/github.py` & `unstructured-0.7.6/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.6/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.6/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/local.py` & `unstructured-0.7.6/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.6/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/s3.py` & `unstructured-0.7.6/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/slack.py` & `unstructured-0.7.6/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.6/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.6/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/interfaces.py` & `unstructured-0.7.6/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/ingest/main.py` & `unstructured-0.7.6/unstructured/ingest/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,29 @@
 )
 @click.option(
     "--biomed-api-until",
     default=None,
     help="Until parameter for OA Web Service API.",
 )
 @click.option(
+    "--biomed-max-retries",
+    default=1,
+    help="Max requests to OA Web Service API.",
+)
+@click.option(
+    "--biomed-max-request-time",
+    default=45,
+    help="(In seconds) Max request time to OA Web Service API.",
+)
+@click.option(
+    "--biomed-decay",
+    default=0.3,
+    help="(In float) Factor to multiply the delay between retries.",
+)
+@click.option(
     "--wikipedia-page-title",
     default=None,
     help='Title of a Wikipedia page, e.g. "Open source software".',
 )
 @click.option(
     "--wikipedia-auto-suggest",
     default=True,
@@ -409,14 +424,17 @@
     drive_service_account_key,
     drive_recursive,
     drive_extension,
     biomed_path,
     biomed_api_id,
     biomed_api_from,
     biomed_api_until,
+    biomed_max_retries,
+    biomed_max_request_time,
+    biomed_decay,
     wikipedia_page_title,
     wikipedia_auto_suggest,
     github_url,
     gitlab_url,
     git_access_token,
     git_branch,
     git_file_glob,
@@ -716,14 +734,17 @@
         doc_connector = BiomedConnector(  # type: ignore
             standard_config=standard_config,
             config=SimpleBiomedConfig(
                 path=biomed_path,
                 id_=biomed_api_id,
                 from_=biomed_api_from,
                 until=biomed_api_until,
+                max_retries=biomed_max_retries,
+                request_timeout=biomed_max_request_time,
+                decay=biomed_decay,
             ),
         )
     elif local_input_path:
         from unstructured.ingest.connector.local import (
             LocalConnector,
             SimpleLocalConfig,
         )
```

### Comparing `unstructured-0.7.5/unstructured/nlp/english-words.txt` & `unstructured-0.7.6/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/nlp/english_words.py` & `unstructured-0.7.6/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/nlp/patterns.py` & `unstructured-0.7.6/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/nlp/tokenize.py` & `unstructured-0.7.6/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/partition/__init__.py` & `unstructured-0.7.6/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/partition/api.py` & `unstructured-0.7.6/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/partition/auto.py` & `unstructured-0.7.6/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from unstructured.partition.odt import partition_odt
 from unstructured.partition.pdf import partition_pdf
 from unstructured.partition.ppt import partition_ppt
 from unstructured.partition.pptx import partition_pptx
 from unstructured.partition.rst import partition_rst
 from unstructured.partition.rtf import partition_rtf
 from unstructured.partition.text import partition_text
+from unstructured.partition.tsv import partition_tsv
 from unstructured.partition.xlsx import partition_xlsx
 from unstructured.partition.xml import partition_xml
 
 
 def partition(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
@@ -207,14 +208,16 @@
         )
     elif filetype == FileType.JSON:
         elements = partition_json(filename=filename, file=file)
     elif (filetype == FileType.XLSX) or (filetype == FileType.XLS):
         elements = partition_xlsx(filename=filename, file=file)
     elif filetype == FileType.CSV:
         elements = partition_csv(filename=filename, file=file)
+    elif filetype == FileType.TSV:
+        elements = partition_tsv(filename=filename, file=file)
     elif filetype == FileType.EMPTY:
         elements = []
     else:
         msg = "Invalid file" if not filename else f"Invalid file {filename}"
         raise ValueError(f"{msg}. The {filetype} file type is not supported in partition.")
 
     for element in elements:
```

### Comparing `unstructured-0.7.5/unstructured/partition/common.py` & `unstructured-0.7.6/unstructured/partition/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,43 +73,45 @@
 
 def _add_element_metadata(
     layout_elements,
     include_page_breaks: bool = False,
     filename: Optional[str] = None,
     filetype: Optional[str] = None,
     url: Optional[str] = None,
+    initial_page_number: Optional[int] = None,
 ) -> List[Element]:
     """Adds document metadata to the document element. Document metadata includes information
     like the filename, source url, and page number."""
     elements: List[Element] = []
-    page_number: int = 1
+    page_number: Optional[int] = initial_page_number
     for layout_element in layout_elements:
         element = normalize_layout_element(layout_element)
         if hasattr(layout_element, "text_as_html"):
             text_as_html: Optional[str] = layout_element.text_as_html
         else:
             text_as_html = None
         # NOTE(robinson) - defer to the page number that's already in the metadata
         # if it's available
         if hasattr(element, "metadata"):
             page_number = element.metadata.page_number or page_number
-
         metadata = ElementMetadata(
             filename=filename,
             filetype=filetype,
             url=url,
             page_number=page_number,
             text_as_html=text_as_html,
         )
         if isinstance(element, list):
             for _element in element:
                 _element.metadata = metadata.merge(_element.metadata)
             elements.extend(element)
         elif isinstance(element, PageBreak):
-            page_number += 1
+            if page_number is not None:
+                page_number += 1
+            element.metadata = metadata.merge(element.metadata)
             if include_page_breaks:
                 elements.append(element)
         else:
             element.metadata = metadata.merge(element.metadata)
             elements.append(element)
     return elements
```

### Comparing `unstructured-0.7.5/unstructured/partition/csv.py` & `unstructured-0.7.6/unstructured/partition/csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, List, Optional, Union, cast
 
 import lxml.html
 import pandas as pd
 
-from unstructured.documents.elements import Element, ElementMetadata, Table
+from unstructured.documents.elements import (
+    Element,
+    ElementMetadata,
+    Table,
+    process_metadata,
+)
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.CSV)
 def partition_csv(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
+    **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Excel Documents in .csv format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.7.5/unstructured/partition/doc.py` & `unstructured-0.7.6/unstructured/partition/doc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import os
 import tempfile
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import convert_office_doc, exactly_one
 from unstructured.partition.docx import partition_docx
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.DOC)
-def partition_doc(filename: Optional[str] = None, file: Optional[IO] = None) -> List[Element]:
+def partition_doc(
+    filename: Optional[str] = None,
+    file: Optional[IO] = None,
+    include_page_breaks: bool = True,
+    **kwargs,
+) -> List[Element]:
     """Partitions Microsoft Word Documents in .doc format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
@@ -37,10 +43,14 @@
         _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
 
     base_filename, _ = os.path.splitext(filename_no_path)
 
     with tempfile.TemporaryDirectory() as tmpdir:
         convert_office_doc(filename, tmpdir, target_format="docx")
         docx_filename = os.path.join(tmpdir, f"{base_filename}.docx")
-        elements = partition_docx(filename=docx_filename, metadata_filename=filename)
+        elements = partition_docx(
+            filename=docx_filename,
+            metadata_filename=filename,
+            include_page_breaks=include_page_breaks,
+        )
 
     return elements
```

### Comparing `unstructured-0.7.5/unstructured/partition/email.py` & `unstructured-0.7.6/unstructured/partition/email.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from unstructured.documents.elements import (
     Element,
     ElementMetadata,
     Image,
     NarrativeText,
     Text,
     Title,
+    process_metadata,
 )
 from unstructured.documents.email_elements import (
     MetaData,
     ReceivedInfo,
     Recipient,
     Sender,
     Subject,
@@ -178,22 +179,24 @@
     image_raw_info = element.text[start:end]
     image_info = clean_extra_whitespace(image_raw_info.split(":")[1])
     element.text = element.text.replace("[image: " + image_info[:-1] + "]", "")
 
     return Image(text=image_info[:-1]), element
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.EML)
 def partition_email(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     content_source: str = "text/html",
     encoding: Optional[str] = None,
     include_headers: bool = False,
+    **kwargs,
 ) -> List[Element]:
     """Partitions an .eml documents into its constituent elements.
     Parameters
     ----------
      filename
         A string defining the target filename path.
     file
```

### Comparing `unstructured-0.7.5/unstructured/partition/epub.py` & `unstructured-0.7.6/unstructured/partition/rst.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
-@add_metadata_with_filetype(FileType.EPUB)
-def partition_epub(
+@process_metadata()
+@add_metadata_with_filetype(FileType.RST)
+def partition_rst(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     include_page_breaks: bool = False,
+    **kwargs,
 ) -> List[Element]:
-    """Partitions an EPUB document. The document is first converted to HTML and then
-    partitoned using partiton_html.
+    """Partitions an RST document. The document is first converted to HTML and then
+    partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it
     """
     return convert_and_partition_html(
-        source_format="epub",
+        source_format="rst",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
     )
```

### Comparing `unstructured-0.7.5/unstructured/partition/html.py` & `unstructured-0.7.6/unstructured/partition/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from typing import IO, Dict, List, Optional
 
 import requests
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.documents.html import HTMLDocument
 from unstructured.documents.xml import VALID_PARSERS
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.file_conversion import convert_file_to_html_text
 from unstructured.file_utils.filetype import (
     FileType,
     add_metadata_with_filetype,
     document_to_element_list,
 )
 from unstructured.partition.common import (
     exactly_one,
 )
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.HTML)
 def partition_html(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     encoding: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     parser: VALID_PARSERS = None,
+    **kwargs,
 ) -> List[Element]:
     """Partitions an HTML document into its constituent elements.
 
     Parameters
     ----------
      filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.7.5/unstructured/partition/image.py` & `unstructured-0.7.6/unstructured/partition/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.partition.common import exactly_one
 from unstructured.partition.pdf import partition_pdf_or_image
 
 
+@process_metadata()
 def partition_image(
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = None,
     template: Optional[str] = None,
     token: Optional[str] = None,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
     strategy: str = "auto",
+    **kwargs,
 ) -> List[Element]:
     """Parses an image into a list of interpreted elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.7.5/unstructured/partition/json.py` & `unstructured-0.7.6/unstructured/partition/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import json
 import re
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import exactly_one
 from unstructured.staging.base import dict_to_elements
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.JSON)
 def partition_json(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
+    **kwargs,
 ) -> List[Element]:
     """Partitions an .json document into its constituent elements."""
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     exactly_one(filename=filename, file=file, text=text)
```

### Comparing `unstructured-0.7.5/unstructured/partition/md.py` & `unstructured-0.7.6/unstructured/partition/md.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from typing import IO, List, Optional, Union
 
 import markdown
 import requests
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.documents.xml import VALID_PARSERS
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one
 from unstructured.partition.html import partition_html
 
 
 def optional_decode(contents: Union[str, bytes]) -> str:
     if isinstance(contents, bytes):
         return contents.decode("utf-8")
     return contents
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.MD)
 def partition_md(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     parser: VALID_PARSERS = None,
+    **kwargs,
 ) -> List[Element]:
     # Verify that only one of the arguments was provided
     if text is None:
         text = ""
     exactly_one(filename=filename, file=file, text=text, url=url)
 
     if filename is not None:
```

### Comparing `unstructured-0.7.5/unstructured/partition/msg.py` & `unstructured-0.7.6/unstructured/partition/msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import tempfile
 from typing import IO, Dict, List, Optional
 
 import msg_parser
 
-from unstructured.documents.elements import Element, ElementMetadata
+from unstructured.documents.elements import Element, ElementMetadata, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one
 from unstructured.partition.email import convert_to_iso_8601
 from unstructured.partition.html import partition_html
 from unstructured.partition.text import partition_text
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.MSG)
 def partition_msg(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
+    **kwargs,
 ) -> List[Element]:
     """Partitions a MSFT Outlook .msg file
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.7.5/unstructured/partition/odt.py` & `unstructured-0.7.6/unstructured/partition/odt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.docx import convert_and_partition_docx
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.ODT)
-def partition_odt(filename: Optional[str] = None, file: Optional[IO] = None) -> List[Element]:
+def partition_odt(
+    filename: Optional[str] = None,
+    file: Optional[IO] = None,
+    **kwargs,
+) -> List[Element]:
     """Partitions Open Office Documents in .odt format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
```

### Comparing `unstructured-0.7.5/unstructured/partition/pdf.py` & `unstructured-0.7.6/unstructured/partition/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 
 import pdf2image
 from pdfminer.high_level import extract_pages
 from pdfminer.utils import open_filename
 from PIL import Image
 
 from unstructured.cleaners.core import clean_extra_whitespace
-from unstructured.documents.elements import Element, ElementMetadata, PageBreak
+from unstructured.documents.elements import (
+    Element,
+    ElementMetadata,
+    PageBreak,
+    process_metadata,
+)
 from unstructured.file_utils.filetype import (
     FileType,
     add_metadata_with_filetype,
     document_to_element_list,
 )
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition import _partition_via_api
@@ -22,25 +27,27 @@
     spooled_to_bytes_io_if_needed,
 )
 from unstructured.partition.strategies import determine_pdf_or_image_strategy
 from unstructured.partition.text import element_from_text, partition_text
 from unstructured.utils import requires_dependencies
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.PDF)
 def partition_pdf(
     filename: str = "",
     file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
     token: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     infer_table_structure: bool = False,
     ocr_languages: str = "eng",
+    **kwargs,
 ) -> List[Element]:
     """Parses a pdf document into a list of interpreted elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
```

### Comparing `unstructured-0.7.5/unstructured/partition/ppt.py` & `unstructured-0.7.6/unstructured/partition/ppt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import tempfile
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import convert_office_doc, exactly_one
 from unstructured.partition.pptx import partition_pptx
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.PPT)
 def partition_ppt(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     include_page_breaks: bool = False,
+    **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .ppt format into their document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.7.5/unstructured/partition/pptx.py` & `unstructured-0.7.6/unstructured/partition/pptx.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ElementMetadata,
     ListItem,
     NarrativeText,
     PageBreak,
     Table,
     Text,
     Title,
+    process_metadata,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import (
     convert_ms_office_table_to_text,
     exactly_one,
     spooled_to_bytes_io_if_needed,
 )
@@ -23,20 +24,22 @@
     is_possible_narrative_text,
     is_possible_title,
 )
 
 OPENXML_SCHEMA_NAME = "{http://schemas.openxmlformats.org/drawingml/2006/main}"
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.PPTX)
 def partition_pptx(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = True,
     metadata_filename: Optional[str] = None,
+    **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .pptx format into its document elements.
 
     Parameters
     ----------
      filename
         A string defining the target filename path.
@@ -80,15 +83,16 @@
                         page_number=metadata.page_number,
                     )
                     elements.append(Table(text=text_table, metadata=metadata))
                 continue
             if not shape.has_text_frame:
                 continue
             # NOTE(robinson) - avoid processing shapes that are not on the actual slide
-            if shape.top < 0 or shape.left < 0:
+            # NOTE - skip check if no top or left position (shape displayed top left)
+            if (shape.top and shape.left) and (shape.top < 0 or shape.left < 0):
                 continue
             for paragraph in shape.text_frame.paragraphs:
                 text = paragraph.text
                 if text.strip() == "":
                     continue
                 if _is_bulleted_paragraph(paragraph):
                     elements.append(ListItem(text=text, metadata=metadata))
@@ -103,15 +107,15 @@
             elements.append(PageBreak())
 
     return elements
 
 
 def _order_shapes(shapes):
     """Orders the shapes from top to bottom and left to right."""
-    return sorted(shapes, key=lambda x: (x.top, x.left))
+    return sorted(shapes, key=lambda x: (x.top or 0, x.left or 0))
 
 
 def _is_bulleted_paragraph(paragraph) -> bool:
     """Determines if the paragraph is bulleted by looking for a bullet character prefix. Bullet
     characters in the openxml schema are represented by buChar"""
     paragraph_xml = paragraph._p.get_or_add_pPr()
     buChar = paragraph_xml.find(f"{OPENXML_SCHEMA_NAME}buChar")
```

### Comparing `unstructured-0.7.5/unstructured/partition/rst.py` & `unstructured-0.7.6/unstructured/partition/rtf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
-@add_metadata_with_filetype(FileType.RST)
-def partition_rst(
+@process_metadata()
+@add_metadata_with_filetype(FileType.RTF)
+def partition_rtf(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     include_page_breaks: bool = False,
+    **kwargs,
 ) -> List[Element]:
-    """Partitions an RST document. The document is first converted to HTML and then
-    partitioned using partition_html.
+    """Partitions an RTF document. The document is first converted to HTML and then
+    partitioned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it
     """
     return convert_and_partition_html(
-        source_format="rst",
+        source_format="rtf",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
     )
```

### Comparing `unstructured-0.7.5/unstructured/partition/rtf.py` & `unstructured-0.7.6/unstructured/partition/epub.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
-@add_metadata_with_filetype(FileType.RTF)
-def partition_rtf(
+@process_metadata()
+@add_metadata_with_filetype(FileType.EPUB)
+def partition_epub(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     include_page_breaks: bool = False,
+    **kwargs,
 ) -> List[Element]:
-    """Partitions an RTF document. The document is first converted to HTML and then
-    partitioned using partiton_html.
+    """Partitions an EPUB document. The document is first converted to HTML and then
+    partitoned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it
     """
     return convert_and_partition_html(
-        source_format="rtf",
+        source_format="epub",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
     )
```

### Comparing `unstructured-0.7.5/unstructured/partition/strategies.py` & `unstructured-0.7.6/unstructured/partition/strategies.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 ):
     """Determines what strategy to use for processing PDFs or images, accounting for fallback
     logic if some dependencies are not available."""
     pytesseract_installed = dependency_exists("pytesseract")
     unstructured_inference_installed = dependency_exists("unstructured_inference")
 
     if is_image:
+        # Note(yuming): There is no fast strategy for images,
+        # use ocr_only as a fallback plan for consistency with PDFs.
+        # This can be removed once unstructured-api use auto as the default strategy.
+        if strategy == "fast":
+            strategy = "ocr_only"
         validate_strategy(strategy, "image")
         pdf_text_extractable = False
     else:
         validate_strategy(strategy, "pdf")
         pdf_text_extractable = is_pdf_text_extractable(filename=filename, file=file)
 
     if strategy == "auto":
```

### Comparing `unstructured-0.7.5/unstructured/partition/text.py` & `unstructured-0.7.6/unstructured/partition/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Address,
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     Text,
     Title,
+    process_metadata,
 )
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition.common import exactly_one
 from unstructured.partition.text_type import (
     is_bulleted_text,
@@ -23,23 +24,25 @@
 )
 
 
 def split_by_paragraph(content: str) -> List[str]:
     return re.split(PARAGRAPH_PATTERN, content)
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.TXT)
 def partition_text(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
     encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
+    **kwargs,
 ) -> List[Element]:
     """Partitions an .txt documents into its constituent elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
```

### Comparing `unstructured-0.7.5/unstructured/partition/text_type.py` & `unstructured-0.7.6/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/partition/xlsx.py` & `unstructured-0.7.6/unstructured/partition/xlsx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, List, Optional, Union, cast
 
 import lxml.html
 import pandas as pd
 
-from unstructured.documents.elements import Element, ElementMetadata, Table
+from unstructured.documents.elements import (
+    Element,
+    ElementMetadata,
+    Table,
+    process_metadata,
+)
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.XLSX)
 def partition_xlsx(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
+    **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Excel Documents in .xlsx format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.7.5/unstructured/partition/xml.py` & `unstructured-0.7.6/unstructured/partition/xml.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import xml.etree.ElementTree as ET
 from tempfile import SpooledTemporaryFile
-from typing import IO, BinaryIO, Optional, Union, cast
+from typing import IO, BinaryIO, List, Optional, Union, cast
 
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 from unstructured.partition.text import partition_text
 
 
 def is_leaf(elem):
@@ -34,24 +35,26 @@
         for subelem in elem.iter():
             if is_leaf(subelem):
                 leaf_elements.append(subelem.text)
 
     return "\n".join(leaf_elements)  # type: ignore
 
 
+@process_metadata()
 @add_metadata_with_filetype(FileType.XML)
 def partition_xml(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     xml_keep_tags: bool = False,
     xml_path: str = ".",
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
     encoding: Optional[str] = None,
-):
+    **kwargs,
+) -> List[Element]:
     """Partitions an XML document into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
```

### Comparing `unstructured-0.7.5/unstructured/staging/argilla.py` & `unstructured-0.7.6/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/base.py` & `unstructured-0.7.6/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/baseplate.py` & `unstructured-0.7.6/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/datasaur.py` & `unstructured-0.7.6/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/huggingface.py` & `unstructured-0.7.6/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/label_box.py` & `unstructured-0.7.6/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/label_studio.py` & `unstructured-0.7.6/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/prodigy.py` & `unstructured-0.7.6/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/staging/weaviate.py` & `unstructured-0.7.6/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured/utils.py` & `unstructured-0.7.6/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.5/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.6/unstructured.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.5
+Version: 0.7.6
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -25,15 +25,15 @@
           [![Downloads](https://static.pepy.tech/badge/unstructured/month)](https://pepy.tech/project/unstructured)
         
         </div>
         
         <div>
           <p align="center">
           <a
-          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1nlh1ot5d-dfY7zCRlhFboZrIWLA4Qgw">
+          href="https://join.slack.com/t/unstructuredw-kbe4326/shared_invite/zt-1x7cgo0pg-PTptXWylzPQF9xZolzCnwQ">
             <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" />
           </a>
           <a href="https://www.linkedin.com/company/unstructuredio/">
             <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
           </a>
         </div>
         
@@ -106,16 +106,19 @@
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
+        | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
+        | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks |
+        | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
         
         
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.5 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.6 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -69,16 +69,19 @@
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
 Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
-Include Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes |
-None | | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Include Page Breaks | | TSV Files (`.tsv`) | `partition_tsv` | N/A | Yes | None
+| | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | | Word
+Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | Word Documents
+(`.doc`) | `partition_doc` | N/A | Yes | Include Page Breaks | | Word Documents
+(`.docx`) | `partition_docx` | N/A | Yes | Include Page Breaks | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.5/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.6/unstructured.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 unstructured/partition/ppt.py
 unstructured/partition/pptx.py
 unstructured/partition/rst.py
 unstructured/partition/rtf.py
 unstructured/partition/strategies.py
 unstructured/partition/text.py
 unstructured/partition/text_type.py
+unstructured/partition/tsv.py
 unstructured/partition/xlsx.py
 unstructured/partition/xml.py
 unstructured/staging/__init__.py
 unstructured/staging/argilla.py
 unstructured/staging/base.py
 unstructured/staging/baseplate.py
 unstructured/staging/datasaur.py
```

