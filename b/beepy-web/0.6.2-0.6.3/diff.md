# Comparing `tmp/beepy_web-0.6.2.tar.gz` & `tmp/beepy_web-0.6.3.tar.gz`

## Comparing `beepy_web-0.6.2.tar` & `beepy_web-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.6.2/.python-version
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy.css
--rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 beepy_web-0.6.2/dev-requirements.txt
--rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 beepy_web-0.6.2/js.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.6.2/requirements.txt
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/actions.py
--rw-r--r--   0        0        0    13271 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/attrs.py
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/children.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/context.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/context_menu.py
--rwxr-xr-x   0        0        0     2926 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/dev.py
--rw-r--r--   0        0        0    28583 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/framework.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/import_hooks.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/init.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/listeners.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/local_storage.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/modal.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/plot.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/router.py
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/style.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/table.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/tabs.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/tags.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/trackable.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/types.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/utils.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.6.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.6.2/LICENSE
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 beepy_web-0.6.2/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 beepy_web-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 beepy_web-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.6.3/.python-version
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy.css
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 beepy_web-0.6.3/dev-requirements.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.6.3/requirements.txt
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/actions.py
+-rw-r--r--   0        0        0    13271 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/attrs.py
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/children.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/context.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/context_menu.py
+-rwxr-xr-x   0        0        0     2800 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/dev.py
+-rw-r--r--   0        0        0    28583 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/framework.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/import_hooks.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/init.py
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/js.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/listeners.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/local_storage.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/modal.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/plot.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/router.py
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/style.py
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/table.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/tabs.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/tags.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/trackable.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/types.py
+-rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 beepy_web-0.6.3/beepy/utils.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 beepy_web-0.6.3/README.md
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 beepy_web-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 beepy_web-0.6.3/PKG-INFO
```

### Comparing `beepy_web-0.6.2/beepy.css` & `beepy_web-0.6.3/beepy.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy.js` & `beepy_web-0.6.3/beepy.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/js.py` & `beepy_web-0.6.3/beepy/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/__init__.py` & `beepy_web-0.6.3/beepy/init.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/attrs.py` & `beepy_web-0.6.3/beepy/attrs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/children.py` & `beepy_web-0.6.3/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/context.py` & `beepy_web-0.6.3/beepy/context.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/context_menu.py` & `beepy_web-0.6.3/beepy/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/dev.py` & `beepy_web-0.6.3/beepy/dev.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 #!/usr/bin/env python3
 import os
 
-try:
-    import websockets as _
-except ImportError:
-    print('Did you forget to install dev-requirements.txt?')
-    exit(1)
-
 import sys
 import time
 import asyncio
 import http.server
 import socketserver
 from threading import Thread
 from websockets.server import serve
```

### Comparing `beepy_web-0.6.2/beepy/framework.py` & `beepy_web-0.6.3/beepy/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from beepy.types import safe_html, Renderer, Mounter, WebBase, AttrType, ContentType
 from beepy.utils import (
     log, NONE_TYPE, _PY_TAG_ATTRIBUTE, __CONFIG__, _debugger, get_random_name, to_kebab_case, IN_BROWSER, to_js
 )
 from beepy.context import OVERWRITE, SUPER, CONTENT, _SPECIAL_CHILD_STRINGS, _MetaContext, Context
 
 
-__version__ = '0.6.2'
+__version__ = '0.6.3'
 __CONFIG__['version'] = __version__
 
 
 if IN_BROWSER:
     js.Element.__str__ = lambda self: f'<{self.tagName.lower()}/>'
 _current__lifecycle_method: dict[str, dict[int, 'Tag']] = {}
```

### Comparing `beepy_web-0.6.2/beepy/import_hooks.py` & `beepy_web-0.6.3/beepy/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/listeners.py` & `beepy_web-0.6.3/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/local_storage.py` & `beepy_web-0.6.3/beepy/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/modal.py` & `beepy_web-0.6.3/beepy/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/router.py` & `beepy_web-0.6.3/beepy/router.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/style.py` & `beepy_web-0.6.3/beepy/style.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/table.py` & `beepy_web-0.6.3/beepy/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/tabs.py` & `beepy_web-0.6.3/beepy/tabs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/tags.py` & `beepy_web-0.6.3/beepy/tags.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/trackable.py` & `beepy_web-0.6.3/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/types.py` & `beepy_web-0.6.3/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/beepy/utils.py` & `beepy_web-0.6.3/beepy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import dataclasses
 import json
 import math
 import re
 import sys
 import string
 import random
-# TODO: add some param to use shadow root directlyimport inspect
+# TODO: add some param to use shadow root directly
 import traceback
 import asyncio
 from functools import wraps
-from typing import Any
 from datetime import datetime
 from importlib import import_module
 
 import js
 import micropip
 from pyodide import http as pyodide_http
 import beepy
```

### Comparing `beepy_web-0.6.2/.gitignore` & `beepy_web-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/LICENSE` & `beepy_web-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/README.md` & `beepy_web-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.2/PKG-INFO` & `beepy_web-0.6.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.6.2
+Version: 0.6.3
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.10
+Provides-Extra: dev
+Requires-Dist: micropip; extra == 'dev'
+Requires-Dist: pyodide==0.19.0a1; extra == 'dev'
+Requires-Dist: watchdog; extra == 'dev'
+Requires-Dist: websockets; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # 🐝 BeePy
 
 ## The _frontend_ web framework for python 
 ### Thanks for [Pyodide](https://pyodide.org/) - port of Python to [Emscripten](https://emscripten.org/), based on [WASM](https://webassembly.org/).
 ### Use Python in browser to build modern frontend via BeePy!
```

