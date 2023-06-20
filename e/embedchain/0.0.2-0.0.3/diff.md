# Comparing `tmp/embedchain-0.0.2.tar.gz` & `tmp/embedchain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.0.2.tar", last modified: Tue Jun 20 12:35:12 2023, max compression
+gzip compressed data, was "embedchain-0.0.3.tar", last modified: Tue Jun 20 15:38:46 2023, max compression
```

## Comparing `embedchain-0.0.2.tar` & `embedchain-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.321033 embedchain-0.0.2/
--rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.2/LICENSE
--rw-r--r--   0 tj         (501) staff       (20)     5278 2023-06-20 12:35:12.320897 embedchain-0.0.2/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)     4795 2023-06-20 12:34:13.000000 embedchain-0.0.2/README.md
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.318299 embedchain-0.0.2/embedchain/
--rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/__init__.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.320022 embedchain-0.0.2/embedchain/chunkers/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/base_chunker.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.2/embedchain/chunkers/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)     4417 2023-06-20 11:23:20.000000 embedchain-0.0.2/embedchain/embedchain.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.320685 embedchain-0.0.2/embedchain/loaders/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/loaders/__init__.py
--rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/loaders/pdf_file.py
--rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.2/embedchain/loaders/web_page.py
--rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/loaders/youtube_video.py
--rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/utils.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.319158 embedchain-0.0.2/embedchain.egg-info/
--rw-r--r--   0 tj         (501) staff       (20)     5278 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/SOURCES.txt
--rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/dependency_links.txt
--rw-r--r--   0 tj         (501) staff       (20)       95 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/requires.txt
--rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/top_level.txt
--rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-20 12:35:12.321069 embedchain-0.0.2/setup.cfg
--rw-r--r--   0 tj         (501) staff       (20)      958 2023-06-20 12:12:37.000000 embedchain-0.0.2/setup.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.807260 embedchain-0.0.3/
+-rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.3/LICENSE
+-rw-r--r--   0 tj         (501) staff       (20)     6151 2023-06-20 15:38:46.807106 embedchain-0.0.3/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)     5668 2023-06-20 15:38:37.000000 embedchain-0.0.3/README.md
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.799258 embedchain-0.0.3/embedchain/
+-rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/__init__.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.806274 embedchain-0.0.3/embedchain/chunkers/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.3/embedchain/chunkers/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     4451 2023-06-20 15:38:37.000000 embedchain-0.0.3/embedchain/embedchain.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.806888 embedchain-0.0.3/embedchain/loaders/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/loaders/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/loaders/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.3/embedchain/loaders/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/loaders/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.3/embedchain/utils.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 15:38:46.800103 embedchain-0.0.3/embedchain.egg-info/
+-rw-r--r--   0 tj         (501) staff       (20)     6151 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tj         (501) staff       (20)      103 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/requires.txt
+-rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-20 15:38:46.000000 embedchain-0.0.3/embedchain.egg-info/top_level.txt
+-rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-20 15:38:46.807297 embedchain-0.0.3/setup.cfg
+-rw-r--r--   0 tj         (501) staff       (20)      966 2023-06-20 15:38:37.000000 embedchain-0.0.3/setup.py
```

### Comparing `embedchain-0.0.2/LICENSE` & `embedchain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.2/PKG-INFO` & `embedchain-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: embedchain is a framework to easily create bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # embedchain
 
-embedchain is a framework to easily create bots over any dataset.
+embedchain is a framework to easily create LLM powered bots over any dataset.
+
+It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 * If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
-app = app()
+naval_chat_bot = App()
 
-app.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
-app.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
-app.add("web_page", "https://nav.al/feedback")
-app.add("web_page", "https://nav.al/agi")
+naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
+naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
+naval_chat_bot.add("web_page", "https://nav.al/feedback")
+naval_chat_bot.add("web_page", "https://nav.al/agi")
 
-app.query("How to do a startup?")
+naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
+# answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
 
 First make sure that you have the package installed. If not, then install it using `pip`
 
 ```bash
 pip install embedchain
 ```
 
 ## Usage
 
-* We use OpenAI's embedding model to create embeddings for chunks and ChatGPT API as LLM to get answer given the relevant docs. Make sure that you have an OpenAI account and an API key.
+* We use OpenAI's embedding model to create embeddings for chunks and ChatGPT API as LLM to get answer given the relevant docs. Make sure that you have an OpenAI account and an API key. If you have dont have an API key, you can create one by visiting [this link](https://platform.openai.com/account/api-keys).
 
 * Once you have the API key, set it in an environment variable called `OPENAI_API_KEY`
 
