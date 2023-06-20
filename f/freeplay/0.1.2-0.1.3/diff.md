# Comparing `tmp/freeplay-0.1.2.tar.gz` & `tmp/freeplay-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.2.tar", max compression
+gzip compressed data, was "freeplay-0.1.3.tar", max compression
```

## Comparing `freeplay-0.1.2.tar` & `freeplay-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.2/README.md
--rw-r--r--   0        0        0       62 2023-05-18 23:25:20.631072 freeplay-0.1.2/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.2/freeplay/api_support.py
--rw-r--r--   0        0        0     3107 2023-05-26 16:05:17.190253 freeplay-0.1.2/freeplay/freeplay.py
--rw-r--r--   0        0        0    15646 2023-06-13 17:35:43.716269 freeplay-0.1.2/freeplay/freeplay_encapsulated.py
--rw-r--r--   0        0        0      391 2023-06-13 17:37:00.131493 freeplay-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.3/README.md
+-rw-r--r--   0        0        0       62 2023-05-18 23:25:20.631072 freeplay-0.1.3/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.3/freeplay/api_support.py
+-rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.3/freeplay/errors.py
+-rw-r--r--   0        0        0     3107 2023-05-26 16:05:17.190253 freeplay-0.1.3/freeplay/freeplay.py
+-rw-r--r--   0        0        0    16543 2023-06-16 16:10:27.584703 freeplay-0.1.3/freeplay/freeplay_encapsulated.py
+-rw-r--r--   0        0        0      391 2023-06-20 19:15:43.760617 freeplay-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.3/PKG-INFO
```

### Comparing `freeplay-0.1.2/freeplay/api_support.py` & `freeplay-0.1.3/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.2/freeplay/freeplay.py` & `freeplay-0.1.3/freeplay/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.2/freeplay/freeplay_encapsulated.py` & `freeplay-0.1.3/freeplay/freeplay_encapsulated.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
+import logging
 import time
 from abc import abstractmethod, ABC
 from dataclasses import dataclass
-from typing import Optional, Generator
+from typing import Optional, Generator, Any, cast
 
 import anthropic  # type: ignore
 import openai
 
 from . import api_support
+from .errors import TemplateNotFoundError, APIKeyMissingError, AuthorizationError, FreeplayError
 
+JsonDom = dict[str, Any]
+
+logger = logging.getLogger(__name__)
 
 @dataclass
 class CompletionResponse:
     content: str
     is_complete: bool
 
 
-# This is used to map the templates coming back from the create session call.
-# We don't use this because it has the encoded metadata in the content. See
-# the PromptTemplateWithMetadata which maps the templates from the specific
-# get prompt templates API call.
 @dataclass
 class PromptTemplate:
     name: str
     content: str
 
 
 @dataclass
@@ -36,20 +37,14 @@
 
 @dataclass
 class PromptTemplates:
     templates: list[PromptTemplateWithMetadata]
 
 
 @dataclass
-class ProjectSession:
-    session_id: str
-    prompt_templates: list[PromptTemplate]
-
-
-@dataclass
 class CompletionChunk:
     text: str
     is_complete: bool
 
 
 class Flavor(ABC):
     @property
@@ -79,27 +74,35 @@
             if parameter_key in kwargs:
                 model_params[parameter_key] = kwargs[parameter_key]
             else:
                 model_params[parameter_key] = default_value
         return model_params
 
 
-class OpenAIText(Flavor):
-    record_format_type = "openai_text"
-    _model_params_with_defaults = {
-        "model": "text-davinci-003"
-    }
-
+class OpenAI(Flavor, ABC):
     def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
         super().__init__()
         if openai_api_base:
             openai.api_base = openai_api_base
 
+        if not openai_api_key or not openai_api_key.strip():
+            raise APIKeyMissingError("OpenAI API key not set. It must be set to make calls to the service.")
+
         openai.api_key = openai_api_key
 
+
+class OpenAIText(OpenAI):
+    record_format_type = "openai_text"
+    _model_params_with_defaults = {
+        "model": "text-davinci-003"
+    }
+
+    def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
+        super().__init__(openai_api_key, openai_api_base)
+
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         return prompt_template.content.format(**variables)
 
     def call_service(self, formatted_prompt: str, **kwargs: str) -> Optional[CompletionResponse]:
         completion = openai.Completion.create(
             prompt=formatted_prompt,
             **self._get_model_params(**kwargs)
@@ -123,26 +126,22 @@
         for chunk in completion:
             yield CompletionChunk(
                 text=chunk.choices[0].text,
                 is_complete=chunk.choices[0].finish_reason == "stop"
             )
 
 
-class OpenAIChat(Flavor):
+class OpenAIChat(OpenAI):
     record_format_type = "openai_chat"
     _model_params_with_defaults = {
         "model": "gpt-3.5-turbo"
     }
 
     def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
-        super().__init__()
-        if openai_api_base:
-            openai.api_base = openai_api_base
-
-        openai.api_key = openai_api_key
+        super().__init__(openai_api_key, openai_api_base)
 
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         # Extract messages JSON to enable formatting of individual content fields of each message. If we do not
         # extract the JSON, current variable interpolation will fail on JSON curly braces.
         messages_as_json = json.loads(prompt_template.content)
         formatted_messages = [
             {"content": message['content'].format(**variables), "role": message['role']} for message in
@@ -240,20 +239,24 @@
             **kwargs: str
     ) -> None:
         self.api_base = api_base
         self.freeplay_api_key = freeplay_api_key
         self.flavor = flavor
         self.extra_init_args = kwargs
 
-    def create_session(self, project_id: str) -> ProjectSession:
-        return api_support.post(
-            target_type=ProjectSession,
-            api_key=self.freeplay_api_key,
-            url=f'{self.api_base}/projects/{project_id}/sessions/tag/latest'
-        )
+    def create_session(self, project_id: str) -> JsonDom:
+        response = api_support.post_raw(api_key=self.freeplay_api_key,
+                                        url=f'{self.api_base}/projects/{project_id}/sessions/tag/latest')
+
+        if response.status_code == 201:
+            return cast(dict[str, Any], json.loads(response.content))
+        elif response.status_code == 401:
+            raise AuthorizationError()
+        else:
+            raise FreeplayError(f'Unknown response while creating a session. Response code: {response.status_code}')
 
     def get_prompts(self, project_id: str) -> PromptTemplates:
         prompts = api_support.get(
             target_type=PromptTemplates,
             api_key=self.freeplay_api_key,
             url=f'{self.api_base}/projects/{project_id}/templates/all/latest'
         )
@@ -265,21 +268,24 @@
             prompts: PromptTemplates,
             template_name: str,
             variables: dict[str, str]
     ) -> Optional[CompletionResponse]:
         # format prompt
         templates = [t for t in prompts.templates if t.name == template_name]
         if len(templates) == 0:
