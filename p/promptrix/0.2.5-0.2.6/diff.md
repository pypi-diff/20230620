# Comparing `tmp/promptrix-0.2.5.tar.gz` & `tmp/promptrix-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.2.5.tar", last modified: Sun Jun 18 19:19:27 2023, max compression
+gzip compressed data, was "promptrix-0.2.6.tar", last modified: Tue Jun 20 03:27:33 2023, max compression
```

## Comparing `promptrix-0.2.5.tar` & `promptrix-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.5/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2177 2023-06-18 19:19:27.511229 promptrix-0.2.5/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.2.5/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      847 2023-06-18 19:19:17.000000 promptrix-0.2.5/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-18 19:19:27.511229 promptrix-0.2.5/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.5/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2900 2023-06-15 03:37:36.000000 promptrix-0.2.5/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.5/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.5/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.5/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.5/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2445 2023-06-15 17:06:28.000000 promptrix-0.2.5/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5738 2023-06-14 19:26:14.000000 promptrix-0.2.5/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.5/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-14 19:25:22.000000 promptrix-0.2.5/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-14 20:55:08.000000 promptrix-0.2.5/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.5/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/promptrixTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2177 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.940387 promptrix-0.2.6/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.6/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-06-20 03:27:33.940387 promptrix-0.2.6/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.2.6/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      833 2023-06-20 03:24:19.000000 promptrix-0.2.6/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-20 03:27:33.940387 promptrix-0.2.6/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.936387 promptrix-0.2.6/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.940387 promptrix-0.2.6/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.6/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2580 2023-06-19 22:45:55.000000 promptrix-0.2.6/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.6/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.6/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.6/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.6/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2445 2023-06-15 17:06:28.000000 promptrix-0.2.6/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5738 2023-06-14 19:26:14.000000 promptrix-0.2.6/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.6/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-14 19:25:22.000000 promptrix-0.2.6/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-19 22:47:47.000000 promptrix-0.2.6/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.6/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.6/src/promptrix/promptrixTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:27:33.940387 promptrix-0.2.6/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-20 03:27:33.000000 promptrix-0.2.6/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.2.5/LICENSE` & `promptrix-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/PKG-INFO` & `promptrix-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.5
+Version: 0.2.6
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
-Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
+Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `promptrix-0.2.5/README.md` & `promptrix-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/pyproject.toml` & `promptrix-0.2.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
 #documentation = "https://github.com/Stevenic/promptrix-py/README.md"
@@ -28,9 +28,9 @@
     "tiktoken",
     "pyyaml",
     'importlib-metadata; python_version<"3.9"',
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/Stevenic/promptrix-py"
+"Homepage" = "https://tuuyi.io/promptrix"
 "Bug Tracker" = "https://github.com/Stevenic/promptrix-py/issues"
```

### Comparing `promptrix-0.2.5/src/promptrix/AssistantMessage.py` & `promptrix-0.2.6/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/ConversationHistory.py` & `promptrix-0.2.6/src/promptrix/ConversationHistory.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         self.variable = variable
         self.userPrefix = userPrefix
         self.assistantPrefix = assistantPrefix
 
     async def renderAsText(self, memory, functions, tokenizer, maxTokens):
         history = memory.get(self.variable)
         if history is None: history=[]
-        #print(f'*****ConversationHistory renderAsText {len(history)}')
         tokens = 0
         budget = min(self.tokens, maxTokens) if self.tokens > 1.0 else maxTokens
         separatorLength = len(tokenizer.encode(self.separator))
         lines = []
         for i in range(len(history)-1, -1, -1):
             msg = history[i]
             message = Utilities.to_string(tokenizer, msg['content'])
@@ -27,21 +26,19 @@
                 tokens += length
                 lines.insert(0, line)
                 continue
             if tokens + length > budget:
                 break
             tokens += length
             lines.insert(0, line)
-        #print(f'*****ConversationHistory renderAsText exit lines {len(lines)}')
         return RenderedPromptSection(output=self.separator.join(lines), length=tokens, tooLong=tokens > maxTokens)
 
     async def renderAsMessages(self, memory, functions, tokenizer, maxTokens):
         history = memory.get(self.variable)
         if history is None: history = []
-        #print(f'*****ConversationHistory renderAsMessages {len(history)}')
         tokens = 0
         budget = min(self.tokens, maxTokens) if self.tokens > 1.0 else maxTokens
         messages = []
         for i in range(len(history)-1, -1, -1):
             msg = history[i]
             message = {'role':msg['role'], 'content':Utilities.to_string(tokenizer, msg['content'])}
             length = len(tokenizer.encode(message['content']))
@@ -49,10 +46,9 @@
                 tokens += length
                 messages.insert(0, message)
                 continue
             if tokens + length > budget:
                 break
             tokens += length
             messages.insert(0, message)
-        #print(f'*****ConversationHistory renderAsMessages exit messages {len(messages)}')
         
         return RenderedPromptSection(output=messages, length=tokens, tooLong=tokens > maxTokens)
```

### Comparing `promptrix-0.2.5/src/promptrix/FunctionRegistry.py` & `promptrix-0.2.6/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.2.6/src/promptrix/GPT3Tokenizer.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/GroupSection.py` & `promptrix-0.2.6/src/promptrix/GroupSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/LayoutEngine.py` & `promptrix-0.2.6/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/PromptSectionBase.py` & `promptrix-0.2.6/src/promptrix/PromptSectionBase.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/TemplateSection.py` & `promptrix-0.2.6/src/promptrix/TemplateSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/TextSection.py` & `promptrix-0.2.6/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/UserMessage.py` & `promptrix-0.2.6/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/Utilities.py` & `promptrix-0.2.6/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/VolatileMemory.py` & `promptrix-0.2.6/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix/promptrixTypes.py` & `promptrix-0.2.6/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.5/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.2.6/src/promptrix.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.5
+Version: 0.2.6
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
-Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
+Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `promptrix-0.2.5/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.2.6/src/promptrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

