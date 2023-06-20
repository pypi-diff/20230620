# Comparing `tmp/embrace-4.2.1.tar.gz` & `tmp/embrace-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embrace-4.2.1.tar", last modified: Wed May 24 12:03:35 2023, max compression
+gzip compressed data, was "embrace-4.2.2.tar", last modified: Tue Jun 20 15:31:49 2023, max compression
```

## Comparing `embrace-4.2.1.tar` & `embrace-4.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.197627 embrace-4.2.1/
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-24 12:02:20.000000 embrace-4.2.1/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-05-24 12:03:35.197758 embrace-4.2.1/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)    11800 2023-05-24 12:02:20.000000 embrace-4.2.1/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.195308 embrace-4.2.1/embrace/
--rw-r--r--   0 oliver    (1001) wheel        (0)      804 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1938 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9891 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/module.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8810 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/parsing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     6260 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/pool.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1897 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/poolvalidators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    28346 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/query.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3682 2023-05-24 12:02:20.000000 embrace-4.2.1/embrace/util.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.196375 embrace-4.2.1/embrace.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      450 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       15 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/requires.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        8 2023-05-24 12:03:34.000000 embrace-4.2.1/embrace.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      748 2023-05-24 12:03:35.198356 embrace-4.2.1/setup.cfg
--rwxr-xr-x   0 oliver    (1001) wheel        (0)      635 2023-05-24 12:02:20.000000 embrace-4.2.1/setup.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-24 12:03:35.197446 embrace-4.2.1/tests/
--rw-r--r--   0 oliver    (1001) wheel        (0)     6390 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_module.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3342 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_parsing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1626 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_pool.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    19059 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_query.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1010 2023-05-24 12:02:20.000000 embrace-4.2.1/tests/test_util.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.298836 embrace-4.2.2/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-06-20 15:30:49.000000 embrace-4.2.2/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-06-20 15:31:49.299010 embrace-4.2.2/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11800 2023-06-20 15:30:49.000000 embrace-4.2.2/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.296341 embrace-4.2.2/embrace/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      804 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1938 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9891 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/module.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9156 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/parsing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     6260 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/pool.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1897 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/poolvalidators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    28346 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/query.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3682 2023-06-20 15:30:49.000000 embrace-4.2.2/embrace/util.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.297490 embrace-4.2.2/embrace.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12509 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      450 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       15 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/requires.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        8 2023-06-20 15:31:48.000000 embrace-4.2.2/embrace.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      748 2023-06-20 15:31:49.299755 embrace-4.2.2/setup.cfg
+-rwxr-xr-x   0 oliver    (1001) wheel        (0)      635 2023-06-20 15:30:49.000000 embrace-4.2.2/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-06-20 15:31:49.298637 embrace-4.2.2/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     6390 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_module.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3518 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_parsing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1626 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_pool.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    19059 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_query.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1010 2023-06-20 15:30:49.000000 embrace-4.2.2/tests/test_util.py
```

### Comparing `embrace-4.2.1/LICENSE.txt` & `embrace-4.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/PKG-INFO` & `embrace-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embrace
-Version: 4.2.1
+Version: 4.2.2
 Summary: Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 Home-page: https://hg.sr.ht/~olly/embrace-sql
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: sql hugsql pugsql orm anti-orm files dapper
 Classifier: Development Status :: 4 - Beta
```

### Comparing `embrace-4.2.1/README.rst` & `embrace-4.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace/__init__.py` & `embrace-4.2.2/embrace/__init__.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace/exceptions.py` & `embrace-4.2.2/embrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace/module.py` & `embrace-4.2.2/embrace/module.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace/parsing.py` & `embrace-4.2.2/embrace/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import Iterable
 from typing import Callable
 from typing import List
 from typing import Mapping
 from typing import Union
 from typing import Tuple
 from typing import Sequence
+from typing import Iterator
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from embrace.query import Query
 
 import sqlparse
 
