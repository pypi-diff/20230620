# Comparing `tmp/mangadexSdk-0.0.8.tar.gz` & `tmp/mangadexSdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangadexSdk-0.0.8.tar", last modified: Tue Sep 14 01:11:10 2021, max compression
+gzip compressed data, was "mangadexSdk-0.0.9.tar", last modified: Sun Jan  9 00:51:22 2022, max compression
```

## Comparing `mangadexSdk-0.0.8.tar` & `mangadexSdk-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2021-09-14 01:11:10.006420 mangadexSdk-0.0.8/
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     1070 2021-05-14 01:39:40.000000 mangadexSdk-0.0.8/LICENSE
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     4219 2021-09-14 01:11:10.006420 mangadexSdk-0.0.8/PKG-INFO
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     3633 2021-05-14 05:40:08.000000 mangadexSdk-0.0.8/README.md
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      104 2021-05-20 03:50:29.000000 mangadexSdk-0.0.8/pyproject.toml
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      674 2021-09-14 01:11:10.010419 mangadexSdk-0.0.8/setup.cfg
-drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2021-09-14 01:11:10.002419 mangadexSdk-0.0.8/src/
-drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2021-09-14 01:11:10.006420 mangadexSdk-0.0.8/src/mangadexSdk/
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      184 2021-05-20 04:20:25.000000 mangadexSdk-0.0.8/src/mangadexSdk/__init__.py
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      118 2021-05-20 04:34:49.000000 mangadexSdk-0.0.8/src/mangadexSdk/constants.py
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     5646 2021-08-01 03:57:21.000000 mangadexSdk-0.0.8/src/mangadexSdk/mangaDex.py
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)    12755 2021-07-17 05:01:35.000000 mangadexSdk-0.0.8/src/mangadexSdk/requestTypes.py
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     6817 2021-09-14 01:09:12.000000 mangadexSdk-0.0.8/src/mangadexSdk/responseTypes.py
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     1345 2021-05-20 04:20:25.000000 mangadexSdk-0.0.8/src/mangadexSdk/serializable.py
-drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2021-09-14 01:11:10.006420 mangadexSdk-0.0.8/src/mangadexSdk.egg-info/
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     4219 2021-09-14 01:11:09.000000 mangadexSdk-0.0.8/src/mangadexSdk.egg-info/PKG-INFO
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      380 2021-09-14 01:11:09.000000 mangadexSdk-0.0.8/src/mangadexSdk.egg-info/SOURCES.txt
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)        1 2021-09-14 01:11:09.000000 mangadexSdk-0.0.8/src/mangadexSdk.egg-info/dependency_links.txt
--rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)       12 2021-09-14 01:11:09.000000 mangadexSdk-0.0.8/src/mangadexSdk.egg-info/top_level.txt
+drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2022-01-09 00:51:22.805175 mangadexSdk-0.0.9/
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     1070 2021-05-14 01:39:40.000000 mangadexSdk-0.0.9/LICENSE
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     4219 2022-01-09 00:51:22.805175 mangadexSdk-0.0.9/PKG-INFO
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     3633 2021-05-14 05:40:08.000000 mangadexSdk-0.0.9/README.md
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      104 2021-05-20 03:50:29.000000 mangadexSdk-0.0.9/pyproject.toml
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      674 2022-01-09 00:51:22.805175 mangadexSdk-0.0.9/setup.cfg
+drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2022-01-09 00:51:22.797175 mangadexSdk-0.0.9/src/
+drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2022-01-09 00:51:22.805175 mangadexSdk-0.0.9/src/mangadexSdk/
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      184 2021-05-20 04:20:25.000000 mangadexSdk-0.0.9/src/mangadexSdk/__init__.py
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      118 2021-05-20 04:34:49.000000 mangadexSdk-0.0.9/src/mangadexSdk/constants.py
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     5646 2021-08-01 03:57:21.000000 mangadexSdk-0.0.9/src/mangadexSdk/mangaDex.py
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)    12755 2021-07-17 05:01:35.000000 mangadexSdk-0.0.9/src/mangadexSdk/requestTypes.py
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     7129 2022-01-09 00:43:07.000000 mangadexSdk-0.0.9/src/mangadexSdk/responseTypes.py
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     1345 2021-05-20 04:20:25.000000 mangadexSdk-0.0.9/src/mangadexSdk/serializable.py
+drwxrwxr-x   0 jfrancis  (1000) jfrancis  (1000)        0 2022-01-09 00:51:22.805175 mangadexSdk-0.0.9/src/mangadexSdk.egg-info/
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)     4219 2022-01-09 00:51:22.000000 mangadexSdk-0.0.9/src/mangadexSdk.egg-info/PKG-INFO
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)      380 2022-01-09 00:51:22.000000 mangadexSdk-0.0.9/src/mangadexSdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)        1 2022-01-09 00:51:22.000000 mangadexSdk-0.0.9/src/mangadexSdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 jfrancis  (1000) jfrancis  (1000)       12 2022-01-09 00:51:22.000000 mangadexSdk-0.0.9/src/mangadexSdk.egg-info/top_level.txt
```

### Comparing `mangadexSdk-0.0.8/LICENSE` & `mangadexSdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mangadexSdk-0.0.8/PKG-INFO` & `mangadexSdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangadexSdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: An SDK for easily accessing information from the Mangadex v5 API.
 Home-page: https://github.com/jasonfrancis/mangadexSDK
 Author: Jason Francis
 Author-email: jkfranci@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jasonfrancis/mangadexSDK/issues
 Platform: UNKNOWN
