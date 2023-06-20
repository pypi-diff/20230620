# Comparing `tmp/langchain_wenxin-0.5.0.tar.gz` & `tmp/langchain_wenxin-0.6.0.tar.gz`

## Comparing `langchain_wenxin-0.5.0.tar` & `langchain_wenxin-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,18 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/README.md
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 langchain_wenxin-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/chat_models.py
+-rw-r--r--   0        0        0    17115 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/chat_models/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/chat_models/test_wenxin.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/llms/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/integration_tests/llms/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/tools/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/tests/tools/test_callbacks.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/README.md
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 langchain_wenxin-0.6.0/PKG-INFO
```

### Comparing `langchain_wenxin-0.5.0/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.6.0/src/langchain_wenxin/llms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 """Wrapper around Baidu Wenxin APIs."""
 import json
 import logging
 import time
 import warnings
 from typing import Any, Dict, Generator, List, Mapping, Optional, Tuple
 
+import aiohttp
 import requests
 import sseclient
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
-from langchain.chat_models.base import BaseChatModel
 from langchain.llms.base import LLM
-from langchain.schema import (
-    AIMessage,
-    BaseMessage,
-    ChatGeneration,
-    ChatResult,
-    HumanMessage,
-)
 from langchain.utils import get_from_dict_or_env
 from pydantic import BaseModel, Extra, root_validator
 
 logger = logging.getLogger(__name__)
 
 
 class WenxinClient():
@@ -63,23 +56,116 @@
         )
         r.raise_for_status()
         response = r.json()
         self.access_token = response["access_token"]
         self.access_token_expires = now_timestamp + response["expires_in"]
         return self.access_token
 
+    async def async_grant_token(self) -> str:
+        """Async grant access token from Baidu Cloud."""
+        now_timestamp = int(time.time())
+        if self.access_token and now_timestamp < self.access_token_expires:
+            return self.access_token
+
+        # Here we are using aiohttp to make the request.
+        # It is used in a context manager fashion to ensure cleanup.
+        async with aiohttp.ClientSession() as session:
+            async with session.get(
+                url=self.WENXIN_TOKEN_URL,
+                params={
+                    "grant_type": "client_credentials",
+                    "client_id": self.baidu_api_key,
+                    "client_secret": self.baidu_secret_key,
+                },
+                timeout=5,
+            ) as r:
+                r.raise_for_status()
+                response = await r.json()
+
+        self.access_token = response["access_token"]
+        self.access_token_expires = now_timestamp + response["expires_in"]
+        return self.access_token
+
     @staticmethod
     def construct_message(prompt: str, history: List[Tuple[str, str]]) -> List[Any]:
         messages = []
         for human, ai in history:
             messages.append({"role": "user", "content": human})
             messages.append({"role": "assistant", "content": ai})
         messages.append({"role": "user", "content": prompt})
         return messages
 
+    def completion(self, model: str, prompt: str, history: List[Tuple[str, str]], **params) -> Any:
+        """Call out to Wenxin's generate endpoint.
+
+        Args:
+            model: The model to use.
+            prompt: The prompt to pass into the model.
+            **params: Additional parameters to pass to the API.
+
+        Returns:
+            The response generated by the model.
+        """
+        params["messages"] = self.construct_message(prompt, history)
+        params["stream"] = False
+        url = self.completions_url(model)
+        logger.debug(f"call wenxin: url[{url}], params[{params}]")
+        r = requests.post(
+            url=url,
+            params={"access_token": self.grant_token()},
+            json=params,
+            timeout=self.request_timeout,
+        )
+        r.raise_for_status()
+        response = r.json()
+        error_code = response.get("error_code", 0)
+        if error_code != 0:
+            error_msg = response.get("error_msg", "Unknown error")
+            msg = f"call wenxin failed, error_code: {error_code}, error_msg: {error_msg}"
+            raise Exception(msg)
+
+        return response
+
+    async def acompletion(self, model: str, prompt: str, history: List[Tuple[str, str]], **params) -> Any:
+        """Async all out to Wenxin's generate endpoint.
+
+        Args:
+            model: The model to use.
+            prompt: The prompt to pass into the model.
+            **params: Additional parameters to pass to the API.
+
+        Returns:
+            The response generated by the model.
+        """
+        import aiohttp
+        params["messages"] = self.construct_message(prompt, history)
+        params["stream"] = False
+        url = self.completions_url(model)
+        logger.debug(f"async call wenxin: url[{url}], params[{params}]")
+
+        # Here we are using aiohttp to make the request.
+        # It is used in a context manager fashion to ensure cleanup.
+        async with aiohttp.ClientSession() as session:
+            async with session.post(
+                url=url,
+                params={"access_token": await self.async_grant_token()},
+                json=params,
+                timeout=self.request_timeout,
+            ) as r:
+                r.raise_for_status()
+                response = await r.json()
+
+        error_code = response.get("error_code", 0)
+        if error_code != 0:
+            error_msg = response.get("error_msg", "Unknown error")
+            msg = f"call wenxin failed, error_code: {error_code}, error_msg: {error_msg}"
+            raise Exception(msg)
+
+        return response
+
     def completion_stream(self, model: str, prompt: str,
                           history: List[Tuple[str, str]], **params) -> Generator:
         """Call out to Wenxin's generate endpoint.
 
         Args:
             model: The model to use.
             prompt: The prompt to pass into the model.
@@ -110,44 +196,65 @@
             return response
 
         client = sseclient.SSEClient(r)
         for event in client.events():
             data = json.loads(event.data)
             yield data
 
-    def completion(self, model: str, prompt: str, history: List[Tuple[str, str]], **params) -> Any:
-        """Call out to Wenxin's generate endpoint.
+    async def acompletion_stream(self, model: str, prompt: str,
+                          history: List[Tuple[str, str]], **params) -> Generator:
+        """Async call out to Wenxin's generate endpoint.
 
         Args:
             model: The model to use.
             prompt: The prompt to pass into the model.
             **params: Additional parameters to pass to the API.
 
         Returns:
-            The response generated by the model.
+            Generator: The response generated by the model.
         """
         params["messages"] = self.construct_message(prompt, history)
