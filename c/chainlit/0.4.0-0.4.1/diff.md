# Comparing `tmp/chainlit-0.4.0.tar.gz` & `tmp/chainlit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.4.0.tar", max compression
+gzip compressed data, was "chainlit-0.4.1.tar", max compression
```

## Comparing `chainlit-0.4.0.tar` & `chainlit-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     2495 2023-06-16 08:44:12.198934 chainlit-0.4.0/README.md
--rw-r--r--   0        0        0     7443 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/__main__.py
--rw-r--r--   0        0        0     1316 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/action.py
--rw-r--r--   0        0        0      700 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/cache.py
--rw-r--r--   0        0        0     3882 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/cli/deploy.py
--rw-r--r--   0        0        0     1147 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/cli/mock.py
--rw-r--r--   0        0        0      716 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/cli/utils.py
--rw-r--r--   0        0        0     9838 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/client.py
--rw-r--r--   0        0        0     6349 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/config.py
--rw-r--r--   0        0        0     6060 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/element.py
--rw-r--r--   0        0        0     5113 2023-06-16 08:43:26.999049 chainlit-0.4.0/chainlit/emitter.py
--rw-r--r--   0        0        0     5666 2023-06-16 08:44:38.262832 chainlit-0.4.0/chainlit/frontend/dist/assets/index-0cc9e355.css
--rw-r--r--   0        0        0  2132824 2023-06-16 08:44:38.262832 chainlit-0.4.0/chainlit/frontend/dist/assets/index-9e4bccd1.js
--rw-r--r--   0        0        0     8889 2023-06-16 08:44:38.254832 chainlit-0.4.0/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-06-16 08:44:38.262832 chainlit-0.4.0/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-06-16 08:44:37.014836 chainlit-0.4.0/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      793 2023-06-16 08:44:38.262832 chainlit-0.4.0/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      417 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/hello.py
--rw-r--r--   0        0        0      292 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/lc/agent.py
--rw-r--r--   0        0        0    13195 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/lc/callbacks.py
--rw-r--r--   0        0        0      398 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/logger.py
--rw-r--r--   0        0        0     1623 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/markdown.py
--rw-r--r--   0        0        0    11948 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/message.py
--rw-r--r--   0        0        0    13827 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/server.py
--rw-r--r--   0        0        0      884 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/session.py
--rw-r--r--   0        0        0      950 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/sync.py
--rw-r--r--   0        0        0     2358 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/telemetry.py
--rw-r--r--   0        0        0     1525 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/types.py
--rw-r--r--   0        0        0     1213 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-06-16 08:43:27.007049 chainlit-0.4.0/chainlit/version.py
--rw-r--r--   0        0        0     1022 2023-06-16 08:43:27.007049 chainlit-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 chainlit-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2586 2023-06-20 13:11:34.219457 chainlit-0.4.1/README.md
+-rw-r--r--   0        0        0     7489 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/__main__.py
+-rw-r--r--   0        0        0     1316 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/action.py
+-rw-r--r--   0        0        0     1343 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cache.py
+-rw-r--r--   0        0        0     3882 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0     1147 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/mock.py
+-rw-r--r--   0        0        0      716 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     9838 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/client.py
+-rw-r--r--   0        0        0     7430 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/config.py
+-rw-r--r--   0        0        0     6060 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/element.py
+-rw-r--r--   0        0        0     5113 2023-06-20 13:10:49.875692 chainlit-0.4.1/chainlit/emitter.py
+-rw-r--r--   0        0        0   614554 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/index-51a1a88f.js
+-rw-r--r--   0        0        0  1521126 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/index-68c36c96.js
+-rw-r--r--   0        0        0     5697 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/index-f93cc942.css
+-rw-r--r--   0        0        0     8889 2023-06-20 13:11:58.379330 chainlit-0.4.1/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-06-20 13:11:57.255335 chainlit-0.4.1/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      793 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      417 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/hello.py
+-rw-r--r--   0        0        0      292 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     1080 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/lc/agent.py
+-rw-r--r--   0        0        0    13195 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/lc/callbacks.py
+-rw-r--r--   0        0        0      398 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/logger.py
+-rw-r--r--   0        0        0     1623 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/markdown.py
+-rw-r--r--   0        0        0    11948 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/message.py
+-rw-r--r--   0        0        0    14332 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/server.py
+-rw-r--r--   0        0        0      884 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/session.py
+-rw-r--r--   0        0        0      950 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/sync.py
+-rw-r--r--   0        0        0     2358 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/telemetry.py
+-rw-r--r--   0        0        0     1525 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/types.py
+-rw-r--r--   0        0        0     1213 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/version.py
+-rw-r--r--   0        0        0     1022 2023-06-20 13:10:49.879691 chainlit-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4044 1970-01-01 00:00:00.000000 chainlit-0.4.1/PKG-INFO
```

### Comparing `chainlit-0.4.0/README.md` & `chainlit-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 Chainlit lets you create ChatGPT-like UIs on top of any Python code in minutes! Some of the key features include intermediary steps visualisation, element management & display (images, text, carousel, etc.) as well as cloud deployment.
 
 [![](https://dcbadge.vercel.app/api/server/ZThrUxbAYw?style=flat)](https://discord.gg/ZThrUxbAYw)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/chainlit_io.svg?style=social&label=Follow%20%40chainlit_io)](https://twitter.com/chainlit_io)
 [![CI](https://github.com/Chainlit/chainlit/actions/workflows/ci.yaml/badge.svg)](https://github.com/Chainlit/chainlit/actions/workflows/ci.yaml)
 
+https://github.com/Chainlit/chainlit/assets/13104895/e347e52c-35b2-4c35-8a88-f8ac02dd198e
+
 ## Installation
 
 Open a terminal and run:
 
 ```bash
 $ pip install chainlit
 $ chainlit hello
```

### Comparing `chainlit-0.4.0/chainlit/__init__.py` & `chainlit-0.4.1/chainlit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from chainlit.types import LLMSettings
 from chainlit.message import ErrorMessage
 from chainlit.action import Action
 from chainlit.element import Image, Text, Pdf, Avatar, Pyplot
 from chainlit.message import Message, ErrorMessage, AskUserMessage, AskFileMessage
 from chainlit.user_session import user_session
 from chainlit.sync import run_sync, make_async
+from chainlit.cache import cache
 
 if LANGCHAIN_INSTALLED:
     from chainlit.lc.callbacks import (
         ChainlitCallbackHandler,
         AsyncChainlitCallbackHandler,
     )
 
@@ -245,8 +246,9 @@
     "on_stop",
     "action_callback",
     "sleep",
     "ChainlitCallbackHandler",
     "AsyncChainlitCallbackHandler",
     "run_sync",
     "make_async",
+    "cache",
 ]
```

### Comparing `chainlit-0.4.0/chainlit/action.py` & `chainlit-0.4.1/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/cli/__init__.py` & `chainlit-0.4.1/chainlit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/cli/auth.py` & `chainlit-0.4.1/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/cli/deploy.py` & `chainlit-0.4.1/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/cli/mock.py` & `chainlit-0.4.1/chainlit/cli/mock.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/cli/utils.py` & `chainlit-0.4.1/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/client.py` & `chainlit-0.4.1/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/config.py` & `chainlit-0.4.1/chainlit/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Any, Callable, List, Dict, TYPE_CHECKING
 import os
 import sys
 import tomli
 from pydantic.dataclasses import dataclass
 from dataclasses_json import dataclass_json
-from importlib import machinery
+from importlib import util
 from chainlit.logger import logger
 from chainlit.version import __version__
 
 if TYPE_CHECKING:
     from chainlit.action import Action
 
 PACKAGE_ROOT = os.path.dirname(__file__)
@@ -99,14 +99,39 @@
     on_message: Optional[Callable[[str], Any]] = None
     lc_agent_is_async: Optional[bool] = None
     lc_run: Optional[Callable[[Any, str], str]] = None
     lc_postprocess: Optional[Callable[[Any], str]] = None
     lc_factory: Optional[Callable[[], Any]] = None
     lc_rename: Optional[Callable[[str], str]] = None
 
+    def validate(self):
+        requires_one_of = [
+            "lc_factory",
+            "on_message",
+            "on_chat_start",
+        ]
+
+        mutually_exclusive = ["lc_factory"]
+
+        # Check if at least one of the required attributes is set
+        if not any(getattr(self, attr) for attr in requires_one_of):
+            raise ValueError(
+                f"Module should at least expose one of {', '.join(requires_one_of)} function"
+            )
+
+        # Check if any mutually exclusive attributes are set together
+        for i, attr1 in enumerate(mutually_exclusive):
+            for attr2 in mutually_exclusive[i + 1 :]:
+                if getattr(self, attr1) and getattr(self, attr2):
+                    raise ValueError(
+                        f"Module should not expose both {attr1} and {attr2} functions"
+                    )
+
+        return True
+
 
 @dataclass_json
 @dataclass()
 class ProjectSettings:
     # Enables Cloud features if provided
     id: Optional[str] = None
     # Whether the app is available to anonymous users or only to team members.
@@ -141,43 +166,34 @@
         with open(config_file, "w", encoding="utf-8") as f:
             f.write(DEFAULT_CONFIG_STR)
             logger.info(f"Created default config file at {config_file}")
     elif log:
         logger.info(f"Config file already exists at {config_file}")
 
 
-def reset_module_config():
-    if not config:
-        return
-
-    config.code = CodeSettings(action_callbacks={})
-
-
 def load_module(target: str):
     """Load the specified module."""
 
-    # Reset the config fields that belonged to the previous module
-    reset_module_config()
-
     # Get the target's directory
     target_dir = os.path.dirname(os.path.abspath(target))
 
     # Add the target's directory to the Python path
     sys.path.insert(0, target_dir)
 
-    loader = machinery.SourceFileLoader(target, target)
-    config.code.module = loader.load_module()
+    spec = util.spec_from_file_location(target, target)
+    module = util.module_from_spec(spec)
+    spec.loader.exec_module(module)
 
     # Remove the target's directory from the Python path
     sys.path.pop(0)
 
+    config.code.validate()
 
-def load_config():
-    """Load the configuration from the config file."""
-    init_config()
+
+def load_settings():
     with open(config_file, "rb") as f:
         toml_dict = tomli.load(f)
         # Load project settings
         project_config = toml_dict.get("project", {})
         ui_settings = toml_dict.get("UI", {})
         meta = toml_dict.get("meta")
 
@@ -189,23 +205,47 @@
         lc_cache_path = os.path.join(config_dir, ".langchain.db")
 
         project_settings = ProjectSettings(
             lc_cache_path=lc_cache_path, **project_config
         )
         ui_settings = UISettings(**ui_settings)
 
-        if not project_settings.public and not project_settings.project_id:
+        if not project_settings.public and not project_settings.id:
             raise ValueError("Project ID is required when public is set to false.")
 
-        config = ChainlitConfig(
-            chainlit_server=chainlit_server,
-            chainlit_prod_url=chainlit_prod_url,
-            ui=ui_settings,
-            run=RunSettings(),
-            project=project_settings,
-            code=CodeSettings(action_callbacks={}),
-        )
+        return {
+            "ui": ui_settings,
+            "project": project_settings,
+            "code": CodeSettings(action_callbacks={}),
+        }
+
+
+def reload_config():
+    """Reload the configuration from the config file."""
+    global config
+    if config is None:
+        return
+
+    settings = load_settings()
+
+    config.code = settings["code"]
+    config.ui = settings["ui"]
+    config.project = settings["project"]
+
+
+def load_config():
+    """Load the configuration from the config file."""
+    init_config()
+
+    settings = load_settings()
+
+    config = ChainlitConfig(
+        chainlit_server=chainlit_server,
+        chainlit_prod_url=chainlit_prod_url,
+        run=RunSettings(),
+        **settings,
+    )
 
     return config
 
 
 config = load_config()
```

### Comparing `chainlit-0.4.0/chainlit/element.py` & `chainlit-0.4.1/chainlit/element.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/emitter.py` & `chainlit-0.4.1/chainlit/emitter.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/frontend/dist/assets/index-0cc9e355.css` & `chainlit-0.4.1/chainlit/frontend/dist/assets/index-f93cc942.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-body{margin:0;padding:0;font-family:Inter,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}.markdown-body *:first-child{margin-top:0}.markdown-body *:last-child{margin-bottom:0}.markdown-body p{white-space:break-spaces}.DraftEditor-editorContainer,.DraftEditor-root,.public-DraftEditor-content{height:inherit;text-align:initial}.public-DraftEditor-content[contenteditable=true]{-webkit-user-modify:read-write-plaintext-only}.DraftEditor-root{position:relative}.DraftEditor-editorContainer{background-color:#fff0;border-left:.1px solid transparent;position:relative;z-index:1}.public-DraftEditor-block{position:relative}.DraftEditor-alignLeft .public-DraftStyleDefault-block{text-align:left}.DraftEditor-alignLeft .public-DraftEditorPlaceholder-root{left:0;text-align:left}.DraftEditor-alignCenter .public-DraftStyleDefault-block{text-align:center}.DraftEditor-alignCenter .public-DraftEditorPlaceholder-root{margin:0 auto;text-align:center;width:100%}.DraftEditor-alignRight .public-DraftStyleDefault-block{text-align:right}.DraftEditor-alignRight .public-DraftEditorPlaceholder-root{right:0;text-align:right}.public-DraftEditorPlaceholder-root{color:#9197a3;position:absolute;width:100%;z-index:1}.public-DraftEditorPlaceholder-hasFocus{color:#bdc1c9}.DraftEditorPlaceholder-hidden{display:none}.public-DraftStyleDefault-block{position:relative;white-space:pre-wrap}.public-DraftStyleDefault-ltr{direction:ltr;text-align:left}.public-DraftStyleDefault-rtl{direction:rtl;text-align:right}.public-DraftStyleDefault-listLTR{direction:ltr}.public-DraftStyleDefault-listRTL{direction:rtl}.public-DraftStyleDefault-ol,.public-DraftStyleDefault-ul{margin:16px 0;padding:0}.public-DraftStyleDefault-depth0.public-DraftStyleDefault-listLTR{margin-left:1.5em}.public-DraftStyleDefault-depth0.public-DraftStyleDefault-listRTL{margin-right:1.5em}.public-DraftStyleDefault-depth1.public-DraftStyleDefault-listLTR{margin-left:3em}.public-DraftStyleDefault-depth1.public-DraftStyleDefault-listRTL{margin-right:3em}.public-DraftStyleDefault-depth2.public-DraftStyleDefault-listLTR{margin-left:4.5em}.public-DraftStyleDefault-depth2.public-DraftStyleDefault-listRTL{margin-right:4.5em}.public-DraftStyleDefault-depth3.public-DraftStyleDefault-listLTR{margin-left:6em}.public-DraftStyleDefault-depth3.public-DraftStyleDefault-listRTL{margin-right:6em}.public-DraftStyleDefault-depth4.public-DraftStyleDefault-listLTR{margin-left:7.5em}.public-DraftStyleDefault-depth4.public-DraftStyleDefault-listRTL{margin-right:7.5em}.public-DraftStyleDefault-unorderedListItem{list-style-type:square;position:relative}.public-DraftStyleDefault-unorderedListItem.public-DraftStyleDefault-depth0{list-style-type:disc}.public-DraftStyleDefault-unorderedListItem.public-DraftStyleDefault-depth1{list-style-type:circle}.public-DraftStyleDefault-orderedListItem{list-style-type:none;position:relative}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-listLTR:before{left:-36px;position:absolute;text-align:right;width:30px}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-listRTL:before{position:absolute;right:-36px;text-align:left;width:30px}.public-DraftStyleDefault-orderedListItem:before{content:counter(ol0) ". ";counter-increment:ol0}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth1:before{content:counter(ol1,lower-alpha) ". ";counter-increment:ol1}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth2:before{content:counter(ol2,lower-roman) ". ";counter-increment:ol2}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth3:before{content:counter(ol3) ". ";counter-increment:ol3}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth4:before{content:counter(ol4,lower-alpha) ". ";counter-increment:ol4}.public-DraftStyleDefault-depth0.public-DraftStyleDefault-reset{counter-reset:ol0}.public-DraftStyleDefault-depth1.public-DraftStyleDefault-reset{counter-reset:ol1}.public-DraftStyleDefault-depth2.public-DraftStyleDefault-reset{counter-reset:ol2}.public-DraftStyleDefault-depth3.public-DraftStyleDefault-reset{counter-reset:ol3}.public-DraftStyleDefault-depth4.public-DraftStyleDefault-reset{counter-reset:ol4}.react-resizable{position:relative}.react-resizable-handle{position:absolute;width:20px;height:20px;background-repeat:no-repeat;background-origin:content-box;box-sizing:border-box;background-image:url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2IDYiIHN0eWxlPSJiYWNrZ3JvdW5kLWNvbG9yOiNmZmZmZmYwMCIgeD0iMHB4IiB5PSIwcHgiIHdpZHRoPSI2cHgiIGhlaWdodD0iNnB4Ij48ZyBvcGFjaXR5PSIwLjMwMiI+PHBhdGggZD0iTSA2IDYgTCAwIDYgTCAwIDQuMiBMIDQgNC4yIEwgNC4yIDQuMiBMIDQuMiAwIEwgNiAwIEwgNiA2IEwgNiA2IFoiIGZpbGw9IiMwMDAwMDAiLz48L2c+PC9zdmc+);background-position:bottom right;padding:0 3px 3px 0}.react-resizable-handle-sw{bottom:0;left:0;cursor:sw-resize;transform:rotate(90deg)}.react-resizable-handle-se{bottom:0;right:0;cursor:se-resize}.react-resizable-handle-nw{top:0;left:0;cursor:nw-resize;transform:rotate(180deg)}.react-resizable-handle-ne{top:0;right:0;cursor:ne-resize;transform:rotate(270deg)}.react-resizable-handle-w,.react-resizable-handle-e{top:50%;margin-top:-10px;cursor:ew-resize}.react-resizable-handle-w{left:0;transform:rotate(135deg)}.react-resizable-handle-e{right:0;transform:rotate(315deg)}.react-resizable-handle-n,.react-resizable-handle-s{left:50%;margin-left:-10px;cursor:ns-resize}.react-resizable-handle-n{top:0;transform:rotate(225deg)}.react-resizable-handle-s{bottom:0;transform:rotate(45deg)}
+body{margin:0;padding:0;font-family:Inter,sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}.markdown-body{overflow-x:auto}.markdown-body *:first-child{margin-top:0}.markdown-body *:last-child{margin-bottom:0}.markdown-body p{white-space:break-spaces}.DraftEditor-editorContainer,.DraftEditor-root,.public-DraftEditor-content{height:inherit;text-align:initial}.public-DraftEditor-content[contenteditable=true]{-webkit-user-modify:read-write-plaintext-only}.DraftEditor-root{position:relative}.DraftEditor-editorContainer{background-color:#fff0;border-left:.1px solid transparent;position:relative;z-index:1}.public-DraftEditor-block{position:relative}.DraftEditor-alignLeft .public-DraftStyleDefault-block{text-align:left}.DraftEditor-alignLeft .public-DraftEditorPlaceholder-root{left:0;text-align:left}.DraftEditor-alignCenter .public-DraftStyleDefault-block{text-align:center}.DraftEditor-alignCenter .public-DraftEditorPlaceholder-root{margin:0 auto;text-align:center;width:100%}.DraftEditor-alignRight .public-DraftStyleDefault-block{text-align:right}.DraftEditor-alignRight .public-DraftEditorPlaceholder-root{right:0;text-align:right}.public-DraftEditorPlaceholder-root{color:#9197a3;position:absolute;width:100%;z-index:1}.public-DraftEditorPlaceholder-hasFocus{color:#bdc1c9}.DraftEditorPlaceholder-hidden{display:none}.public-DraftStyleDefault-block{position:relative;white-space:pre-wrap}.public-DraftStyleDefault-ltr{direction:ltr;text-align:left}.public-DraftStyleDefault-rtl{direction:rtl;text-align:right}.public-DraftStyleDefault-listLTR{direction:ltr}.public-DraftStyleDefault-listRTL{direction:rtl}.public-DraftStyleDefault-ol,.public-DraftStyleDefault-ul{margin:16px 0;padding:0}.public-DraftStyleDefault-depth0.public-DraftStyleDefault-listLTR{margin-left:1.5em}.public-DraftStyleDefault-depth0.public-DraftStyleDefault-listRTL{margin-right:1.5em}.public-DraftStyleDefault-depth1.public-DraftStyleDefault-listLTR{margin-left:3em}.public-DraftStyleDefault-depth1.public-DraftStyleDefault-listRTL{margin-right:3em}.public-DraftStyleDefault-depth2.public-DraftStyleDefault-listLTR{margin-left:4.5em}.public-DraftStyleDefault-depth2.public-DraftStyleDefault-listRTL{margin-right:4.5em}.public-DraftStyleDefault-depth3.public-DraftStyleDefault-listLTR{margin-left:6em}.public-DraftStyleDefault-depth3.public-DraftStyleDefault-listRTL{margin-right:6em}.public-DraftStyleDefault-depth4.public-DraftStyleDefault-listLTR{margin-left:7.5em}.public-DraftStyleDefault-depth4.public-DraftStyleDefault-listRTL{margin-right:7.5em}.public-DraftStyleDefault-unorderedListItem{list-style-type:square;position:relative}.public-DraftStyleDefault-unorderedListItem.public-DraftStyleDefault-depth0{list-style-type:disc}.public-DraftStyleDefault-unorderedListItem.public-DraftStyleDefault-depth1{list-style-type:circle}.public-DraftStyleDefault-orderedListItem{list-style-type:none;position:relative}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-listLTR:before{left:-36px;position:absolute;text-align:right;width:30px}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-listRTL:before{position:absolute;right:-36px;text-align:left;width:30px}.public-DraftStyleDefault-orderedListItem:before{content:counter(ol0) ". ";counter-increment:ol0}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth1:before{content:counter(ol1,lower-alpha) ". ";counter-increment:ol1}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth2:before{content:counter(ol2,lower-roman) ". ";counter-increment:ol2}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth3:before{content:counter(ol3) ". ";counter-increment:ol3}.public-DraftStyleDefault-orderedListItem.public-DraftStyleDefault-depth4:before{content:counter(ol4,lower-alpha) ". ";counter-increment:ol4}.public-DraftStyleDefault-depth0.public-DraftStyleDefault-reset{counter-reset:ol0}.public-DraftStyleDefault-depth1.public-DraftStyleDefault-reset{counter-reset:ol1}.public-DraftStyleDefault-depth2.public-DraftStyleDefault-reset{counter-reset:ol2}.public-DraftStyleDefault-depth3.public-DraftStyleDefault-reset{counter-reset:ol3}.public-DraftStyleDefault-depth4.public-DraftStyleDefault-reset{counter-reset:ol4}.react-resizable{position:relative}.react-resizable-handle{position:absolute;width:20px;height:20px;background-repeat:no-repeat;background-origin:content-box;box-sizing:border-box;background-image:url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2IDYiIHN0eWxlPSJiYWNrZ3JvdW5kLWNvbG9yOiNmZmZmZmYwMCIgeD0iMHB4IiB5PSIwcHgiIHdpZHRoPSI2cHgiIGhlaWdodD0iNnB4Ij48ZyBvcGFjaXR5PSIwLjMwMiI+PHBhdGggZD0iTSA2IDYgTCAwIDYgTCAwIDQuMiBMIDQgNC4yIEwgNC4yIDQuMiBMIDQuMiAwIEwgNiAwIEwgNiA2IEwgNiA2IFoiIGZpbGw9IiMwMDAwMDAiLz48L2c+PC9zdmc+);background-position:bottom right;padding:0 3px 3px 0}.react-resizable-handle-sw{bottom:0;left:0;cursor:sw-resize;transform:rotate(90deg)}.react-resizable-handle-se{bottom:0;right:0;cursor:se-resize}.react-resizable-handle-nw{top:0;left:0;cursor:nw-resize;transform:rotate(180deg)}.react-resizable-handle-ne{top:0;right:0;cursor:ne-resize;transform:rotate(270deg)}.react-resizable-handle-w,.react-resizable-handle-e{top:50%;margin-top:-10px;cursor:ew-resize}.react-resizable-handle-w{left:0;transform:rotate(135deg)}.react-resizable-handle-e{right:0;transform:rotate(315deg)}.react-resizable-handle-n,.react-resizable-handle-s{left:50%;margin-left:-10px;cursor:ns-resize}.react-resizable-handle-n{top:0;transform:rotate(225deg)}.react-resizable-handle-s{bottom:0;transform:rotate(45deg)}
```

### Comparing `chainlit-0.4.0/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.4.1/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.4.1/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/frontend/dist/favicon.svg` & `chainlit-0.4.1/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/frontend/dist/index.html` & `chainlit-0.4.1/chainlit/frontend/dist/index.html`

 * *Files 27% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <link
       href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
       rel="stylesheet"
     />
     <script>
       const global = globalThis;
     </script>
-    <script type="module" crossorigin src="/assets/index-9e4bccd1.js"></script>
-    <link rel="stylesheet" href="/assets/index-0cc9e355.css">
+    <script type="module" crossorigin src="/assets/index-68c36c96.js"></script>
+    <link rel="stylesheet" href="/assets/index-f93cc942.css">
   </head>
   <body>
     <div id="root"></div>
     
   </body>
 </html>
```

### Comparing `chainlit-0.4.0/chainlit/lc/agent.py` & `chainlit-0.4.1/chainlit/lc/agent.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/lc/callbacks.py` & `chainlit-0.4.1/chainlit/lc/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/markdown.py` & `chainlit-0.4.1/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/message.py` & `chainlit-0.4.1/chainlit/message.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/server.py` & `chainlit-0.4.1/chainlit/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     FileResponse,
     PlainTextResponse,
 )
 from fastapi_socketio import SocketManager
 from starlette.middleware.cors import CORSMiddleware
 import asyncio
 
-from chainlit.config import config, load_module, DEFAULT_HOST
+from chainlit.config import config, load_module, reload_config, DEFAULT_HOST
 from chainlit.session import Session, sessions
 from chainlit.user_session import user_sessions
 from chainlit.client import CloudClient
 from chainlit.emitter import ChainlitEmitter
 from chainlit.markdown import get_markdown_str
 from chainlit.action import Action
 from chainlit.message import Message, ErrorMessage
@@ -42,48 +42,67 @@
     if not config.run.headless:
         if host == DEFAULT_HOST:
             url = f"http://localhost:{port}"
         else:
             url = f"http://{host}:{port}"
 
         logger.info(f"Your app is available at {url}")
+
+        # Add a delay before opening the browser
+        await asyncio.sleep(1)
         webbrowser.open(url)
 
     watch_task = None
     stop_event = asyncio.Event()
 
     if config.run.watch:
 
         async def watch_files_for_changes():
+            extensions = [".py"]
+            files = ["chainlit.md", "config.toml"]
             async for changes in awatch(config.root, stop_event=stop_event):
                 for change_type, file_path in changes:
                     file_name = os.path.basename(file_path)
                     file_ext = os.path.splitext(file_name)[1]
 
-                    if file_ext.lower() == ".py" or file_name.lower() == "chainlit.md":
-                        logger.info(f"File {change_type.name}: {file_name}")
+                    if file_ext.lower() in extensions or file_name.lower() in files:
+                        logger.info(
+                            f"File {change_type.name}: {file_name}. Reloading app..."
+                        )
+
+                        try:
+                            reload_config()
+                        except Exception as e:
+                            logger.error(f"Error reloading config: {e}")
+                            break
 
                         # Reload the module if the module name is specified in the config
                         if config.run.module_name:
-                            load_module(config.run.module_name)
+                            try:
+                                load_module(config.run.module_name)
+                            except Exception as e:
+                                logger.error(f"Error reloading module: {e}")
+                                break
 
                         await socket.emit("reload", {})
 
                         break
 
         watch_task = asyncio.create_task(watch_files_for_changes())
 
     try:
         yield
-    except KeyboardInterrupt:
-        logger.error("KeyboardInterrupt received, stopping the watch task...")
     finally:
         if watch_task:
-            stop_event.set()
-            await watch_task
+            try:
+                stop_event.set()
+                watch_task.cancel()
+                await watch_task
+            except asyncio.exceptions.CancelledError:
+                pass
 
 
 root_dir = os.path.dirname(os.path.abspath(__file__))
 build_dir = os.path.join(root_dir, "frontend/dist")
 
 app = FastAPI(lifespan=lifespan)
 
@@ -215,55 +234,46 @@
 
 @socket.on("connect")
 async def connect(sid, environ):
     user_env = environ.get("HTTP_USER_ENV")
     authorization = environ.get("HTTP_AUTHORIZATION")
     cloud_client = None
 
-    # Check decorated functions
-    if (
-        not config.code.lc_factory
-        and not config.code.on_message
-        and not config.code.on_chat_start
-    ):
-        logger.error(
-            "Module should at least expose one of @langchain_factory, @on_message or @on_chat_start function"
-        )
-        return False
-
     # Check authorization
     if not config.project.public and not authorization:
         # Refuse connection if the app is private and no access token is provided
         trace_event("no_access_token")
-        logger.error("No access token provided")
+        logger.error("Connection refused: No access token provided")
         return False
     elif authorization and config.project.id:
         # Create the cloud client
         cloud_client = CloudClient(
             project_id=config.project.id,
             session_id=sid,
             access_token=authorization,
         )
         is_project_member = await cloud_client.is_project_member()
         if not is_project_member:
-            logger.error("You are not a member of this project")
+            logger.error("Connection refused: You are not a member of this project")
             return False
 
     # Check user env
     if config.project.user_env:
         # Check if requested user environment variables are provided
         if user_env:
             user_env = json.loads(user_env)
             for key in config.project.user_env:
                 if key not in user_env:
                     trace_event("missing_user_env")
-                    logger.error("Missing user environment variable: " + key)
+                    logger.error(
+                        "Connection refused: Missing user environment variable: " + key
+                    )
                     return False
         else:
-            logger.error("Missing user environment variables")
+            logger.error("Connection refused: Missing user environment variables")
             return False
 
     # Create the session
 
     # Function to send a message to this particular session
     def emit_fn(event, data):
         if sid in sessions:
```

### Comparing `chainlit-0.4.0/chainlit/session.py` & `chainlit-0.4.1/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/sync.py` & `chainlit-0.4.1/chainlit/sync.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/telemetry.py` & `chainlit-0.4.1/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/types.py` & `chainlit-0.4.1/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/chainlit/user_session.py` & `chainlit-0.4.1/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.0/pyproject.toml` & `chainlit-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "0.4.0"
+version = "0.4.1"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'langchain']
 description = "A faster way to build chatbot UIs."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
```

### Comparing `chainlit-0.4.0/PKG-INFO` & `chainlit-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.4.0
+Version: 0.4.1
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -40,14 +40,16 @@
 
 Chainlit lets you create ChatGPT-like UIs on top of any Python code in minutes! Some of the key features include intermediary steps visualisation, element management & display (images, text, carousel, etc.) as well as cloud deployment.
 
 [![](https://dcbadge.vercel.app/api/server/ZThrUxbAYw?style=flat)](https://discord.gg/ZThrUxbAYw)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/chainlit_io.svg?style=social&label=Follow%20%40chainlit_io)](https://twitter.com/chainlit_io)
 [![CI](https://github.com/Chainlit/chainlit/actions/workflows/ci.yaml/badge.svg)](https://github.com/Chainlit/chainlit/actions/workflows/ci.yaml)
 
+https://github.com/Chainlit/chainlit/assets/13104895/e347e52c-35b2-4c35-8a88-f8ac02dd198e
+
 ## Installation
 
 Open a terminal and run:
 
 ```bash
 $ pip install chainlit
 $ chainlit hello
```

