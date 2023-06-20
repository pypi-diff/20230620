# Comparing `tmp/dashscope-1.2.0-py3-none-any.whl.zip` & `tmp/dashscope-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,47 +1,49 @@
-Zip file size: 53720 bytes, number of entries: 45
--rw-r--r--  2.0 unx      990 b- defN 23-May-30 06:21 dashscope/__init__.py
+Zip file size: 56147 bytes, number of entries: 47
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jun-20 06:30 dashscope/__init__.py
 -rw-r--r--  2.0 unx    13474 b- defN 23-May-16 06:21 dashscope/cli.py
 -rw-r--r--  2.0 unx     3445 b- defN 23-Mar-30 08:43 dashscope/deployment.py
 -rw-r--r--  2.0 unx     3753 b- defN 23-Mar-30 08:43 dashscope/file.py
 -rw-r--r--  2.0 unx     4808 b- defN 23-Mar-30 08:43 dashscope/finetune.py
 -rw-r--r--  2.0 unx     1696 b- defN 23-Mar-30 08:43 dashscope/model.py
--rw-r--r--  2.0 unx       22 b- defN 23-May-31 02:36 dashscope/version.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-20 10:39 dashscope/version.py
 -rw-r--r--  2.0 unx      239 b- defN 23-May-16 06:21 dashscope/aigc/__init__.py
 -rw-r--r--  2.0 unx     8844 b- defN 23-May-17 12:24 dashscope/aigc/conversation.py
 -rw-r--r--  2.0 unx     5064 b- defN 23-May-17 12:24 dashscope/aigc/generation.py
 -rw-r--r--  2.0 unx     7669 b- defN 23-May-16 06:21 dashscope/aigc/image_synthesis.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/api_entities/__init__.py
 -rw-r--r--  2.0 unx    10361 b- defN 23-Apr-06 08:21 dashscope/api_entities/aiohttp_request.py
 -rw-r--r--  2.0 unx     5331 b- defN 23-May-30 06:21 dashscope/api_entities/api_request_data.py
 -rw-r--r--  2.0 unx     4057 b- defN 23-Apr-06 03:24 dashscope/api_entities/api_request_factory.py
 -rw-r--r--  2.0 unx      928 b- defN 23-May-24 01:18 dashscope/api_entities/base_request.py
--rw-r--r--  2.0 unx     8130 b- defN 23-May-16 06:21 dashscope/api_entities/dashscope_response.py
--rw-r--r--  2.0 unx     9457 b- defN 23-May-16 06:21 dashscope/api_entities/http_request.py
+-rw-r--r--  2.0 unx     9654 b- defN 23-Jun-20 06:30 dashscope/api_entities/dashscope_response.py
+-rw-r--r--  2.0 unx     9456 b- defN 23-Jun-20 06:30 dashscope/api_entities/http_request.py
 -rw-r--r--  2.0 unx     8798 b- defN 23-Apr-05 03:15 dashscope/api_entities/sync_http_request.py
 -rw-r--r--  2.0 unx    15705 b- defN 23-May-16 06:21 dashscope/api_entities/websocket_request.py
--rw-r--r--  2.0 unx       35 b- defN 23-Mar-23 09:23 dashscope/audio/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-20 06:30 dashscope/audio/__init__.py
 -rw-r--r--  2.0 unx       75 b- defN 23-Apr-04 06:54 dashscope/audio/asr/__init__.py
 -rw-r--r--  2.0 unx     6946 b- defN 23-Apr-04 01:24 dashscope/audio/asr/transcribe.py
 -rw-r--r--  2.0 unx     5103 b- defN 23-Apr-10 06:30 dashscope/audio/asr/transcription.py
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-20 06:30 dashscope/audio/tts/__init__.py
+-rw-r--r--  2.0 unx     7425 b- defN 23-Jun-20 06:30 dashscope/audio/tts/speech_synthesizer.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/client/__init__.py
--rw-r--r--  2.0 unx    25911 b- defN 23-May-16 06:21 dashscope/client/base_api.py
+-rw-r--r--  2.0 unx    25911 b- defN 23-Jun-20 06:30 dashscope/client/base_api.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/common/__init__.py
 -rw-r--r--  2.0 unx     1986 b- defN 23-Mar-23 09:23 dashscope/common/api_key.py
 -rw-r--r--  2.0 unx     2249 b- defN 23-May-30 06:21 dashscope/common/constants.py
 -rw-r--r--  2.0 unx      869 b- defN 23-Apr-10 12:54 dashscope/common/env.py
 -rw-r--r--  2.0 unx     1592 b- defN 23-May-16 06:21 dashscope/common/error.py
 -rw-r--r--  2.0 unx      984 b- defN 23-Mar-23 09:23 dashscope/common/logging.py
 -rw-r--r--  2.0 unx     4038 b- defN 23-May-16 06:21 dashscope/common/utils.py
 -rw-r--r--  2.0 unx       69 b- defN 23-May-30 06:21 dashscope/embeddings/__init__.py
 -rw-r--r--  2.0 unx     1666 b- defN 23-May-30 06:21 dashscope/embeddings/text_embedding.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/io/__init__.py
 -rw-r--r--  2.0 unx     3941 b- defN 23-May-30 06:21 dashscope/io/input_output.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/protocol/__init__.py
 -rw-r--r--  2.0 unx      561 b- defN 23-Mar-23 09:23 dashscope/protocol/websocket.py