-        params["stream"] = False
+        params["stream"] = True
         url = self.completions_url(model)
         logger.debug(f"call wenxin: url[{url}], params[{params}]")
-        r = requests.post(
-            url=url,
-            params={"access_token": self.grant_token()},
-            json=params,
-            timeout=self.request_timeout,
-        )
-        r.raise_for_status()
-        response = r.json()
-        error_code = response.get("error_code", 0)
-        if error_code != 0:
-            error_msg = response.get("error_msg", "Unknown error")
-            msg = f"call wenxin failed, error_code: {error_code}, error_msg: {error_msg}"
-            raise Exception(msg)
 
-        return response
+        timeout = aiohttp.ClientTimeout(total=self.request_timeout)
+        async with aiohttp.ClientSession(timeout=timeout) as session:
+            async with session.post(
+                url=self.completions_url(model),
+                params={"access_token": await self.async_grant_token()},
+                json=params,
+            ) as r:
+                r.raise_for_status()
+                if not r.headers.get("Content-Type").startswith("text/event-stream"):
+                    response = await r.json()
+                    error_code = response.get("error_code", 0)
+                    if error_code != 0:
+                        error_msg = response.get("error_msg", "Unknown error")
+                        msg = f"call wenxin failed, error_code: {error_code}, error_msg: {error_msg}"
+                        raise Exception(msg)
+                    yield response
+
+                async def read(content):
+                    data = b""
+                    async for chunk in content:
+                        data += chunk
+                        if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                            yield data
+                            data = b""
+                    if data:
+                        yield data
+
+                async for line in read(r.content):
+                    line_decoded = line.decode("utf-8")
+                    if not line_decoded.startswith("data:"):
+                        continue
+                    event_data = line_decoded[5:].strip()
+                    data = json.loads(event_data)
+                    yield data
 
 
 class BaiduCommon(BaseModel):
     client: Any = None  #: :meta private:
     model: str = "ernie-bot"
     """Model name to use. supported models: ernie-bot(wenxin)/ernie-bot-turbo(eb-instant)"""
 
@@ -258,14 +365,15 @@
         return "wenxin-llm"
 
     def _call(
         self,
         prompt: str,
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
+        **kwargs: Any,
     ) -> str:
         r"""Call out to Baidu Wenxin's completion endpoint.
 
         Args:
             prompt: The prompt to pass into the model.
             stop: Optional list of stop words to use when generating (not used.).
 
@@ -275,33 +383,65 @@
         Example:
             .. code-block:: python
 
                 prompt = "What are the biggest risks facing humanity?"
                 response = model(prompt)
 
         """
+        params = {**self._default_params, **kwargs}
         if self.streaming:
             stream_resp = self.client.completion_stream(
                 model=self.model,
                 prompt=prompt,
                 history=[],
-                **self._default_params,
+                **params,
             )
             current_completion = ""
             for data in stream_resp:
                 result = data["result"]
                 if run_manager:
