# Comparing `tmp/alphawave-0.2.5.tar.gz` & `tmp/alphawave-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.5.tar", last modified: Sun Jun 18 19:21:17 2023, max compression
+gzip compressed data, was "alphawave-0.2.6.tar", last modified: Tue Jun 20 03:28:42 2023, max compression
```

## Comparing `alphawave-0.2.5.tar` & `alphawave-0.2.6.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.5/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9472 2023-06-18 19:21:17.265798 alphawave-0.2.5/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.5/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      925 2023-06-18 19:21:09.000000 alphawave-0.2.5/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-18 19:21:17.265798 alphawave-0.2.5/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.261798 alphawave-0.2.5/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9228 2023-06-17 19:16:02.000000 alphawave-0.2.5/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.5/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.5/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5978 2023-06-17 19:12:44.000000 alphawave-0.2.5/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.5/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9094 2023-06-18 19:09:29.000000 alphawave-0.2.5/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8570 2023-06-18 03:50:01.000000 alphawave-0.2.5/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.5/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.5/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.5/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.5/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.5/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.5/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.5/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.5/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9472 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1585 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      125 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16065 2023-06-18 16:59:38.000000 alphawave-0.2.5/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.5/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2643 2023-06-18 02:59:07.000000 alphawave-0.2.5/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.5/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.5/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.5/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.5/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.5/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.5/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3547 2023-06-16 16:10:31.000000 alphawave-0.2.5/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.5/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.5/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.5/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.5/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3741 2023-06-18 18:11:10.000000 alphawave-0.2.5/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2515 2023-06-18 03:44:14.000000 alphawave-0.2.5/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    19050 2023-06-17 23:10:50.000000 alphawave-0.2.5/src/alphawave_pyexts/conversation.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13351 2023-06-18 03:42:44.000000 alphawave-0.2.5/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1032 2023-06-18 00:09:12.000000 alphawave-0.2.5/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1402 2023-06-16 20:15:32.000000 alphawave-0.2.5/src/alphawave_pyexts/searchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6615 2023-06-18 17:44:47.000000 alphawave-0.2.5/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.5/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.5/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.5/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.571413 alphawave-0.2.6/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.6/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9458 2023-06-20 03:28:42.571413 alphawave-0.2.6/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.6/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      911 2023-06-20 03:26:31.000000 alphawave-0.2.6/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-20 03:28:42.571413 alphawave-0.2.6/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9149 2023-06-19 22:47:22.000000 alphawave-0.2.6/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.6/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.6/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-19 15:45:37.000000 alphawave-0.2.6/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.2.6/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.2.6/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8916 2023-06-19 16:39:38.000000 alphawave-0.2.6/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.6/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.6/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.6/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.6/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.6/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.6/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.6/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.6/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9458 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1614 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      125 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16612 2023-06-19 22:45:42.000000 alphawave-0.2.6/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.6/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.2.6/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.6/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.6/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.6/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.6/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.6/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.6/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3546 2023-06-19 15:47:21.000000 alphawave-0.2.6/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.6/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.6/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.6/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.2.6/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4433 2023-06-19 22:44:06.000000 alphawave-0.2.6/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.2.6/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10457 2023-06-18 23:46:33.000000 alphawave-0.2.6/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    19050 2023-06-17 23:10:50.000000 alphawave-0.2.6/src/alphawave_pyexts/conversation.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.2.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.2.6/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1402 2023-06-16 20:15:32.000000 alphawave-0.2.6/src/alphawave_pyexts/searchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6689 2023-06-19 03:02:57.000000 alphawave-0.2.6/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.6/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.6/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.6/tests/testSchema.py
```

### Comparing `alphawave-0.2.5/LICENSE` & `alphawave-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/PKG-INFO` & `alphawave-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.5
+Version: 0.2.6
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
-Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
+Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `alphawave-0.2.5/README.md` & `alphawave-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/pyproject.toml` & `alphawave-0.2.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
 
@@ -35,9 +35,9 @@
     "openai",
     "nltk",
     'importlib-metadata; python_version<"3.9"',
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/Stevenic/alphawave-py"
+"Homepage" = "https://tuuyi.io/alphawave"
 "Bug Tracker" = "https://github.com/Stevenic/alphawave-py/issues"
```

### Comparing `alphawave-0.2.5/src/alphawave/AlphaWave.py` & `alphawave-0.2.6/src/alphawave/AlphaWave.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 class AlphaWave(AsyncIOEventEmitter):
     def __init__(self, **kwargs):
         super().__init__()
         self.options = AlphaWaveOptions(
         )
         update_dataclass(self.options, **kwargs)