--rw-r--r--  2.0 unx    11413 b- defN 23-May-31 02:36 dashscope-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7201 b- defN 23-May-31 02:36 dashscope-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 02:36 dashscope-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-May-31 02:36 dashscope-1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-31 02:36 dashscope-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3863 b- defN 23-May-31 02:36 dashscope-1.2.0.dist-info/RECORD
-45 files, 191425 bytes uncompressed, 47514 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx    11413 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7201 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4049 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/RECORD
+47 files, 200904 bytes uncompressed, 49645 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -66,14 +66,20 @@
 
 Filename: dashscope/audio/asr/transcribe.py
 Comment: 
 
 Filename: dashscope/audio/asr/transcription.py
 Comment: 
 
+Filename: dashscope/audio/tts/__init__.py
+Comment: 
+
+Filename: dashscope/audio/tts/speech_synthesizer.py
+Comment: 
+
 Filename: dashscope/client/__init__.py
 Comment: 
 
 Filename: dashscope/client/base_api.py
 Comment: 
 
 Filename: dashscope/common/__init__.py
@@ -111,26 +117,26 @@
 
 Filename: dashscope/protocol/__init__.py
 Comment: 
 
 Filename: dashscope/protocol/websocket.py
 Comment: 
 
-Filename: dashscope-1.2.0.dist-info/LICENSE
+Filename: dashscope-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: dashscope-1.2.0.dist-info/METADATA
+Filename: dashscope-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: dashscope-1.2.0.dist-info/WHEEL
+Filename: dashscope-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: dashscope-1.2.0.dist-info/entry_points.txt
+Filename: dashscope-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: dashscope-1.2.0.dist-info/top_level.txt
+Filename: dashscope-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dashscope-1.2.0.dist-info/RECORD
+Filename: dashscope-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dashscope/__init__.py

```diff
@@ -1,24 +1,38 @@
 import logging
 from logging import NullHandler
 
 from dashscope.aigc.conversation import Conversation, History, HistoryItem
 from dashscope.aigc.generation import Generation
 from dashscope.aigc.image_synthesis import ImageSynthesis
 from dashscope.audio.asr.transcription import Transcription
+from dashscope.audio.tts.speech_synthesizer import SpeechSynthesizer
 from dashscope.common.api_key import save_api_key
 from dashscope.common.env import (api_key, api_key_file_path,
                                   base_http_api_url, base_websocket_api_url)
 from dashscope.deployment import Deployment
 from dashscope.embeddings.text_embedding import TextEmbedding
 from dashscope.file import File
 from dashscope.finetune import FineTune
 from dashscope.model import Model
 
 __all__ = [
-    base_http_api_url, base_websocket_api_url, api_key, api_key_file_path,
-    save_api_key, Conversation, Generation, History, HistoryItem,
-    ImageSynthesis, Transcription, File, Deployment, FineTune, Model,
-    TextEmbedding
+    base_http_api_url,
+    base_websocket_api_url,
+    api_key,
+    api_key_file_path,
+    save_api_key,
+    Conversation,
+    Generation,
+    History,
+    HistoryItem,
+    ImageSynthesis,
+    Transcription,
+    File,
+    Deployment,
+    FineTune,
+    Model,
+    TextEmbedding,
+    SpeechSynthesizer,
 ]
 
 logging.getLogger(__name__).addHandler(NullHandler())
```

