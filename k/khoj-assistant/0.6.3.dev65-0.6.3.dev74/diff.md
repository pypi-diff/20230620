# Comparing `tmp/khoj_assistant-0.6.3.dev65.tar.gz` & `tmp/khoj_assistant-0.6.3.dev74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jun 18 09:26:03 2023, max compression
+gzip compressed data, last modified: Tue Jun 20 01:11:35 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev65.tar` & `khoj_assistant-0.6.3.dev74.tar`

### file list

```diff
@@ -1,67 +1,71 @@
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/__init__.py
--rw-r--r--   0        0        0    10848 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17706 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9707 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    12550 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4526 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    11901 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3027 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4008 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/LICENSE
--rw-r--r--   0        0        0    22877 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/README.md
--rw-r--r--   0        0        0     2785 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/pyproject.toml
--rw-r--r--   0        0        0    25217 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10848 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17819 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     1363 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      647 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/base_data_integration.html
+-rw-r--r--   0        0        0      657 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0     9527 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     2151 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     3671 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     5756 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    12370 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     2872 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0   275822 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0   205167 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13196 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     3866 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3070 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4158 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/LICENSE
+-rw-r--r--   0        0        0    22877 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/README.md
+-rw-r--r--   0        0        0     2785 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/pyproject.toml
+-rw-r--r--   0        0        0    25217 2023-06-20 01:11:35.000000 khoj_assistant-0.6.3.dev74/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev74/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/main.py` & `khoj_assistant-0.6.3.dev74/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self.new_config = self.current_config
 
         # Initialize Configure Window
         self.setWindowTitle("Khoj")
         self.setFixedWidth(600)
 
         # Set Window Icon
-        icon_path = constants.web_directory / "assets/icons/favicon-144x144.png"
+        icon_path = constants.web_directory / "assets/icons/favicon-128x128.png"
         self.setWindowIcon(QtGui.QIcon(f"{icon_path.absolute()}"))
 
         # Initialize Configure Window Layout
         self.wlayout = QtWidgets.QVBoxLayout()
 
         # Add Settings Panels for each Search Type to Configure Window Layout
         self.search_settings_panels = []
@@ -224,14 +224,16 @@
                 if isinstance(child, SearchCheckBox):
                     # Search Type Disabled
                     if not child.isChecked() and child.search_type in self.new_config["content-type"]:
                         del self.new_config["content-type"][child.search_type]
                     # Search Type (re)-Enabled
                     if child.isChecked():
                         current_search_config = self.current_config["content-type"].get(child.search_type, {})