-
+        #display_dataclass(self.options)
     async def completePrompt(self, input=None):
-        client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'log_repairs'))
+        client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, logRepairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'logRepairs'))
 
         if self.options.input_variable:
             if input:
                 memory.set(input_variable, input)
             else:
                 input = memory.get(input_variable) if memory.has(input_variable) else ''
         elif not input:
@@ -125,29 +125,27 @@
         except Exception as err:
             return {
                 'status': 'error',
                 'message': str(err)
             }
 
     def addInputToHistory(self, memory, variable, input):
-        #print(f'***** Alphawave addInputToHistory {variable}')
         if variable and input is not None and len(input) > 0:
             history = memory.get(variable) or []
             history.append({'role': 'user', 'content': input})
             if len(history) > self.options.max_history_messages:
-                history = history[self.options.max_history_messages:]
+                history = history[int(self.options.max_history_messages/2):]
             memory.set(variable, history)
 
     def addResponseToHistory(self, memory, variable, message):
-        #print(f'***** Alphawave addResponseToHistory {variable}')
         if variable:
             history = memory.get(variable) or []
             history.append(message)
             if len(history) > self.options.max_history_messages:
-                history = history[self.options.max_history_messages:]
+                history = history[int(self.options.max_history_messages/2):]
             memory.set(variable, history)
 
     async def repairResponse(self, fork, functions, tokenizer, response, validation, remaining_attempts):
         client, prompt, prompt_options, memory, functions, history_variable, input_variable, max_history_messages, max_repair_attempts, tokenizer, validator, log_repairs = get_values(self.options, ('client', 'prompt', 'prompt_options', 'memory', 'functions', 'history_variable', 'input_variable', 'max_history_messages', 'max_repair_attempts', 'tokenizer', 'validator', 'log_repairs'))
 
         # Are we out of attempts?
         feedback = validation.get('feedback', 'The response was invalid. Try another strategy.')
```

### Comparing `alphawave-0.2.5/src/alphawave/Colorize.py` & `alphawave-0.2.6/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.6/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.6/src/alphawave/JSONResponseValidator.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,56 +74,61 @@
         parsed=[]
         try:
             parsed = Response.parse_all_objects(text)
         except Exception as e:
             raise e
         if len(parsed) == 0:
             template = extract_json_template(self.schema)
+            #print(f'***** JSONResponseValidator failure len(parsed) == 0')
             return {
                 'type': 'Validation',
                 'valid': False,
-                'feedback': self.missing_json_feedback#+f' using this template: {template}'
+                'feedback': self.missing_json_feedback+f' using this template: {template} '
             }
 
         # Validate the response against the schema
         if self.schema:
             errors = None
             for i in range(len(parsed) - 1, -1, -1):
                 obj = parsed[i]
                 try:
                     try:
                         obj = self.parse_dict(obj) if type(obj) == str else obj
                     except Exception as e:
                         pass
                     validate(obj, self.schema)
+                    #print(f'***** JSONResponseValidator validation passed!')
                     return {
                         'type': 'Validation',
                         'valid': True,
                         'value': obj
                     }
                 except ValidationError as e:
                     path = str(list(e.relative_schema_path)[1:-1]).replace('[','').replace(']',"").replace(', ', ':')
                     if not errors:
                         errors = e
                     template = extract_json_template(self.schema)
+                    #print(f'***** JSONResponseValidator ValidationError exception {str(e)}')
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(errors)}'#. respond using this template: {template}'
+                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(errors)}. respond using this template: {template} '
                     }
                 except Exception as e:
                     template = extract_json_template(self.schema)
+                    #print(f'***** JSONResponseValidator validator generic exception {str(e)}')
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(e)}'#spond using this template: {template}'
+                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(e)}. respond using this template: {template} '
                     }      
     
         else:
             # Return the last object
+            #print(f'***** JSONResponseValidator exit last object {parsed[-1]}')
             return {
                 'type': 'Validation',
                 'valid': True,
                 'value': parsed[-1]
             }
 
     def get_error_fix(self, error: ValidationError) -> str:
```

### Comparing `alphawave-0.2.5/src/alphawave/OSClient.py` & `alphawave-0.2.6/src/alphawave/OSClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,16 +84,14 @@
         startTime = time.time()
         max_input_tokens = 1500
         if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
             max_input_tokens = options.max_input_tokens
         
         if hasattr(options, 'completion_type') and options.completion_type == 'text':
             result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
-        if hasattr(options, 'completion_type') and options.completion_type == 'text':
-            result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated text completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
             if self.options.logRequests:
                 print(Colorize.title('PROMPT:'))
                 for msg in result.output:
                     if not isinstance(msg, dict):
                         msg = msg.__dict__
