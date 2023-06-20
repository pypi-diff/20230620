# Comparing `tmp/api_inference_community-0.0.8.tar.gz` & `tmp/api_inference_community-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_inference_community-0.0.8.tar", last modified: Fri Jun 18 07:50:41 2021, max compression
+gzip compressed data, was "api_inference_community-0.0.9.tar", last modified: Thu Jul  8 10:15:20 2021, max compression
```

## Comparing `api_inference_community-0.0.8.tar` & `api_inference_community-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-06-18 07:50:41.042166 api_inference_community-0.0.8/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       35 2021-05-28 12:33:53.000000 api_inference_community-0.0.8/MANIFEST.in
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      384 2021-06-18 07:50:41.042166 api_inference_community-0.0.8/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3790 2021-05-28 12:33:53.000000 api_inference_community-0.0.8/README.md
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-06-18 07:50:41.042166 api_inference_community-0.0.8/api_inference_community/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4441 2021-06-15 08:33:36.000000 api_inference_community-0.0.8/api_inference_community/routes.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     8153 2021-06-17 14:43:52.000000 api_inference_community-0.0.8/api_inference_community/validation.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-06-18 07:50:41.042166 api_inference_community-0.0.8/api_inference_community.egg-info/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      384 2021-06-18 07:50:41.000000 api_inference_community-0.0.8/api_inference_community.egg-info/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      409 2021-06-18 07:50:41.000000 api_inference_community-0.0.8/api_inference_community.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2021-06-18 07:50:41.000000 api_inference_community-0.0.8/api_inference_community.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2021-06-10 08:11:26.000000 api_inference_community-0.0.8/api_inference_community.egg-info/not-zip-safe
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       83 2021-06-18 07:50:41.000000 api_inference_community-0.0.8/api_inference_community.egg-info/requires.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       24 2021-06-18 07:50:41.000000 api_inference_community-0.0.8/api_inference_community.egg-info/top_level.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       83 2021-06-18 07:50:09.000000 api_inference_community-0.0.8/requirements.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      380 2021-06-18 07:50:41.046166 api_inference_community-0.0.8/setup.cfg
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      557 2021-06-18 07:50:27.000000 api_inference_community-0.0.8/setup.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-07-08 10:15:20.138655 api_inference_community-0.0.9/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       35 2021-05-28 12:33:53.000000 api_inference_community-0.0.9/MANIFEST.in
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      384 2021-07-08 10:15:20.138655 api_inference_community-0.0.9/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3790 2021-05-28 12:33:53.000000 api_inference_community-0.0.9/README.md
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-07-08 10:15:20.134655 api_inference_community-0.0.9/api_inference_community/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4574 2021-07-08 09:21:51.000000 api_inference_community-0.0.9/api_inference_community/routes.py
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)     8655 2021-07-08 09:33:06.000000 api_inference_community-0.0.9/api_inference_community/validation.py
+drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2021-07-08 10:15:20.138655 api_inference_community-0.0.9/api_inference_community.egg-info/
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      384 2021-07-08 10:15:20.000000 api_inference_community-0.0.9/api_inference_community.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      409 2021-07-08 10:15:20.000000 api_inference_community-0.0.9/api_inference_community.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2021-07-08 10:15:20.000000 api_inference_community-0.0.9/api_inference_community.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2021-06-10 08:11:26.000000 api_inference_community-0.0.9/api_inference_community.egg-info/not-zip-safe
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       83 2021-07-08 10:15:20.000000 api_inference_community-0.0.9/api_inference_community.egg-info/requires.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       24 2021-07-08 10:15:20.000000 api_inference_community-0.0.9/api_inference_community.egg-info/top_level.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)       83 2021-07-08 09:21:51.000000 api_inference_community-0.0.9/requirements.txt
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      380 2021-07-08 10:15:20.138655 api_inference_community-0.0.9/setup.cfg
+-rw-r--r--   0 nicolas   (1000) nicolas   (1000)      557 2021-07-08 10:14:05.000000 api_inference_community-0.0.9/setup.py
```

### Comparing `api_inference_community-0.0.8/README.md` & `api_inference_community-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `api_inference_community-0.0.8/api_inference_community/routes.py` & `api_inference_community-0.0.9/api_inference_community/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import base64
 import logging
 import os
 import time
-import base64
 from typing import Any, Dict
 
 from api_inference_community.validation import ffmpeg_convert, normalize_payload
 from pydantic import ValidationError
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
 
@@ -96,15 +96,21 @@
             return Response(data, headers=headers, status_code=status_code)
         elif task == "audio-to-audio":
             waveforms, sampling_rate, labels = outputs
             items = []
             headers["content-type"] = "application/json"
             for waveform, label in zip(waveforms, labels):
                 data = ffmpeg_convert(waveform, sampling_rate)
-                items.append({"label": label, "blob": base64.b64encode(data).decode("utf-8"), "content-type": "audio/flac"})
+                items.append(
+                    {
+                        "label": label,
+                        "blob": base64.b64encode(data).decode("utf-8"),
+                        "content-type": "audio/flac",
+                    }
+                )
             return JSONResponse(items, headers=headers, status_code=status_code)
 
     return JSONResponse(
         outputs,
         headers=headers,
         status_code=status_code,
     )
```

### Comparing `api_inference_community-0.0.8/api_inference_community/validation.py` & `api_inference_community-0.0.9/api_inference_community/validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,14 +128,26 @@
         rows = list(table.values())
         n = len(rows[0])
         if all(len(x) == n for x in rows):
             return table
         raise ValueError("All rows in the table must be the same length")
 
 
+class StructuredDataClassificationInputsCheck(BaseModel):
+    data: Dict[str, List[str]]
+
+    @validator("data")
+    def all_rows_must_have_same_length(cls, data: Dict[str, List[str]]):
+        rows = list(data.values())
+        n = len(rows[0])
+        if all(len(x) == n for x in rows):
+            return data
+        raise ValueError("All rows in the data must be the same length")
+
+
 class StringOrStringBatchInputCheck(BaseModel):
     __root__: Union[List[str], str]
 
     @validator("__root__")
     def input_must_not_be_empty(cls, __root__: Union[List[str], str]):
         if isinstance(__root__, list):
             if len(__root__) == 0:
@@ -160,22 +172,24 @@
 
 INPUTS_MAPPING = {
     "conversational": ConversationalInputsCheck,
     "question-answering": QuestionInputsCheck,
     "feature-extraction": StringOrStringBatchInputCheck,
     "sentence-similarity": SentenceSimilarityInputsCheck,
     "table-question-answering": TableQuestionAnsweringInputsCheck,
+    "structured-data-classification": StructuredDataClassificationInputsCheck,
     "fill-mask": StringInput,
     "summarization": StringInput,
     "text2text-generation": StringInput,
     "text-generation": StringInput,
     "text-classification": StringInput,
     "token-classification": StringInput,
     "translation": StringInput,
     "zero-shot-classification": StringInput,
+    "text-to-speech": StringInput,
 }
 
 BATCH_ENABLED_PIPELINES = ["feature-extraction"]
 
 
 def check_params(params, tag):
     if tag in PARAMS_MAPPING:
```

### Comparing `api_inference_community-0.0.8/setup.py` & `api_inference_community-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="api_inference_community",
-    version="0.0.8",
+    version="0.0.9",
     description="A package with helper tools to build an API Inference docker app for Hugging Face API inference using huggingface_hub",
     url="http://github.com/huggingface/api-inference-community",
     author="Nicolas Patry",
     author_email="nicolas@huggingface.co",
     license="MIT",
     packages=["api_inference_community"],
     python_requires=">=3.6.0",
```

