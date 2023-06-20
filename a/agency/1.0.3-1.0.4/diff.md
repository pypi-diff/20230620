# Comparing `tmp/agency-1.0.3.tar.gz` & `tmp/agency-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.0.3.tar", max compression
+gzip compressed data, was "agency-1.0.4.tar", max compression
```

## Comparing `agency-1.0.3.tar` & `agency-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,9 @@
--rw-r--r--   0        0        0    35148 2023-06-17 00:45:31.301980 agency-1.0.3/LICENSE
--rw-r--r--   0        0        0    24997 2023-06-17 00:45:31.301980 agency-1.0.3/README.md
--rw-r--r--   0        0        0       40 2023-06-17 00:45:31.301980 agency-1.0.3/agency/__init__.py
--rw-r--r--   0        0        0    10347 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agent.py
--rw-r--r--   0        0        0        0 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/__init__.py
--rw-r--r--   0        0        0     2791 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/chattyai.py
--rw-r--r--   0        0        0     2202 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/host.py
--rw-r--r--   0        0        0     2729 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/openai_completion_agent.py
--rw-r--r--   0        0        0     7797 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/openai_function_agent.py
--rw-r--r--   0        0        0     1519 2023-06-17 00:45:31.301980 agency-1.0.3/agency/agents/prompt_methods.py
--rw-r--r--   0        0        0      801 2023-06-17 00:45:31.301980 agency-1.0.3/agency/schema.py
--rwxr-xr-x   0        0        0     3261 2023-06-17 00:45:31.301980 agency-1.0.3/agency/space.py
--rw-r--r--   0        0        0        0 2023-06-17 00:45:31.301980 agency-1.0.3/agency/spaces/__init__.py
--rw-r--r--   0        0        0     6646 2023-06-17 00:45:31.301980 agency-1.0.3/agency/spaces/templates/index.html
--rw-r--r--   0        0        0     4027 2023-06-17 00:45:31.301980 agency-1.0.3/agency/spaces/web_app.py
--rw-r--r--   0        0        0     4280 2023-06-17 00:45:31.301980 agency-1.0.3/agency/util.py
--rw-r--r--   0        0        0      554 2023-06-17 00:45:34.749985 agency-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    25833 1970-01-01 00:00:00.000000 agency-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-20 04:23:57.867662 agency-1.0.4/LICENSE
+-rw-r--r--   0        0        0    25161 2023-06-20 04:23:57.867662 agency-1.0.4/README.md
+-rw-r--r--   0        0        0       40 2023-06-20 04:23:57.871662 agency-1.0.4/agency/__init__.py
+-rw-r--r--   0        0        0    10347 2023-06-20 04:23:57.871662 agency-1.0.4/agency/agent.py
+-rw-r--r--   0        0        0      801 2023-06-20 04:23:57.871662 agency-1.0.4/agency/schema.py
+-rwxr-xr-x   0        0        0     3261 2023-06-20 04:23:57.871662 agency-1.0.4/agency/space.py
+-rw-r--r--   0        0        0     4280 2023-06-20 04:23:57.871662 agency-1.0.4/agency/util.py
+-rw-r--r--   0        0        0      517 2023-06-20 04:23:59.359765 agency-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    25841 1970-01-01 00:00:00.000000 agency-1.0.4/PKG-INFO
```

### Comparing `agency-1.0.3/LICENSE` & `agency-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.0.3/README.md` & `agency-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 A fast and minimal actor model framework for building agent-integrated systems
 
 
 ## What is `agency`?
 
 `agency` defines a common communication and action framework for integrating
-AI agents, humans, and traditional computing systems.
+AI agents with traditional computing systems, and even humans in a way where
+all can easily communicate.
 
-`agency` allows you to establish shared environments called "spaces" where any
+`agency` allows you to create shared environments called "spaces" where any
 number of humans, artificial, or other computing systems may equally address
 each other as individual "agents" that you may perform "actions" on.
 
 `agency` handles the details of the common messaging protocol and allows
 discovering and invoking actions across all parties, automatically handling
 things such as reporting exceptions, enforcing access restrictions, and more.
 
@@ -25,22 +26,19 @@
 - people
 - ...
 - anything
 
 
 # Install
 > **WARNING:**\
