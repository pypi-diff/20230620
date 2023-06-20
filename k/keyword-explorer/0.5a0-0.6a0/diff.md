# Comparing `tmp/keyword_explorer-0.5a0.tar.gz` & `tmp/keyword_explorer-0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\keyword_explorer-0.5a0.tar", last modified: Tue May  2 13:38:22 2023, max compression
+gzip compressed data, was "dist\keyword_explorer-0.6a0.tar", last modified: Tue Jun 20 14:11:49 2023, max compression
```

## Comparing `keyword_explorer-0.5a0.tar` & `keyword_explorer-0.6a0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/
--rw-rw-rw-   0        0        0     1115 2022-03-09 16:58:07.000000 keyword_explorer-0.5a0/LICENSE
--rw-rw-rw-   0        0        0     2014 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/PKG-INFO
--rw-rw-rw-   0        0        0      577 2022-08-03 13:33:36.000000 keyword_explorer-0.5a0/README
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/
--rw-rw-rw-   0        0        0     7854 2023-02-22 22:28:46.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/AppBase.py
--rw-rw-rw-   0        0        0    26285 2023-04-24 17:14:48.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/ContextExplorer.py
--rw-rw-rw-   0        0        0     4113 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/GoogleExplorer.py
--rw-rw-rw-   0        0        0    17258 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/KeywordExplorer.py
--rw-rw-rw-   0        0        0    15540 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/ModelExplorer.py
--rw-rw-rw-   0        0        0    37366 2023-03-15 14:09:02.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/NarrativeExplorer.py
--rw-rw-rw-   0        0        0    29399 2023-04-12 13:32:31.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/NarrativeExplorer2.py
--rw-rw-rw-   0        0        0    16372 2023-03-17 19:53:40.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TerrainFromGML.py
--rw-rw-rw-   0        0        0    10386 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TweetCountExplorer.py
--rw-rw-rw-   0        0        0    27254 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TweetDownloader.py
--rw-rw-rw-   0        0        0    40960 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/TweetEmbedExplorer.py
--rw-rw-rw-   0        0        0    11243 2023-04-12 13:23:32.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/WikiPageviewExplorer.py
--rw-rw-rw-   0        0        0        0 2022-03-02 13:40:13.000000 keyword_explorer-0.5a0/keyword_explorer/Apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/OpenAI/
--rw-rw-rw-   0        0        0    17090 2023-04-25 20:28:22.000000 keyword_explorer-0.5a0/keyword_explorer/OpenAI/OpenAIComms.py
--rw-rw-rw-   0        0        0    23382 2023-04-18 22:38:59.000000 keyword_explorer-0.5a0/keyword_explorer/OpenAI/OpenAIEmbeddings.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/
--rw-rw-rw-   0        0        0     8404 2022-01-04 13:05:33.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/DefinedColors.py
--rw-rw-rw-   0        0        0     8055 2020-09-18 13:05:26.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/DefinedColors_GOES.py
--rw-rw-rw-   0        0        0     1825 2023-03-17 19:53:40.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/ExampleHand.py
--rw-rw-rw-   0        0        0     3078 2019-10-16 17:42:36.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/HelloWorld.py
--rw-rw-rw-   0        0        0     3354 2023-03-17 19:54:27.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/LinePrimitives.py
--rw-rw-rw-   0        0        0     1405 2019-10-16 17:42:36.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/MouseEventHandler.py
--rw-rw-rw-   0        0        0     5866 2023-03-17 19:53:40.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/Pandas_main.py
--rw-rw-rw-   0        0        0     5078 2021-12-29 16:05:04.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/Primitives.py
--rw-rw-rw-   0        0        0     6339 2019-10-16 17:42:36.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/ProceduralCube.py
--rw-rw-rw-   0        0        0    14012 2023-03-17 19:54:41.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/ShapePrimitives.py
--rw-rw-rw-   0        0        0        0 2019-07-10 17:34:16.000000 keyword_explorer-0.5a0/keyword_explorer/Panda3D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/
--rw-rw-rw-   0        0        0    19367 2023-01-13 20:15:17.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TweetKeywords.py
--rw-rw-rw-   0        0        0     4693 2022-09-07 17:20:53.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Base.py
--rw-rw-rw-   0        0        0     8853 2022-12-05 20:54:31.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Counts.py
--rw-rw-rw-   0        0        0        0 2022-02-01 19:48:49.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/__init__.py
--rw-rw-rw-   0        0        0     8625 2022-12-18 12:34:08.000000 keyword_explorer-0.5a0/keyword_explorer/TwitterV2/tweet_lookup.py
--rw-rw-rw-   0        0        0        0 2022-03-02 13:40:28.000000 keyword_explorer-0.5a0/keyword_explorer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/
--rw-rw-rw-   0        0        0     3932 2022-10-27 13:43:22.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/HFaceGPT.py
--rw-rw-rw-   0        0        0     6158 2022-10-25 15:59:55.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/PatternCounter.py
--rw-rw-rw-   0        0        0        0 2022-10-14 11:54:53.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/__init__.py
--rw-rw-rw-   0        0        0     5070 2022-10-13 19:45:32.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/test1.py
--rw-rw-rw-   0        0        0     2069 2021-04-15 17:58:09.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/test2.py
--rw-rw-rw-   0        0        0     3090 2021-04-21 13:27:35.000000 keyword_explorer-0.5a0/keyword_explorer/huggingface/test3.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/mastodon/
--rw-rw-rw-   0        0        0        0 2022-12-02 14:15:20.000000 keyword_explorer-0.5a0/keyword_explorer/mastodon/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-01-13 15:06:40.000000 keyword_explorer-0.5a0/keyword_explorer/mastodon/post_lookup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/
--rw-rw-rw-   0        0        0     1633 2023-04-13 19:13:26.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/Buttons.py
--rw-rw-rw-   0        0        0      458 2021-09-20 14:28:52.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/CanvasData.py
--rw-rw-rw-   0        0        0    13329 2022-08-30 14:28:42.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/CanvasFrame.py
--rw-rw-rw-   0        0        0     2356 2023-02-23 21:54:28.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/Checkboxes.py
--rw-rw-rw-   0        0        0     1967 2022-09-30 13:29:58.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/ConsoleDprint.py
--rw-rw-rw-   0        0        0     2667 2022-06-15 13:06:41.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/DataField.py
--rw-rw-rw-   0        0        0     1728 2022-08-17 14:36:57.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/DateEntryField.py
--rw-rw-rw-   0        0        0     9542 2023-03-15 17:03:25.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/GPT3EmbeddingFrame.py
--rw-rw-rw-   0        0        0    12835 2023-03-22 14:00:45.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/GPT3GeneratorFrame.py
--rw-rw-rw-   0        0        0     1823 2022-09-23 19:53:54.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/LabeledParam.py
--rw-rw-rw-   0        0        0     5269 2023-04-20 18:56:29.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/ListField.py
--rw-rw-rw-   0        0        0     6046 2022-09-26 14:56:22.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/MoveableNode.py
--rw-rw-rw-   0        0        0      613 2023-03-21 22:11:34.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/SelectParam.py
--rw-rw-rw-   0        0        0     7019 2022-03-01 16:44:28.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextComparePopup.py
--rw-rw-rw-   0        0        0     5144 2023-01-31 13:58:52.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextField.py
--rw-rw-rw-   0        0        0     7912 2022-03-01 16:46:29.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TkCanvasBase.py
--rw-rw-rw-   0        0        0     1163 2022-08-01 14:40:36.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/ToolTip.py
--rw-rw-rw-   0        0        0     4145 2022-09-07 17:40:13.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicCombo.py
--rw-rw-rw-   0        0        0     3954 2023-04-20 18:44:25.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicComboExt.py
--rw-rw-rw-   0        0        0        0 2021-09-24 12:22:20.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtilsExt/
--rw-rw-rw-   0        0        0    22026 2023-04-26 15:26:09.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtilsExt/GPTContextFrame.py
--rw-rw-rw-   0        0        0        0 2023-02-23 15:04:56.000000 keyword_explorer-0.5a0/keyword_explorer/tkUtilsExt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/keyword_explorer/utils/
--rw-rw-rw-   0        0        0     6872 2022-10-13 19:07:46.000000 keyword_explorer-0.5a0/keyword_explorer/utils/CorporaGenerator.py
--rw-rw-rw-   0        0        0    34486 2023-03-15 22:25:18.000000 keyword_explorer-0.5a0/keyword_explorer/utils/ManifoldReduction.py
--rw-rw-rw-   0        0        0     3568 2022-10-14 12:47:24.000000 keyword_explorer-0.5a0/keyword_explorer/utils/MySqlInterface.py
--rw-rw-rw-   0        0        0    16560 2023-03-16 15:23:45.000000 keyword_explorer-0.5a0/keyword_explorer/utils/NetworkxGraphing.py
--rw-rw-rw-   0        0        0     1609 2023-03-14 20:38:59.000000 keyword_explorer-0.5a0/keyword_explorer/utils/SharedObjects.py
--rw-rw-rw-   0        0        0     8686 2022-01-21 15:29:51.000000 keyword_explorer-0.5a0/keyword_explorer/utils/TextSimilarity.py
--rw-rw-rw-   0        0        0       67 2022-08-18 21:37:11.000000 keyword_explorer-0.5a0/keyword_explorer/utils/app_test.py
--rw-rw-rw-   0        0        0      408 2022-01-14 14:47:24.000000 keyword_explorer-0.5a0/keyword_explorer/utils/excel_to_latex.py
--rw-rw-rw-   0        0        0      483 2021-03-22 11:48:23.000000 keyword_explorer-0.5a0/keyword_explorer/utils/find_transformer_models.py
--rw-rw-rw-   0        0        0     4670 2023-03-06 13:15:31.000000 keyword_explorer-0.5a0/keyword_explorer/utils/google_search.py
--rw-rw-rw-   0        0        0     4090 2022-03-04 20:54:01.000000 keyword_explorer-0.5a0/keyword_explorer/utils/wikipedia_search.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/
--rw-rw-rw-   0        0        0     2014 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3244 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      168 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 13:38:21.000000 keyword_explorer-0.5a0/keyword_explorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-03-29 19:08:22.000000 keyword_explorer-0.5a0/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-05-02 13:38:22.000000 keyword_explorer-0.5a0/setup.cfg
--rw-rw-rw-   0        0        0     3272 2023-05-02 13:37:07.000000 keyword_explorer-0.5a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/
+-rw-rw-rw-   0        0        0     1115 2022-03-09 16:58:07.000000 keyword_explorer-0.6a0/LICENSE
+-rw-rw-rw-   0        0        0     1987 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2022-08-03 13:33:36.000000 keyword_explorer-0.6a0/README
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/
+-rw-rw-rw-   0        0        0     7858 2023-05-22 20:04:26.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/AppBase.py
+-rw-rw-rw-   0        0        0    27509 2023-06-20 12:18:53.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/ContextExplorer.py
+-rw-rw-rw-   0        0        0     4113 2023-04-12 13:23:32.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/GoogleExplorer.py
+-rw-rw-rw-   0        0        0    17258 2023-04-12 13:23:32.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/KeywordExplorer.py
+-rw-rw-rw-   0        0        0    15540 2023-04-12 13:23:32.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/ModelExplorer.py
+-rw-rw-rw-   0        0        0    37366 2023-03-15 14:09:02.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/NarrativeExplorer.py
+-rw-rw-rw-   0        0        0    29399 2023-04-12 13:32:31.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/NarrativeExplorer2.py
+-rw-rw-rw-   0        0        0    16372 2023-03-17 19:53:40.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/TerrainFromGML.py
+-rw-rw-rw-   0        0        0    10386 2023-04-12 13:23:32.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/TweetCountExplorer.py
+-rw-rw-rw-   0        0        0    27254 2023-04-12 13:23:32.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/TweetDownloader.py
+-rw-rw-rw-   0        0        0    40960 2023-04-12 13:23:32.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/TweetEmbedExplorer.py
+-rw-rw-rw-   0        0        0    12131 2023-06-01 12:30:55.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/WikiPageviewExplorer.py
+-rw-rw-rw-   0        0        0        0 2022-03-02 13:40:13.000000 keyword_explorer-0.6a0/keyword_explorer/Apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/OpenAI/
+-rw-rw-rw-   0        0        0    17117 2023-06-20 12:18:53.000000 keyword_explorer-0.6a0/keyword_explorer/OpenAI/OpenAIComms.py
+-rw-rw-rw-   0        0        0    25348 2023-06-20 12:18:53.000000 keyword_explorer-0.6a0/keyword_explorer/OpenAI/OpenAIEmbeddings.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/
+-rw-rw-rw-   0        0        0     8404 2022-01-04 13:05:33.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/DefinedColors.py
+-rw-rw-rw-   0        0        0     8055 2020-09-18 13:05:26.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/DefinedColors_GOES.py
+-rw-rw-rw-   0        0        0     1825 2023-03-17 19:53:40.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/ExampleHand.py
+-rw-rw-rw-   0        0        0     3078 2019-10-16 17:42:36.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/HelloWorld.py
+-rw-rw-rw-   0        0        0     3354 2023-03-17 19:54:27.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/LinePrimitives.py
+-rw-rw-rw-   0        0        0     1405 2019-10-16 17:42:36.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/MouseEventHandler.py
+-rw-rw-rw-   0        0        0     5866 2023-03-17 19:53:40.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/Pandas_main.py
+-rw-rw-rw-   0        0        0     5078 2021-12-29 16:05:04.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/Primitives.py
+-rw-rw-rw-   0        0        0     6339 2019-10-16 17:42:36.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/ProceduralCube.py
+-rw-rw-rw-   0        0        0    14012 2023-03-17 19:54:41.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/ShapePrimitives.py
+-rw-rw-rw-   0        0        0        0 2019-07-10 17:34:16.000000 keyword_explorer-0.6a0/keyword_explorer/Panda3D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/TwitterV2/
+-rw-rw-rw-   0        0        0    19367 2023-01-13 20:15:17.000000 keyword_explorer-0.6a0/keyword_explorer/TwitterV2/TweetKeywords.py
+-rw-rw-rw-   0        0        0     4693 2022-09-07 17:20:53.000000 keyword_explorer-0.6a0/keyword_explorer/TwitterV2/TwitterV2Base.py
+-rw-rw-rw-   0        0        0     8853 2022-12-05 20:54:31.000000 keyword_explorer-0.6a0/keyword_explorer/TwitterV2/TwitterV2Counts.py
+-rw-rw-rw-   0        0        0        0 2022-02-01 19:48:49.000000 keyword_explorer-0.6a0/keyword_explorer/TwitterV2/__init__.py
+-rw-rw-rw-   0        0        0     8625 2022-12-18 12:34:08.000000 keyword_explorer-0.6a0/keyword_explorer/TwitterV2/tweet_lookup.py
+-rw-rw-rw-   0        0        0        0 2022-03-02 13:40:28.000000 keyword_explorer-0.6a0/keyword_explorer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/huggingface/
+-rw-rw-rw-   0        0        0     3932 2022-10-27 13:43:22.000000 keyword_explorer-0.6a0/keyword_explorer/huggingface/HFaceGPT.py
+-rw-rw-rw-   0        0        0     6158 2022-10-25 15:59:55.000000 keyword_explorer-0.6a0/keyword_explorer/huggingface/PatternCounter.py
+-rw-rw-rw-   0        0        0        0 2022-10-14 11:54:53.000000 keyword_explorer-0.6a0/keyword_explorer/huggingface/__init__.py
+-rw-rw-rw-   0        0        0     5070 2022-10-13 19:45:32.000000 keyword_explorer-0.6a0/keyword_explorer/huggingface/test1.py
+-rw-rw-rw-   0        0        0     2069 2021-04-15 17:58:09.000000 keyword_explorer-0.6a0/keyword_explorer/huggingface/test2.py
+-rw-rw-rw-   0        0        0     3090 2021-04-21 13:27:35.000000 keyword_explorer-0.6a0/keyword_explorer/huggingface/test3.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/mastodon/
+-rw-rw-rw-   0        0        0        0 2022-12-02 14:15:20.000000 keyword_explorer-0.6a0/keyword_explorer/mastodon/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-01-13 15:06:40.000000 keyword_explorer-0.6a0/keyword_explorer/mastodon/post_lookup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/
+-rw-rw-rw-   0        0        0     1633 2023-04-13 19:13:26.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/Buttons.py
+-rw-rw-rw-   0        0        0      458 2021-09-20 14:28:52.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/CanvasData.py
+-rw-rw-rw-   0        0        0    13329 2022-08-30 14:28:42.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/CanvasFrame.py
+-rw-rw-rw-   0        0        0     2356 2023-02-23 21:54:28.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/Checkboxes.py
+-rw-rw-rw-   0        0        0     1967 2022-09-30 13:29:58.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/ConsoleDprint.py
+-rw-rw-rw-   0        0        0     2667 2022-06-15 13:06:41.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/DataField.py
+-rw-rw-rw-   0        0        0     1728 2022-08-17 14:36:57.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/DateEntryField.py
+-rw-rw-rw-   0        0        0     9542 2023-03-15 17:03:25.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/GPT3EmbeddingFrame.py
+-rw-rw-rw-   0        0        0    12835 2023-03-22 14:00:45.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/GPT3GeneratorFrame.py
+-rw-rw-rw-   0        0        0     1823 2022-09-23 19:53:54.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/LabeledParam.py
+-rw-rw-rw-   0        0        0     5269 2023-04-20 18:56:29.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/ListField.py
+-rw-rw-rw-   0        0        0     6046 2022-09-26 14:56:22.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/MoveableNode.py
+-rw-rw-rw-   0        0        0      613 2023-03-21 22:11:34.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/SelectParam.py
+-rw-rw-rw-   0        0        0     7019 2022-03-01 16:44:28.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/TextComparePopup.py
+-rw-rw-rw-   0        0        0     5144 2023-01-31 13:58:52.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/TextField.py
+-rw-rw-rw-   0        0        0     7912 2022-03-01 16:46:29.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/TkCanvasBase.py
+-rw-rw-rw-   0        0        0     1163 2022-08-01 14:40:36.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/ToolTip.py
+-rw-rw-rw-   0        0        0     4145 2022-09-07 17:40:13.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/TopicCombo.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 18:44:25.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/TopicComboExt.py
+-rw-rw-rw-   0        0        0        0 2021-09-24 12:22:20.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtilsExt/
+-rw-rw-rw-   0        0        0    22238 2023-06-20 12:18:53.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtilsExt/GPTContextFrame.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 15:04:56.000000 keyword_explorer-0.6a0/keyword_explorer/tkUtilsExt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer/utils/
+-rw-rw-rw-   0        0        0     6872 2022-10-13 19:07:46.000000 keyword_explorer-0.6a0/keyword_explorer/utils/CorporaGenerator.py
+-rw-rw-rw-   0        0        0    34486 2023-03-15 22:25:18.000000 keyword_explorer-0.6a0/keyword_explorer/utils/ManifoldReduction.py
+-rw-rw-rw-   0        0        0     3319 2023-05-04 20:58:37.000000 keyword_explorer-0.6a0/keyword_explorer/utils/MySqlInterface.py
+-rw-rw-rw-   0        0        0    16615 2023-05-10 12:04:04.000000 keyword_explorer-0.6a0/keyword_explorer/utils/NetworkxGraphing.py
+-rw-rw-rw-   0        0        0     1609 2023-03-14 20:38:59.000000 keyword_explorer-0.6a0/keyword_explorer/utils/SharedObjects.py
+-rw-rw-rw-   0        0        0     8686 2022-01-21 15:29:51.000000 keyword_explorer-0.6a0/keyword_explorer/utils/TextSimilarity.py
+-rw-rw-rw-   0        0        0       67 2023-05-04 15:27:23.000000 keyword_explorer-0.6a0/keyword_explorer/utils/app_test.py
+-rw-rw-rw-   0        0        0      419 2023-06-06 21:07:23.000000 keyword_explorer-0.6a0/keyword_explorer/utils/excel_to_latex.py
+-rw-rw-rw-   0        0        0      483 2021-03-22 11:48:23.000000 keyword_explorer-0.6a0/keyword_explorer/utils/find_transformer_models.py
+-rw-rw-rw-   0        0        0     4670 2023-03-06 13:15:31.000000 keyword_explorer-0.6a0/keyword_explorer/utils/google_search.py
+-rw-rw-rw-   0        0        0     4530 2023-06-01 12:41:20.000000 keyword_explorer-0.6a0/keyword_explorer/utils/wikipedia_search.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/keyword_explorer.egg-info/
+-rw-rw-rw-   0        0        0     1987 2023-06-20 14:11:48.000000 keyword_explorer-0.6a0/keyword_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3244 2023-06-20 14:11:48.000000 keyword_explorer-0.6a0/keyword_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:11:48.000000 keyword_explorer-0.6a0/keyword_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      168 2023-06-20 14:11:48.000000 keyword_explorer-0.6a0/keyword_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 14:11:48.000000 keyword_explorer-0.6a0/keyword_explorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-03-29 19:08:22.000000 keyword_explorer-0.6a0/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-06-20 14:11:49.000000 keyword_explorer-0.6a0/setup.cfg
+-rw-rw-rw-   0        0        0     3245 2023-06-20 14:10:13.000000 keyword_explorer-0.6a0/setup.py
```

### Comparing `keyword_explorer-0.5a0/LICENSE` & `keyword_explorer-0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/PKG-INFO` & `keyword_explorer-0.6a0/keyword_explorer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: keyword_explorer
-Version: 0.5a0
-Summary: A set of tools for producing and exploring keywords on Twitter and the Wikipedia
+Name: keyword-explorer
+Version: 0.6a0
+Summary: A set of tools for computational sociology using LLMs
 Home-page: https://github.com/pgfeldman/KeywordExplorer
 Author: Philip Feldman
 Author-email: phil@philfeldman.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keyword_explorer-0.5a0/README` & `keyword_explorer-0.6a0/README`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/AppBase.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/AppBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         dt = datetime.now()
         self.logfile = "{}/{}_{}.csv".format(Path.home(), self.app_name, dt.strftime("%Y-%m-%d-%H-%M-%S"))
         self.log_action("session", {"session start":dt.strftime("%H:%M:%S")})
 
 
     def setup_app(self):
         self.app_name = "AppBase"
-        self.app_version = "3.10.2022"
+        self.app_version = "1.27.2023"
         self.geom = (600, 150)
 
 
     def build_view(self):
         row = 0
 
         self.title("{} (v {})".format(self.app_name, self.app_version))
@@ -150,14 +150,16 @@
     def clean_text(self, s:str) -> str:
         char_list = [s[j] for j in range(len(s)) if ord(s[j]) in range(65536)]
         s=''
         for j in char_list:
             s=s+j
         return s
 
+
+
     def log_action(self, task:str, row_info:Dict, mode:str = "a"):
         with open(self.logfile, mode, encoding="utf-8") as fio:
             dt = datetime.now()
             ds = dt.strftime("%H:%M:%S")
             s = "time, {}, task, {}".format(ds, task)
             for key, val in row_info.items():
                 if isinstance(val, str):
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/ContextExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/ContextExplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import tkinter as tk
 from tkinter import ttk
 import tkinter.messagebox as message
 from datetime import datetime
 from tkinter import filedialog
 from enum import Enum
-import matplotlib.colors as mcolors
+from pypdf import PdfReader
 
 import pandas as pd
 
 from keyword_explorer.Apps.AppBase import AppBase
 from keyword_explorer.tkUtils.Buttons import Buttons
 from keyword_explorer.tkUtils.ToolTip import ToolTip
 from keyword_explorer.tkUtils.Checkboxes import Checkboxes
@@ -74,15 +74,15 @@
         self.experiment_id_list = []
         self.so.add_object("generate_model_combo", self.generate_model_combo, TopicComboExt)
         self.so.add_object("MySqlInterface", self.msi, MySqlInterface)
         # self.test_data_callback()
 
     def setup_app(self):
         self.app_name = "ContextExplorer"
-        self.app_version = "4.24.2023"
+        self.app_version = "6.19.2023"
         self.geom = (910, 790)
         self.oai = OpenAIComms()
         self.oae = OpenAIEmbeddings()
         self.so = SharedObjects()
         self.msi = MySqlInterface(user_name="root", db_name="gpt_summary")
 
         if not self.oai.key_exists():
@@ -221,15 +221,15 @@
         self.regex_field = DataField(tab, row, 'Parse regex:', text_width, label_width=label_width)
         self.regex_field.set_text(r"([\.!?()]+)")
         ToolTip(self.regex_field.tk_entry, "The regex used to parse the file. Editable")
         row = self.regex_field.get_next_row()
 
         self.action_buttons2 = Buttons(tab, row, "Actions")
         b = self.action_buttons2.add_button("Test", self.test_file_callback, width=-1)
-        ToolTip(b, "Performs a small test on 100 lines of text and does not save to DB")
+        ToolTip(b, "Performs a small test on 10 lines of text and does not save to DB")
         b = self.action_buttons2.add_button("Load File", self.load_file_callback, width=-1)
         ToolTip(b, "Loads new text into a project, splits into chunks and finds embeddings")
 
     def set_style_callback(self, event:tk.Event = None):
         print("ContextExplorer.set_style_callback(): event = {}".format(event))
         buttons:Buttons = self.so.get_object("context_buttons")
         style_str = self.style_list.get_selected()
@@ -437,19 +437,35 @@
         print("ContextExplorer.load_file_callback()")
         group_name = self.target_group_field.get_text().strip()
         text_name = self.target_text_name.get_text().strip()
         regex_str = self.regex_field.get_text()
         if len(group_name) < 3 or len(text_name) < 3:
             tk.messagebox.showwarning("Warning!", "Please set text and model fields")
             return
-        result = filedialog.askopenfilename(filetypes=(("Text files", "*.txt"),("All Files", "*.*")), title="Load text file")
+        result = filedialog.askopenfilename(filetypes=(("Text and pdf files", "*.txt *.pdf"),("All Files", "*.*")), title="Load text file")
         textfile = result.split("/")[-1]
         s:str
         if result:
-            s_list = self.oae.parse_text_file(result, r_str=regex_str)
+            s_list = []
+            if result.endswith(".pdf"):
+                s_list = self.oae.parse_pdf_file(result, r_str=regex_str)
+            elif result.endswith(".txt"):
+                s_list = self.oae.parse_text_file(result, r_str=regex_str)
+            else:
+                print("ContextExplorer.load_file_callback: unable to open file {}".format(result))
+                return
+
+            # look to see if we can find 'references' on a single row
+            for i in range(len(s_list)):
+                s = s_list[i]
+                if s.lower() == 'references':
+                    print("ContextExplorer.load_file_callback(): truncating references (rows {} - {})".format(i-1, len(s_list)))
+                    s_list = s_list[:i-1]
+                    break
+
             answer = tk.messagebox.askyesno("Warning!", "This will read, process, and store large amounts of data\ntarget = [{}]\ngroup = [{}]\nfile = [{}]\nlines = [{:,}]\nProceed?".format(
                 text_name, group_name, textfile, len(s_list)))
             if answer == True:
                 engine = self.generate_model_combo.get_text()
                 level = int(self.target_level_combo.get_text())
                 print("ContextExplorer.load_file_callback(): Getting embeddings")
                 df = self.oae.get_embeddings(s_list)
@@ -468,23 +484,36 @@
         print("ContextExplorer.test_file_callback()")
         group_name = self.target_group_field.get_text()
         text_name = self.target_text_name.get_text()
         regex_str = self.regex_field.get_text()
         if len(group_name) < 3 or len(text_name) < 3:
             tk.messagebox.showwarning("Warning!", "Please set text and model fields")
             return
-        result = filedialog.askopenfilename(filetypes=(("Text files", "*.txt"),("All Files", "*.*")), title="Load text file")
+        result = filedialog.askopenfilename(filetypes=(("Text and pdf files", "*.txt *.pdf"),("All Files", "*.*")), title="Load text file")
+        print("test file = {}".format(result))
+
         s:str
-        num_rows = 100
+        num_rows = 10
         if result:
-            s_list = self.oae.parse_text_file(result, r_str=regex_str)
+            s_list = []
+            if result.endswith(".pdf"):
+                s_list = self.oae.parse_pdf_file(result, r_str=regex_str)
+            elif result.endswith(".txt"):
+                s_list = self.oae.parse_text_file(result, r_str=regex_str)
+            else:
+                print("ContextExplorer.test_file_callback: unable to open file {}".format(result))
+                return
+
             # build a proxy db results List
             results = []
             for i in range(num_rows):
-                d = {"text_id":i, "parsed_text":s_list[i]}
+                s = s_list[i]
+                if s.lower() == 'references':
+                    break
+                d = {"text_id":i, "parsed_text":s}
                 results.append(d)
             row_dict:Dict
             count = 0
             words_to_summarize = 300
             #engine = self.oae.DEFAULT_SUMMARY_MODEL
             engine = self.generate_model_combo.get_text()
             print("\tUsing {}".format(engine))
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/GoogleExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/GoogleExplorer.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/KeywordExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/KeywordExplorer.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/ModelExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/ModelExplorer.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/NarrativeExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/NarrativeExplorer.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/NarrativeExplorer2.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/NarrativeExplorer2.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/TerrainFromGML.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/TerrainFromGML.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/TweetCountExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/TweetCountExplorer.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/TweetDownloader.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/TweetDownloader.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/TweetEmbedExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/TweetEmbedExplorer.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Apps/WikiPageviewExplorer.py` & `keyword_explorer-0.6a0/keyword_explorer/Apps/WikiPageviewExplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,17 @@
         b = self.views_action_buttons.add_button("Plot", self.plot_callback, width=-1)
         ToolTip(b, "Plot page views")
         b = self.views_action_buttons.add_button("Save", self.save_callback, width=-1)
         ToolTip(b, "Save page views to Excel file")
         b = self.views_action_buttons.add_button("Show Pages", self.show_pages_callback, width=-1)
         ToolTip(b, "Launch each Wikipedia page as a separate tab in the default browser")
         row = self.views_action_buttons.get_next_row()
+        b = self.views_action_buttons.add_button("Save Text", self.save_page_text_callback, width=-1)
+        ToolTip(b, "Save each Wikipedia page as a separate text file in the specified directory")
+        row = self.views_action_buttons.get_next_row()
 
     def build_page_view_params(self, lf:tk.LabelFrame, text_width:int, label_width:int):
         row = 0
         self.sample_list = ListField(lf, row, "Sample", width=text_width, label_width=label_width, static_list=True)
         self.sample_list.set_text(text='daily, monthly')
         self.sample_list.set_callback(self.set_time_sample_callback)
         self.set_time_sample_callback()
@@ -214,14 +217,27 @@
                     d[start_time_str] = vd.views
             df = pd.DataFrame(l)
             with pd.ExcelWriter(filename) as writer:
                 df.to_excel(writer, sheet_name='Page Views')
                 writer.save()
             self.log_action("save", {"filename":filename})
 
+    def save_page_text_callback(self):
+        folder_selected = filedialog.askdirectory()
+        topic_list = self.wiki_pages_text_field.get_list("\n")
+        for topic in topic_list:
+            if len(topic) > 2:
+                print("Getting text for page [{}]:".format(topic))
+                s = ws.get_page(topic, debug=False)
+                filename = "{}/{}.txt".format(folder_selected, topic)
+                print("\tSaving to {}".format(filename))
+                with open(filename, 'w', encoding="utf-8") as f:
+                    f.write(s)
+                # print("{}\n\t{}".format(filename, s))
+
     def show_pages_callback(self):
         topic_list = self.wiki_pages_text_field.get_list("\n")
         for topic in topic_list:
             query = topic.replace(" ", "_")
             query = query.replace("&", "%26")
             url_str = "https://en.wikipedia.org/wiki/{}".format(query)
             webbrowser.open(url_str)
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/OpenAI/OpenAIComms.py` & `keyword_explorer-0.6a0/keyword_explorer/OpenAI/OpenAIComms.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,28 +73,28 @@
                     frequency_penalty = frequency_penalty,
                     messages=[cu.to_dict() for cu in unit_list]
                 )
                 d = response['choices'][0]
                 s = d['message']['content']
                 return s.strip()
 
-            except (openai.error.RateLimitError, openai.error.APIConnectionError, openai.error.APIError) as e:
+            except (openai.error.RateLimitError, openai.error.APIConnectionError, openai.error.APIError, openai.error.ServiceUnavailableError) as e:
                 print("\nOpenAIComms.get_chat_complete(): {}".format(e.user_message))
                 sleeptime = (waitcount+1) * time_to_wait
                 print("\twaiting {} seconds {} of {}".format(sleeptime, waitcount, waitmax))
                 time.sleep(sleeptime)
                 waitcount += 1
                 if waitcount > waitmax:
                     return self.ERROR_MSG
 
     def get_prompt_result_params(self, prompt:str, engine:str = "text-davinci-003", max_tokens:int = 30, temperature:float = 0.4, top_p:float = 1, logprobs:int = 1,
                                  num_responses:int = 1, presence_penalty:float = 0.3, frequency_penalty:float = 0.3) -> str:
 
         if any([x in engine for x in self.chat_models]):
-            print("OpenAICommsget_prompt_result_params(): Using Chat interface")
+            print("OpenAIComms.get_prompt_result_params(): Using Chat interface")
             l = [ChatUnit(prompt, CHAT_ROLES.USER)]
             return self.get_chat_complete(l, engine=engine, max_tokens=max_tokens, temperature=temperature, top_p=top_p,
                                           presence_penalty=presence_penalty, frequency_penalty=frequency_penalty)
 
         goodread = False
         waitcount = 0
         waitmax = 0
@@ -304,15 +304,15 @@
         print(result)
 
 def chat_main():
     oai = OpenAIComms()
 
 
     print("\navailable text models:")
-    lm = oai.list_models(exclude_list = ["whisper", "embed", "similarity", "code", "edit", "search", "audio", "instruct", "2020", "if", "insert"])
+    lm = oai.list_models(exclude_list = ["whisper", "embed", "similarity", "code", "edit", "search", "audio", "2020", "if", "insert"])
     for m in sorted(lm):
         print(m)
 
     l = []
     l.append(ChatUnit("You are a helpful assistant.", CHAT_ROLES.SYSTEM))
     l.append(ChatUnit("Who won the world series in 2020?", CHAT_ROLES.USER))
     l.append(ChatUnit("The Los Angeles Dodgers won the World Series in 2020.", CHAT_ROLES.ASSIST))
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/OpenAI/OpenAIEmbeddings.py` & `keyword_explorer-0.6a0/keyword_explorer/OpenAI/OpenAIEmbeddings.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import openai
 import openai.embeddings_utils as oaiu
 import pandas as pd
 import re
 import ast
 import pickle
+from pypdf import PdfReader
 
 from keyword_explorer.OpenAI.OpenAIComms import OpenAIComms
 from keyword_explorer.utils.MySqlInterface import MySqlInterface
 
 from typing import List, Dict, Pattern, TextIO, Any
 
 class OpenAIEmbeddings:
@@ -73,47 +74,63 @@
         response = self.msi.read_data(sql)
         d:Dict
         to_return = []
         for d in response:
             to_return.append("{}: {}".format(d['id'], d['parsed_text']))
         return to_return
 
-    def parse_text_file(self, filename:str, r_str:str = r"([\.!?()]+)", default_print:int = 0, min_chars = 10) -> List:
+    def parse_content(self, raw_text:str, r_str:str = r"([\.!?()]+)", default_print:int = 0, min_chars:int = 10) -> List:
+        # print("OpenAIEmbeddings:parse_content r_str = {}".format(r_str))
         cr_regex = re.compile("\n+")
-        print("OpenAIEmbeddings:parse_text_file r_str = {}".format(r_str))
         reg = re.compile(r_str)
-        #f = open(filename, mode="r", encoding="G-8", errors='ignore')
-        f = open(filename, mode="r", encoding="utf-8", errors='replace')
-
-        s = f.read()
-        f.close()
-
-        s = cr_regex.sub(" ", s)
-        l = reg.split(s)
+        l = cr_regex.split(raw_text)
         s1:str
         s2:str
         s_list = []
         i = 0
         while i < len(l):
-            s1 = l[i].strip()
+            s = reg.sub(" ", l[i])
+            s1 = s.strip()
             while i < len(l)-1:
                 s2 = l[i+1]
                 if len(s2) < min_chars:
                     s1 += s2
                     i += 1
                 else:
                     break
             s_list.append(s1)
             i += 1
 
         for i in range(default_print):
-            print("OpenAIEmbeddings:parse_text_file{}".format(s_list[i]))
+            print("OpenAIEmbeddings:parse_file_str{}".format(s_list[i]))
+
+        return s_list
+
+    def parse_text_file(self, filename:str, r_str:str = r"([\.!?()]+)", default_print:int = 0, min_chars = 10) -> List:
+        f = open(filename, mode="r", encoding="utf-8", errors='replace')
+
+        s = f.read()
+        f.close()
+        s_list = self.parse_content(s, r_str, default_print, min_chars)
 
         return s_list
 
+    def parse_pdf_file(self, filename:str, r_str:str = r"([\.!?()]+)", default_print:int = 0, min_chars = 10) -> List:
+        reader = PdfReader(filename)
+        number_of_pages = len(reader.pages)
+        full_list = []
+        print("\tnumber of pages = {}".format(number_of_pages))
+        for i in range(number_of_pages):
+            print("\tParsing page {} of {}".format(i, number_of_pages))
+            page = reader.pages[i]
+            text = page.extract_text()
+            s_list = self.parse_content(text, r_str=r_str)
+            full_list.extend(s_list)
+        return full_list
+
     def get_embeddings(self, text_list:List, submit_size:int = 10, max:int = -1) -> pd.DataFrame:
         d_list = []
         ed:Dict
         md:Dict
         num_text = len(text_list)
         # for i in range(0, num_text+submit_size-1, submit_size):
         #    s_list = text_list[i:min(num_text, i+submit_size])
@@ -272,29 +289,42 @@
         vals = (project_id,)
         results = self.msi.read_data(sql, vals)
 
         num_lines = len(results)
         count = 0
         level = 1
         summary_count = 0
+        old_summary = "unset"
         while count < num_lines:
             d = self.build_text_to_summarize(results, count, words_to_summarize)
             # run the query and store the result. Update the parsed text table with the summary id
             summary = self.oac.get_prompt_result_params(d['query'], engine=engine, temperature=0, presence_penalty=0.8, frequency_penalty=0, max_tokens=max_tokens)
+            if summary == old_summary:
+                print("OpenAIEmbeddings.summarize_raw_text() Same summary error, returning early!")
+                print("\t{}".format(d))
+                return summary_count
+            old_summary = summary
+
             sql = "insert into table_summary_text (source, level, summary_text, origins) values (%s, %s, %s, %s)"
             vals = (project_id, level, summary, str(d['origins']))
             row_id = self.msi.write_sql_values_get_row(sql, vals)
             summary_count += 1
-            print("[{}] {}".format(row_id, summary))
+            if num_lines > 0:
+                print("[{}] ({} of {} = {:.2f}%) {}".format(row_id, count, num_lines, float(count/num_lines)*100, summary))
 
             for r in d['row_list']:
                 sql = "update table_parsed_text set summary_id = %s where id = %s"
                 vals = (row_id, r)
                 self.msi.write_sql_values_get_row(sql, vals)
-            count = d['count']
+
+            if d['count'] > count:
+                count = d['count']
+            else:
+                print("OpenAIEmbeddings.summarize_raw_text() manually incrementing count from {} to {}".format(count, count + 1))
+                count += 1
 
         return summary_count
 
     def summarize_summary_text(self, text_name:str, group_name:str, source_level:int, max_lines = -1, words_to_summarize = 200, database="gpt_summary", user="root") -> int:
         # take some set of lines from the parsed text table and produce summary lines in the summary text table
         d:Dict
 
@@ -437,14 +467,28 @@
             to_return.append("line {}: {}".format(d['id'], d['parsed_text']))
 
         return to_return
 
     def close_db(self):
         self.msi.close()
 
+    def tk_filter_string(self, input_string:str) -> str:
+        """
+        Filters the input string to remove characters outside the allowed range for Tkinter (U+0000 to U+FFFF).
+
+        Args:
+        input_string (str): The input string containing the characters to be filtered.
+
+        Returns:
+        str: A new string with disallowed characters removed.
+        """
+        allowed_range = range(0x0000, 0xFFFF + 1)
+        filtered_string = ''.join([c for c in input_string if ord(c) in allowed_range])
+        return filtered_string
+
 
 def store_embeddings_main(text_name:str, group_name:str, file_str:str):
     oae = OpenAIEmbeddings()
     s_list = oae.parse_text_file(file_str, 10, default_print=10) # can be obtained here: https://www.gutenberg.org/files/2701/2701-h/2701-h.htm
     df = oae.get_embeddings(s_list[:100])
     #df = oae.get_embeddings(s_list)
     print(df)
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/DefinedColors.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/DefinedColors.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/DefinedColors_GOES.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/DefinedColors_GOES.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/ExampleHand.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/ExampleHand.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/HelloWorld.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/HelloWorld.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/LinePrimitives.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/LinePrimitives.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/MouseEventHandler.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/MouseEventHandler.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/Pandas_main.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/Pandas_main.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/Primitives.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/Primitives.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/ProceduralCube.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/ProceduralCube.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/Panda3D/ShapePrimitives.py` & `keyword_explorer-0.6a0/keyword_explorer/Panda3D/ShapePrimitives.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TweetKeywords.py` & `keyword_explorer-0.6a0/keyword_explorer/TwitterV2/TweetKeywords.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Base.py` & `keyword_explorer-0.6a0/keyword_explorer/TwitterV2/TwitterV2Base.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/TwitterV2Counts.py` & `keyword_explorer-0.6a0/keyword_explorer/TwitterV2/TwitterV2Counts.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/TwitterV2/tweet_lookup.py` & `keyword_explorer-0.6a0/keyword_explorer/TwitterV2/tweet_lookup.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/huggingface/HFaceGPT.py` & `keyword_explorer-0.6a0/keyword_explorer/huggingface/HFaceGPT.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/huggingface/PatternCounter.py` & `keyword_explorer-0.6a0/keyword_explorer/huggingface/PatternCounter.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/huggingface/test1.py` & `keyword_explorer-0.6a0/keyword_explorer/huggingface/test1.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/huggingface/test2.py` & `keyword_explorer-0.6a0/keyword_explorer/huggingface/test2.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/huggingface/test3.py` & `keyword_explorer-0.6a0/keyword_explorer/huggingface/test3.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/mastodon/post_lookup.py` & `keyword_explorer-0.6a0/keyword_explorer/mastodon/post_lookup.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/Buttons.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/Buttons.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/CanvasFrame.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/CanvasFrame.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/Checkboxes.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/Checkboxes.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/ConsoleDprint.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/ConsoleDprint.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/DataField.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/DataField.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/DateEntryField.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/DateEntryField.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/GPT3EmbeddingFrame.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/GPT3EmbeddingFrame.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/GPT3GeneratorFrame.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/GPT3GeneratorFrame.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/LabeledParam.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/LabeledParam.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/ListField.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/ListField.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/MoveableNode.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/MoveableNode.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/SelectParam.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/SelectParam.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextComparePopup.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/TextComparePopup.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TextField.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/TextField.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TkCanvasBase.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/TkCanvasBase.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/ToolTip.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/ToolTip.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicCombo.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/TopicCombo.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtils/TopicComboExt.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtils/TopicComboExt.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/tkUtilsExt/GPTContextFrame.py` & `keyword_explorer-0.6a0/keyword_explorer/tkUtilsExt/GPTContextFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,16 @@
         self.context_text_field.set_text(full_question)
 
         origins = oae.get_origins_text(origins_list)
         self.sources_text_field.clear()
         self.sources_text_field.set_text("\n\n".join(origins))
 
         self.dp.dprint("Submitting Question: {}".format(question))
-        answer = oae.get_response(full_question, model=model)
+        answer = oae.get_response(full_question, model=model, max_tokens=512)
+        answer = oae.tk_filter_string(answer)
         self.response_text_field.set_text(answer)
 
     def auto_question_callback(self, type = PROMPT_TYPE.QUESTION):
         print("GPTContextFrame.auto_question_callback()")
         if self.project_df.empty:
             tk.messagebox.showwarning("Warning!", "Please import data first")
             return
@@ -252,16 +253,18 @@
 
         generate_model_combo:TopicComboExt = self.so.get_object("generate_model_combo")
         model = generate_model_combo.get_text()
         print("\tusing model {}".format(model))
 
         oae = OpenAIEmbeddings()
         question = oae.get_response(context_str, max_tokens=512, model=model)
+        question = oae.tk_filter_string(question)
         if type == PROMPT_TYPE.QUESTION:
-            self.prompt_text_field.set_text(question)
+            self.context_prompt.set_text(question)
+            self.prompt_text_field.set_text("{}. Use the style of a white paper.".format(question))
         else:
             self.response_text_field.set_text(question)
         self.tab_control.select(0)
 
 
 
     def get_summmary_callback(self):
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/CorporaGenerator.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/CorporaGenerator.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/ManifoldReduction.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/ManifoldReduction.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/MySqlInterface.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/MySqlInterface.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,22 +83,19 @@
         return self.last_query
 
     def close(self):
         self.connection.close()
 
 
 if __name__ == '__main__':
-    msi = MySqlInterface("root", "twitter_v2")
-    sql = "insert into table_experiment (name, date) values (%s, %s)"
-    values = ("Test1", datetime.now())
-    result = msi.write_sql_values_get_row(sql, values)
-    print(result)
-    # sql = "select * from post_view ORDER BY post_time;"
-    # sql = "select topic_id, forum_id, topic_title from phpbb_topics"
-    # print("{}".format(msi.read_data(sql)))
+    msi = MySqlInterface("root", "gpt_summary")
+    sql = "describe table_parsed_text"
+    result = msi.read_data(sql)
+    for d in result:
+        print(d)
     msi.close()
 
 '''
 Create a list of all words
 Create a timeline of all words
 Plot that and see if any patterns present themselves
 '''
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/NetworkxGraphing.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/NetworkxGraphing.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,13 +390,16 @@
             weapon_id = i*weapons_per_warrior + j
             source = "weapon_{}".format(weapon_id)
             ng.add_connected_nodes(source, target)
 
     filename = "operators.graphml"
     ng.to_graphml(filename, graph_creator="phil", node_attributes=['type'])
 
+    stats(ng, "War Elephants", 100)
+    plt.show()
+
 print("\n----------------------\n")
 
 if __name__ == '__main__':
-    chess_example()
+    # chess_example()
     # country_example()
-    # war_elephants_example()
+    war_elephants_example()
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/SharedObjects.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/SharedObjects.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/TextSimilarity.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/TextSimilarity.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/google_search.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/google_search.py`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/keyword_explorer/utils/wikipedia_search.py` & `keyword_explorer-0.6a0/keyword_explorer/utils/wikipedia_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,16 +90,29 @@
 
 def evaluate(node_name:str, debug:bool = True) -> [str, int]:
     node_name = get_closest_wiki_page(node_name, threshold=0.5, debug=debug)
     node_name = node_name.replace(" ", "_")
     weight = get_wiki_pageviews(node_name)
     return node_name, weight
 