-            return None
+            raise TemplateNotFoundError(f'Could not find template with name "{template_name}"')
         target_template = templates[0]
         formatted_prompt = self.flavor.format(target_template, variables)
 
         # make call
         start = int(time.time())
-        completion_response = self.flavor.call_service(formatted_prompt=formatted_prompt, **self.extra_init_args)
+        try:
+            completion_response = self.flavor.call_service(formatted_prompt=formatted_prompt, **self.extra_init_args)
+        except Exception as e:
+            raise FreeplayError("Error calling service") from e
         end = int(time.time())
 
         return_content = completion_response.content if completion_response else ""
         is_complete = completion_response.is_complete if completion_response else False
 
         # record data
         self.__record_call(
@@ -300,15 +306,15 @@
             prompts: PromptTemplates,
             template_name: str,
             variables: dict[str, str]
     ) -> Generator[CompletionChunk, None, None]:
         # format prompt
         templates = [t for t in prompts.templates if t.name == template_name]
         if len(templates) == 0:
-            return None
+            raise TemplateNotFoundError(f'Could not find template with name "{template_name}"')
         target_template = templates[0]
         formatted_prompt = self.flavor.format(target_template, variables)
 
         # make call
         start = int(time.time())
         completion_response = self.flavor.call_service_stream(formatted_prompt=formatted_prompt,
                                                               **self.extra_init_args)
@@ -350,19 +356,23 @@
             "tag": "",
             "inputs": variables,
             "prompt_content": formatted_prompt,
             "return_content": completion_content,
             "format_type": self.flavor.record_format_type,
             "is_complete": completion_is_complete
         }
-        _recorded_response = api_support.post_raw(
-            api_key=self.freeplay_api_key,
-            url=f'{self.api_base}/v1/record',
-            payload=record_payload
-        )
+
+        try:
+            _recorded_response = api_support.post_raw(
+                api_key=self.freeplay_api_key,
+                url=f'{self.api_base}/v1/record',
+                payload=record_payload
+            )
+        except Exception:
+            logger.warning(f'There was an error recording to FreePlay. Session will not be logged.')
 
 
 class Session:
     def __init__(
             self,
             call_support: CallSupport,
             session_id: str,
@@ -395,50 +405,52 @@
 
 # This SDK prototype does not support full functionality of either OpenAI's API or Freeplay's
 # The simplifications are:
 #  - Always assumes there is a single choice returned, does not support multiple
 #  - Always uses the 'latest' tag for project versions. Doesn't support configurable tags
 #  - Does not support recording a tag from a call
 #  - Does not support an "escape hatch" to allow use of features we don't explicitly expose
-#  - Error handling is poor--returns None with no further information
 class Freeplay:
     def __init__(
             self,
             flavor: Flavor,
             freeplay_api_key: str,
             api_base: str,
             **kwargs: str
     ) -> None:
+        if not freeplay_api_key or not freeplay_api_key.strip():
+            raise APIKeyMissingError("Freeplay API key not set. It must be set to the Freeplay API.")
+
         self.call_support = CallSupport(flavor, freeplay_api_key, api_base, **kwargs)
 
     def create_session(self, project_id: str) -> Session:
         project_session = self.call_support.create_session(project_id)
         prompts = self.call_support.get_prompts(project_id)
-        return Session(self.call_support, project_session.session_id, prompts)
+        return Session(self.call_support, project_session['session_id'], prompts)
 
     def get_completion(
             self,
             project_id: str,
             template_name: str,
             variables: dict[str, str]
     ) -> Optional[CompletionResponse]:
         project_session = self.call_support.create_session(project_id)
         prompts = self.call_support.get_prompts(project_id)
 
-        return self.call_support.prepare_and_make_call(project_session.session_id,
+        return self.call_support.prepare_and_make_call(project_session['session_id'],
                                                        prompts,
                                                        template_name,
                                                        variables)
 
     def get_completion_stream(
             self,
             project_id: str,
             template_name: str,
             variables: dict[str, str]
     ) -> Generator[CompletionChunk, None, None]:
         project_session = self.call_support.create_session(project_id)
         prompts = self.call_support.get_prompts(project_id)
 
-        return self.call_support.prepare_and_make_call_stream(project_session.session_id,
+        return self.call_support.prepare_and_make_call_stream(project_session['session_id'],
                                                               prompts,
                                                               template_name,
                                                               variables)
```

### Comparing `freeplay-0.1.2/PKG-INFO` & `freeplay-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

