# Comparing `tmp/heygptcli-0.1.2.tar.gz` & `tmp/heygptcli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heygptcli-0.1.2.tar", max compression
+gzip compressed data, was "heygptcli-0.1.3.tar", max compression
```

## Comparing `heygptcli-0.1.2.tar` & `heygptcli-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-18 11:19:57.231599 heygptcli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/__init__.py
--rw-r--r--   0        0        0      717 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/api.py
--rwxr-xr-x   0        0        0     4804 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/cli.py
--rw-r--r--   0        0        0     2249 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/constant.py
--rw-r--r--   0        0        0     2804 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/core.py
--rw-r--r--   0        0        0     1897 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/serve.py
--rw-r--r--   0        0        0      153 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/serve_prompts.py
--rw-r--r--   0        0        0      849 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/utils.py
--rw-r--r--   0        0        0      677 2023-06-18 11:19:57.231599 heygptcli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-20 17:30:39.875805 heygptcli-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 17:30:39.875805 heygptcli-0.1.3/heygpt/__init__.py
+-rw-r--r--   0        0        0      717 2023-06-20 17:30:39.875805 heygptcli-0.1.3/heygpt/api.py
+-rwxr-xr-x   0        0        0     5048 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/cli.py
+-rw-r--r--   0        0        0     2249 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/constant.py
+-rw-r--r--   0        0        0     3440 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/core.py
+-rw-r--r--   0        0        0     1897 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/serve.py
+-rw-r--r--   0        0        0      153 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/serve_prompts.py
+-rw-r--r--   0        0        0      849 2023-06-20 17:30:39.879805 heygptcli-0.1.3/heygpt/utils.py
+-rw-r--r--   0        0        0      677 2023-06-20 17:30:39.879805 heygptcli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.3/PKG-INFO
```

### Comparing `heygptcli-0.1.2/heygpt/api.py` & `heygptcli-0.1.3/heygpt/api.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.2/heygpt/cli.py` & `heygptcli-0.1.3/heygpt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import uvicorn
 import rich
 from rich.prompt import Prompt
 import typer
 
 from heygpt.utils import log
-from heygpt.constant import load_promps, prompt_items_url
+from heygpt.constant import load_promps, prompt_items_url, openai_model
 from heygpt.core import (
     sh,
     completion_openai_gpt,
     completion_bard,
     make_prompt,
     wisper,
     print_md,
@@ -27,25 +27,33 @@
 HeyGPT CLI\n\nA simple command line tool to generate text using OpenAI GPT-3 or Bard base on ready made templated promts.
 \n\n\nFor debug logs use: `export LOG_LEVEL=DEBUG` or `set LOG_LEVEL=DEBUG` on windows."""
 )
 
 
 @app.command(help="Ask query or task to gpt using prompt templates")
 def ask(
-    bard: bool = typer.Option(False, "--bard", "-b", help="Use bard instead of gpt-3."),
+    bard: bool = typer.Option(
+        False, "--bard", "-b", help="Use bard instead of openai."
+    ),
     no_prompt: bool = typer.Option(
         False, "--no-prompt", "-n", help="Ask without anyprompt templates."
     ),
     text: str = typer.Option(
         str, help="Optional provide text query as an input argument."
     ),
     tag: Annotated[Optional[List[str]], typer.Option()] = [],
     save: str = typer.Option(
         "", "--output", "-o", help="save output to file availabe formats: md"
     ),
+    model: str = typer.Option(
+        openai_model,
+        "--model",
+        "-m",
+        help="OpenAI model name. info: https://platform.openai.com/docs/models/gpt-3",
+    ),
 ):
     tags: str = " #".join(tag)
     command: str = ""
 
     # print(tags)
     # return
     if not no_prompt:
@@ -85,15 +93,17 @@
         print()
         text = Prompt.ask("[blue]Enter text")
 
     # log.debug(text)
     if bard:
         content = completion_bard(command=command, text=text, _print=True)
     else:
-        completion = completion_openai_gpt(command=command, text=text, _print=True)
+        completion = completion_openai_gpt(
+            command=command, text=text, model=model, _print=True
+        )
         content = completion
 
     # typer.echo("\n---------- output ----------\n")
 
     if save != "":
         with open(f"{save}", "w") as f:
             f.write(content)
```

### Comparing `heygptcli-0.1.2/heygpt/constant.py` & `heygptcli-0.1.3/heygpt/constant.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.2/heygpt/core.py` & `heygptcli-0.1.3/heygpt/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bardapi import Bard
 from rich.console import Console
 from rich.markdown import Markdown
 from prompt_toolkit import prompt
 from prompt_toolkit.completion import FuzzyWordCompleter
 
 from heygpt.constant import configs, genrtare_prompt_url, openai_model
+from heygpt.utils import log
 
 console = Console()
 
 openai.api_key = os.getenv("OPENAI_API_KEY", configs.get("openai_key"))
 
 
 def sh(command):
@@ -26,41 +27,63 @@
 
 def ask_prompt_input(items: list, title="Select item"):
     completer = FuzzyWordCompleter(items)
     text = prompt(f"{title}: ", completer=completer, complete_while_typing=True)
     return text
 
 
-def completion_openai_gpt(text: str = None, command: str = "", _print=False):
+def completion_openai_gpt(
+    text: str = None, command: str = "", model=openai_model, _print=False
+):
     """
     ref: https://docs.openai.com/api-reference/completions/create
     """
     out = ""
+    log.debug(f"model: {model}")
 
     if not text:
         raise Exception("No text found")
 
-    completion = openai.ChatCompletion.create(
-        model=openai_model,
-        stream=True,
-        messages=[
-            {
-                "role": "system",
-                "content": "Output has to be in markdown supported format",
-            },
-            {"role": "user", "content": command + "\nTask: " + text},
-        ],
-        # stop="",
-    )
-
-    for chunk in completion:
-        # Process each chunk as needed
-        c = chunk["choices"][0]["delta"].get("content", "")
-        out += c
-        if _print:
+    if command != "":
+        _command = command + "\nTask: " + text
+    else:
+        _command = text
+
+    if "gpt-3" in model:
+        completion = openai.ChatCompletion.create(
+            model=model,
+            stream=True,
+            messages=[
+                {
+                    "role": "system",
+                    "content": "Output has to be in markdown supported format",
+                },
+                {"role": "user", "content": _command},
+            ],
+            # stop="",
+        )
+
+        for chunk in completion:
+            # Process each chunk as needed
+            c = chunk["choices"][0]["delta"].get("content", "")
+            out += c
+            if _print:
+                console.print(c, end="", markup=True)
+    else:
+        completion = openai.Completion.create(
+            model=model,
+            prompt=_command,
+            temperature=0.9,
+            max_tokens=1000,
+            stream=True,
+            top_p=1,
+        )
+        for chunk in completion:
+            c = chunk["choices"][0]["text"]
+            out += c
             console.print(c, end="", markup=True)
 
     return out
 
 
 def completion_bard(text: str, command: str = "", _print=False):
     """
```

### Comparing `heygptcli-0.1.2/heygpt/serve.py` & `heygptcli-0.1.3/heygpt/serve.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.2/heygpt/utils.py` & `heygptcli-0.1.3/heygpt/utils.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.2/pyproject.toml` & `heygptcli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heygptcli"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Rishang <rishang@localhost.com>"]
 readme = "README.md"
 packages = [
   { include = "heygpt" }
 ]
```

### Comparing `heygptcli-0.1.2/PKG-INFO` & `heygptcli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heygptcli
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Rishang
 Author-email: rishang@localhost.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