## dashscope/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.2.0'
+__version__ = '1.3.0'
```

## dashscope/api_entities/dashscope_response.py

```diff
@@ -1,11 +1,11 @@
 import json
 from dataclasses import dataclass
 from http import HTTPStatus
-from typing import Any, List
+from typing import Any, Dict, List
 
 
 @dataclass(init=False)
 class DictMixin(dict):
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
@@ -188,14 +188,61 @@
             return TranscriptionResponse(status_code=api_response.status_code,
                                          request_id=api_response.request_id,
                                          code=api_response.code,
                                          message=api_response.message)
 
 
 @dataclass(init=False)
+class SpeechSynthesisOutput(DictMixin):
+    sentence: Dict[str, Any]
+
+    def __init__(self, sentence: Dict[str, Any], **kwargs):
+        super().__init__(sentence=sentence, **kwargs)
+
+
+@dataclass(init=False)
+class SpeechSynthesisUsage(DictMixin):
+    characters: int
+
+    def __init__(self, characters: int = 0, **kwargs):
+        super().__init__(characters=characters, **kwargs)
+
+
+@dataclass(init=False)
+class SpeechSynthesisResponse(DashScopeAPIResponse):
+    output: SpeechSynthesisOutput
+    usage: SpeechSynthesisUsage
+
+    @staticmethod
+    def from_api_response(api_response: DashScopeAPIResponse):
+        if api_response.status_code == HTTPStatus.OK:
+            output = None
+            usage = None
+            if api_response.output is not None:
+                output = SpeechSynthesisOutput(**api_response.output)
+            if api_response.usage is not None:
+                usage = SpeechSynthesisUsage(**api_response.usage)
+
+            return SpeechSynthesisResponse(
+                status_code=api_response.status_code,
+                request_id=api_response.request_id,
+                code=api_response.code,
+                message=api_response.message,
+                output=output,
+                usage=usage)
+
+        else:
+            return SpeechSynthesisResponse(
+                status_code=api_response.status_code,
+                request_id=api_response.request_id,
+                code=api_response.code,
+                message=api_response.message)
+
+
+@dataclass(init=False)
 class ImageSynthesisResult(DictMixin):
     url: str
 
     def __init__(self, url: str = '', **kwargs) -> None:
         super().__init__(url=url, **kwargs)
```

## dashscope/api_entities/http_request.py

```diff
@@ -1,12 +1,11 @@
 import json
 from http import HTTPStatus
 
 import requests
-
 from dashscope.api_entities.base_request import BaseRequest
 from dashscope.api_entities.dashscope_response import DashScopeAPIResponse
 from dashscope.common.constants import (DEFAULT_REQUEST_TIMEOUT_SECONDS,
                                         SSE_CONTENT_TYPE, HTTPMethod,
                                         StreamResultMode)
 from dashscope.common.error import UnsupportedHTTPMethod
 from dashscope.common.logging import logger
```

## dashscope/audio/__init__.py

```diff
@@ -1,3 +1,3 @@
-from . import asr
+from . import asr, tts
 
-__all__ = [asr]
+__all__ = [asr, tts]
```

## dashscope/client/base_api.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
 import time
 from http import HTTPStatus
 from typing import List, Union
 
 import aiohttp
-import requests
 
 import dashscope
+import requests
 from dashscope.api_entities.api_request_factory import _build_api_request
 from dashscope.api_entities.dashscope_response import DashScopeAPIResponse
 from dashscope.common.api_key import get_default_api_key
 from dashscope.common.constants import (DEFAULT_REQUEST_TIMEOUT_SECONDS,
                                         REPEATABLE_STATUS, TaskStatus)
 from dashscope.common.error import InvalidParameter, InvalidTask, ModelRequired
 from dashscope.common.logging import logger
```

## Comparing `dashscope-1.2.0.dist-info/LICENSE` & `dashscope-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dashscope-1.2.0.dist-info/METADATA` & `dashscope-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashscope
-Version: 1.2.0
+Version: 1.3.0
 Summary: dashscope client sdk library
 Home-page: https://dashscope.aliyun.com/
 Author: Alibaba
 Author-email: dashscope@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

