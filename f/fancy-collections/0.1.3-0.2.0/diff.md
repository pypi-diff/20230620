# Comparing `tmp/fancy_collections-0.1.3.tar.gz` & `tmp/fancy_collections-0.2.0-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancy_collections-0.1.3.tar", last modified: Tue Feb 21 15:58:19 2023, max compression
+gzip compressed data, was "fancy_collections-0.2.0.tar", last modified: Mon Jun 19 15:57:19 2023, max compression
```

## Comparing `fancy_collections-0.1.3.tar` & `fancy_collections-0.2.0-2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-02-21 15:58:19.737149 fancy_collections-0.1.3/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 fancy_collections-0.1.3/LICENSE
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1043 2023-02-21 15:58:19.737149 fancy_collections-0.1.3/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      467 2022-12-17 23:31:27.000000 fancy_collections-0.1.3/README.md
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-02-21 15:58:19.733149 fancy_collections-0.1.3/fancy_collections/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      208 2023-02-20 20:19:59.000000 fancy_collections-0.1.3/fancy_collections/__init__.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     9608 2023-02-21 12:08:51.000000 fancy_collections-0.1.3/fancy_collections/core.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     6233 2023-02-21 15:45:06.000000 fancy_collections-0.1.3/fancy_collections/formatting.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     5895 2023-02-20 20:38:24.000000 fancy_collections-0.1.3/fancy_collections/lib.py
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-02-21 15:58:19.733149 fancy_collections-0.1.3/fancy_collections.egg-info/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1043 2023-02-21 15:58:19.000000 fancy_collections-0.1.3/fancy_collections.egg-info/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      406 2023-02-21 15:58:19.000000 fancy_collections-0.1.3/fancy_collections.egg-info/SOURCES.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2023-02-21 15:58:19.000000 fancy_collections-0.1.3/fancy_collections.egg-info/dependency_links.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       69 2023-02-21 15:58:19.000000 fancy_collections-0.1.3/fancy_collections.egg-info/requires.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       18 2023-02-21 15:58:19.000000 fancy_collections-0.1.3/fancy_collections.egg-info/top_level.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      791 2023-02-21 15:45:51.000000 fancy_collections-0.1.3/pyproject.toml
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2023-02-21 15:58:19.737149 fancy_collections-0.1.3/setup.cfg
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-02-21 15:58:19.737149 fancy_collections-0.1.3/tests/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     4154 2023-02-16 12:26:41.000000 fancy_collections-0.1.3/tests/test_axis.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1172 2023-02-16 12:26:32.000000 fancy_collections-0.1.3/tests/test_frame.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       22 2023-02-16 11:15:19.000000 fancy_collections-0.1.3/tests/test_lib.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 15:57:19.367072 fancy_collections-0.2.0/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 fancy_collections-0.2.0/LICENSE
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1043 2023-06-19 15:57:19.367072 fancy_collections-0.2.0/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      467 2022-12-17 23:31:27.000000 fancy_collections-0.2.0/README.md
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 15:57:19.367072 fancy_collections-0.2.0/fancy_collections/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      208 2023-02-20 20:19:59.000000 fancy_collections-0.2.0/fancy_collections/__init__.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)    10009 2023-06-19 15:49:47.000000 fancy_collections-0.2.0/fancy_collections/core.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     6233 2023-02-21 15:45:06.000000 fancy_collections-0.2.0/fancy_collections/formatting.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     5895 2023-02-20 20:38:24.000000 fancy_collections-0.2.0/fancy_collections/lib.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 15:57:19.367072 fancy_collections-0.2.0/fancy_collections.egg-info/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1043 2023-06-19 15:57:19.000000 fancy_collections-0.2.0/fancy_collections.egg-info/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      427 2023-06-19 15:57:19.000000 fancy_collections-0.2.0/fancy_collections.egg-info/SOURCES.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2023-06-19 15:57:19.000000 fancy_collections-0.2.0/fancy_collections.egg-info/dependency_links.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       69 2023-06-19 15:57:19.000000 fancy_collections-0.2.0/fancy_collections.egg-info/requires.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       18 2023-06-19 15:57:19.000000 fancy_collections-0.2.0/fancy_collections.egg-info/top_level.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      791 2023-06-19 11:05:46.000000 fancy_collections-0.2.0/pyproject.toml
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2023-06-19 15:57:19.367072 fancy_collections-0.2.0/setup.cfg
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 15:57:19.367072 fancy_collections-0.2.0/tests/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     4120 2023-06-19 15:54:20.000000 fancy_collections-0.2.0/tests/test_axis.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1172 2023-02-16 12:26:32.000000 fancy_collections-0.2.0/tests/test_frame.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       22 2023-02-16 11:15:19.000000 fancy_collections-0.2.0/tests/test_lib.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      740 2023-06-19 11:15:15.000000 fancy_collections-0.2.0/tests/test_pickle.py
```

### Comparing `fancy_collections-0.1.3/LICENSE` & `fancy_collections-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fancy_collections-0.1.3/PKG-INFO` & `fancy_collections-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fancy_collections
-Version: 0.1.3
+Version: 0.2.0
 Summary: Some useful collection classes.
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/fancy-collections
 Project-URL: Bug Tracker, https://github.com/palmb/fancy-collections/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `fancy_collections-0.1.3/fancy_collections/core.py` & `fancy_collections-0.2.0/fancy_collections/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 from __future__ import annotations
 
 import functools