@@ -155,25 +153,25 @@
         url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/completions"
         return self.post(url, request)
 
     def createChatCompletion(self, request: CreateChatCompletionRequest) -> requests.Response:
         url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/chat/completions"
         return self.post(url, request)
 
-    def post(self, url: str, body: object) -> requests.Response:
+    def post(self, url: str, request: object) -> requests.Response:
         requestHeaders = {
             'Content-Type': 'application/json',
             'User-Agent': self.UserAgent
         }
         result = ''
         try:
-            result = ut.ask_LLM(self.options.model,
-                                body.messages,
-                                self.options.max_tokens,
-                                self.options.temperature,
-                                self.options.top_p,
+            result = ut.ask_LLM(request.model,
+                                request.messages,
+                                request.max_tokens,
+                                request.temperature,
+                                request.top_p,
                                 self.options.endpoint,
                                 self.options.port
                                 )
         except Exception as e:
             return PromptResponse(status='error',message=str(e))
         return PromptResponse(status='success', message=result)
```

### Comparing `alphawave-0.2.5/src/alphawave/OpenAIClient.py` & `alphawave-0.2.6/src/alphawave/OpenAIClient.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,14 +112,19 @@
                 completion = response.json().get('choices')[0]
                 return {'status': 'success', 'message': completion.get('message', {'role': 'assistant', 'content': ''})}
             elif response.status_code == 429:
                 if self.options['logRequests']:
                     print(Colorize.title('HEADERS:'))
                     print(Colorize.output(response.headers))
                 return {'status': 'rate_limited', 'message': 'The chat completion API returned a rate limit error.'}
+            elif response.status_code == 503:
+                if self.options['logRequests']:
+                    print(Colorize.title('HEADERS:'))
+                    print(Colorize.output(response.headers))
+                return {'status': 'server unavailable', 'message': 'The chat completion API returned server unavailable or overloaded.'}
             else:
                 return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status_code}: {response.reason}"}
 
     def addRequestHeaders(self, headers: Dict[str, str], options: OpenAIClientOptions):
         headers['Authorization'] = f"Bearer {options['apiKey']}"
         if options['organization']:
             headers['OpenAI-Organization'] = options['organization']
```

### Comparing `alphawave-0.2.5/src/alphawave/RepairTestClient.py` & `alphawave-0.2.6/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/Response.py` & `alphawave-0.2.6/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/TestClient.py` & `alphawave-0.2.6/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/TestClientTest.py` & `alphawave-0.2.6/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.6/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/internalTypes.py` & `alphawave-0.2.6/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave/jsonParser.py` & `alphawave-0.2.6/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.6/src/alphawave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.5
+Version: 0.2.6
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
-Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
+Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `alphawave-0.2.5/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.6/src/alphawave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/alphawave_agents/SchemaBasedCommand.py
 src/alphawave_agents/SentimentAnalysis.py
 src/alphawave_agents/SetPropertyCommand.py
 src/alphawave_agents/__init__.py
 src/alphawave_agents/agentTypes.py
 src/alphawave_pyexts/LLMClient.py
 src/alphawave_pyexts/SearchCommand.py
+src/alphawave_pyexts/chat.py
 src/alphawave_pyexts/conversation.py
 src/alphawave_pyexts/searchCommand.py
 src/alphawave_pyexts/utilityV2.py
 src/alphawave_pyexts/llmsearch/google_search_concurrent.py
 src/alphawave_pyexts/llmsearch/search_service.py
 tests/testOSClient.py
 tests/testOpenAiClient.py
```

### Comparing `alphawave-0.2.5/src/alphawave_agents/Agent.py` & `alphawave-0.2.6/src/alphawave_agents/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,24 @@
 PromptInstructionSection = TemplateSection("\n".join([
     "Return a JSON object with your thoughts and the next command to perform",
     "Only respond with the JSON format below and based your plan on the commands above",
     "Response Format:",
     '{"thoughts":{"thought":"<your current thought>","reasoning":"<self reflect on why you made this decision>","plan":"- short bulleted\n- list that conveys\n- long-term plan"},"command":{"name":"<command name>","input":{"<name>":"<value>"}}}'
 ]), 'system')
 
