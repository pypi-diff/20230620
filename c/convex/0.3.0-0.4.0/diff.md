# Comparing `tmp/convex-0.3.0.tar.gz` & `tmp/convex-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convex-0.3.0.tar", max compression
+gzip compressed data, was "convex-0.4.0.tar", max compression
```

## Comparing `convex-0.3.0.tar` & `convex-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11343 2023-04-11 18:46:13.543061 convex-0.3.0/LICENSE
--rw-r--r--   0        0        0     9588 2023-04-18 23:43:48.499613 convex-0.3.0/README.md
--rw-r--r--   0        0        0     3529 2023-04-18 23:43:48.499788 convex-0.3.0/convex/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 18:46:13.543422 convex-0.3.0/convex/py.typed
--rw-r--r--   0        0        0    21018 2023-04-11 18:46:13.543566 convex-0.3.0/convex/values.py
--rw-r--r--   0        0        0     1258 2023-04-18 23:43:48.499938 convex-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10517 1970-01-01 00:00:00.000000 convex-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-02-25 00:40:22.088939 convex-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10544 2023-06-20 20:09:34.647736 convex-0.4.0/README.md
+-rw-r--r--   0        0        0     3805 2023-06-20 20:09:34.647888 convex-0.4.0/convex/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-25 00:40:22.089306 convex-0.4.0/convex/py.typed
+-rw-r--r--   0        0        0    19746 2023-06-20 20:09:34.648774 convex-0.4.0/convex/values.py
+-rw-r--r--   0        0        0     1285 2023-06-20 20:09:34.649316 convex-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11473 1970-01-01 00:00:00.000000 convex-0.4.0/PKG-INFO
```

### Comparing `convex-0.3.0/LICENSE` & `convex-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `convex-0.3.0/README.md` & `convex-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 >>> client.mutation("sendMessage", dict(author="Me", body="Hello!"))
 ```
 
 To find the url of your convex backend, open the deployment you want to work
 with in the appropriate project in the
 [Convex dashboard](https://dashboard.convex.dev) and click "Settings" where the
 Deployment URL should be visible. To find out which queries, mutations, and
-actions are available check the Functions pane in the Dashboard
+actions are available check the Functions pane in the dashboard.
 
 To see logs emitted from Convex functions, set the debug mode to True.
 
 ```python
 >>> client.set_debug(True)
 ```
 
@@ -166,12 +166,48 @@
 >>> s
 ConvexMap([({'a': 1.0}, 123.0), ('b', 456.0)])
 ```
 
 ConvexMaps perform a copy of each inserted key/value pair, so they require more
 memory than Python's builtin dictionaries.
 
+# Pagination
+
+[Paginated queries](https://docs.convex.dev/database/pagination) are queries
+that accept pagination options as an argument and can be called repeatedly to
+produce additional "pages" of results.
+
+For a paginated query like this:
+
+```javascript
+import { query } from "./_generated/server";
+
+export default query(async ({ db }, { paginationOpts }) => {
+  return await db.query("messages").order("desc").paginate(paginationOpts);
+});
+```
+
+and returning all results 5 at a time in Python looks like this:
+
+```python
+import convex
+client = convex.ConvexClient('https://happy-animal-123.convex.cloud')
+
+done = False
+cursor = None
+data = []
+
+while not done:
+    result = client.query('listMessages', {"paginationOpts": {"numItems": 5, "cursor": cursor}})
+    cursor = result['continueCursor']
+    done = result["isDone"]
+    data.extend(result['page'])
+    print('got', len(result['page']), 'results')
+
+print('collected', len(data), 'results')
+```
+
 # Versioning
 
 While we are pre-1.0.0, we'll update the minor version for large changes, and
 the patch version for small bugfixes. We may make backwards incompatible changes
 to the python client's API, but we will limit those to minor version bumps.
```

### Comparing `convex-0.3.0/convex/__init__.py` & `convex-0.4.0/convex/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """The official Python client for [Convex](https://convex.dev/)."""
+import warnings
 from typing import Any, Dict, Optional
 
 import requests
 from requests.exceptions import HTTPError
 
 from .values import (
     CoercibleToConvexValue,
     ConvexMap,
     ConvexSet,
     ConvexValue,
-    Id,
     JsonValue,
     convex_to_json,
     json_to_convex,
 )
 
 __all__ = [
-    "Id",
     "JsonValue",
     "ConvexValue",
     "convex_to_json",
     "json_to_convex",
     "ConvexError",
     "ConvexClient",
     "ConvexSet",
     "ConvexMap",
 ]
 
 
-__version__ = "0.3.0"  # Also update in pyproject.toml
+__version__ = "0.4.0"  # Also update in pyproject.toml
 
 
 class ConvexExecutionError(Exception):
     """Convex execution error on server."""
 
 
 FunctionArgs = Optional[Dict[str, CoercibleToConvexValue]]
@@ -86,14 +85,19 @@
         r = requests.post(url, json=data, headers=headers)
         response = r.json()
 
         if "logLines" in response:
             for line in response["logLines"]:
                 print(line)
 
+        deprecation_state = r.headers.get("x-convex-deprecation-state")
+        deprecation_msg = r.headers.get("x-convex-deprecation-message")
+        if deprecation_state and deprecation_msg:
+            warnings.warn(f"{deprecation_state}: {deprecation_msg}", stacklevel=1)
+
         try:
             r.raise_for_status()
         except HTTPError:
             raise Exception(
                 f"{r.status_code} {response['code']}: {response['message']}"
             )
```

### Comparing `convex-0.3.0/convex/values.py` & `convex-0.4.0/convex/values.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Value types supported by Convex."""
 import base64
 import collections
-import dataclasses
 import json
 import math
 import re
 import struct
 import sys
 from collections import abc
 from typing import (
@@ -41,15 +40,14 @@
     abc = ReplacementAbc()
 
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
 
 __all__ = [
-    "Id",
     "JsonValue",
     "ConvexValue",
     "convex_to_json",
     "strict_convex_to_json",
     "json_to_convex",
 ]
 
@@ -60,15 +58,14 @@
 ConvexValue = Union[
     None,
     bool,
     str,
     float,
     List["ConvexValue"],
     Dict[str, "ConvexValue"],
-    "Id",
     Set["ConvexValue"],
     Dict,
     bytes,
     "ConvexSet",
     "ConvexMap",
     "ConvexInt64",
 ]
@@ -123,44 +120,14 @@
     if not IDENTIFIER_REGEX.match(k):
         raise ValueError(
             f"Field name {k} must only contain alphanumeric characters or underscores "
             "and can't start with a number."
         )
 
 
-@dataclasses.dataclass
-class Id:
-    """Id objects represent references to Convex documents.
-
-    They contain a `table_name`
-    string specifying a Convex table (tables can be viewed in
-    [the dashboard](https://dashboard.convex.dev)) and a globably unique `id`
-    string. If you'd like to learn more about the `id` string's format, see
-    [our docs](https://docs.convex.dev/api/classes/values.GenericId).
-    """
-
-    table_name: str
-    id: str
-
-    @classmethod
-    def from_json(cls, obj: Any) -> "Id":
-        """Convert from JSON to Id."""
-        if not isinstance(obj["$id"], str):
-            raise ValueError(f"Object {obj} isn't a valid Id: $id isn't a string.")
-        parts = obj["$id"].split("|")
-        if len(parts) != 2:
-            raise ValueError(f"Object {obj} isn't a valid Id: Wrong number of parts.")
-        return Id(parts[0], parts[1])
-
-    def to_json(self) -> JsonValue:
-        """Convert from Id to JSON."""
-        idString = f"{self.table_name}|{self.id}"
-        return {"$id": idString}
-
-
 def is_special_float(v: float) -> bool:
     """Return True if value cannot be serialized to JSON."""
     return (
         math.isnan(v) or not math.isfinite(v) or (v == 0 and math.copysign(1, v) == -1)
     )
 
 
@@ -211,20 +178,20 @@
 
 
 def convex_to_json(v: CoercibleToConvexValue) -> JsonValue:
     """Convert Convex-serializable values to JSON-serializable objects.
 
     Convex types are described at https://docs.convex.dev/using/types and
     include Python builtin types str, int, float, bool, bytes, None, list, and
-    dict; as well as instances of the Id, ConvexSet, and ConvexMap classes.
+    dict; as well as instances of the ConvexSet and ConvexMap classes.
 
     >>> convex_to_json({'a': 1.0})
     {'a': 1.0}
-    >>> convex_to_json(Id("messages", "mqMw7arHuQa8TWcCXl8faAW"))
-    {'$id': 'messages|mqMw7arHuQa8TWcCXl8faAW'}
+    >>> convex_to_json(ConvexSet([1.0, 2.0, 3.0]))
+    {'$set': [1.0, 2.0, 3.0]}
 
     In addition to these basic Convex values, many Python types can be coerced
     to Convex values: for example, builtin sets:
 
     >>> convex_to_json(set([1.0, 2.0, 3.0]))
     {'$set': [1.0, 2.0, 3.0]}
 
@@ -262,16 +229,14 @@
         return v
     if type(v) is bytes:
         return buffer_to_json(v)
     if type(v) is dict:
         return mapping_to_object_json(v, coerce)
     if type(v) is list:
         return iterable_to_array_json(v, coerce)
-    if type(v) is Id:
-        return v.to_json()
     if type(v) is ConvexSet:
         return v.to_json()
     if type(v) is ConvexMap:
         return v.to_json()
     if type(v) is ConvexInt64:
         return v.to_json()
 
@@ -297,16 +262,14 @@
         return float_to_json(v)
     if isinstance(v, str):
         return v
     if isinstance(v, bytes):
         return buffer_to_json(v)
     if isinstance(v, dict):
         return mapping_to_object_json(v, coerce)
-    if isinstance(v, Id):
-        return v.to_json()
     if isinstance(v, list):
         return iterable_to_array_json(v, coerce)
     if isinstance(v, ConvexSet):
         return v.to_json()
     if isinstance(v, ConvexMap):
         return v.to_json()
 
@@ -339,16 +302,14 @@
     if v is None:
         return None
     if isinstance(v, list):
         convex_values: ConvexValue = [json_to_convex(x) for x in v]
         return convex_values
     if isinstance(v, dict) and len(v) == 1:
         attr = list(v.keys())[0]
-        if attr == "$id":
-            return Id.from_json(v)
         if attr == "$bytes":
             data_str = cast(str, v["$bytes"])
             return base64.standard_b64decode(data_str)
         if attr == "$integer":
             data_str = cast(str, v["$integer"])
             (i,) = struct.unpack("<q", base64.standard_b64decode(data_str))
             return ConvexInt64(cast(int, i))
```

### Comparing `convex-0.3.0/pyproject.toml` & `convex-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convex"
-version = "0.3.0"  # Also update in __init__.py
+version = "0.4.0"  # Also update in __init__.py
 description = "Python client for the reactive backend-as-a-service Convex."
 authors = ["Convex, Inc. <support@convex.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://convex.dev"
 repository = "https://github.com/get-convex/convex-py"
 documentation = "https://docs.convex.dev"
@@ -39,7 +39,10 @@
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 testpaths = [
     "tests",
     "integration",
     "convex"
 ]
+
+[tool.mypy]
+strict = true
```

### Comparing `convex-0.3.0/PKG-INFO` & `convex-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convex
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python client for the reactive backend-as-a-service Convex.
 Home-page: https://convex.dev
 License: Apache-2.0
 Author: Convex, Inc.
 Author-email: support@convex.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -54,15 +54,15 @@
 >>> client.mutation("sendMessage", dict(author="Me", body="Hello!"))
 ```
 
 To find the url of your convex backend, open the deployment you want to work
 with in the appropriate project in the
 [Convex dashboard](https://dashboard.convex.dev) and click "Settings" where the
 Deployment URL should be visible. To find out which queries, mutations, and
-actions are available check the Functions pane in the Dashboard
+actions are available check the Functions pane in the dashboard.
 
 To see logs emitted from Convex functions, set the debug mode to True.
 
 ```python
 >>> client.set_debug(True)
 ```
 
@@ -189,13 +189,49 @@
 >>> s
 ConvexMap([({'a': 1.0}, 123.0), ('b', 456.0)])
 ```
 
 ConvexMaps perform a copy of each inserted key/value pair, so they require more
 memory than Python's builtin dictionaries.
 
+# Pagination
+
+[Paginated queries](https://docs.convex.dev/database/pagination) are queries
+that accept pagination options as an argument and can be called repeatedly to
+produce additional "pages" of results.
+
+For a paginated query like this:
+
+```javascript
+import { query } from "./_generated/server";
+
+export default query(async ({ db }, { paginationOpts }) => {
+  return await db.query("messages").order("desc").paginate(paginationOpts);
+});
+```
+
+and returning all results 5 at a time in Python looks like this:
+
+```python
+import convex
+client = convex.ConvexClient('https://happy-animal-123.convex.cloud')
+
+done = False
+cursor = None
+data = []
+
+while not done:
+    result = client.query('listMessages', {"paginationOpts": {"numItems": 5, "cursor": cursor}})
+    cursor = result['continueCursor']
+    done = result["isDone"]
+    data.extend(result['page'])
+    print('got', len(result['page']), 'results')
+
+print('collected', len(data), 'results')
+```
+
 # Versioning
 
 While we are pre-1.0.0, we'll update the minor version for large changes, and
 the patch version for small bugfixes. We may make backwards incompatible changes
 to the python client's API, but we will limit those to minor version bumps.
```