-                    run_manager.on_llm_new_token(result)
+                    run_manager.on_llm_new_token(result, **data)
                 current_completion += result
             return current_completion
         response = self.client.completion(
             model=self.model,
             prompt=prompt,
             history=[],
-            **self._default_params,
+            **params,
+        )
+        return response["result"]
+
+    async def _acall(
+        self,
+        prompt: str,
+        stop: Optional[List[str]] = None,
+        run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
+        **kwargs: Any,
+    ) -> str:
+        """Call out to Wenxin's completion endpoint asynchronously."""
+        params = {**self._default_params, **kwargs}
+        if self.streaming:
+            stream_resp = self.client.acompletion_stream(
+                model=self.model,
+                prompt=prompt,
+                history=[],
+                **params,
+            )
+            current_completion = ""
+            async for data in stream_resp:
+                delta = data["result"]
+                current_completion += delta
+                if run_manager:
+                    await run_manager.on_llm_new_token(delta, **data)
+            return current_completion
+        response = await self.client.acompletion(
+            model=self.model,
+            prompt=prompt,
+            history=[],
+            **params,
         )
         return response["result"]
 
     def stream(self, prompt: str, stop: Optional[List[str]] = None) -> Generator:
         r"""Call Baidu Wenxin completion_stream and return the resulting generator.
 
         BETA: this is a beta feature while we figure out the right abstraction.
@@ -319,109 +459,12 @@
 
 
                 prompt = "Write a poem about a stream."
                 generator = wenxin.stream(prompt)
                 for token in generator:
                     yield token
         """
-        for r in self.client.completion_stream(
+        return self.client.completion_stream(
+            model=self.model,
             prompt=prompt,
             history=[],
-            **self._default_params):
-            yield r["result"]
-
-
-class ChatWenxin(BaseChatModel, BaiduCommon):
-    r"""Wrapper around Baidu Wenxin's large language model.
-
-    To use, you should have the ``requests`` python package installed, and the
-    environment variable ``BAIDU_API_KEY`` and ``BAIDU_SECRET_KEY``, or pass
-    it as a named parameter to the constructor.
-
-    Example:
-        .. code-block:: python
-            from langchain_wenxin.llms import ChatWenxin
-            model = ChatWenxin(model="wenxin", baidu_api_key="my-api-key",
-                           baidu_secret_key="my-secret-key")
-
-            # Simplest invocation:
-            response = model("What are the biggest risks facing humanity?")
-    """
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-
-    @property
-    def _llm_type(self) -> str:
-        """Return type of chat model."""
-        return "wenxin-chat"
-
-    def _convert_messages_to_prompt(
-            self, messages: List[BaseMessage]) -> Tuple[str, List[Tuple[str, str]]]:
-        """Format a list of messages into prompt and history.
-
-        Args:
-            messages (List[BaseMessage]): List of BaseMessage to combine.
-
-        Returns:
-            str: Prompt
-            List[Tuple[str, str]]: History
-        """
-        history = []
-        pair = [None, None]
-        order_error = "It must be in the order of user, assistant."
-        last_message_error = "The last message must be a human message."
-        for message in messages[:-1]:
-            if message.type == "system":
-                history.append((message.content, "OK\n"))
-            if pair[0] is None:
-                if message.type == "human":
-                    pair[0] = message.content
-                else:
-                    raise ValueError(order_error)
-            elif message.type == "ai":
-                pair[1] = message.content
-                history.append(tuple(pair))
-                pair = [None, None]
-            else:
-                raise ValueError(order_error)
-        if not isinstance(messages[-1], HumanMessage):
-            raise ValueError(last_message_error)
-        return messages[-1].content, history
-
-    def _generate(
-        self,
-        messages: List[BaseMessage],
-        stop: Optional[List[str]] = None,
-        run_manager: Optional[CallbackManagerForLLMRun] = None,
-    ) -> ChatResult:
-        prompt, history = self._convert_messages_to_prompt(messages)
-        params: Dict[str, Any] = {"prompt": prompt,
-                                  "history": history, **self._default_params}
-
-        if self.streaming:
-            completion = ""
-            stream_resp = self.client.completion_stream(**params)
-            for delta in stream_resp:
-                result = delta["result"]
-                completion += result
-                if run_manager:
-                    run_manager.on_llm_new_token(
-                        result,
-                    )
-        else:
-            response = self.client.completion(**params)
-            completion = response
-        message = AIMessage(content=completion)
-        return ChatResult(generations=[ChatGeneration(message=message)])
-
-    async def _agenerate(
-        self,
-        messages: List[BaseMessage],
-        stop: Optional[List[str]] = None,
-        run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
-    ) -> ChatResult:
-        async_not_implemented_error = "Async not implemented for Wenxin Chat Model."
-        raise NotImplementedError(async_not_implemented_error)
-
+            **self._default_params)
```

### Comparing `langchain_wenxin-0.5.0/src/langchain_wenxin/retrievers.py` & `langchain_wenxin-0.6.0/src/langchain_wenxin/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.5.0/.gitignore` & `langchain_wenxin-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.5.0/LICENSE.txt` & `langchain_wenxin-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.5.0/README.md` & `langchain_wenxin-0.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,29 +24,51 @@
 
 ```bash
 export BAIDU_API_KEY="xxxxx"                            
 export BAIDU_SECRET_KEY="xxxxx"
 ```
 
 ```python3
-from langchain_wenxin.llms import Wenxin,ChatWenxin
+from langchain_wenxin.llms import Wenxin
 
 # Wenxin model
 llm = Wenxin(model="ernie-bot-turbo")
 print(llm("你好"))
 
+# stream call
+for i in llm.stream("你好"):
+    print(i)
+
+# async call
+import asyncio
+print(asyncio.run(llm._acall("你好")))
+
 # Wenxin chat model
+from langchain_wenxin.chat_models import ChatWenxin
 from langchain.schema import HumanMessage
 llm = ChatWenxin()
 print(llm([HumanMessage(content="你好")]))
 ```
 
 Support models:
 