+PromptInstructionSection_py = TemplateSection(\
+"""
+Reason step by step how to answer the users query below.
+Return a JSON object with your thoughts and the next command to perform, using the following format and available commands.
+Response Format:
+
+{\"reasoning\":\"<reflections on how to construct an answerto the user query>\",\"plan\":\"concise plan for constructing answer\",\"command\":{\"name\":\"<command name of next action to perform>\",\"input\":{\"<key>\":\"<value>\"}}</s>"
+"""
+                                              , 'system')
+
 @dataclass
 class AgentOptions:
     client: PromptCompletionClient
     context_variable: Optional[str] = None
     prompt: Union[str, list[str], PromptSection] = None
     prompt_options: PromptCompletionOptions = None
     agent_variable: Optional[str] = None
@@ -267,23 +277,22 @@
             if 'context' in state:
                 self.memory.set(self.options['context_variable'], state['context'])
 
             # Create prompt
             history_variable = self.get_agent_history_variable(agent_id)
             sections = [agent_prompt]
             sections.append(AgentCommandSection(self._commands))
-            sections.append(PromptInstructionSection)
+            pis = PromptInstructionSection
+            if not (self._options['prompt_options']['model']).lower().startswith('gpt'):
+                pis = PromptInstructionSection_py
+            sections.append(pis)
             prompt = Prompt([
                 GroupSection(sections, 'system'),
                 ConversationHistory(history_variable, 1.0, True)
             ])
-            #prompt = Prompt([
-            #    agent_prompt, AgentCommandSection(self._commands), PromptInstructionSection,
-            #    ConversationHistory(history_variable, 1.0, True)
-            #])
             if input:
                 prompt.sections.append(TextSection(input, 'user', -1, True, '\n', 'user'))
                 # Ensure input variable is set otherwise the history will be wrong.
                 self.memory.set(self.options['input_variable'], input)
 
 
             if execute_initial_thought and self._options['initial_thought']:
@@ -298,15 +307,15 @@
                 if state['totalSteps'] == 0 and self._options['initial_thought']:
                     history = self.memory.get(history_variable) or []
                     message = {'role': 'assistant', 'content': json.dumps(self._options['initial_thought'])}
                     history.append(message)
                     self.memory.set(history_variable, history)
 
                 # Create command validator
-                validator = AgentCommandValidator(self._commands)
+                validator = AgentCommandValidator(self._commands, self._options['prompt_options']['model'])
 
                 # Create a wave for the prompt
                 wave = AlphaWave(
                     client = self._options['client'],
                     prompt = prompt,
                     prompt_options = self._options['prompt_options'],
                     functions = self._options['functions'],
```

### Comparing `alphawave-0.2.5/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.6/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.6/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from pyee import AsyncIOEventEmitter
 from typing import Dict, Any, Union
-from alphawave_agents.agentTypes import Command, AgentThought, AgentThoughtSchema
+from alphawave_agents.agentTypes import Command, AgentThought, AgentThoughtSchema, AgentThoughtSchema_py
 from alphawave.JSONResponseValidator import JSONResponseValidator
 import traceback
 
 class AgentCommandValidator:
-    def __init__(self, commands: dict[str, Command]):
-        self._thought_validator = JSONResponseValidator(AgentThoughtSchema, 'No valid JSON objects were found in the response. Return a valid JSON object with your thoughts and the next command to perform.')
+    def __init__(self, commands: dict[str, Command], model: str):
+        if model.lower().startswith('gpt'):
+            self._thought_validator = JSONResponseValidator(AgentThoughtSchema, 'No valid JSON objects were found in the response. Return a valid JSON object with your thoughts and the next command to perform.')
+        else:
+            self._thought_validator = JSONResponseValidator(AgentThoughtSchema_py, 'No valid JSON objects were found in the response. Return a valid JSON object with your thoughts and the next command to perform.')
+
         self._commands = commands
 
     async def validate_response(self, memory, functions, tokenizer, response, remaining_attempts) -> Union[AgentThought, None]:
         # Validate that the response contains a thought
         try:
           validation_result = self._thought_validator.validate_response(memory, functions, tokenizer, response, remaining_attempts)
           if not validation_result['valid']:
```

### Comparing `alphawave-0.2.5/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.6/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.6/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.6/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.6/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.6/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.6/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.6/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyee import AsyncIOEventEmitter
 from jsonschema import validate, ValidationError
 from typing import Any, Dict, Optional, Union
-#import json
+import json
 from promptrix.promptrixTypes import PromptMemory, PromptFunctions, Tokenizer
 from dataclasses import dataclass, asdict
 import traceback
 
 @dataclass
 class CommandSchema:
     def __init__(self, type: str, title: str='', description: str='', returns: Optional[str] = None):
```

### Comparing `alphawave-0.2.5/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.6/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.6/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.6/src/alphawave_agents/agentTypes.py`

 * *Files 22% similar despite different names*

```diff
@@ -50,7 +50,24 @@
                 "input": {"type": "object"}
             },
             "required": ["name"]
         }
     },
     "required": ["thoughts", "command"]
 }
