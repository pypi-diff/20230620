# Comparing `tmp/openicl-0.1.7.tar.gz` & `tmp/openicl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openicl-0.1.7.tar", last modified: Thu Jun  1 10:30:56 2023, max compression
+gzip compressed data, was "openicl-0.1.8.tar", last modified: Tue Jun 20 08:54:59 2023, max compression
```

## Comparing `openicl-0.1.7.tar` & `openicl-0.1.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.939597 openicl-0.1.7/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11357 2023-03-03 05:33:05.000000 openicl-0.1.7/LICENSE
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4375 2023-06-01 10:30:56.939597 openicl-0.1.7/PKG-INFO
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3746 2023-06-01 10:18:08.000000 openicl-0.1.7/README.md
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      182 2023-03-06 07:33:42.000000 openicl-0.1.7/openicl/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11390 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_dataset_reader.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/icl_evaluator/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      276 2023-03-01 07:54:05.000000 openicl-0.1.7/openicl/icl_evaluator/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      855 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_acc_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      486 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_api_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      207 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_base_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      456 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_bleu_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      454 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_rouge_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      712 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_squad_evaluator.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/icl_inferencer/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      240 2023-04-11 06:15:47.000000 openicl-0.1.7/openicl/icl_inferencer/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    13690 2023-06-01 10:29:50.000000 openicl-0.1.7/openicl/icl_inferencer/icl_base_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     5410 2023-04-11 06:15:47.000000 openicl-0.1.7/openicl/icl_inferencer/icl_channel_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7887 2023-03-28 09:22:25.000000 openicl-0.1.7/openicl/icl_inferencer/icl_cot_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7691 2023-03-28 09:20:03.000000 openicl-0.1.7/openicl/icl_inferencer/icl_gen_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     9631 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_inferencer/icl_ppl_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8639 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_prompt_template.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/icl_retriever/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      370 2023-03-09 05:12:30.000000 openicl-0.1.7/openicl/icl_retriever/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8148 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_retriever/icl_base_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3504 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_bm25_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6538 2023-03-13 05:42:49.000000 openicl-0.1.7/openicl/icl_retriever/icl_dpp_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7594 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_retriever/icl_mdl_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2774 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_random_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6165 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_topk_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     5279 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_votek_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2024 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_zero_retriever.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.939597 openicl-0.1.7/openicl/utils/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       23 2023-03-06 10:38:54.000000 openicl-0.1.7/openicl/utils/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3523 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/api_service.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      218 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/calculate.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1150 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/check_type.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1931 2023-03-01 07:54:05.000000 openicl-0.1.7/openicl/utils/collators.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2224 2023-03-16 06:06:21.000000 openicl-0.1.7/openicl/utils/icl_common_utils.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1108 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/logging.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl.egg-info/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4375 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/PKG-INFO
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1407 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        1 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      222 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/requires.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        8 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/top_level.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       38 2023-06-01 10:30:56.939597 openicl-0.1.7/setup.cfg
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1737 2023-06-01 10:15:55.000000 openicl-0.1.7/setup.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-20 08:54:59.358788 openicl-0.1.8/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11357 2023-03-03 05:33:05.000000 openicl-0.1.8/LICENSE
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4439 2023-06-20 08:54:59.358788 openicl-0.1.8/PKG-INFO
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3810 2023-06-20 08:48:15.000000 openicl-0.1.8/README.md
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-20 08:54:59.348788 openicl-0.1.8/openicl/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      182 2023-03-06 07:33:42.000000 openicl-0.1.8/openicl/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11390 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_dataset_reader.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-20 08:54:59.348788 openicl-0.1.8/openicl/icl_evaluator/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      276 2023-03-01 07:54:05.000000 openicl-0.1.8/openicl/icl_evaluator/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      855 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_evaluator/icl_acc_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      486 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_evaluator/icl_api_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      207 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_evaluator/icl_base_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      456 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_evaluator/icl_bleu_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      454 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_evaluator/icl_rouge_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      712 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_evaluator/icl_squad_evaluator.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-20 08:54:59.358788 openicl-0.1.8/openicl/icl_inferencer/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      240 2023-04-11 06:15:47.000000 openicl-0.1.8/openicl/icl_inferencer/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    13816 2023-06-20 08:39:17.000000 openicl-0.1.8/openicl/icl_inferencer/icl_base_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     5410 2023-04-11 06:15:47.000000 openicl-0.1.8/openicl/icl_inferencer/icl_channel_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7887 2023-03-28 09:22:25.000000 openicl-0.1.8/openicl/icl_inferencer/icl_cot_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7691 2023-03-28 09:20:03.000000 openicl-0.1.8/openicl/icl_inferencer/icl_gen_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     9631 2023-03-28 05:42:46.000000 openicl-0.1.8/openicl/icl_inferencer/icl_ppl_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8639 2023-03-28 05:42:46.000000 openicl-0.1.8/openicl/icl_prompt_template.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-20 08:54:59.358788 openicl-0.1.8/openicl/icl_retriever/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      370 2023-03-09 05:12:30.000000 openicl-0.1.8/openicl/icl_retriever/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8148 2023-03-28 05:42:46.000000 openicl-0.1.8/openicl/icl_retriever/icl_base_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3504 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_retriever/icl_bm25_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6538 2023-03-13 05:42:49.000000 openicl-0.1.8/openicl/icl_retriever/icl_dpp_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7594 2023-03-28 05:42:46.000000 openicl-0.1.8/openicl/icl_retriever/icl_mdl_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2774 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_retriever/icl_random_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6165 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_retriever/icl_topk_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     5279 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_retriever/icl_votek_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2024 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/icl_retriever/icl_zero_retriever.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-20 08:54:59.358788 openicl-0.1.8/openicl/utils/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       23 2023-03-06 10:38:54.000000 openicl-0.1.8/openicl/utils/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3523 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/utils/api_service.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      218 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/utils/calculate.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1150 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/utils/check_type.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1931 2023-03-01 07:54:05.000000 openicl-0.1.8/openicl/utils/collators.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2224 2023-03-16 06:06:21.000000 openicl-0.1.8/openicl/utils/icl_common_utils.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1108 2023-03-13 09:11:56.000000 openicl-0.1.8/openicl/utils/logging.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-20 08:54:59.348788 openicl-0.1.8/openicl.egg-info/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4439 2023-06-20 08:54:59.000000 openicl-0.1.8/openicl.egg-info/PKG-INFO
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1407 2023-06-20 08:54:59.000000 openicl-0.1.8/openicl.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        1 2023-06-20 08:54:59.000000 openicl-0.1.8/openicl.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      249 2023-06-20 08:54:59.000000 openicl-0.1.8/openicl.egg-info/requires.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        8 2023-06-20 08:54:59.000000 openicl-0.1.8/openicl.egg-info/top_level.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       38 2023-06-20 08:54:59.358788 openicl-0.1.8/setup.cfg
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1764 2023-06-20 08:54:19.000000 openicl-0.1.8/setup.py
```

### Comparing `openicl-0.1.7/LICENSE` & `openicl-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/PKG-INFO` & `openicl-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openicl
-Version: 0.1.7
+Version: 0.1.8
 Summary: An open source framework for in-context learning.
 Home-page: https://github.com/Shark-NLP/OpenICL
 Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye
 Keywords: AI,NLP,in-context learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,23 +26,26 @@
   <a href="#installation">Installation</a> •
   <a href="https://arxiv.org/abs/2303.02913">Paper</a> •
   <a href="https://github.com/Shark-NLP/OpenICL/tree/main/examples">Examples</a> •
   <a href="https://openicl.readthedocs.io/en/latest/index.html">Docs</a> •
   <a href="#citation">Citation</a> 
 </p>
 