@@ -271,25 +272,37 @@
             for items in bind_parameters[p]
         )
     else:
         raise ValueError(f"Unsupported param_type {pt}")
 
 
 def make_sequence_placeholder(
-    params,
-    param_gen,
-    placeholder_counter,
+    params: Union[List[Any], Dict[str, Any]],
+    param_gen: Callable[[str, int], str],
+    placeholder_counter: Iterator[int],
     items: List,
 ) -> str:
-    names = [f"_{ix}" for ix in range(1, len(items) + 1)]
+    """
+    Return a placeholder for a sequence of parameters, in the format::
+
+        ?, ?, ?, ...
+
+    Or::
+
+        :_1, :_2, :_3, ...
+
+    Modify ``params`` in place to include the placeholders.
+    """
+    numbers = [next(placeholder_counter) for ix in range(len(items))]
+    names = [f"_{n}" for n in numbers]
     if isinstance(params, list):
         params.extend(items)
     else:
         params.update(zip(names, items))
-    return ", ".join(param_gen(n, next(placeholder_counter)) for n in names)  # type: ignore
+    return ", ".join(param_gen(name, c) for name, c in zip(names, numbers))
 
 
 _param_styles = {
     "qmark": (True, lambda name, c: "?"),
     "numeric": (True, lambda name, c: f":{c}"),
     "format": (True, lambda name, c: "%s"),
     "pyformat": (False, lambda name, c: f"%({name})s"),
```

### Comparing `embrace-4.2.1/embrace/pool.py` & `embrace-4.2.2/embrace/pool.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace/poolvalidators.py` & `embrace-4.2.2/embrace/poolvalidators.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace/query.py` & `embrace-4.2.2/embrace/query.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace/util.py` & `embrace-4.2.2/embrace/util.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/embrace.egg-info/PKG-INFO` & `embrace-4.2.2/embrace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embrace
-Version: 4.2.1
+Version: 4.2.2
 Summary: Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 Home-page: https://hg.sr.ht/~olly/embrace-sql
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: sql hugsql pugsql orm anti-orm files dapper
 Classifier: Development Status :: 4 - Beta
```

### Comparing `embrace-4.2.1/setup.cfg` & `embrace-4.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = embrace
-version = 4.2.1
+version = 4.2.2
 description = Embrace SQL keeps your SQL queries in SQL files. An anti-ORM inspired by HugSQL and PugSQL
 long_description = file: README.rst
 author = Oliver Cope
 author_email = oliver@redgecko.org
 keywords = sql hugsql pugsql orm anti-orm files dapper
 url = https://hg.sr.ht/~olly/embrace-sql
 license = Apache
```

### Comparing `embrace-4.2.1/setup.py` & `embrace-4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/tests/test_module.py` & `embrace-4.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/tests/test_parsing.py` & `embrace-4.2.2/tests/test_parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,22 @@
         "qmark",
         ":t*:a",
         {"a": [("x", "y"), (1, 2)]},
         "(?, ?), (?, ?)",
         ("x", "y", 1, 2),
     )
 
+    test(
+        "named",
+        ":tuple*:a",
+        {"a": [("x", "y"), (1, 2)]},
+        "(:_1, :_2), (:_3, :_4)",
+        {"_1": "x", "_2": "y", "_3": 1, "_4": 2},
+    )
+
     # it escapes percent signs
     test("format", ":a % :b", {"a": 3, "b": 2}, "%s %% %s", (3, 2))
     test(
         "pyformat",
         ":a % :b",
         {"a": 3, "b": 2},
         "%(a)s %% %(b)s",
```

### Comparing `embrace-4.2.1/tests/test_pool.py` & `embrace-4.2.2/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/tests/test_query.py` & `embrace-4.2.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `embrace-4.2.1/tests/test_util.py` & `embrace-4.2.2/tests/test_util.py`

 * *Files identical despite different names*