-```bash
-export OPENAI_API_KEY='sk-xxxxxxxx'
+```python
+import os
+os.environ["OPENAI_API_KEY"] = "sk-xxxx"
 ```
 
 * Next import the `App` class from embedchain and use `.add` function to add any dataset.
 
 ```python
 
 from embedchain import App
 
 naval_ravikant_chat_bot_app = App()
 
-naval_ravikant_chat_bot_app.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
-naval_ravikant_chat_bot_app.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
-naval_ravikant_chat_bot_app.add("web_page", "https://nav.al/agi")
+naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
+naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
+naval_chat_bot.add("web_page", "https://nav.al/feedback")
+naval_chat_bot.add("web_page", "https://nav.al/agi")
 ```
 
 * If there is any other app instance in your script or app, you can change the import as
 
 ```python
 from embedchain import App as EmbedChainApp
 
@@ -76,40 +81,41 @@
 
 from embedchain import App as ECApp
 ```
 
 * Now you app is created. You can use `.query` function to get the answer for any query.
 
 ```python
-print(app.query("How to do a startup?"))
+print(naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
+# answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 ## Format supported
 
 We support the following formats:
 
-* Youtube Video
+### Youtube Video
 
 To add any youtube video to your app, use the data_type (first argument to `.add`) as `youtube_video`. Eg:
 
 ```python
 app.add('youtube_video', 'a_valid_youtube_url_here')
 ```
 
-* PDF File
+### PDF File
 
 To add any pdf file, use the data_type as `pdf_file`. Eg:
 
 ```python
 app.add('pdf_file', 'a_valid_url_where_pdf_file_can_be_accessed')
 ```
 
 Note that we do not support password protected pdfs as of now.
 
-* Web Page
+### Web Page
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
@@ -142,15 +148,15 @@
 
 In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
-- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data,
+- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
 - [OpenAI's ChatGPT API](https://platform.openai.com/docs/guides/gpt/chat-completions-api) as LLM to get answers given the context
 - [Chroma](https://github.com/chroma-core/chroma) as the vector database to store embeddings
 
 # Author
 
 * Taranjeet Singh ([@taranjeetio](https://twitter.com/taranjeetio))
```

### Comparing `embedchain-0.0.2/README.md` & `embedchain-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 # embedchain
 
-embedchain is a framework to easily create bots over any dataset.
+embedchain is a framework to easily create LLM powered bots over any dataset.
+
+It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 * If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
-app = app()
+naval_chat_bot = App()
 
-app.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
-app.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
-app.add("web_page", "https://nav.al/feedback")
-app.add("web_page", "https://nav.al/agi")
+naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
+naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
+naval_chat_bot.add("web_page", "https://nav.al/feedback")
+naval_chat_bot.add("web_page", "https://nav.al/agi")
 
-app.query("How to do a startup?")
+naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
+# answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
 
 First make sure that you have the package installed. If not, then install it using `pip`
 
 ```bash
 pip install embedchain
 ```
 
 ## Usage
 
-* We use OpenAI's embedding model to create embeddings for chunks and ChatGPT API as LLM to get answer given the relevant docs. Make sure that you have an OpenAI account and an API key.
+* We use OpenAI's embedding model to create embeddings for chunks and ChatGPT API as LLM to get answer given the relevant docs. Make sure that you have an OpenAI account and an API key. If you have dont have an API key, you can create one by visiting [this link](https://platform.openai.com/account/api-keys).
 
 * Once you have the API key, set it in an environment variable called `OPENAI_API_KEY`
 
-```bash
-export OPENAI_API_KEY='sk-xxxxxxxx'
+```python
+import os
+os.environ["OPENAI_API_KEY"] = "sk-xxxx"
 ```
 
 * Next import the `App` class from embedchain and use `.add` function to add any dataset.
 
 ```python
 
 from embedchain import App
 
 naval_ravikant_chat_bot_app = App()
 
-naval_ravikant_chat_bot_app.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
-naval_ravikant_chat_bot_app.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
-naval_ravikant_chat_bot_app.add("web_page", "https://nav.al/agi")
+naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
+naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
+naval_chat_bot.add("web_page", "https://nav.al/feedback")
+naval_chat_bot.add("web_page", "https://nav.al/agi")
 ```
 
 * If there is any other app instance in your script or app, you can change the import as
 
 ```python
 from embedchain import App as EmbedChainApp
 
@@ -62,40 +67,41 @@
 
 from embedchain import App as ECApp
 ```
 
 * Now you app is created. You can use `.query` function to get the answer for any query.
 
 ```python
-print(app.query("How to do a startup?"))
+print(naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
+# answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 ## Format supported
 
 We support the following formats:
 
-* Youtube Video
+### Youtube Video
 
 To add any youtube video to your app, use the data_type (first argument to `.add`) as `youtube_video`. Eg:
 
 ```python
 app.add('youtube_video', 'a_valid_youtube_url_here')
 ```
 
-* PDF File
+### PDF File
 
 To add any pdf file, use the data_type as `pdf_file`. Eg:
 
 ```python
 app.add('pdf_file', 'a_valid_url_where_pdf_file_can_be_accessed')
 ```
 
 Note that we do not support password protected pdfs as of now.
 
-* Web Page
+### Web Page
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
@@ -128,15 +134,15 @@
 
 In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
-- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data,
+- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
 - [OpenAI's ChatGPT API](https://platform.openai.com/docs/guides/gpt/chat-completions-api) as LLM to get answers given the context
 - [Chroma](https://github.com/chroma-core/chroma) as the vector database to store embeddings
 
 # Author
 
 * Taranjeet Singh ([@taranjeetio](https://twitter.com/taranjeetio))
```

### Comparing `embedchain-0.0.2/embedchain/chunkers/base_chunker.py` & `embedchain-0.0.3/embedchain/chunkers/base_chunker.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.2/embedchain/embedchain.py` & `embedchain-0.0.3/embedchain/embedchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         metadatas = embeddings_data["metadatas"]
         ids = embeddings_data["ids"]
         self.collection.add(
             documents=documents,
             metadatas=metadatas,
             ids=ids
         )
-        print(f"Docs count: {self.collection.count()}")
+        print(f"Successfully saved {url}. Total chunks count: {self.collection.count()}")
 
     def load_and_embed(self, loader, chunker, url):
         return self.load_embeddings_to_db(loader, chunker, url)
 
     def _format_result(self, results):
         return [
             (Document(page_content=result[0], metadata=result[1] or {}), result[2])
```

### Comparing `embedchain-0.0.2/embedchain/loaders/pdf_file.py` & `embedchain-0.0.3/embedchain/loaders/pdf_file.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.2/embedchain/loaders/web_page.py` & `embedchain-0.0.3/embedchain/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.2/embedchain/loaders/youtube_video.py` & `embedchain-0.0.3/embedchain/loaders/youtube_video.py`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.2/embedchain.egg-info/PKG-INFO` & `embedchain-0.0.3/embedchain.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 Metadata-Version: 2.1
 Name: embedchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: embedchain is a framework to easily create bots over any dataset
 Home-page: https://github.com/embedchain/embedchain
 Author: Taranjeet Singh
 Author-email: reachtotj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # embedchain
 
-embedchain is a framework to easily create bots over any dataset.
+embedchain is a framework to easily create LLM powered bots over any dataset.
+
+It abstracts the enitre process of loading dataset, chunking it, creating embeddings and then storing in vector database.
 
 You can add a single or multiple dataset using `.add` function and then use `.query` function to find an answer from the added datasets.
 
 * If you want to create a Naval Ravikant bot which has 1 youtube video, 1 book as pdf and 2 of his blog posts, all you need to do is add the links to the videos, pdf and blog posts and embedchain will create a bot for you.
 
 ```python
 
 from embedchain import App
 
-app = app()
+naval_chat_bot = App()
 
-app.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
-app.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
-app.add("web_page", "https://nav.al/feedback")
-app.add("web_page", "https://nav.al/agi")
+naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
+naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
+naval_chat_bot.add("web_page", "https://nav.al/feedback")
+naval_chat_bot.add("web_page", "https://nav.al/agi")
 
-app.query("How to do a startup?")
+naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?")
+# answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 # Getting Started
 
 ## Installation
 
 First make sure that you have the package installed. If not, then install it using `pip`
 
 ```bash
 pip install embedchain
 ```
 
 ## Usage
 
-* We use OpenAI's embedding model to create embeddings for chunks and ChatGPT API as LLM to get answer given the relevant docs. Make sure that you have an OpenAI account and an API key.
+* We use OpenAI's embedding model to create embeddings for chunks and ChatGPT API as LLM to get answer given the relevant docs. Make sure that you have an OpenAI account and an API key. If you have dont have an API key, you can create one by visiting [this link](https://platform.openai.com/account/api-keys).
 
 * Once you have the API key, set it in an environment variable called `OPENAI_API_KEY`
 
-```bash
-export OPENAI_API_KEY='sk-xxxxxxxx'
+```python
+import os
+os.environ["OPENAI_API_KEY"] = "sk-xxxx"
 ```
 
 * Next import the `App` class from embedchain and use `.add` function to add any dataset.
 
 ```python
 
 from embedchain import App
 
 naval_ravikant_chat_bot_app = App()
 
-naval_ravikant_chat_bot_app.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
-naval_ravikant_chat_bot_app.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
-naval_ravikant_chat_bot_app.add("web_page", "https://nav.al/agi")
+naval_chat_bot.add("youtube_video", "https://www.youtube.com/watch?v=3qHkcs3kG44")
+naval_chat_bot.add("pdf_file", "https://navalmanack.s3.amazonaws.com/Eric-Jorgenson_The-Almanack-of-Naval-Ravikant_Final.pdf")
+naval_chat_bot.add("web_page", "https://nav.al/feedback")
+naval_chat_bot.add("web_page", "https://nav.al/agi")
 ```
 
 * If there is any other app instance in your script or app, you can change the import as
 
 ```python
 from embedchain import App as EmbedChainApp
 
@@ -76,40 +81,41 @@
 
 from embedchain import App as ECApp
 ```
 
 * Now you app is created. You can use `.query` function to get the answer for any query.
 
 ```python
-print(app.query("How to do a startup?"))
+print(naval_chat_bot.query("What unique capacity does Naval argue humans possess when it comes to understanding explanations or concepts?"))
+# answer: Naval argues that humans possess the unique capacity to understand explanations or concepts to the maximum extent possible in this physical reality.
 ```
 
 ## Format supported
 
 We support the following formats:
 
-* Youtube Video
+### Youtube Video
 
 To add any youtube video to your app, use the data_type (first argument to `.add`) as `youtube_video`. Eg:
 
 ```python
 app.add('youtube_video', 'a_valid_youtube_url_here')
 ```
 
-* PDF File
+### PDF File
 
 To add any pdf file, use the data_type as `pdf_file`. Eg:
 
 ```python
 app.add('pdf_file', 'a_valid_url_where_pdf_file_can_be_accessed')
 ```
 
 Note that we do not support password protected pdfs as of now.
 
-* Web Page
+### Web Page
 
 To add any web page, use the data_type as `web_page`. Eg:
 
 ```python
 app.add('web_page', 'a_valid_web_page_url')
 ```
 
@@ -142,15 +148,15 @@
 
 In the first release, we are making it easier for anyone to get a chatbot over any dataset up and running in less than a minute. All you need to do is create an app instance, add the data sets using `.add` function and then use `.query` function to get the relevant answer.
 
 # Tech Stack
 
 embedchain is built on the following stack:
 
-- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data,
+- [langchain](https://github.com/hwchase17/langchain) as an LLM framework to load, chunk and index data
 - [OpenAI's Ada embedding model](https://platform.openai.com/docs/guides/embeddings) to create embeddings
 - [OpenAI's ChatGPT API](https://platform.openai.com/docs/guides/gpt/chat-completions-api) as LLM to get answers given the context
 - [Chroma](https://github.com/chroma-core/chroma) as the vector database to store embeddings
 
 # Author
 
 * Taranjeet Singh ([@taranjeetio](https://twitter.com/taranjeetio))
```

### Comparing `embedchain-0.0.2/embedchain.egg-info/SOURCES.txt` & `embedchain-0.0.3/embedchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedchain-0.0.2/setup.py` & `embedchain-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="embedchain",
-    version="0.0.2",
+    version="0.0.3",
     author="Taranjeet Singh",
     author_email="reachtotj@gmail.com",
     description="embedchain is a framework to easily create bots over any dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/embedchain/embedchain",
     packages=setuptools.find_packages(),
@@ -20,14 +20,14 @@
     ],
     python_requires='>=3.8',
     py_modules=["embedchain"],
     install_requires=[
         "langchain>=0.0.205",
         "requests",
         "openai",
-        "chromadb",
+        "chromadb>=0.3.26",
         "youtube-transcript-api",
         "beautifulsoup4",
         "pypdf",
         "pytube",
     ]
 )
```