## Comparing `dashscope-1.2.0.dist-info/RECORD` & `dashscope-1.3.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-dashscope/__init__.py,sha256=Uo6lr2monCnWLUmNEsXIz-VLfAqiDULpVQbyRXPIYEw,990
+dashscope/__init__.py,sha256=OIQFNWbRNTCTCTZZaTR0dw1sR20Bvsrh5krvV_v7B-I,1131
 dashscope/cli.py,sha256=FHz1UGh8dCDBV25FQttJM1uxZT3rNKGDp_krfCel7rY,13474
 dashscope/deployment.py,sha256=OA7FMkFTXwKDTcLLZe57_ZlCk38S29krdijy-_W64G4,3445
 dashscope/file.py,sha256=maMrfMB5_WVltYEyGN4QcAH0Xxj0eHkScisP8AXx4RQ,3753
 dashscope/finetune.py,sha256=jUj43EmwtCDYNqMvjKimuCQigG0Ux2EvZBypGcmkqHg,4808
 dashscope/model.py,sha256=kLXawzbbq4VkFFFjruz06MkuY-uEMUWCqs-4quqV7Us,1696
-dashscope/version.py,sha256=U3f_Jgr3zpgiYG2kLcvcT05TQsVzN9Kktg_f3Q9OZFA,22
+dashscope/version.py,sha256=zi_LaUT_OsChAtsPXbOeRpQkCohSsOyeXfavQPM0GoE,22
 dashscope/aigc/__init__.py,sha256=llQdhMk9N11SKlTSAvYK-E4xT46GcXUAF51I-oDDDMM,239
 dashscope/aigc/conversation.py,sha256=H46NzB7CvCNBVFeD61bG-IBxcdfe3hjenszvI4M0AeY,8844
 dashscope/aigc/generation.py,sha256=LwyYEu-aRZGbXBilaaYQqkk2MF7Ojc1kBl-UU8nOAbI,5064
 dashscope/aigc/image_synthesis.py,sha256=zZhpny20azLinMhhvAgyLY4qHugtl1EEApJQ5vuHNZI,7669
 dashscope/api_entities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dashscope/api_entities/aiohttp_request.py,sha256=LpUM-BGKTHUeBnZ6cOfmdlp4-7czWLkhdNSzS2ydOh0,10361
 dashscope/api_entities/api_request_data.py,sha256=THH0jHQazlmjGId0e8-4aJG5jH71_jMm-CulGCZ6DV4,5331
 dashscope/api_entities/api_request_factory.py,sha256=4COz8WMEJOBP2_7jkW62Rua21SpoyrthCOMT0yg_z_k,4057
 dashscope/api_entities/base_request.py,sha256=y1SmJQ2csMy43y3c66BrC_usfn93XmJyhyu3Ge5aRKI,928
-dashscope/api_entities/dashscope_response.py,sha256=jaBqecBjJz1OqL_8YqfSQ328p1LPHiA4gwugDBUotVA,8130
-dashscope/api_entities/http_request.py,sha256=fP8E54rX2Sz2aiYSAqT9mEiRjtSFSy_-hBnDsfAq3dk,9457
+dashscope/api_entities/dashscope_response.py,sha256=slVvNjW-tu3Di6HNVV4FnZ3dMyS1HiL1CnWrELJS5rs,9654
+dashscope/api_entities/http_request.py,sha256=7_qMWX-stOgci4A-hlv_R88QYOQzHL8VEkLUlFILd7c,9456
 dashscope/api_entities/sync_http_request.py,sha256=Yn1ursuviL5enxs87hraKkUBenQLyiHDV487KKQq5A0,8798
 dashscope/api_entities/websocket_request.py,sha256=dUU6-wRP28IZQDDL_OTytQxpzKwXKMJcCijii06bheI,15705
-dashscope/audio/__init__.py,sha256=b8cHgjJF9VyvYAvEOGJykcQhLGejnOaJd6yXUlp6oH4,35
+dashscope/audio/__init__.py,sha256=vlw0TFVRdeRWfzmJxhzarVUqkMs-DZNf4GiMtm3C8XE,45
 dashscope/audio/asr/__init__.py,sha256=kgQYk8-q7lg64oBD7sRhCuZECvOWswmoA-zRoeU2aqw,75
 dashscope/audio/asr/transcribe.py,sha256=tJYu2u9qdnoTDmv__KIUDZ1u1LEc8mUX78vqacvxMtI,6946
 dashscope/audio/asr/transcription.py,sha256=niqgLGcvpsnv1LR2JFFinN7Gan92CJiMV_DrhfbY9e8,5103
