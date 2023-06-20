# Comparing `tmp/pymultithreading-0.2.0.tar.gz` & `tmp/pymultithreading-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-0.2.0.tar", last modified: Sun Jun 18 08:05:59 2023, max compression
+gzip compressed data, was "pymultithreading-0.2.1.tar", last modified: Tue Jun 20 14:54:13 2023, max compression
```

## Comparing `pymultithreading-0.2.0.tar` & `pymultithreading-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 08:05:59.893159 pymultithreading-0.2.0/
--rw-rw-rw-   0        0        0       98 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2045 2023-06-18 08:05:59.893159 pymultithreading-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:05:59.877154 pymultithreading-0.2.0/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.0/multithreading/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.2.0/multithreading/base.py
--rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.2.0/multithreading/document.py
--rw-rw-rw-   0        0        0    12586 2023-06-18 08:05:34.000000 pymultithreading-0.2.0/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:05:59.892158 pymultithreading-0.2.0/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 08:05:59.894159 pymultithreading-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-06-18 08:05:50.000000 pymultithreading-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:54:13.219979 pymultithreading-0.2.1/
+-rw-rw-rw-   0        0        0       98 2023-06-20 14:54:12.000000 pymultithreading-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2045 2023-06-20 14:54:13.219979 pymultithreading-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.1/build.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:54:13.203977 pymultithreading-0.2.1/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.1/multithreading/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.2.1/multithreading/base.py
+-rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.2.1/multithreading/document.py
+-rw-rw-rw-   0        0        0    12621 2023-06-20 14:51:22.000000 pymultithreading-0.2.1/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:54:13.218977 pymultithreading-0.2.1/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2045 2023-06-20 14:54:13.000000 pymultithreading-0.2.1/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-06-20 14:54:13.000000 pymultithreading-0.2.1/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:54:13.000000 pymultithreading-0.2.1/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-20 14:54:13.000000 pymultithreading-0.2.1/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-20 14:54:13.000000 pymultithreading-0.2.1/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-06-20 14:54:12.000000 pymultithreading-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:54:13.220978 pymultithreading-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-06-20 14:54:02.000000 pymultithreading-0.2.1/setup.py
```

### Comparing `pymultithreading-0.2.0/PKG-INFO` & `pymultithreading-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.0/README.md` & `pymultithreading-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.0/build.py` & `pymultithreading-0.2.1/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.0/multithreading/base.py` & `pymultithreading-0.2.1/multithreading/base.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.2.0/multithreading/process.py` & `pymultithreading-0.2.1/multithreading/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # process.py
 
 import datetime as dt
 import threading
 import time
 from abc import ABCMeta
 from typing import (
-    Any, Optional, Dict, Callable, Iterable, Union
+    Any, Optional, Dict, Callable,
+    Iterable, Union, TypeVar, Generic
 )
 
 from represent import BaseModel, Modifiers
 
 __all__ = [
     "Caller",
     "CallDefinition",
     "CallsResults",
     "multi_threaded_call",
     "multi_threaded_defined_call",
     "wait_call_completion",
     "ProcessTime",
     "ProcessInfo",
     "find_caller",
-    "CallerInfo",
     "CallResults"
 ]
 
 class ProcessInfo(BaseModel, metaclass=ABCMeta):
     """A class to contain the info of a call to the callers."""
 
     modifiers = Modifiers(properties=True)
@@ -55,29 +55,30 @@
         :return: The call time.
         """
 
         return self.end - self.start
     # end time
 # end CallInfo
 
-
 class ProcessTime(ProcessInfo):
     """A class to contain the info of a call to the callers."""
 # end ProcessTime
 
-class CallerInfo(ProcessInfo):
-    """A class to represent a function caller object."""
+ReturnType = TypeVar("ReturnType")
+
+class CallResults(BaseModel, Generic[ReturnType]):
+    """A class to represent a container for the call results."""
 
     modifiers = Modifiers(excluded=["thread"], force=True)
 
     __slots__ = "returns", "thread"
 
     def __init__(
             self,
-            returns: Optional[Any] = None,
+            returns: Optional[ReturnType] = None,
             thread: Optional[threading.Thread] = None,
             start: Optional[dt.datetime] = None,
             end: Optional[dt.datetime] = None,
 
     ) -> None:
         """
         Defines the class attributes.
@@ -86,33 +87,29 @@
         """
 
         super().__init__(start=start, end=end)
 
         self.returns = returns
         self.thread = thread
     # end __init__
-# end Caller
-
-class CallResults(CallerInfo):
-    """A class to represent a container for the call results."""
 # end CallResults
 
-class Caller(BaseModel):
+class Caller(BaseModel, Generic[ReturnType]):
     """A class to represent a function caller object."""
 
     modifiers = Modifiers(excluded=["thread", "results"])
 
     __slots__ = (
         "target", "identifier", "args", "kwargs",
         "thread", "results", "complete", "called"
     )
 
     def __init__(
             self,
-            target: Callable,
+            target: Callable[..., ReturnType],
             identifier: Optional[Any] = None,
             args: Optional[Iterable[Any]] = None,
             kwargs: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         Defines the class attributes.
 
@@ -130,15 +127,15 @@
         self.complete = False
         self.called = False
 
         self.thread: Optional[threading.Thread] = None
         self.results: Optional[CallResults] = None
     # end __init__
 
-    def __call__(self, *args: Any, **kwargs: Any) -> CallResults:
+    def __call__(self, *args: Any, **kwargs: Any) -> CallResults[ReturnType]:
         """
         Calls the function and saves the response.
 
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
 
         :return: The returned response.
@@ -147,21 +144,21 @@
         start = dt.datetime.now()
 
         self.args = args or self.args
         self.kwargs = kwargs or self.kwargs
 
         self.called = True
 
-        returns = self.target(*self.args, **self.kwargs)
+        returns: ReturnType = self.target(*self.args, **self.kwargs)
 
         self.complete = True
 
         end = dt.datetime.now()
 
-        self.results = CallResults(
+        self.results = CallResults[ReturnType](
             start=start, end=end,
             thread=self.thread, returns=returns
         )
 
         return self.results
     # end __call__
```

### Comparing `pymultithreading-0.2.0/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-0.2.1/pymultithreading.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.2.0/pyproject.toml` & `pymultithreading-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '0.2.0'
+version = '0.2.1'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-0.2.0/setup.py` & `pymultithreading-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='0.2.0',
+        version='0.2.1',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

