# Comparing `tmp/revChatGPT-6.3.4.tar.gz` & `tmp/revChatGPT-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.3.4.tar", last modified: Mon Jun 19 08:42:43 2023, max compression
+gzip compressed data, was "revChatGPT-6.4.0.tar", last modified: Tue Jun 20 05:14:34 2023, max compression
```

## Comparing `revChatGPT-6.3.4.tar` & `revChatGPT-6.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.614160 revChatGPT-6.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-19 08:42:43.000000 revChatGPT-6.3.4/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:42:43.618160 revChatGPT-6.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-19 08:42:14.000000 revChatGPT-6.3.4/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.896348 revChatGPT-6.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.896348 revChatGPT-6.4.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58782 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23882 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 05:14:34.000000 revChatGPT-6.4.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:14:34.900348 revChatGPT-6.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 05:14:02.000000 revChatGPT-6.4.0/tests/test_recipient.py
```

### Comparing `revChatGPT-6.3.4/LICENSE` & `revChatGPT-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.4/PKG-INFO` & `revChatGPT-6.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.4
+Version: 6.4.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.3.4/README.md` & `revChatGPT-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.4/setup.py` & `revChatGPT-6.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="6.3.4",
+    version="6.4.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-6.3.4/src/revChatGPT/V1.py` & `revChatGPT-6.4.0/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from typing import Generator
 from typing import NoReturn
 
 import httpx
 import requests
 from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
