# Comparing `tmp/murkrow-0.8.0.tar.gz` & `tmp/murkrow-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murkrow-0.8.0.tar", max compression
+gzip compressed data, was "murkrow-0.9.0.tar", max compression
```

## Comparing `murkrow-0.8.0.tar` & `murkrow-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 murkrow-0.8.0/LICENSE
--rw-r--r--   0        0        0     1536 2023-04-06 23:55:12.092008 murkrow-0.8.0/README.md
--rw-r--r--   0        0        0     1005 2023-06-19 15:04:22.472498 murkrow-0.8.0/murkrow/__init__.py
--rw-r--r--   0        0        0     3419 2023-04-07 18:17:08.297847 murkrow-0.8.0/murkrow/display.py
--rw-r--r--   0        0        0     2792 2023-06-19 14:58:53.616286 murkrow-0.8.0/murkrow/messaging.py
--rw-r--r--   0        0        0     6500 2023-06-19 14:58:53.616665 murkrow-0.8.0/murkrow/murkrow.py
--rw-r--r--   0        0        0     2729 2023-06-19 14:58:53.617052 murkrow-0.8.0/murkrow/registry.py
--rw-r--r--   0        0        0     1958 2023-06-19 15:04:22.472302 murkrow-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-04-06 23:40:21.688686 murkrow-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0      624 2023-04-07 20:27:18.344406 murkrow-0.8.0/tests/test_murkrow.py
--rw-r--r--   0        0        0     2454 1970-01-01 00:00:00.000000 murkrow-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 murkrow-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1536 2023-04-06 23:55:12.092008 murkrow-0.9.0/README.md
+-rw-r--r--   0        0        0     1005 2023-06-19 15:35:53.811036 murkrow-0.9.0/murkrow/__init__.py
+-rw-r--r--   0        0        0     3419 2023-04-07 18:17:08.297847 murkrow-0.9.0/murkrow/display.py
+-rw-r--r--   0        0        0     2792 2023-06-19 14:58:53.616286 murkrow-0.9.0/murkrow/messaging.py
+-rw-r--r--   0        0        0     6978 2023-06-19 15:35:47.366679 murkrow-0.9.0/murkrow/murkrow.py
+-rw-r--r--   0        0        0     2729 2023-06-19 14:58:53.617052 murkrow-0.9.0/murkrow/registry.py
+-rw-r--r--   0        0        0     1958 2023-06-19 15:35:53.810861 murkrow-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-06 23:40:21.688686 murkrow-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      624 2023-04-07 20:27:18.344406 murkrow-0.9.0/tests/test_murkrow.py
+-rw-r--r--   0        0        0     2454 1970-01-01 00:00:00.000000 murkrow-0.9.0/PKG-INFO
```

### Comparing `murkrow-0.8.0/LICENSE` & `murkrow-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `murkrow-0.8.0/README.md` & `murkrow-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `murkrow-0.8.0/murkrow/__init__.py` & `murkrow-0.9.0/murkrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 a commanding presence. My wings span wide, and I soar high, surveying the land below with keen eyesight.
 I am the king of the skies, the lord of the avian realm. Squawk!
 
 """
 
 __author__ = """Kyle Kelley"""
 __email__ = 'rgbkrk@gmail.com'
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 
 # Export Markdown from display
 
 from .display import Markdown
 from .messaging import ai, assistant, assistant_function_call, function_result, human, narrate, system, user
 from .murkrow import Session
```

### Comparing `murkrow-0.8.0/murkrow/display.py` & `murkrow-0.9.0/murkrow/display.py`

 * *Files identical despite different names*

### Comparing `murkrow-0.8.0/murkrow/messaging.py` & `murkrow-0.9.0/murkrow/messaging.py`

 * *Files identical despite different names*

### Comparing `murkrow-0.8.0/murkrow/murkrow.py` & `murkrow-0.9.0/murkrow/murkrow.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,20 +32,22 @@
     Nice to hear!
 
     """
 
     messages: List[Message]
     model: str
     function_registry: FunctionRegistry
+    auto_continue: bool
 
     def __init__(
         self,
         *initial_context: Union[Message, str],
         model="gpt-3.5-turbo-0613",
         function_registry: Optional[FunctionRegistry] = None,
+        auto_continue: bool = True,
     ):
         """Initialize a `Murkrow` object with an optional initial context of messages.
 
         >>> from murkrow import Murkrow, narrate
         >>> murkrow = Murkrow(narrate("You are a large bird"))
         >>> murkrow.chat("What are you?")
         I am a large bird.
@@ -54,21 +56,22 @@
         if initial_context is None:
             initial_context = []  # type: ignore
 
         self.messages: List[Message] = []
 
         self.append(*initial_context)
         self.model = model
+        self.auto_continue = auto_continue
 
         if function_registry is None:
             self.function_registry = FunctionRegistry()
         else:
             self.function_registry = function_registry
 
-    def chat(self, *messages: Union[Message, str]):
+    def chat(self, *messages: Union[Message, str], auto_continue: Optional[bool] = None):
         """Send messages to the chat model and display the response.
 
         Args:
             messages (str | Message): One or more messages to send to the chat, can be strings or Message objects.
 
         """
         self.append(*messages)
@@ -88,17 +91,14 @@
         function_args = None
 
         in_function = False
 
         for result in resp:  # Go through the results of the stream
             choice = result['choices'][0]  # Get the first choice, since we're not doing bulk
 
-            # TODO: When moving from a content delta to a function call delta, we need to flush the
-            #       Markdown display and instead show the function call being built out
-
             if 'delta' in choice:  # If there is a delta in the result
                 delta = choice['delta']
                 if 'content' in delta and delta['content'] is not None:  # If the delta contains content
                     mark.append(delta['content'])  # Extend the markdown with the content
 
                 elif 'function_call' in delta:  # If the delta contains a function call
                     # Previous message finished
@@ -152,14 +152,31 @@
                 if not in_function:
                     # Wrap up the previous assistant
                     self.messages.append(assistant(mark.message))
 
                 if 'max_tokens' in choice['finish_reason']:
                     mark.append("\n...MAX TOKENS REACHED...\n")
 
+        # In priority order:
+        #
+        # `auto_continue` argument
+        # `self.auto_continue`
+        #
+        # If `auto_continue` is False, then `self.auto_continue` is ignored
+        continuing = False
+
+        if auto_continue is not None:
+            continuing = auto_continue
+        elif self.auto_continue:
+            continuing = True
+
+        if continuing and self.messages[-1]['role'] == 'function':
+            # Automatically let the LLM continue from our function result
+            self.chat()
+
     def append(self, *messages: Union[Message, str]):
         """Append messages to the conversation history.
 
         Note: this does not send the messages on until `chat` is called.
 
         Args:
             messages (str | Message): One or more messages to append to the conversation.
```

### Comparing `murkrow-0.8.0/murkrow/registry.py` & `murkrow-0.9.0/murkrow/registry.py`

 * *Files identical despite different names*

### Comparing `murkrow-0.8.0/pyproject.toml` & `murkrow-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "murkrow"
-version = "0.8.0"
+version = "0.9.0"
 homepage = "https://github.com/rgbkrk/murkrow"
 description = "Markdown for LLMs."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `murkrow-0.8.0/tests/test_murkrow.py` & `murkrow-0.9.0/tests/test_murkrow.py`

 * *Files identical despite different names*

### Comparing `murkrow-0.8.0/PKG-INFO` & `murkrow-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murkrow
-Version: 0.8.0
+Version: 0.9.0
 Summary: Markdown for LLMs.
 Home-page: https://github.com/rgbkrk/murkrow
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