-- ernie-bot: 标准模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
+- ernie-bot: Standard model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
     - Also named `wenxin` for compatibility.
-- ernie-bot-turbo: 快速模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
+- ernie-bot-turbo: Fast model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
     - Also named `eb-instant` for compatibility.
 
+## Development
+
+```bash
+# Create virtual environment
+hatch env create
+# Activate virtual environment
+hatch shell
+# Run test
+export BAIDU_API_KEY="xxxxxxxx"
+export BAIDU_SECRET_KEY="xxxxxxxx"
+hatch run test
+```
+
 ## License
 
 `langchain-wenxin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `langchain_wenxin-0.5.0/pyproject.toml` & `langchain_wenxin-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,28 +25,30 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "langchain>=0.0.175",
   "requests",
   "sseclient-py",
   "numpy",
+  "aiohttp",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/langchain-wenxin#readme"
 Issues = "https://github.com/unknown/langchain-wenxin/issues"
 Source = "https://github.com/unknown/langchain-wenxin"
 
 [tool.hatch.version]
 path = "src/langchain_wenxin/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "pytest-asyncio",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `langchain_wenxin-0.5.0/PKG-INFO` & `langchain_wenxin-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.5.0
+Version: 0.6.0
 Project-URL: Documentation, https://github.com/unknown/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/unknown/langchain-wenxin/issues
 Project-URL: Source, https://github.com/unknown/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: aiohttp
 Requires-Dist: langchain>=0.0.175
 Requires-Dist: numpy
 Requires-Dist: requests
 Requires-Dist: sseclient-py
 Description-Content-Type: text/markdown
 
 # langchain-wenxin - Langchain Baidu WENXINWORKSHOP wrapper
@@ -49,29 +50,51 @@
 
 ```bash
 export BAIDU_API_KEY="xxxxx"                            
 export BAIDU_SECRET_KEY="xxxxx"
 ```
 
 ```python3
-from langchain_wenxin.llms import Wenxin,ChatWenxin
+from langchain_wenxin.llms import Wenxin
 
 # Wenxin model
 llm = Wenxin(model="ernie-bot-turbo")
 print(llm("你好"))
 
+# stream call
+for i in llm.stream("你好"):
+    print(i)
+
+# async call
+import asyncio
+print(asyncio.run(llm._acall("你好")))
+
 # Wenxin chat model
+from langchain_wenxin.chat_models import ChatWenxin
 from langchain.schema import HumanMessage
 llm = ChatWenxin()
 print(llm([HumanMessage(content="你好")]))
 ```
 
 Support models:
 
-- ernie-bot: 标准模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
+- ernie-bot: Standard model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
     - Also named `wenxin` for compatibility.
-- ernie-bot-turbo: 快速模型，<https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
+- ernie-bot-turbo: Fast model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
     - Also named `eb-instant` for compatibility.
 
+## Development
+
+```bash
+# Create virtual environment
+hatch env create
+# Activate virtual environment
+hatch shell
+# Run test
+export BAIDU_API_KEY="xxxxxxxx"
+export BAIDU_SECRET_KEY="xxxxxxxx"
+hatch run test
+```
+
 ## License
 
 `langchain-wenxin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