+dashscope/audio/tts/__init__.py,sha256=fbnieZX9yNFNh5BsxLpLXb63jlxzxrdCJakV3ignjlQ,194
+dashscope/audio/tts/speech_synthesizer.py,sha256=wKcpUo6L1yc0OZUajUh0xbtYubTkm-M89IGSAyDwLBo,7425
 dashscope/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dashscope/client/base_api.py,sha256=eAPdh02tsA7AA9ORImQQ7bMAaLe0SNuXJFbYWDoZASM,25911
+dashscope/client/base_api.py,sha256=k9cBZDmJ9et9aXpYckp02MH1hdAMN6TKjk1AsFe-Xfo,25911
 dashscope/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dashscope/common/api_key.py,sha256=5Stp0odL5JSuIO3qJBp23QNppuGbqhhvKPS66qbMs0I,1986
 dashscope/common/constants.py,sha256=4AUIydT7uZqWg0_nB2mGHR1s5LSSYpuC4Tr4wIyW930,2249
 dashscope/common/env.py,sha256=oQOZW5JyEeTSde394un2lpDJ5RBh4fMU9hBfbtrKKkc,869
 dashscope/common/error.py,sha256=zbWWjgBXWFNtyVBMQpjuLhOKN4k5XlyByrHn1yWy4Qc,1592
 dashscope/common/logging.py,sha256=ecGxylG3bWES_Xv5-BD6ep4_0Ciu7F6ZPBjiZtu9Jx4,984
 dashscope/common/utils.py,sha256=F5GOEMIzB2Sh1ohzx_nNgGKe752F92aQQpsaqFh-4nM,4038
 dashscope/embeddings/__init__.py,sha256=InVIZayFfGZq9Q13Mok6c_ocdV3PCFcbxjURBcLYMEg,69
 dashscope/embeddings/text_embedding.py,sha256=nI-d4zcuZA_tpfu7ktI5SZ8V-dGngVclZwxGFAh4qmE,1666
 dashscope/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dashscope/io/input_output.py,sha256=iZ1X1x1btdoZK2VeC9JsKkag2eaXwqfNT3Q6SrmRi2w,3941
 dashscope/protocol/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dashscope/protocol/websocket.py,sha256=z-v6PGx3L4zYBANuC48s7SWSQSwRCDoh0zcfhv9Bf8U,561
-dashscope-1.2.0.dist-info/LICENSE,sha256=Izp5L1DF1Mbza6qojkqNNWlE_mYLnr4rmzx2EBF8YFw,11413
-dashscope-1.2.0.dist-info/METADATA,sha256=x26ZZj80h2i7W-_rYZU5UcVa90A3tdUqHLqZWePTxs0,7201
-dashscope-1.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dashscope-1.2.0.dist-info/entry_points.txt,sha256=raEp5dOuj8whJ7yqZlDM8WQ5p2RfnGrGNo0QLQEnatY,50
-dashscope-1.2.0.dist-info/top_level.txt,sha256=woqavFJK9zas5xTqynmALqOtlafghjsk63Xk86powTU,10
-dashscope-1.2.0.dist-info/RECORD,,
+dashscope-1.3.0.dist-info/LICENSE,sha256=Izp5L1DF1Mbza6qojkqNNWlE_mYLnr4rmzx2EBF8YFw,11413
+dashscope-1.3.0.dist-info/METADATA,sha256=8HX7YB2f0qpcDbW5QhivJfOL5up9hQfpjtJRnBQjVKM,7201
+dashscope-1.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dashscope-1.3.0.dist-info/entry_points.txt,sha256=raEp5dOuj8whJ7yqZlDM8WQ5p2RfnGrGNo0QLQEnatY,50
+dashscope-1.3.0.dist-info/top_level.txt,sha256=woqavFJK9zas5xTqynmALqOtlafghjsk63Xk86powTU,10
+dashscope-1.3.0.dist-info/RECORD,,
```