+import warnings
 from typing import List, Any
 
 import pandas as pd
-from sliceable_dict import TypedSliceDict
+from sliceable_dict import TypedSliceDict, SliceDict
 
 import fancy_collections.lib as lib
 from fancy_collections.formatting import Formatter
 
 
 class Axis:
     def __init__(self, name):
@@ -40,15 +41,15 @@
         except Exception as e:
             raise type(e)(f"Cannot set new {self._name}, because {e}") from None
         finally:
             instance.data = data
 
 
 class IndexMixin:
-    def _get_indexes(self: dict) -> List[pd.Index]:
+    def _get_indexes(self: SliceDict) -> List[pd.Index]:
         indexes = []
         for obj in self.values():
             if isinstance(obj, pd.Index):
                 index = obj
             else:
                 index = obj.index
             indexes.append(index)
@@ -177,14 +178,27 @@
                 data[key] = value
         return self.__class__(data)
 
     def to_dataframe(self, how="outer") -> pd.DataFrame:
         """
         Transform DictOfPandas to a pandas.DataFrame.
 
+        .. deprecated:: 0.2.0
+           use `DictOfPandas.to_pandas()` instead.
+        """
+        warnings.warn(
+            f"`to_dataframe()` is deprecated use `to_pandas()` instead.",
+            category=DeprecationWarning,
+        )
+        return self.to_pandas(how)
+
+    def to_pandas(self, how="outer") -> pd.DataFrame:
+        """
+        Transform DictOfPandas to a pandas.DataFrame.
+
         Because a pandas.DataFrame can not handle data of different
         length, but DictOfPandas can, the missing data is filled with
         NaNs or is dropped, depending on the keyword `how`.
 
         Items of type `pandas.Index` will become `pandas.Series` with
         identical index and values as the original Index.
 
@@ -224,27 +238,27 @@
         >>> di   # doctest: +NORMALIZE_WHITESPACE
             a |     b |     c |
         ===== | ===== | ===== |
         0  11 | 0  22 | 1  33 |
         1  11 | 1  22 | 4  33 |
               | 2  22 | 7  33 |
 
-        >>> di.to_dataframe()   # doctest: +NORMALIZE_WHITESPACE
-        columns     a     b     c
-        0        11.0  22.0   NaN
-        1        11.0  22.0  33.0
-        2         NaN  22.0   NaN
-        4         NaN   NaN  33.0
-        7         NaN   NaN  33.0
+        >>> di.to_pandas()   # doctest: +NORMALIZE_WHITESPACE
+              a     b     c
+        0  11.0  22.0   NaN
+        1  11.0  22.0  33.0
+        2   NaN  22.0   NaN
+        4   NaN   NaN  33.0
+        7   NaN   NaN  33.0
 
         or is dropped if `how='inner'`
 
-        >>> di.to_dataframe(how='inner')   # doctest: +NORMALIZE_WHITESPACE
-        columns   a   b   c
-        1        11  22  33
+        >>> di.to_pandas(how='inner')   # doctest: +NORMALIZE_WHITESPACE
+              a     b     c
+        1  11.0  22.0  33.0
 
         todo: examples with dataframe
         """
         if how not in ["inner", "outer"]:
             raise ValueError("`how` must be one of 'inner' or 'outer'")
         df = pd.DataFrame(dict(self.flatten(promote_index=True)))
         if how == "inner":