+
+AgentThoughtSchema_py: Dict[str,str] = {
+    "type": "object",
+    "properties": {
+        "reasoning": {"type": "string"},
+        "plan": {"type": "string"},
+        "command": {
+            "type": "object",
+            "properties": {
+                "name": {"type": "string"},
+                "input": {"type": "object"}
+                },
+            "required": ["name"]
+        }
+    },
+    "required": ["reasoning", "plan", "command"]
+}
```

### Comparing `alphawave-0.2.5/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.2.6/src/alphawave_pyexts/LLMClient.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,19 +5,43 @@
 import requests
 from alphawave_pyexts.conversation import Conversation, SeparatorStyle
 import alphawave_pyexts.conversation as cv
 import tkinter as tk
 import time
 
 MODEL_NAME = None; WORKER_ADDR=None; CONTROLLER_ADDRESS = "http://localhost:21001"
+USER_PREFIX = ''
+ASSISTANT_PREFIX = ''
 
 host='192.168.1.195'
 port = 5004
 cv.register_conv_template(Conversation(
-        name="wizard",
+        name="falcon_instruct",
+        system="",
+        roles=("HUMAN", "ASSISTANT"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_TWO,
+        sep=" ",
+        sep2="</s>",
+    )
+)
+cv.register_conv_template(Conversation(
+        name="falcon_instruct2",
+        system="",
+        roles=(" ###HUMAN", " ###ASSISTANT"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_TWO,
+        sep=" ",
+        sep2="</s>",
+    )
+)
+cv.register_conv_template(Conversation(
+        name="falcon_instruct3",
         system="",
         roles=("HUMAN", "ASSISTANT"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep=" ",
         sep2="</s>",
@@ -32,15 +56,18 @@
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep=" ",
         sep2="</s>",
     )
 )
 
 def run_query(model, messages, temp, top_p, max_tokens, host = host, port = port, tkroot = None, tkdisplay=None): 
+    global USER_PREFIX, ASSISTANT_PREFIX
     conv=cv.get_conv_template(model)
+    USER_PREFIX = conv.roles[0]
+    ASSISTANT_PREFIX = conv.roles[1]
     # set this so client can check for run-on, although this test should pbly be here!
     for msg in messages:
         #print(f'  {msg}')
         role = msg['role']
         if role.lower() == 'user':
             role_index = 0
         else:
```

### Comparing `alphawave-0.2.5/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.2.6/src/alphawave_pyexts/SearchCommand.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List
 from colorama import Fore, Style
 from dataclasses import dataclass, asdict
 import copy
 from promptrix.SystemMessage import SystemMessage
+from promptrix.VolatileMemory import VolatileMemory
 from alphawave_agents.agentTypes import TaskResponse
 from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand
 from alphawave_agents.SchemaBasedCommand import CommandSchema as sbcCommandSchema
 from alphawave_pyexts.llmsearch import search_service
 import json
 
 @dataclass
@@ -31,37 +32,38 @@
     },
     required=['query'],
     returns='search result'
 )
 
 
 class SearchCommand(SchemaBasedCommand):
-    def __init__(self, client, model, title=None, name=None, description=None, return_urls=False, max_chars=500):
+    def __init__(self, client, model, title=None, name=None, description=None, return_urls=False, logResponse=False, max_chars=1500):
         super().__init__(search_schema, title, description)
         self.client = client
         self.model = model
         self.return_urls = return_urls
         self.max_chars = max_chars
-
+        self.logResponse = logResponse
+        
     async def execute(self, input: input, memory: Any, functions: Any, tokenizer: Any) -> Any:
         try:
             if type(input) == dict and 'query' in input:
                 query = input['query']
-                response =await search_service.run_chat(self.client, query, self.model, memory, functions, tokenizer)
+                memory = VolatileMemory()  # don't let anything bleed back to surrounding task
+                response =await search_service.run_chat(self.client, query, self.model, memory, functions, tokenizer, self.max_chars)
                 sc_text = ''
                 sc_urls = []
                 if type(response) is list:
                     for item in response:
                         if type(item) == dict and 'url' in item:
                             sc_urls.append(item['url'])
                         if type(item) == dict and 'text' in item:
-                            sc_text = '\n'+(item['text'])
+                            sc_text += '\n'+(item['text'])
                     sc_text = sc_text[:max(len(sc_text)-1, self.max_chars)]
                 if self.return_urls:
                     return {'status':'success', 'message':{'text': sc_text, 'urls':sc_urls}}
                 else:
                     return {'status':'success', 'message':sc_text}
                     
         except Exception as err:
             message = str(err)
-            print(f'***** SearchCommand error {str(err)}')
             return asdict(TaskResponse('TaskResponse', 'error', message))
```

### Comparing `alphawave-0.2.5/src/alphawave_pyexts/conversation.py` & `alphawave-0.2.6/src/alphawave_pyexts/conversation.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.2.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 system_prime = {"role": "system", "content":"You analyze Text with respect to Query and list any relevant information found, including direct quotes from the text, and detailed samples or examples in the text."}
 priming_1 = {"role": "user", "content":"Query:\n"}
 priming_2 = {"role": "user", "content":"List relevant information in the provided text, including direct quotes from the text. If none, respond 'no information'.\nText:\n"}
 
 
 # Define a function to make a single URL request and process the response
-async def process_url(query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer):
+async def process_url(query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer, max_chars):
     start_time = time.time()
     site = ut.extract_site(url)
     result = ''
     try:
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
             options = Options()
@@ -61,47 +61,47 @@
             with webdriver.Chrome(options=options) as dr:
                 #print(f'*****setting page load timeout {timeout}')
                 dr.set_page_load_timeout(timeout)
                 try:
                     dr.get(url)
                     response = dr.page_source
                     result =  await response_text_extract(query_phrase, keywords, keyword_weights, url, response, int(time.time()-start_time),
-                                                          client, model, memory, functions, tokenizer)
+                                                          client, model, memory, functions, tokenizer, max_chars)
                 except selenium.common.exceptions.TimeoutException:
                     return '', url
     except Exception:
         traceback.print_exc()
         print(f"{site} err")
         pass
     #print(f"Processed {site}: {len(response)} / {len(result)} {int((time.time()-start_time)*1000)} ms")
     return result, url
 