```

### Comparing `mangadexSdk-0.0.8/README.md` & `mangadexSdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mangadexSdk-0.0.8/setup.cfg` & `mangadexSdk-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mangadexSdk
-version = 0.0.8
+version = 0.0.9
 author = Jason Francis
 author_email = jkfranci@gmail.com
 description = An SDK for easily accessing information from the Mangadex v5 API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jasonfrancis/mangadexSDK
 project_urls =
```

### Comparing `mangadexSdk-0.0.8/src/mangadexSdk/mangaDex.py` & `mangadexSdk-0.0.9/src/mangadexSdk/mangaDex.py`

 * *Files identical despite different names*

### Comparing `mangadexSdk-0.0.8/src/mangadexSdk/requestTypes.py` & `mangadexSdk-0.0.9/src/mangadexSdk/requestTypes.py`

 * *Files identical despite different names*

### Comparing `mangadexSdk-0.0.8/src/mangadexSdk/responseTypes.py` & `mangadexSdk-0.0.9/src/mangadexSdk/responseTypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,33 +11,38 @@
 	error = 2
 
 class Relationship(Serializable):
 	def __init__(self, id:str, type:str, **kwargs):
 		self.id = id
 		self.type = type
 
+# chapter details from AtHome
+class AtHomeChapter(Serializable):
+	def __init__(self, **kwargs):
+		self.hash = getFromDict(kwargs, "hash")
+		self.data = getFromDict(kwargs, "data")
+		self.dataSaver = getFromDict(kwargs, "dataSaver")
+		super().__init__(serializableProperties=[])
 # At-Home/Server
 class AtHomeServer(Serializable):
 	def __init__(self, baseUrl:str, **kwargs):
 		self.baseUrl = baseUrl
 		self.chapterId = None
-		super().__init__([])
+		self.chapter = getFromDict(kwargs, "chapter", dict())
+		super().__init__([SerializableProperty(AtHomeChapter, self.getAttributeName(self.chapter))])
 	def setChapterId(self, value:str):
 		self.chapterId = value
 
 # Chapter responses
 class ChapterAttributes(Serializable):
-	def __init__(self, volume:int, chapter:str, title:str, translatedLanguage:str, hash:str, data:List[str], dataSaver:List[str], publishAt:str, createdAt:str, updatedAt:str, version:int, **kwargs):
+	def __init__(self, volume:int, chapter:str, title:str, translatedLanguage:str, publishAt:str, createdAt:str, updatedAt:str, version:int, **kwargs):
 		self.volume = volume
 		self.chapter = chapter
 		self.title = title
 		self.translatedLanguage = translatedLanguage
-		self.hash = hash
-		self.data = data
-		self.dataSaver = dataSaver
 		self.publishAt = publishAt
 		self.createdAt = createdAt
 		self.updatedAt = updatedAt
 		self.version = version
 		self.externalUrl = getFromDict(kwargs, "externalUrl")
 
 class Chapter(Serializable):
@@ -48,18 +53,18 @@
 		self.relationships = relationships
 		# Instructions about how to deserialize attributes
 		super().__init__([SerializableProperty(ChapterAttributes, self.getAttributeName(self.attributes)), SerializableProperty(Relationship, self.getAttributeName(self.relationships))])
 	def getPageUrls(self, atHomeServer:AtHomeServer) -> dict:
 		if atHomeServer.chapterId != self.id:
 			raise Exception(f"Chapter.getPageUrls(): Attempting to set page urls for chapter {self.id}, but the provided atHomeServer is for chapter {atHomeServer.chapterId}")
 		output = { "data": [], "dataSaver": [] }
-		for page in self.attributes.data:
-			output["data"].append(f"{atHomeServer.baseUrl}/data/{self.attributes.hash}/{page}")
-		for page in self.attributes.dataSaver:
-			output["dataSaver"].append(f"{atHomeServer.baseUrl}/data-saver/{self.attributes.hash}/{page}")
+		for page in atHomeServer.chapter.data:
+			output["data"].append(f"{atHomeServer.baseUrl}/data/{atHomeServer.chapter.hash}/{page}")
+		for page in atHomeServer.chapter.dataSaver:
+			output["dataSaver"].append(f"{atHomeServer.baseUrl}/data-saver/{atHomeServer.chapter.hash}/{page}")
 		return output
 
 class ChapterResult(Serializable):
 	def __init__(self, result:Result, data:Chapter, **kwargs):
 		self.result = result
 		self.data = data
 		# Instrutions to deserialize data and relationships correctly.
```

### Comparing `mangadexSdk-0.0.8/src/mangadexSdk/serializable.py` & `mangadexSdk-0.0.9/src/mangadexSdk/serializable.py`

 * *Files identical despite different names*

### Comparing `mangadexSdk-0.0.8/src/mangadexSdk.egg-info/PKG-INFO` & `mangadexSdk-0.0.9/src/mangadexSdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangadexSdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: An SDK for easily accessing information from the Mangadex v5 API.
 Home-page: https://github.com/jasonfrancis/mangadexSDK
 Author: Jason Francis
 Author-email: jkfranci@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jasonfrancis/mangadexSDK/issues
 Platform: UNKNOWN
```