-![version](https://img.shields.io/badge/version-0.1.7-blue)
+![version](https://img.shields.io/badge/version-0.1.8-blue)
 
 
 ## Overview
 OpenICL provides an easy interface for in-context learning, with many state-of-the-art retrieval and inference methods built in to facilitate systematic comparison of LMs and fast research prototyping. Users can easily incorporate different retrieval and inference methods, as well as different prompt instructions into their workflow. 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg"  border="0" />
 </div>
 
+## What's News
++ **v0.1.8** Support LLaMA and self-consistency
+
 ## Installation
 Note: OpenICL requires Python 3.8+
 
 **Using Pip**
 ```
 pip install openicl
 ```
```

#### html2text {}

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1 Name: openicl Version: 0.1.7 Summary: An open source
+Metadata-Version: 2.1 Name: openicl Version: 0.1.8 Summary: An open source
 framework for in-context learning. Home-page: https://github.com/Shark-NLP/
 OpenICL Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye Keywords:
 AI,NLP,in-context learning Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Requires-Python: >=3.8.0 Description-Content-Type: text/
 markdown License-File: LICENSE
                  [https://s1.ax1x.com/2023/03/07/ppZfEmq.png]
 ------
     Overview â¢ Installation â¢ Paper â¢ Examples â¢ Docs â¢ Citation
-![version](https://img.shields.io/badge/version-0.1.7-blue) ## Overview OpenICL
+![version](https://img.shields.io/badge/version-0.1.8-blue) ## Overview OpenICL
 provides an easy interface for in-context learning, with many state-of-the-art
 retrieval and inference methods built in to facilitate systematic comparison of
 LMs and fast research prototyping. Users can easily incorporate different
 retrieval and inference methods, as well as different prompt instructions into
 their workflow.
                  [https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg]
-## Installation Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip
-install openicl ``` **Installation for local development:** ``` git clone
-https://github.com/Shark-NLP/OpenICL cd OpenICL pip install -e . ``` ## Quick
-Start Following example shows you how to perform ICL on sentiment
-classification dataset. More examples and tutorials can be found at [examples]
-(https://github.com/Shark-NLP/OpenICL/tree/main/examples) #### Step 1: Load and
-prepare data ```python from datasets import load_dataset from openicl import
-DatasetReader # Loading dataset from huggingface dataset = load_dataset
-('gpt3mix/sst2') # Define a DatasetReader, with specified column names where
-input and output are stored. data = DatasetReader(dataset, input_columns=
-['text'], output_column='label') ``` #### Step 2: Define the prompt template
-(Optional) ```python from openicl import PromptTemplate tp_dict = { 0:
-"Positive Movie Review: ", 1: "Negative Movie Review: " } template =
-PromptTemplate(tp_dict, {'text': ''}, ice_token='') ``` The placeholder `` and
-`` will be replaced by in-context examples and testing input, respectively. For
-more detailed information about `PromptTemplate` (such as string-type template)
-, please see [tutorial1](https://github.com/Shark-NLP/OpenICL/blob/main/
-examples/tutorials/openicl_tutorial1_getting_started.ipynb). #### Step 3:
-Initialize the Retriever ```python from openicl import TopkRetriever # Define a
-retriever using the previous `DataLoader`. # `ice_num` stands for the number of
-data in in-context examples. retriever = TopkRetriever(data, ice_num=8) ```
-Here we use the popular TopK method to build the retriever. #### Step 4:
-Initialize the Inferencer ```python from openicl import PPLInferencer
-inferencer = PPLInferencer(model_name='distilgpt2') ``` #### Step 5: Inference
-and scoring ```python from openicl import AccEvaluator # the inferencer
-requires retriever to collect in-context examples, as well as a template to
-wrap up these examples. predictions = inferencer.inference(retriever,
-ice_template=template) # compute accuracy for the prediction score =
-AccEvaluator().score(predictions=predictions, references=data.references) print
-(score) ``` ## Docs **(updating...)** [OpenICL Documentation](https://
+## What's News + **v0.1.8** Support LLaMA and self-consistency ## Installation
+Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip install openicl ```
+**Installation for local development:** ``` git clone https://github.com/Shark-
+NLP/OpenICL cd OpenICL pip install -e . ``` ## Quick Start Following example
+shows you how to perform ICL on sentiment classification dataset. More examples
+and tutorials can be found at [examples](https://github.com/Shark-NLP/OpenICL/
+tree/main/examples) #### Step 1: Load and prepare data ```python from datasets
+import load_dataset from openicl import DatasetReader # Loading dataset from
+huggingface dataset = load_dataset('gpt3mix/sst2') # Define a DatasetReader,
+with specified column names where input and output are stored. data =
+DatasetReader(dataset, input_columns=['text'], output_column='label') ``` ####
+Step 2: Define the prompt template (Optional) ```python from openicl import
+PromptTemplate tp_dict = { 0: "Positive Movie Review: ", 1: "Negative Movie
+Review: " } template = PromptTemplate(tp_dict, {'text': ''}, ice_token='') ```
+The placeholder `` and `` will be replaced by in-context examples and testing
+input, respectively. For more detailed information about `PromptTemplate` (such
+as string-type template) , please see [tutorial1](https://github.com/Shark-NLP/
+OpenICL/blob/main/examples/tutorials/openicl_tutorial1_getting_started.ipynb).
+#### Step 3: Initialize the Retriever ```python from openicl import
+TopkRetriever # Define a retriever using the previous `DataLoader`. # `ice_num`
+stands for the number of data in in-context examples. retriever = TopkRetriever
+(data, ice_num=8) ``` Here we use the popular TopK method to build the
+retriever. #### Step 4: Initialize the Inferencer ```python from openicl import
+PPLInferencer inferencer = PPLInferencer(model_name='distilgpt2') ``` #### Step
+5: Inference and scoring ```python from openicl import AccEvaluator # the
+inferencer requires retriever to collect in-context examples, as well as a
+template to wrap up these examples. predictions = inferencer.inference
+(retriever, ice_template=template) # compute accuracy for the prediction score
+= AccEvaluator().score(predictions=predictions, references=data.references)
+print(score) ``` ## Docs **(updating...)** [OpenICL Documentation](https://
 openicl.readthedocs.io/en/latest/index.html) ## Citation If you find this
 repository helpful, feel free to cite our paper: ```bibtex @article
 {wu2023openicl, title={OpenICL: An Open-Source Framework for In-context
 Learning}, author={Zhenyu Wu, Yaoxiang Wang, Jiacheng Ye, Jiangtao Feng,
 Jingjing Xu, Yu Qiao, Zhiyong Wu}, journal={arXiv preprint arXiv:2303.02913},
 year={2023} } ```
```

### Comparing `openicl-0.1.7/README.md` & `openicl-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,26 @@
   <a href="#installation">Installation</a> •
   <a href="https://arxiv.org/abs/2303.02913">Paper</a> •
   <a href="https://github.com/Shark-NLP/OpenICL/tree/main/examples">Examples</a> •
   <a href="https://openicl.readthedocs.io/en/latest/index.html">Docs</a> •
   <a href="#citation">Citation</a> 
 </p>
 
-![version](https://img.shields.io/badge/version-0.1.7-blue)
+![version](https://img.shields.io/badge/version-0.1.8-blue)
 
 
 ## Overview
 OpenICL provides an easy interface for in-context learning, with many state-of-the-art retrieval and inference methods built in to facilitate systematic comparison of LMs and fast research prototyping. Users can easily incorporate different retrieval and inference methods, as well as different prompt instructions into their workflow. 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg"  border="0" />
 </div>
 
+## What's News
++ **v0.1.8** Support LLaMA and self-consistency
+
 ## Installation
 Note: OpenICL requires Python 3.8+
 
 **Using Pip**
 ```
 pip install openicl
 ```
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
                  [https://s1.ax1x.com/2023/03/07/ppZfEmq.png]
 ------
     Overview â¢ Installation â¢ Paper â¢ Examples â¢ Docs â¢ Citation
-![version](https://img.shields.io/badge/version-0.1.7-blue) ## Overview OpenICL
+![version](https://img.shields.io/badge/version-0.1.8-blue) ## Overview OpenICL
 provides an easy interface for in-context learning, with many state-of-the-art
 retrieval and inference methods built in to facilitate systematic comparison of
 LMs and fast research prototyping. Users can easily incorporate different
 retrieval and inference methods, as well as different prompt instructions into
 their workflow.
                  [https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg]
-## Installation Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip
-install openicl ``` **Installation for local development:** ``` git clone
-https://github.com/Shark-NLP/OpenICL cd OpenICL pip install -e . ``` ## Quick
-Start Following example shows you how to perform ICL on sentiment
-classification dataset. More examples and tutorials can be found at [examples]
-(https://github.com/Shark-NLP/OpenICL/tree/main/examples) #### Step 1: Load and
-prepare data ```python from datasets import load_dataset from openicl import
-DatasetReader # Loading dataset from huggingface dataset = load_dataset
-('gpt3mix/sst2') # Define a DatasetReader, with specified column names where
-input and output are stored. data = DatasetReader(dataset, input_columns=
-['text'], output_column='label') ``` #### Step 2: Define the prompt template
-(Optional) ```python from openicl import PromptTemplate tp_dict = { 0:
-"Positive Movie Review: ", 1: "Negative Movie Review: " } template =
-PromptTemplate(tp_dict, {'text': ''}, ice_token='') ``` The placeholder `` and
-`` will be replaced by in-context examples and testing input, respectively. For
-more detailed information about `PromptTemplate` (such as string-type template)
-, please see [tutorial1](https://github.com/Shark-NLP/OpenICL/blob/main/
-examples/tutorials/openicl_tutorial1_getting_started.ipynb). #### Step 3:
-Initialize the Retriever ```python from openicl import TopkRetriever # Define a
-retriever using the previous `DataLoader`. # `ice_num` stands for the number of
-data in in-context examples. retriever = TopkRetriever(data, ice_num=8) ```
-Here we use the popular TopK method to build the retriever. #### Step 4:
-Initialize the Inferencer ```python from openicl import PPLInferencer
-inferencer = PPLInferencer(model_name='distilgpt2') ``` #### Step 5: Inference
-and scoring ```python from openicl import AccEvaluator # the inferencer
-requires retriever to collect in-context examples, as well as a template to
-wrap up these examples. predictions = inferencer.inference(retriever,
-ice_template=template) # compute accuracy for the prediction score =
-AccEvaluator().score(predictions=predictions, references=data.references) print
-(score) ``` ## Docs **(updating...)** [OpenICL Documentation](https://
+## What's News + **v0.1.8** Support LLaMA and self-consistency ## Installation
+Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip install openicl ```
+**Installation for local development:** ``` git clone https://github.com/Shark-
+NLP/OpenICL cd OpenICL pip install -e . ``` ## Quick Start Following example
+shows you how to perform ICL on sentiment classification dataset. More examples
+and tutorials can be found at [examples](https://github.com/Shark-NLP/OpenICL/
+tree/main/examples) #### Step 1: Load and prepare data ```python from datasets
+import load_dataset from openicl import DatasetReader # Loading dataset from
+huggingface dataset = load_dataset('gpt3mix/sst2') # Define a DatasetReader,
+with specified column names where input and output are stored. data =
+DatasetReader(dataset, input_columns=['text'], output_column='label') ``` ####
+Step 2: Define the prompt template (Optional) ```python from openicl import
+PromptTemplate tp_dict = { 0: "Positive Movie Review: ", 1: "Negative Movie
+Review: " } template = PromptTemplate(tp_dict, {'text': ''}, ice_token='') ```
+The placeholder `` and `` will be replaced by in-context examples and testing
+input, respectively. For more detailed information about `PromptTemplate` (such
+as string-type template) , please see [tutorial1](https://github.com/Shark-NLP/
+OpenICL/blob/main/examples/tutorials/openicl_tutorial1_getting_started.ipynb).
+#### Step 3: Initialize the Retriever ```python from openicl import
+TopkRetriever # Define a retriever using the previous `DataLoader`. # `ice_num`
+stands for the number of data in in-context examples. retriever = TopkRetriever
+(data, ice_num=8) ``` Here we use the popular TopK method to build the
+retriever. #### Step 4: Initialize the Inferencer ```python from openicl import
+PPLInferencer inferencer = PPLInferencer(model_name='distilgpt2') ``` #### Step
+5: Inference and scoring ```python from openicl import AccEvaluator # the
+inferencer requires retriever to collect in-context examples, as well as a
+template to wrap up these examples. predictions = inferencer.inference
+(retriever, ice_template=template) # compute accuracy for the prediction score
+= AccEvaluator().score(predictions=predictions, references=data.references)
+print(score) ``` ## Docs **(updating...)** [OpenICL Documentation](https://
 openicl.readthedocs.io/en/latest/index.html) ## Citation If you find this
 repository helpful, feel free to cite our paper: ```bibtex @article
 {wu2023openicl, title={OpenICL: An Open-Source Framework for In-context
 Learning}, author={Zhenyu Wu, Yaoxiang Wang, Jiacheng Ye, Jiangtao Feng,
 Jingjing Xu, Yu Qiao, Zhiyong Wu}, journal={arXiv preprint arXiv:2303.02913},
 year={2023} } ```
```

### Comparing `openicl-0.1.7/openicl/icl_dataset_reader.py` & `openicl-0.1.8/openicl/icl_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_evaluator/icl_acc_evaluator.py` & `openicl-0.1.8/openicl/icl_evaluator/icl_acc_evaluator.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_evaluator/icl_squad_evaluator.py` & `openicl-0.1.8/openicl/icl_evaluator/icl_squad_evaluator.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_inferencer/icl_base_inferencer.py` & `openicl-0.1.8/openicl/icl_inferencer/icl_base_inferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         else:
             if self.api_name == 'opt-175b':
                 self.__init_tokenizer(self.tokenizer_name)
         
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
         if self.model is not None:
             self.model.to(self.device)
+        self.model.eval()  
         self.max_model_token_num = max_model_token_num
         self.batch_size = batch_size
         self.output_json_filepath = output_json_filepath
         self.output_json_filename = output_json_filename
         if not os.path.exists(self.output_json_filepath):
             os.makedirs(self.output_json_filepath)
 
@@ -95,14 +96,15 @@
             :obj:`List:` A list of string, each representing the results of one inference.
         """
         raise NotImplementedError("Method hasn't been implemented yet")
 
     def __init_model(self, model_name, model_config, model_parallel, device_map, no_split_module_classes):
         if not isinstance(model_name, str):
             self.model = model_name
+            self.model_name = ''  # set model name to null since we pass the loaded model already
             return
         if not model_parallel:
             if model_config is not None:
                 self.model = self.__get_hf_model_from_config(model_name, model_config)
             else:
                 self.model = self.__get_hf_model_from_name(model_name)
         else:
```

### Comparing `openicl-0.1.7/openicl/icl_inferencer/icl_channel_inferencer.py` & `openicl-0.1.8/openicl/icl_inferencer/icl_channel_inferencer.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_inferencer/icl_cot_inferencer.py` & `openicl-0.1.8/openicl/icl_inferencer/icl_cot_inferencer.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_inferencer/icl_gen_inferencer.py` & `openicl-0.1.8/openicl/icl_inferencer/icl_gen_inferencer.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_inferencer/icl_ppl_inferencer.py` & `openicl-0.1.8/openicl/icl_inferencer/icl_ppl_inferencer.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_prompt_template.py` & `openicl-0.1.8/openicl/icl_prompt_template.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_base_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_base_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_bm25_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_dpp_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_dpp_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_mdl_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_mdl_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_random_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_random_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_topk_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_topk_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_votek_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_votek_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/icl_retriever/icl_zero_retriever.py` & `openicl-0.1.8/openicl/icl_retriever/icl_zero_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/utils/api_service.py` & `openicl-0.1.8/openicl/utils/api_service.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/utils/check_type.py` & `openicl-0.1.8/openicl/utils/check_type.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/utils/collators.py` & `openicl-0.1.8/openicl/utils/collators.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/utils/icl_common_utils.py` & `openicl-0.1.8/openicl/utils/icl_common_utils.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl/utils/logging.py` & `openicl-0.1.8/openicl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/openicl.egg-info/PKG-INFO` & `openicl-0.1.8/openicl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openicl
-Version: 0.1.7
+Version: 0.1.8
 Summary: An open source framework for in-context learning.
 Home-page: https://github.com/Shark-NLP/OpenICL
 Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye
 Keywords: AI,NLP,in-context learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,23 +26,26 @@
   <a href="#installation">Installation</a> •
   <a href="https://arxiv.org/abs/2303.02913">Paper</a> •
   <a href="https://github.com/Shark-NLP/OpenICL/tree/main/examples">Examples</a> •
   <a href="https://openicl.readthedocs.io/en/latest/index.html">Docs</a> •
   <a href="#citation">Citation</a> 
 </p>
 
-![version](https://img.shields.io/badge/version-0.1.7-blue)
+![version](https://img.shields.io/badge/version-0.1.8-blue)
 
 
 ## Overview
 OpenICL provides an easy interface for in-context learning, with many state-of-the-art retrieval and inference methods built in to facilitate systematic comparison of LMs and fast research prototyping. Users can easily incorporate different retrieval and inference methods, as well as different prompt instructions into their workflow. 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg"  border="0" />
 </div>
 
+## What's News
++ **v0.1.8** Support LLaMA and self-consistency
+
 ## Installation
 Note: OpenICL requires Python 3.8+
 
 **Using Pip**
 ```
 pip install openicl
 ```
```

#### html2text {}

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1 Name: openicl Version: 0.1.7 Summary: An open source
+Metadata-Version: 2.1 Name: openicl Version: 0.1.8 Summary: An open source
 framework for in-context learning. Home-page: https://github.com/Shark-NLP/
 OpenICL Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye Keywords:
 AI,NLP,in-context learning Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Requires-Python: >=3.8.0 Description-Content-Type: text/
 markdown License-File: LICENSE
                  [https://s1.ax1x.com/2023/03/07/ppZfEmq.png]
 ------
     Overview â¢ Installation â¢ Paper â¢ Examples â¢ Docs â¢ Citation
-![version](https://img.shields.io/badge/version-0.1.7-blue) ## Overview OpenICL
+![version](https://img.shields.io/badge/version-0.1.8-blue) ## Overview OpenICL
 provides an easy interface for in-context learning, with many state-of-the-art
 retrieval and inference methods built in to facilitate systematic comparison of
 LMs and fast research prototyping. Users can easily incorporate different
 retrieval and inference methods, as well as different prompt instructions into
 their workflow.
                  [https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg]
-## Installation Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip
-install openicl ``` **Installation for local development:** ``` git clone
-https://github.com/Shark-NLP/OpenICL cd OpenICL pip install -e . ``` ## Quick
-Start Following example shows you how to perform ICL on sentiment
-classification dataset. More examples and tutorials can be found at [examples]
-(https://github.com/Shark-NLP/OpenICL/tree/main/examples) #### Step 1: Load and
-prepare data ```python from datasets import load_dataset from openicl import
-DatasetReader # Loading dataset from huggingface dataset = load_dataset
-('gpt3mix/sst2') # Define a DatasetReader, with specified column names where
-input and output are stored. data = DatasetReader(dataset, input_columns=
-['text'], output_column='label') ``` #### Step 2: Define the prompt template
-(Optional) ```python from openicl import PromptTemplate tp_dict = { 0:
-"Positive Movie Review: ", 1: "Negative Movie Review: " } template =
-PromptTemplate(tp_dict, {'text': ''}, ice_token='') ``` The placeholder `` and
-`` will be replaced by in-context examples and testing input, respectively. For
-more detailed information about `PromptTemplate` (such as string-type template)
-, please see [tutorial1](https://github.com/Shark-NLP/OpenICL/blob/main/
-examples/tutorials/openicl_tutorial1_getting_started.ipynb). #### Step 3:
-Initialize the Retriever ```python from openicl import TopkRetriever # Define a
-retriever using the previous `DataLoader`. # `ice_num` stands for the number of
-data in in-context examples. retriever = TopkRetriever(data, ice_num=8) ```
-Here we use the popular TopK method to build the retriever. #### Step 4:
-Initialize the Inferencer ```python from openicl import PPLInferencer
-inferencer = PPLInferencer(model_name='distilgpt2') ``` #### Step 5: Inference
-and scoring ```python from openicl import AccEvaluator # the inferencer
-requires retriever to collect in-context examples, as well as a template to
-wrap up these examples. predictions = inferencer.inference(retriever,
-ice_template=template) # compute accuracy for the prediction score =
-AccEvaluator().score(predictions=predictions, references=data.references) print
-(score) ``` ## Docs **(updating...)** [OpenICL Documentation](https://
+## What's News + **v0.1.8** Support LLaMA and self-consistency ## Installation
+Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip install openicl ```
+**Installation for local development:** ``` git clone https://github.com/Shark-
+NLP/OpenICL cd OpenICL pip install -e . ``` ## Quick Start Following example
+shows you how to perform ICL on sentiment classification dataset. More examples
+and tutorials can be found at [examples](https://github.com/Shark-NLP/OpenICL/
+tree/main/examples) #### Step 1: Load and prepare data ```python from datasets
+import load_dataset from openicl import DatasetReader # Loading dataset from
+huggingface dataset = load_dataset('gpt3mix/sst2') # Define a DatasetReader,
+with specified column names where input and output are stored. data =
+DatasetReader(dataset, input_columns=['text'], output_column='label') ``` ####
+Step 2: Define the prompt template (Optional) ```python from openicl import
+PromptTemplate tp_dict = { 0: "Positive Movie Review: ", 1: "Negative Movie
+Review: " } template = PromptTemplate(tp_dict, {'text': ''}, ice_token='') ```
+The placeholder `` and `` will be replaced by in-context examples and testing
+input, respectively. For more detailed information about `PromptTemplate` (such
+as string-type template) , please see [tutorial1](https://github.com/Shark-NLP/
+OpenICL/blob/main/examples/tutorials/openicl_tutorial1_getting_started.ipynb).
+#### Step 3: Initialize the Retriever ```python from openicl import
+TopkRetriever # Define a retriever using the previous `DataLoader`. # `ice_num`
+stands for the number of data in in-context examples. retriever = TopkRetriever
+(data, ice_num=8) ``` Here we use the popular TopK method to build the
+retriever. #### Step 4: Initialize the Inferencer ```python from openicl import
+PPLInferencer inferencer = PPLInferencer(model_name='distilgpt2') ``` #### Step
+5: Inference and scoring ```python from openicl import AccEvaluator # the
+inferencer requires retriever to collect in-context examples, as well as a
+template to wrap up these examples. predictions = inferencer.inference
+(retriever, ice_template=template) # compute accuracy for the prediction score
+= AccEvaluator().score(predictions=predictions, references=data.references)
+print(score) ``` ## Docs **(updating...)** [OpenICL Documentation](https://
 openicl.readthedocs.io/en/latest/index.html) ## Citation If you find this
 repository helpful, feel free to cite our paper: ```bibtex @article
 {wu2023openicl, title={OpenICL: An Open-Source Framework for In-context
 Learning}, author={Zhenyu Wu, Yaoxiang Wang, Jiacheng Ye, Jiangtao Feng,
 Jingjing Xu, Yu Qiao, Zhiyong Wu}, journal={arXiv preprint arXiv:2303.02913},
 year={2023} } ```
```

### Comparing `openicl-0.1.7/openicl.egg-info/SOURCES.txt` & `openicl-0.1.8/openicl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openicl-0.1.7/setup.py` & `openicl-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     def run(self):
         self.do_egg_install()
         import nltk
         nltk.download('punkt')
 
 
 REQUIRES = """
-transformers
+transformers==4.28.1
+tokenizers==0.13.3
 accelerate
 datasets>=2.7.1
 evaluate>=0.3.0
 faiss_gpu>=1.7.2
 nltk>=3.8
 numpy>=1.23.4
 openai>=0.27.1
@@ -35,15 +36,15 @@
 with open("README.md") as f:
     readme = f.read()
 
 
 def do_setup():
     setup(
         name="openicl",
-        version='0.1.7',
+        version='0.1.8',
         description="An open source framework for in-context learning.",
         url="https://github.com/Shark-NLP/OpenICL",
         author='Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye',
         long_description=readme,
         long_description_content_type="text/markdown",
         cmdclass={'download_nltk': DownloadNLTK},
         install_requires=get_install_requires(),
```