-Running `agency` may result in exposing your computer to access by any connected
-`Agent` class. Please understand the risks before using this software and do not
-configure it for OS access otherwise.\
-\
-If you want to enable OS access, to allow for file I/O for example, I HIGHLY
-RECOMMEND running your project within a Docker container to prevent direct
-access to your host, allowing you to limit the resources and directories that
-may be accessed.
+> Running `agency` may result in exposing your computer to access by any connected `Agent` class. Please understand the risks before using this software and configure your environment safely.
+>
+> If, for example, you want to enable OS access, I HIGHLY RECOMMEND running your project within a Docker container to prevent direct access to your host, allowing you to limit the resources and directories that may be accessed.
+>
+> If you need it, an example Dockerfile can be found in the [examples/demo](./examples/demo) directory.
 
 ```sh
 pip install agency
 ```
 
 
 # API Overview
@@ -56,54 +54,54 @@
 languages. All agents may expose "actions" that other agents can discover and
 invoke at run time. Actions also specify an access policy, allowing you to
 monitor and control actions to ensure safety.
 
 A `Space` is also an `Agent` and is used to group multiple agents together. A
 space can be thought of as both a collection of agents and a facilitator for
 their communication. An agent cannot communicate with others until it is first
-added to a space.
-
-Spaces may be nested, allowing for namespacing and hierarchical organization of
-the agents in your application.
+added to a space. Spaces may be nested, allowing for namespacing and
+hierarchical organization of the agents in your application.
 
 To summarize, the two classes of `Agent` and `Space` together create a simple
 API for creating applications that may mix AI, human, and traditional computing
 systems, in a way that is intended for all to equally understand and use.
 
 Let's walk through a thorough example to see how this works in practice.
 
 
 # Example Walkthrough
 
-> Please note that the example agent classes used in this walkthrough are
-implemented for you to explore and try out, but should be considered "proof of
-concept" quality at this time.
-
-The following snippet is the full resulting implementation (minus imports) of
-the example walkthrough that you can try out on your own, including two OpenAI
-agent examples and the HuggingFace based `ChattyAI`. Note that `Space.run()`
-starts a thread, so we simply keep the application alive with a while loop.
+The snippet below is an example application taken from the demo located at
+[./examples/demo/](./examples/demo/). A Dockerfile and basic instructions for
+how to run the demo are located in that directory.
+
+The demo includes two OpenAI agent classes, the HuggingFace based `ChattyAI`,
+operating system access, and a web application hosted at
+`http://localhost:8080`. Note that `Space.run()` starts a thread, so we simply
+keep the application alive with a while loop.
+
+The walkthrough that follows details how this demo application works.
 
 ```python
 # demo.py
 
 if __name__ == '__main__':
 
     space = Space("DemoSpace")
 
     space.add(
+        ChattyAI("Chatty",
+            model="EleutherAI/gpt-neo-125m"))
+
+    space.add(
         WebApp("WebApp",
             demo_user_id="Dan", # hardcoded for simplicity
             port='8080'))
 
     space.add(
-        ChattyAI("Chatty",
-            model="EleutherAI/gpt-neo-125m"))
-
-    space.add(
         Host("Host"))
 
     space.add(
         OpenAIFunctionAgent("FunctionAI",
             model="gpt-3.5-turbo-16k",
             openai_api_key=os.getenv("OPENAI_API_KEY"),
             # user_id determines the "user" role in the OpenAI chat
@@ -122,15 +120,16 @@
     while True:
         time.sleep(1)
 ```
 
 
 ## Creating a `Space`
 
-Let's start by instantiating a demo space.
+Now let's see how this is implemented. Let's start by instantiating the demo
+space.
 
 ```python
 space = Space("DemoSpace")
 ```
 
 `Space`'s, like all `Agent`'s, must be given an `id`. So the line above
 instantiates a single space called `"DemoSpace"` that we can now add agents to.
@@ -245,17 +244,14 @@
 enough to support any use case while remaining human readable.
 
 Note that the `"thoughts"` field is defined as a distinct argument for providing
 a natural language explanation to accompany any action, but as of this writing
 `ChattyAI` does not make use of it. `OpenAICompletionAgent` discussed below,
 does.
 
-For more details on the common message schema see
-[schema.py](./agency/schema.py).
-
 
 ## Access Control
 
 All actions must declare an access policy like the following example seen above
 the `ChattyAI._action__say()` method:
 
 ```python
@@ -656,15 +652,16 @@
 * This library makes use of threads for each individual agent. Multithreading
   is limited by python's GIL, meaning if you run a CPU bound model other agents
   will have to wait for their "turn". This goes for anything else you might
   define as an "agent", if it is CPU heavy it will block other agents. Note that
   I/O does not block, so networked backends or services will execute in
   parallel.
 
-  Other forms of multiprocessing to avoid the GIL will be considered.
+  Other multiprocessing approaches to avoid the GIL are
+  [in development](https://github.com/operand/agency/issues/25).
 
 * This API does NOT assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
   of representing many things uniquely and independently. This is a core feature
@@ -705,17 +702,16 @@
 ```
 
 The test suite is currently set up to run on pull requests to the `main` branch.
 
 
 # Roadmap
 