-def main():
+def get_page(node_name:str, debug:bool = True) ->str:
+    node_name = get_closest_wiki_page(node_name, threshold=0.5, debug=debug)
+    print("\tget_page({})".format(node_name))
+    # node_name = node_name.replace(" ", "_")
+    page:wikipedia.WikipediaPage
+    page = wikipedia.page(node_name, auto_suggest=False)
+    if debug:
+        print(page.content)
+    return page.content
+
+def eval_main():
     print("wikimedia_scratch")
     l = ["Virtue_ethics", "simpson characters"]
     for key in l:
         node_name, weight = evaluate(key)
         print("{} = {}\n".format(node_name, weight))
 
+def main():
+    get_page("Solar System")
+
 if __name__ == "__main__":
     main()
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer.egg-info/PKG-INFO` & `keyword_explorer-0.6a0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: keyword-explorer
-Version: 0.5a0
-Summary: A set of tools for producing and exploring keywords on Twitter and the Wikipedia
+Name: keyword_explorer
+Version: 0.6a0
+Summary: A set of tools for computational sociology using LLMs
 Home-page: https://github.com/pgfeldman/KeywordExplorer
 Author: Philip Feldman
 Author-email: phil@philfeldman.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keyword_explorer-0.5a0/keyword_explorer.egg-info/SOURCES.txt` & `keyword_explorer-0.6a0/keyword_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyword_explorer-0.5a0/setup.py` & `keyword_explorer-0.6a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 **ModelExplorer** is a Python desktop app that lets a user interact with a finetuned GPT-2 model trained using EmbeddingExplorer
 
 Full documentation is available at https://github.com/pgfeldman/KeywordExplorer#readme'''
 
 setup(
     name='keyword_explorer',
-    version= "0.5.alpha",
+    version= "0.6.alpha",
     packages=['keyword_explorer',
               'keyword_explorer.utils',
               'keyword_explorer.TwitterV2',
               'keyword_explorer.mastodon',
               'keyword_explorer.tkUtils',
               'keyword_explorer.tkUtilsExt',
               'keyword_explorer.OpenAI',
               'keyword_explorer.Panda3D',
               'keyword_explorer.huggingface',
               'keyword_explorer.Apps'],
     url='https://github.com/pgfeldman/KeywordExplorer',
     license='MIT',
     author='Philip Feldman',
     author_email='phil@philfeldman.com',
-    description='A set of tools for producing and exploring keywords on Twitter and the Wikipedia',
+    description='A set of tools for computational sociology using LLMs',
     long_description=long_s,
     install_requires=[
         'pandas',
         'matplotlib',
         'numpy',
         'scikit-learn',
         'requests',
```