+                        if current_search_config == None:
+                            current_search_config = {}
                         default_search_config = self.get_default_config(search_type=child.search_type)
                         self.new_config["content-type"][child.search_type.value] = merge_dicts(
                             current_search_config, default_search_config
                         )
                 elif isinstance(child, FileBrowser) and child.search_type in self.new_config["content-type"]:
                     if child.search_type.value == SearchType.Image:
                         self.new_config["content-type"][child.search_type.value]["input-directories"] = (
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/desktop/system_tray.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """Create System Tray with Menu.  Menu contain options to
     1. Open Search Page on the Web Interface
     2. Open App Configuration Screen
     3. Quit Application
     """
 
     # Create the system tray with icon
-    icon_path = constants.web_directory / "assets/icons/favicon-144x144.png"
+    icon_path = constants.web_directory / "assets/icons/favicon-128x128.png"
     icon = QtGui.QIcon(f"{icon_path.absolute()}")
     tray = QtWidgets.QSystemTrayIcon(icon)
     tray.setVisible(True)
 
     # Create the menu and menu actions
     menu = QtWidgets.QMenu()
     menu_actions = [
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/web/chat.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 <html>
     <head>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0 maximum-scale=1.0">
         <title>Khoj</title>
 
-        <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 144 144%22><text y=%22.86em%22 font-size=%22144%22>🦅</text></svg>">
-        <link rel="icon" type="image/png" sizes="144x144" href="/static/assets/icons/favicon-144x144.png">
+        <link rel="icon" type="image/png" sizes="128x128" href="/static/assets/icons/favicon-128x128.png">
         <link rel="manifest" href="/static/khoj_chat.webmanifest">
     </head>
     <script>
         function formatDate(date) {
             // Format date in HH:MM, DD MMM YYYY format
             let time_string = date.toLocaleTimeString('en-IN', { hour: '2-digit', minute: '2-digit', hour12: false });
             let date_string = date.toLocaleString('en-IN', { year: 'numeric', month: 'short', day: '2-digit'}).replaceAll('-', ' ');
```

#### html2text {}

```diff
@@ -1,5 +1,4 @@
 
 
-
 ****** Khoj ******
 [                    ]
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 <html>
     <head>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0 maximum-scale=1.0">
         <title>Khoj</title>
 
-        <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 144 144%22><text y=%22.86em%22 font-size=%22144%22>🦅</text></svg>">
-        <link rel="icon" type="image/png" sizes="144x144" href="/static/assets/icons/favicon-144x144.png">
+        <link rel="icon" type="image/png" sizes="128x128" href="/static/assets/icons/favicon-128x128.png">
         <link rel="manifest" href="/static/khoj.webmanifest">
     </head>
     <script type="text/javascript" src="static/assets/org.min.js"></script>
     <script type="text/javascript" src="static/assets/markdown-it.min.js"></script>
 
     <script>
         function render_image(item) {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,6 +1,5 @@
 
 
-
 ****** Khoj ******
  [                    ]
   Update  [Unknown INPUT type]
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev74/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev74/src/khoj/routers/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,24 @@
 
 # Internal Packages
 from khoj.configure import configure_processor, configure_search
 from khoj.processor.conversation.gpt import converse, extract_questions
 from khoj.processor.conversation.utils import message_to_log, message_to_prompt
 from khoj.search_type import image_search, text_search
 from khoj.utils.helpers import log_telemetry, timer
-from khoj.utils.rawconfig import FullConfig, SearchResponse
+from khoj.utils.rawconfig import (
+    FullConfig,
+    SearchResponse,
+    TextContentConfig,
+    ConversationProcessorConfig,
+    GithubContentConfig,
+)
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
+from khoj.utils.yaml import save_config_to_file_updated_state
 
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
 
 
 # Create Routes
@@ -61,14 +68,44 @@
     state.config = updated_config
     with open(state.config_file, "w") as outfile:
         yaml.dump(yaml.safe_load(state.config.json(by_alias=True)), outfile)
         outfile.close()
     return state.config
 
 
+@api.post("/config/data/content_type/github", status_code=200)
+async def set_content_config_github_data(updated_config: GithubContentConfig):
+    state.config.content_type.github = updated_config
+    try:
+        save_config_to_file_updated_state()
+        return {"status": "ok"}
+    except Exception as e:
+        return {"status": "error", "message": str(e)}
+
+
+@api.post("/config/data/content_type/{content_type}", status_code=200)
+async def set_content_config_data(content_type: str, updated_config: TextContentConfig):
+    state.config.content_type[content_type] = updated_config
+    try:
+        save_config_to_file_updated_state()
+        return {"status": "ok"}
+    except Exception as e:
+        return {"status": "error", "message": str(e)}
+
+
+@api.post("/config/data/processor/conversation", status_code=200)
+async def set_processor_conversation_config_data(updated_config: ConversationProcessorConfig):
+    state.config.processor.conversation = updated_config
+    try:
+        save_config_to_file_updated_state()
+        return {"status": "ok"}
+    except Exception as e:
+        return {"status": "error", "message": str(e)}
+
+
 @api.get("/search", response_model=List[SearchResponse])
 def search(
     q: str,
     n: Optional[int] = 5,
     t: Optional[SearchType] = None,
     r: Optional[bool] = False,
     score_threshold: Optional[Union[float, None]] = None,
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev74/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev74/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev74/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev74/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev74/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev74/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 default_config = {
     "content-type": {
         "org": {
             "input-files": None,
             "input-filter": None,
             "compressed-jsonl": "~/.khoj/content/org/org.jsonl.gz",
             "embeddings-file": "~/.khoj/content/org/org_embeddings.pt",
-            "index_heading_entries": False,
+            "index-heading-entries": False,
         },
         "markdown": {
             "input-files": None,
             "input-filter": None,
             "compressed-jsonl": "~/.khoj/content/markdown/markdown.jsonl.gz",
             "embeddings-file": "~/.khoj/content/markdown/markdown_embeddings.pt",
         },
@@ -70,10 +70,11 @@
         "image": {"encoder": "sentence-transformers/clip-ViT-B-32", "model_directory": "~/.khoj/search/image/"},
     },
     "processor": {
         "conversation": {
             "openai-api-key": None,
             "model": "text-davinci-003",
             "conversation-logfile": "~/.khoj/processor/conversation/conversation_logs.json",
+            "chat-model": "gpt-3.5-turbo",
         }
     },
 }
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/rawconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 
 class ConfigBase(BaseModel):
     class Config:
         alias_generator = to_snake_case_from_dash
         allow_population_by_field_name = True
 
+    def __getitem__(self, item):
+        return getattr(self, item)
+
+    def __setitem__(self, key, value):
+        return setattr(self, key, value)
+
 
 class TextConfigBase(ConfigBase):
     compressed_jsonl: Path
     embeddings_file: Path
 
 
 class TextContentConfig(TextConfigBase):
```

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev74/src/khoj/utils/yaml.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,28 @@
 from pathlib import Path
 
 # External Packages
 import yaml
 
 # Internal Packages
 from khoj.utils.rawconfig import FullConfig
+from khoj.utils import state
 
 
 # Do not emit tags when dumping to YAML
 yaml.emitter.Emitter.process_tag = lambda self, *args, **kwargs: None  # type: ignore[assignment]
 
 
+def save_config_to_file_updated_state():
+    with open(state.config_file, "w") as outfile:
+        yaml.dump(yaml.safe_load(state.config.json(by_alias=True)), outfile)
+        outfile.close()
+    return state.config
+
+
 def save_config_to_file(yaml_config: dict, yaml_config_file: Path):
     "Write config to YML file"
     # Create output directory, if it doesn't exist
     yaml_config_file.parent.mkdir(parents=True, exist_ok=True)
 
     with open(yaml_config_file, "w", encoding="utf-8") as config_file:
         yaml.safe_dump(yaml_config, config_file, allow_unicode=True)
```

### Comparing `khoj_assistant-0.6.3.dev65/.gitignore` & `khoj_assistant-0.6.3.dev74/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/LICENSE` & `khoj_assistant-0.6.3.dev74/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/README.md` & `khoj_assistant-0.6.3.dev74/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/pyproject.toml` & `khoj_assistant-0.6.3.dev74/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev65/PKG-INFO` & `khoj_assistant-0.6.3.dev74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev65
+Version: 0.6.3.dev74
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