-async def process_urls(query_phrase, keywords, keyword_weights, urls, search_level, client, model, memory, functions, tokenizer):
+async def process_urls(query_phrase, keywords, keyword_weights, urls, search_level, client, model, memory, functions, tokenizer, max_chars):
     response = []
     start_time = time.time()
     full_text = ''
     in_process = []
     
     # Create a ThreadPoolExecutor with 5 worker threads
     with concurrent.futures.ThreadPoolExecutor(max_workers=4) as executor:
         # initialize scan of google urls
         while True:
             try:
                 while (len(urls) > 0
                        # no sense starting if not much time left
-                       and ((search_level==DEEP_SEARCH and len(full_text) < 9600 and len(in_process) < 8 and time.time() - start_time < 14)
-                            or (search_level==NORMAL_SEARCH and len(full_text) < 6400 and len(in_process) < 7 and time.time()-start_time < 12)
-                            or (search_level==QUICK_SEARCH  and len(full_text) < 4800 and len(in_process) < 6 and time.time()-start_time < 8))):
+                       and ((search_level==DEEP_SEARCH and len(full_text) < 9600 and len(in_process) < 8 and time.time() - start_time < 42)
+                            or (search_level==NORMAL_SEARCH and len(full_text) < 6400 and len(in_process) < 7 and time.time()-start_time < 36)
+                            or (search_level==QUICK_SEARCH  and len(full_text) < 4800 and len(in_process) < 6 and time.time()-start_time < 24))):
                     url = urls[0]
                     urls = urls[1:]
                     # set timeout so we don't wait for a slow site forever
                     timeout = 12-int(time.time()-start_time)
                     if search_level==NORMAL_SEARCH:
                         timeout = timeout+4
-                    future = executor.submit(process_url, query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer)
+                    future = executor.submit(process_url, query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer, max_chars)
                     in_process.append(future)
                 # Process the responses as they arrive
                 for future in in_process:
                     if future.done():
                         in_process.remove(future)
                         try:
                             result, url = await asyncio.wait_for(future.result(), timeout=(max (1, (12-(time.time()-start_time)))))
@@ -113,19 +113,19 @@
                         if len(result) > 0:
                             site = ut.extract_site(url)
                             domain = ut.extract_domain(url)
                             response.append({'source':ut.extract_domain(url), 'url':url, 'text':result})
 
                 # openai seems to timeout a plugin  at about 30 secs, and there is pbly 3-4 sec overhead
                 if ((len(urls) == 0 and len(in_process) == 0)
-                    or (search_level==DEEP_SEARCH and (len(full_text) > 9600) or time.time() - start_time > 42)
+                    or (search_level==DEEP_SEARCH and (len(full_text) > max_chars) or time.time() - start_time > 48)
                     or (search_level==NORMAL_SEARCH and
-                        (len(full_text) > 2400) or time.time()-start_time > 32)
+                        (len(full_text) > max_chars) or time.time()-start_time > 32)
                     or (search_level==QUICK_SEARCH  and
-                        (len(full_text) > 2400) or time.time()-start_time > 28)
+                        (len(full_text) > max_chars) or time.time()-start_time > 24)
                     ):
                     executor.shutdown(wait=False)
                     return response
                 time.sleep(.5)
             except:
                 traceback.print_exc()
         executor.shutdown(wait=False)