-The goal is to maintain a minimal, natural, and practical API for bringing
-human, artificial, and other computing systems together, with the following
-priorities.
+The goal is to maintain a minimal and practical API for bringing human,
+artificial, and other computing systems together, with the following priorities.
 
 
 ## Priorities
 - **Speed**:
   Performance is always a concern. If it's not performant, it's not practical.
   Currently the limitations of python multi-threading are a bottleneck and a
   priority to address.
```

### Comparing `agency-1.0.3/agency/agent.py` & `agency-1.0.4/agency/agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.3/agency/schema.py` & `agency-1.0.4/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.3/agency/space.py` & `agency-1.0.4/agency/space.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.3/agency/util.py` & `agency-1.0.4/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.0.3/pyproject.toml` & `agency-1.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 [tool.poetry]
 name = "agency"
-version = "1.0.3"
+version = "1.0.4"
 description = "A fast and minimal actor model framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
+include = ["agency/**/*"]
+exclude = ["*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncio = "^3.4"
 colorama = "^0.4"
 pydantic = "^1.8"
-transformers = "^4.29"
-torch = "^2.0"
-Flask-SocketIO = "^5.3"
-eventlet = "^0.33"
-openai = "^0.27.8"
+eventlet = "^0.33.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `agency-1.0.3/PKG-INFO` & `agency-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 Metadata-Version: 2.1
 Name: agency
-Version: 1.0.3
+Version: 1.0.4
 Summary: A fast and minimal actor model framework for building agent-integrated systems
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Flask-SocketIO (>=5.3,<6.0)
 Requires-Dist: asyncio (>=3.4,<4.0)
 Requires-Dist: colorama (>=0.4,<0.5)
-Requires-Dist: eventlet (>=0.33,<0.34)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: eventlet (>=0.33.3,<0.34.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
-Requires-Dist: torch (>=2.0,<3.0)
-Requires-Dist: transformers (>=4.29,<5.0)
 Description-Content-Type: text/markdown
 
 # `agency`
 
 A fast and minimal actor model framework for building agent-integrated systems
 
 
 ## What is `agency`?
 
 `agency` defines a common communication and action framework for integrating
-AI agents, humans, and traditional computing systems.
+AI agents with traditional computing systems, and even humans in a way where
+all can easily communicate.
 
-`agency` allows you to establish shared environments called "spaces" where any
+`agency` allows you to create shared environments called "spaces" where any
 number of humans, artificial, or other computing systems may equally address
 each other as individual "agents" that you may perform "actions" on.
 
 `agency` handles the details of the common messaging protocol and allows
 discovering and invoking actions across all parties, automatically handling
 things such as reporting exceptions, enforcing access restrictions, and more.
 
@@ -47,22 +44,19 @@
 - people
 - ...
 - anything
 
 
 # Install
 > **WARNING:**\
-Running `agency` may result in exposing your computer to access by any connected
-`Agent` class. Please understand the risks before using this software and do not
-configure it for OS access otherwise.\
-\
-If you want to enable OS access, to allow for file I/O for example, I HIGHLY
-RECOMMEND running your project within a Docker container to prevent direct
-access to your host, allowing you to limit the resources and directories that
-may be accessed.
+> Running `agency` may result in exposing your computer to access by any connected `Agent` class. Please understand the risks before using this software and configure your environment safely.
+>
+> If, for example, you want to enable OS access, I HIGHLY RECOMMEND running your project within a Docker container to prevent direct access to your host, allowing you to limit the resources and directories that may be accessed.
+>
+> If you need it, an example Dockerfile can be found in the [examples/demo](./examples/demo) directory.
 
 ```sh
 pip install agency
 ```
 
 
 # API Overview
@@ -78,54 +72,54 @@
 languages. All agents may expose "actions" that other agents can discover and
 invoke at run time. Actions also specify an access policy, allowing you to
 monitor and control actions to ensure safety.
 
 A `Space` is also an `Agent` and is used to group multiple agents together. A
 space can be thought of as both a collection of agents and a facilitator for
 their communication. An agent cannot communicate with others until it is first
-added to a space.
-
-Spaces may be nested, allowing for namespacing and hierarchical organization of
-the agents in your application.
+added to a space. Spaces may be nested, allowing for namespacing and
+hierarchical organization of the agents in your application.
 
 To summarize, the two classes of `Agent` and `Space` together create a simple
 API for creating applications that may mix AI, human, and traditional computing
 systems, in a way that is intended for all to equally understand and use.
 
 Let's walk through a thorough example to see how this works in practice.
 
 
 # Example Walkthrough
 
-> Please note that the example agent classes used in this walkthrough are
-implemented for you to explore and try out, but should be considered "proof of
-concept" quality at this time.
-
-The following snippet is the full resulting implementation (minus imports) of
-the example walkthrough that you can try out on your own, including two OpenAI
-agent examples and the HuggingFace based `ChattyAI`. Note that `Space.run()`
-starts a thread, so we simply keep the application alive with a while loop.
+The snippet below is an example application taken from the demo located at
+[./examples/demo/](./examples/demo/). A Dockerfile and basic instructions for
+how to run the demo are located in that directory.
+
+The demo includes two OpenAI agent classes, the HuggingFace based `ChattyAI`,
+operating system access, and a web application hosted at
+`http://localhost:8080`. Note that `Space.run()` starts a thread, so we simply
+keep the application alive with a while loop.
+
+The walkthrough that follows details how this demo application works.
 
 ```python
 # demo.py
 
 if __name__ == '__main__':
 
     space = Space("DemoSpace")
 
     space.add(
+        ChattyAI("Chatty",
+            model="EleutherAI/gpt-neo-125m"))
+
+    space.add(
         WebApp("WebApp",
             demo_user_id="Dan", # hardcoded for simplicity
             port='8080'))
 
     space.add(
-        ChattyAI("Chatty",
-            model="EleutherAI/gpt-neo-125m"))
-
-    space.add(
         Host("Host"))
 
     space.add(
         OpenAIFunctionAgent("FunctionAI",
             model="gpt-3.5-turbo-16k",
             openai_api_key=os.getenv("OPENAI_API_KEY"),
             # user_id determines the "user" role in the OpenAI chat
@@ -144,15 +138,16 @@
     while True:
         time.sleep(1)
 ```
 
 
 ## Creating a `Space`
 
-Let's start by instantiating a demo space.
+Now let's see how this is implemented. Let's start by instantiating the demo
+space.
 
 ```python
 space = Space("DemoSpace")
 ```
 
 `Space`'s, like all `Agent`'s, must be given an `id`. So the line above
 instantiates a single space called `"DemoSpace"` that we can now add agents to.
@@ -267,17 +262,14 @@
 enough to support any use case while remaining human readable.
 
 Note that the `"thoughts"` field is defined as a distinct argument for providing
 a natural language explanation to accompany any action, but as of this writing
 `ChattyAI` does not make use of it. `OpenAICompletionAgent` discussed below,
 does.
 
-For more details on the common message schema see
-[schema.py](./agency/schema.py).
-
 
 ## Access Control
 
 All actions must declare an access policy like the following example seen above
 the `ChattyAI._action__say()` method:
 
 ```python
@@ -678,15 +670,16 @@
 * This library makes use of threads for each individual agent. Multithreading
   is limited by python's GIL, meaning if you run a CPU bound model other agents
   will have to wait for their "turn". This goes for anything else you might
   define as an "agent", if it is CPU heavy it will block other agents. Note that
   I/O does not block, so networked backends or services will execute in
   parallel.
 
-  Other forms of multiprocessing to avoid the GIL will be considered.
+  Other multiprocessing approaches to avoid the GIL are
+  [in development](https://github.com/operand/agency/issues/25).
 
 * This API does NOT assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
   `agency` is intended to allow potentially large numbers of agents, systems,
   and people to come together. A small predefined set of roles gets in the way
   of representing many things uniquely and independently. This is a core feature
@@ -727,17 +720,16 @@
 ```
 
 The test suite is currently set up to run on pull requests to the `main` branch.
 
 
 # Roadmap
 
-The goal is to maintain a minimal, natural, and practical API for bringing
-human, artificial, and other computing systems together, with the following
-priorities.
+The goal is to maintain a minimal and practical API for bringing human,
+artificial, and other computing systems together, with the following priorities.
 
 
 ## Priorities
 - **Speed**:
   Performance is always a concern. If it's not performant, it's not practical.
   Currently the limitations of python multi-threading are a bottleneck and a
   priority to address.
```

