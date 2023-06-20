# Comparing `tmp/beepy_web-0.6.1.tar.gz` & `tmp/beepy_web-0.6.2.tar.gz`

## Comparing `beepy_web-0.6.1.tar` & `beepy_web-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.6.1/.python-version
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy.css
--rw-r--r--   0        0        0    14109 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 beepy_web-0.6.1/dev-requirements.txt
--rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 beepy_web-0.6.1/js.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.6.1/requirements.txt
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/actions.py
--rw-r--r--   0        0        0    13271 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/attrs.py
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/children.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/context.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/context_menu.py
--rwxr-xr-x   0        0        0     2926 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/dev.py
--rw-r--r--   0        0        0    28583 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/framework.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/import_hooks.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/init.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/listeners.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/local_storage.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/modal.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/plot.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/router.py
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/style.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/table.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/tabs.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/tags.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/trackable.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/types.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 beepy_web-0.6.1/beepy/utils.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.6.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.6.1/LICENSE
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 beepy_web-0.6.1/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 beepy_web-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 beepy_web-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 beepy_web-0.6.2/.python-version
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy.css
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 beepy_web-0.6.2/dev-requirements.txt
+-rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 beepy_web-0.6.2/js.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 beepy_web-0.6.2/requirements.txt
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/actions.py
+-rw-r--r--   0        0        0    13271 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/attrs.py
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/children.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/context.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/context_menu.py
+-rwxr-xr-x   0        0        0     2926 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/dev.py
+-rw-r--r--   0        0        0    28583 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/framework.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/import_hooks.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/init.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/listeners.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/local_storage.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/modal.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/plot.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/router.py
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/style.py
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/table.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/tabs.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/tags.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/trackable.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/types.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 beepy_web-0.6.2/beepy/utils.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 beepy_web-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 beepy_web-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 beepy_web-0.6.2/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 beepy_web-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 beepy_web-0.6.2/PKG-INFO
```

### Comparing `beepy_web-0.6.1/beepy.css` & `beepy_web-0.6.2/beepy.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy.js` & `beepy_web-0.6.2/beepy.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -317,18 +317,23 @@
     beepy.__CONFIG__.__loading = true
 
     try { // TODO: add flag parameter for this
         beepy.DEV__hot_reload_ws = new WebSocket('ws://localhost:8998/')
     } catch (e) {} // Dev Hot Reload server is not started
     beepy.DEV__hot_reload = !!beepy.DEV__hot_reload_ws
     if (beepy.DEV__hot_reload) {
+        await apy('import importlib as _dev_importlib; import sys as _dev_sys')
         beepy.DEV__hot_reload_ws.onmessage = async ({
             data
         }) => {
-            await beepy._writeLocalFile(data)
+            // TODO: FIX THIS
+            // `data` - filename, that was changed, but due to enterPythonModule,
+            // we cannot be sure where really file must be pushed
+            // await beepy._writeLocalFile(data)
+            await apy(`_dev_importlib.reload(_dev_sys.modules['${rootFolder}'])`)
             await _main({
                 reload: true
             })
         }
     }
 
     console.log(pyodide._api.sys.version)
```

### Comparing `beepy_web-0.6.1/js.py` & `beepy_web-0.6.2/js.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/__init__.py` & `beepy_web-0.6.2/beepy/__init__.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/attrs.py` & `beepy_web-0.6.2/beepy/attrs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/children.py` & `beepy_web-0.6.2/beepy/children.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/context.py` & `beepy_web-0.6.2/beepy/context.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/context_menu.py` & `beepy_web-0.6.2/beepy/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/dev.py` & `beepy_web-0.6.2/beepy/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/framework.py` & `beepy_web-0.6.2/beepy/framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from beepy.types import safe_html, Renderer, Mounter, WebBase, AttrType, ContentType
 from beepy.utils import (
     log, NONE_TYPE, _PY_TAG_ATTRIBUTE, __CONFIG__, _debugger, get_random_name, to_kebab_case, IN_BROWSER, to_js
 )
 from beepy.context import OVERWRITE, SUPER, CONTENT, _SPECIAL_CHILD_STRINGS, _MetaContext, Context
 
 
-__version__ = '0.6.1'
+__version__ = '0.6.2'
 __CONFIG__['version'] = __version__
 
 
 if IN_BROWSER:
     js.Element.__str__ = lambda self: f'<{self.tagName.lower()}/>'
 _current__lifecycle_method: dict[str, dict[int, 'Tag']] = {}
```

### Comparing `beepy_web-0.6.1/beepy/import_hooks.py` & `beepy_web-0.6.2/beepy/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/init.py` & `beepy_web-0.6.2/beepy/init.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/listeners.py` & `beepy_web-0.6.2/beepy/listeners.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/local_storage.py` & `beepy_web-0.6.2/beepy/local_storage.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/modal.py` & `beepy_web-0.6.2/beepy/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/router.py` & `beepy_web-0.6.2/beepy/router.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/style.py` & `beepy_web-0.6.2/beepy/style.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/table.py` & `beepy_web-0.6.2/beepy/table.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/tabs.py` & `beepy_web-0.6.2/beepy/tabs.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/tags.py` & `beepy_web-0.6.2/beepy/tags.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/trackable.py` & `beepy_web-0.6.2/beepy/trackable.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/types.py` & `beepy_web-0.6.2/beepy/types.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/beepy/utils.py` & `beepy_web-0.6.2/beepy/utils.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/.gitignore` & `beepy_web-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/LICENSE` & `beepy_web-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/README.md` & `beepy_web-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/pyproject.toml` & `beepy_web-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.6.1/PKG-INFO` & `beepy_web-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.6.1
+Version: 0.6.2
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://bee-py.readthedocs.io/en/latest/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