@@ -159,15 +159,19 @@
     return final_text
 
 
 def search(query_phrase):
     sort = '&sort=date-sdate:d:w'
     if 'today' in query_phrase or 'latest' in query_phrase:
         sort = '&sort=date-sdate:d:s'
-    google_query=en.quote(query_phrase)
+    try:
+        google_query=en.quote(query_phrase)
+    except:
+        print(f'googleSearch pblm w query_phrase, ignoring {query_phrase}')
+        return []
     response=[]
     try:
         start_wall_time = time.time()
         url="https://www.googleapis.com/customsearch/v1?key="+ut.google_key+'&cx='+ut.google_cx+'&num=10'+sort+'&q='+google_query
         response = requests.get(url)
         response_json = json.loads(response.text)
     except:
@@ -185,17 +189,17 @@
         urls.append(url)
     return urls
 
 def log_url_process(site, reason, raw_text, extract_text, gpt_text):
     return
 
 
-async def llm_tldr (text, query, client, model, memory, functions, tokenizer):
-    text = text[:4000] # make sure we don't run over token limit
-    prompt = Prompt([UserMessage('Analyze the following Text to identify if there is any content relevant to the query {{$query}}, Respond using this JSON template:\n\n{"relevant": True if there is any text found in the input that is relevant to the query, False otherwise>, "tldr": <relevant extract from Text, or "">}\n\nText:\n\n{{$input}}\n\n. ')])
+async def llm_tldr (text, query, client, model, memory, functions, tokenizer, max_chars):
+    text = text[:max_chars] # make sure we don't run over token limit
+    prompt = Prompt([UserMessage('Analyze the following Text to identify if there is any content relevant to the query {{$query}}, Respond using this JSON template:\n\n{"relevant": True if there is any text found in the input that is relevant to the query, False otherwise>, "tldr": <relevant content found in Text, rewritten as needed for coherence, or "" if nothing found>}\n\nText:\n\n{{$input}}\n\n. ')])
     response_text=''
     completion = None
     schema = {
         'schema_type':'object',
         'title':'tldr',
         'description':'extract query-relevant text',
         'properties':{
@@ -209,25 +213,27 @@
             }
         },
         'required':['relevant', 'tldr'],
         'returns':"extract"
     }
     
     options = PromptCompletionOptions(completion_type='chat', model=model)
-    response = await ut.run_wave(client, {'input':text, 'query':query}, prompt, options, memory, functions, tokenizer, validator=JSONResponseValidator(schema))
+    # don't clutter primary memory with tldr stuff
+    fork = MemoryFork(memory)
+    response = await ut.run_wave(client, {'input':text, 'query':query}, prompt, options, fork, functions, tokenizer, validator=JSONResponseValidator(schema))
     if type(response) == dict and 'status' in response and response['status'] == 'success'and 'message' in response:
         message = response['message']
         if type(message) == dict and 'content' in message and type(message['content']) == dict:
             content = message['content']
             if 'relevant' in content and content['relevant'] == True:
                 return content['tldr']
     return ''
     
 
-async def response_text_extract(query_phrase, keywords, keyword_weights, url, response, get_time, client, model, memory, functions, tokenizer):
+async def response_text_extract(query_phrase, keywords, keyword_weights, url, response, get_time, client, model, memory, functions, tokenizer, max_chars):
     curr=time.time()
     extract_text = ''
     site = ut.extract_site(url)
     if url.endswith('pdf'):
         pass
     else:
         elements = partition_html(text=response)
@@ -237,30 +243,30 @@
             str_elements.append(stre)
         extract_text = extract_subtext(str_elements, query_phrase, keywords, keyword_weights)
     if len(extract_text.strip()) < 8:
         return ''
 
     # now ask openai to extract answer
     response = ''
-    response = await llm_tldr(extract_text, query_phrase, client, model, memory, functions, tokenizer)
+    response = await llm_tldr(extract_text, query_phrase, client, model, memory, functions, tokenizer, max_chars)
     return response
 
 def extract_items_from_numbered_list(text):
     items = ''
     elements = text.split('\n')
     for candidate in elements:
         candidate = candidate.lstrip('. \t')
         if len(candidate) > 4 and candidate[0].isdigit():
             candidate = candidate[1:].lstrip('. ')
             if len(candidate) > 4 and candidate[0].isdigit(): # strip second digit if more than 10 items
                 candidate = candidate[1:].lstrip('. ')
             items += candidate+' '
     return items
 