@@ -284,15 +298,15 @@
             Returns the result as a string.
         """
         return Formatter(self, max_rows, min_rows, show_df_column_names).to_string()
 
     def __eq__(self, other):
         if self is other:
             return True
-        if not isinstance(other, dict):
+        if not isinstance(other, (dict, SliceDict)):
             return False
         if self.keys() != other.keys():
             return False
         # equivalent code:
         # for key in self.keys():
         #     if not _pandasObjEqual(self[key], other[key]):
         #         return False
```

### Comparing `fancy_collections-0.1.3/fancy_collections/formatting.py` & `fancy_collections-0.2.0/fancy_collections/formatting.py`

 * *Files identical despite different names*

### Comparing `fancy_collections-0.1.3/fancy_collections/lib.py` & `fancy_collections-0.2.0/fancy_collections/lib.py`

 * *Files identical despite different names*

### Comparing `fancy_collections-0.1.3/fancy_collections.egg-info/PKG-INFO` & `fancy_collections-0.2.0/fancy_collections.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fancy-collections
-Version: 0.1.3
+Version: 0.2.0
 Summary: Some useful collection classes.
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/fancy-collections
 Project-URL: Bug Tracker, https://github.com/palmb/fancy-collections/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `fancy_collections-0.1.3/pyproject.toml` & `fancy_collections-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fancy_collections"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
   { name="Bert Palm", email="bert.palm.home@gmail.com" },
 ]
 description = "Some useful collection classes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "sliceable-dict >= 0.2.0",
+    "sliceable-dict >= 0.4.0",
     "pandas > 1.0.0",
     "numpy > 1.0.0",
 ]
 
 [project.optional-dependencies]
 tests = [
     'black',
```

### Comparing `fancy_collections-0.1.3/tests/test_axis.py` & `fancy_collections-0.2.0/tests/test_axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 @pytest.mark.parametrize("klass", [ColumnContainer, IndexContainer])
 @pytest.mark.parametrize("kwargs", [dict(), dict(a=99), dict(x=99)])
 @pytest.mark.parametrize("args", [(), ([[1, 2]],), (dict(a="a", b="b"),)])
 def test_creation(klass, args, kwargs):
     inst = klass(*args, **kwargs)
     assert isinstance(inst, klass)
     assert isinstance(inst, SliceDict)
-    assert isinstance(inst, dict)
 
 
 @pytest.mark.parametrize("klass", [ColumnContainer, IndexContainer])
 @pytest.mark.parametrize("attr", dir(dict))
 def test_attrs(klass, attr):
     assert hasattr(klass, attr)
     if issubclass(klass, ColumnContainer):
```

### Comparing `fancy_collections-0.1.3/tests/test_frame.py` & `fancy_collections-0.2.0/tests/test_frame.py`

 * *Files identical despite different names*