-
 from rich.live import Live
 from rich.markdown import Markdown
 
 from . import __version__
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
@@ -203,19 +202,19 @@
         if self.config.get("plugin_ids", []):
             for plugin in self.config.get("plugin_ids"):
                 self.install_plugin(plugin)
         if self.config.get("unverified_plugin_domains", []):
             for domain in self.config.get("unverified_plugin_domains"):
                 if self.config.get("plugin_ids"):
                     self.config["plugin_ids"].append(
-                        self.get_unverified_plugin(domain, install=True).get("id")
+                        self.get_unverified_plugin(domain, install=True).get("id"),
                     )
                 else:
                     self.config["plugin_ids"] = [
-                        self.get_unverified_plugin(domain, install=True).get("id")
+                        self.get_unverified_plugin(domain, install=True).get("id"),
                     ]
 
     @logger(is_timed=True)
     def __check_credentials(self) -> None:
         """Check login info and perform login
 
         Any one of the following is sufficient for login. Multiple login info can be provided at the same time and they will be used in the order listed below.
@@ -364,26 +363,41 @@
             password=self.config.get("password"),
             proxy=self.config.get("proxy"),
         )
         log.debug("Using authenticator to get access token")
 
         self.set_access_token(auth.auth())
 
+    def __arkose_token(self) -> str:
+        headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+        }
+        form_data = "public_key=35536E1E-65B4-4D96-9D97-6ADB7EFF8147&site=https%3A%2F%2Fchat.openai.com&userbrowser=Mozilla%2F5.0%20(X11%3B%20Linux%20x86_64)%20AppleWebKit%2F537.36%20(KHTML%2C%20like%20Gecko)%20Chrome%2F114.0.0.0%20Safari%2F537.36&capi_version=1.5.2&capi_mode=lightbox&style_theme=default&rnd=0.3649022041957759"
+        url = "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147"
+        response = self.session.post(url, data=form_data, headers=headers)
+        self.__check_response(response)
+        return response.json()["token"]
+
     @logger(is_timed=True)
     def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> Generator[dict, None, None]:
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
-        model, message = None, ""
+        message = ""
+
+        if data.get("model", "").startswith("gpt-4"):
+            data["arkose_token"] = self.__arkose_token()
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         response = self.session.post(
             url=f"{self.base_url}conversation",
             data=json.dumps(data),
             timeout=timeout,
@@ -546,18 +560,14 @@
             "action": "next",
             "messages": messages,
             "conversation_id": conversation_id,
             "parent_message_id": parent_id,
             "model": model,
             "history_and_training_disabled": self.disable_history,
         }
-        if model.startswith("gpt-4"):
-            data[
-                "arkose_token"
-            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
 
         yield from self.__send_request(
             data,
             timeout=timeout,
@@ -689,19 +699,14 @@
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
             "history_and_training_disabled": self.disable_history,
         }
-        if model.startswith("gpt-4"):
-            data[
-                "arkose_token"
-            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
-
         yield from self.__send_request(
             data,
             timeout=timeout,
             auto_continue=auto_continue,
         )
 
     @logger(is_timed=False)
@@ -950,26 +955,39 @@
             base_url=base_url,
             lazy_loading=lazy_loading,
         )
 
         # overwrite inherited normal session with async
         self.session = AsyncClient(headers=self.session.headers)
 
+    async def __arkose_token(self) -> str:
+        headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+        }
+        form_data = "public_key=35536E1E-65B4-4D96-9D97-6ADB7EFF8147&site=https%3A%2F%2Fchat.openai.com&userbrowser=Mozilla%2F5.0%20(X11%3B%20Linux%20x86_64)%20AppleWebKit%2F537.36%20(KHTML%2C%20like%20Gecko)%20Chrome%2F114.0.0.0%20Safari%2F537.36&capi_version=1.5.2&capi_mode=lightbox&style_theme=default&rnd=0.3649022041957759"
+        url = "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147"
+        response = await self.session.post(url, data=form_data, headers=headers)
+        self.__check_response(response)
+        return response.json()["token"]
+
     async def __send_request(
         self,
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> AsyncGenerator[dict, None]:
         log.debug("Sending the payload")
 
         cid, pid = data["conversation_id"], data["parent_message_id"]
-        model, message = None, ""
-
+        message = ""
+        if data.get("model", "").startswith("gpt-4"):
+            data["arkose_token"] = await self.__arkose_token()
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         async with self.session.stream(
             "POST",
             url=f"{self.base_url}conversation",
             data=json.dumps(data),
             timeout=timeout,
@@ -1131,18 +1149,14 @@
             "parent_message_id": parent_id,
             "model": model,
             "history_and_training_disabled": self.disable_history,
         }
         plugin_ids = self.config.get("plugin_ids", []) or plugin_ids
         if len(plugin_ids) > 0 and not conversation_id:
             data["plugin_ids"] = plugin_ids
-        if model.startswith("gpt-4"):
-            data[
-                "arkose_token"
-            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
         async for msg in self.__send_request(
             data,
             timeout=timeout,
             auto_continue=auto_continue,
         ):
             yield msg
 
@@ -1260,19 +1274,14 @@
             or (
                 "text-davinci-002-render-paid"
                 if self.config.get("paid")
                 else "text-davinci-002-render-sha"
             ),
             "history_and_training_disabled": self.disable_history,
         }
-        if model.startswith("gpt-4"):
-            data[
-                "arkose_token"
-            ] = f"{generate_random_hex()}|r=ap-southeast-1|meta=3|meta_width=300|metabgclr=transparent|metaiconclr=%23555555|guitextcolor=%23000000|pk=35536E1E-65B4-4D96-9D97-6ADB7EFF8147|at=40|sup=1|rid={random_int(1,99)}|ag=101|cdn_url=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc|lurl=https%3A%2F%2Faudio-ap-southeast-1.arkoselabs.com|surl=https%3A%2F%2Ftcr9i.chat.openai.com|smurl=https%3A%2F%2Ftcr9i.chat.openai.com%2Fcdn%2Ffc%2Fassets%2Fstyle-manager"
-
         async for msg in self.__send_request(
             data=data,
             auto_continue=auto_continue,
             timeout=timeout,
         ):
             yield msg
```

### Comparing `revChatGPT-6.3.4/src/revChatGPT/V3.py` & `revChatGPT-6.4.0/src/revChatGPT/V3.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,14 +178,16 @@
         return self.max_tokens - self.get_token_count(convo_id)
 
     def ask_stream(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
+        model: str = None,
+        pass_history: bool = True,
         **kwargs,
     ):
         """
         Ask a question
         """
         # Make conversation if it doesn't exist
         if convo_id not in self.conversation:
@@ -193,16 +195,16 @@
         self.add_to_conversation(prompt, "user", convo_id=convo_id)
         self.__truncate_conversation(convo_id=convo_id)
         # Get response
         response = self.session.post(
             os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions",
             headers={"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"},
             json={
-                "model": self.engine,
-                "messages": self.conversation[convo_id],
+                "model": model or self.engine,
+                "messages": self.conversation[convo_id] if pass_history else [prompt],
                 "stream": True,
                 # kwargs
                 "temperature": kwargs.get("temperature", self.temperature),
                 "top_p": kwargs.get("top_p", self.top_p),
                 "presence_penalty": kwargs.get(
                     "presence_penalty",
                     self.presence_penalty,
@@ -247,14 +249,16 @@
         self.add_to_conversation(full_response, response_role, convo_id=convo_id)
 
     async def ask_stream_async(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
+        model: str = None,
+        pass_history: bool = True,
         **kwargs,
     ) -> AsyncGenerator[str, None]:
         """
         Ask a question
         """
         # Make conversation if it doesn't exist
         if convo_id not in self.conversation:
@@ -263,16 +267,16 @@
         self.__truncate_conversation(convo_id=convo_id)
         # Get response
         async with self.aclient.stream(
             "post",
             os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions",
             headers={"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"},
             json={
-                "model": self.engine,
-                "messages": self.conversation[convo_id],
+                "model": model or self.engine,
+                "messages": self.conversation[convo_id] if pass_history else [prompt],
                 "stream": True,
                 # kwargs
                 "temperature": kwargs.get("temperature", self.temperature),
                 "top_p": kwargs.get("top_p", self.top_p),
                 "presence_penalty": kwargs.get(
                     "presence_penalty",
                     self.presence_penalty,
@@ -319,14 +323,16 @@
         self.add_to_conversation(full_response, response_role, convo_id=convo_id)
 
     async def ask_async(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
+        model: str = None,
+        pass_history: bool = True,
         **kwargs,
     ) -> str:
         """
         Non-streaming ask
         """
         response = self.ask_stream_async(
             prompt=prompt,
@@ -338,23 +344,27 @@
         return full_response
 
     def ask(
         self,
         prompt: str,
         role: str = "user",
         convo_id: str = "default",
+        model: str = None,
+        pass_history: bool = True,
         **kwargs,
     ) -> str:
         """
         Non-streaming ask
         """
         response = self.ask_stream(
             prompt=prompt,
             role=role,
             convo_id=convo_id,
+            model=model,
+            pass_history=pass_history,
             **kwargs,
         )
         full_response: str = "".join(response)
         return full_response
 
     def rollback(self, n: int = 1, convo_id: str = "default") -> None:
         """
```

### Comparing `revChatGPT-6.3.4/src/revChatGPT/__init__.py` & `revChatGPT-6.4.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.4/src/revChatGPT/__main__.py` & `revChatGPT-6.4.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.4.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.4/src/revChatGPT/typings.py` & `revChatGPT-6.4.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.4/src/revChatGPT/utils.py` & `revChatGPT-6.4.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.3.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.4.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.3.4
+Version: 6.4.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.3.4/tests/test_recipient.py` & `revChatGPT-6.4.0/tests/test_recipient.py`

 * *Files identical despite different names*