-async def search_google(original_query, search_level, query_phrase, keywords, client, model, memory, functions, tokenizer):
+async def search_google(original_query, search_level, query_phrase, keywords, client, model, memory, functions, tokenizer, max_chars):
   start_time = time.time()
   all_urls=[]; urls_used=[]; urls_tried=[]
   index = 0; tried_index = 0
   full_text=''
   keyword_weights = {}
   for keyword in keywords:
       zipf = wf.zipf_frequency(keyword, 'en')
@@ -296,12 +302,12 @@
         if url in gpt_phrase_urls:
             gpt_phrase_urls.remove(url)
 
     # interleave both lists now that duplicates are removed
     urls = [val for tup in zip_longest(orig_phrase_urls, gpt_phrase_urls) for val in tup if val is not None]
     all_urls = copy.deepcopy(urls)
     full_text = \
-        await process_urls(extract_query, keywords, keyword_weights, all_urls, search_level, client, model, memory, functions, tokenizer)
+        await process_urls(extract_query, keywords, keyword_weights, all_urls, search_level, client, model, memory, functions, tokenizer, max_chars)
   except:
       traceback.print_exc()
   return  full_text
```

### Comparing `alphawave-0.2.5/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.2.6/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 import json
 import sys
 import os
 import time
 import traceback
 import readline as rl
+from alphawave.MemoryFork import MemoryFork
 import alphawave_pyexts.llmsearch.google_search_concurrent as gs
 import alphawave_pyexts.utilityV2 as ut
 import asyncio
 history = {}
 
 
-async def run_chat(client, query_string, model,  memory, functions, tokenizer, search_level=gs.QUICK_SEARCH):
+async def run_chat(client, query_string, model,  memory, functions, tokenizer, max_chars=1500, search_level=gs.QUICK_SEARCH):
   #tracemalloc.start()
   response_text = ''
   storeInteraction = True
   try:
     #
-    #### 
-    #
-    query_phrase, keywords = await ut.get_search_phrase_and_keywords(client, query_string, model, memory, functions, tokenizer)
+    fork = MemoryFork(memory)
+    query_phrase, keywords = await ut.get_search_phrase_and_keywords(client, query_string, model, fork, functions, tokenizer)
 
-    try:
-      google_text=\
-        await gs.search_google(query_string, gs.QUICK_SEARCH, query_phrase, keywords, client, model, memory, functions, tokenizer)
-    except:
-      traceback.print_exc()
+    google_text=\
+      await gs.search_google(query_string, gs.QUICK_SEARCH, query_phrase, keywords, client, model, fork, functions, tokenizer, max_chars)
     return google_text
-  except KeyboardInterrupt:
-    traceback.print_exc()
-    raise KeyboardInterrupt
   except:
     traceback.print_exc()
   return ''
 
 if __name__ == '__main__' :
   while True:
     asyncio.run(run_chat(input('Yes?')))
```

### Comparing `alphawave-0.2.5/src/alphawave_pyexts/searchCommand.py` & `alphawave-0.2.6/src/alphawave_pyexts/searchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.2.6/src/alphawave_pyexts/utilityV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 google_key = os.getenv("GOOGLE_KEY")
 google_cx = os.getenv("GOOGLE_CX")
 GOOGLE = 'google'
 
 def ask_LLM(model, gpt_message, max_tokens=100, temp=0.7, top_p=1.0, host = None, port = None, tkroot = None, tkdisplay=None):
     completion = None
     response = ''
+    print(f'***** utility ask_LLL temperature {temp}')
     try:
       if not model.lower().startswith('gpt'):
-        completion = client.run_query(model, gpt_message, temp, top_p, max_tokens, host, port )
+        completion = client.run_query(model, gpt_message, temp, top_p, max_tokens, host, port, tkroot, tkdisplay )
         if completion is not None:
           response = completion
 
       else:
         stream= openai.ChatCompletion.create(
             model=model, messages=gpt_message, max_tokens=max_tokens, temperature=temp, top_p=1, stop='STOP', stream=True)
         response = ''
```

### Comparing `alphawave-0.2.5/tests/testOSClient.py` & `alphawave-0.2.6/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/tests/testOpenAiClient.py` & `alphawave-0.2.6/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.5/tests/testSchema.py` & `alphawave-0.2.6/tests/testSchema.py`

 * *Files identical despite different names*

