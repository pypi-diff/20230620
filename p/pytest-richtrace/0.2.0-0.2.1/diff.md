# Comparing `tmp/pytest_richtrace-0.2.0.tar.gz` & `tmp/pytest_richtrace-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_richtrace-0.2.0.tar", max compression
+gzip compressed data, was "pytest_richtrace-0.2.1.tar", max compression
```

## Comparing `pytest_richtrace-0.2.0.tar` & `pytest_richtrace-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1352 2023-06-02 10:50:35.098255 pytest_richtrace-0.2.0/ReadMe.md
--rw-r--r--   0        0        0      892 2023-06-20 19:08:36.679744 pytest_richtrace-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1431 2023-06-02 10:50:35.114255 pytest_richtrace-0.2.0/src/pytest_richtrace/__init__.py
--rw-r--r--   0        0        0     7081 2023-06-02 10:50:35.115255 pytest_richtrace-0.2.0/src/pytest_richtrace/collection_observer.py
--rw-r--r--   0        0        0     2972 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/console.py
--rw-r--r--   0        0        0     3671 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/event.py
--rw-r--r--   0        0        0     1637 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/events.py
--rw-r--r--   0        0        0       55 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/item.py
--rw-r--r--   0        0        0     7713 2023-06-02 10:50:35.115255 pytest_richtrace-0.2.0/src/pytest_richtrace/plugin.py
--rw-r--r--   0        0        0        0 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/py.typed
--rw-r--r--   0        0        0     4998 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/results.py
--rw-r--r--   0        0        0    27850 2023-06-02 10:50:35.124255 pytest_richtrace-0.2.0/src/pytest_richtrace/rich_reporter.py
--rw-r--r--   0        0        0     6604 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.0/src/pytest_richtrace/test_execution_observer.py
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 pytest_richtrace-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1165 2023-06-20 19:18:52.478654 pytest_richtrace-0.2.1/ReadMe.md
+-rw-r--r--   0        0        0      892 2023-06-20 19:18:56.646668 pytest_richtrace-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1431 2023-06-02 10:50:35.114255 pytest_richtrace-0.2.1/src/pytest_richtrace/__init__.py
+-rw-r--r--   0        0        0     7431 2023-06-20 19:19:55.773854 pytest_richtrace-0.2.1/src/pytest_richtrace/collection_observer.py
+-rw-r--r--   0        0        0     2972 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.1/src/pytest_richtrace/console.py
+-rw-r--r--   0        0        0     3671 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.1/src/pytest_richtrace/event.py
+-rw-r--r--   0        0        0     1637 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.1/src/pytest_richtrace/events.py
+-rw-r--r--   0        0        0       55 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.1/src/pytest_richtrace/item.py
+-rw-r--r--   0        0        0     7713 2023-06-02 10:50:35.115255 pytest_richtrace-0.2.1/src/pytest_richtrace/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.1/src/pytest_richtrace/py.typed
+-rw-r--r--   0        0        0     4998 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.1/src/pytest_richtrace/results.py
+-rw-r--r--   0        0        0    27850 2023-06-02 10:50:35.124255 pytest_richtrace-0.2.1/src/pytest_richtrace/rich_reporter.py
+-rw-r--r--   0        0        0     6604 2023-06-02 10:50:35.123255 pytest_richtrace-0.2.1/src/pytest_richtrace/test_execution_observer.py
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 pytest_richtrace-0.2.1/PKG-INFO
```

### Comparing `pytest_richtrace-0.2.0/pyproject.toml` & `pytest_richtrace-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-richtrace"
-version = "0.2.0"
+version = "0.2.1"
 description = "A pytest plugin that displays the names and information of the pytest hook functions as they are executed."
 authors = ["Simon Kennedy <sffjunkie+code@gmail.com>"]
 license = "Apache-2.0"
 readme = "ReadMe.md"
 packages = [
     { include = "pytest_richtrace", from = "src" },
     { include = "pytest_richtrace/py.typed", from = "src" },
```

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/__init__.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/collection_observer.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/collection_observer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import logging
 import time
+import warnings
 from datetime import datetime, timezone
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 from _pytest._py.path import LocalPath
 from _pytest.pathlib import import_path
 from _pytest.python import Class, Module
 from _pytest.skipping import evaluate_skip_marks, evaluate_xfail_marks
 
 from . import events
 from .event import SOURCE_ID_GENERATOR, EventBus, EventPublisher
 from .item import NodeId
 from .results import SkipInfo, TestRunResults, XfailInfo
 
 
+if TYPE_CHECKING:
+    from typing import Literal
+
+
 class CollectionObserver:
     results: TestRunResults
 
     def __init__(
         self,
         config: pytest.Config,
         results: TestRunResults,
@@ -194,14 +200,23 @@
         self.publisher.publish(
             events.ItemsDeselected,
             item_id=None,
             payload={"items": items},
         )
         return None
 
+    def pytest_warning_recorded(
+        self,
+        warning_message: "warnings.WarningMessage",
+        when: Literal["config", "collect", "runtest"],
+        nodeid: str,
+        location: tuple[str, int, str] | None,
+    ) -> None:
+        ...
+
     @pytest.hookimpl(trylast=True)
     def pytest_collection_finish(self, session: pytest.Session) -> None:
         logging.debug("collector: pytest_collection_finish")
         self.results.collect.finish = datetime.now(tz=timezone.utc)
         self.results.collect.precise_finish = time.perf_counter()
         self.publisher.publish(
             events.CollectionFinished,
```

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/console.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/console.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/event.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/event.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/events.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/events.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/plugin.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/results.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/results.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/rich_reporter.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/rich_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/src/pytest_richtrace/test_execution_observer.py` & `pytest_richtrace-0.2.1/src/pytest_richtrace/test_execution_observer.py`

 * *Files identical despite different names*

### Comparing `pytest_richtrace-0.2.0/PKG-INFO` & `pytest_richtrace-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-richtrace
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pytest plugin that displays the names and information of the pytest hook functions as they are executed.
 License: Apache-2.0
 Author: Simon Kennedy
 Author-email: sffjunkie+code@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,14 @@
 
 # pytest-richtrace
 
 A pytest plugin that dumps the stages of the pytest testing process to the terminal.
 
 It uses `rich` to add formatting to the output.
 
-> **NOTE**: This project is not currently available on pypi.org as it uses the V2 version of pydantic from git and pypi does not allow packages to be uploaded with this use of git URLs.
-
 ## Installation
 
 Install using pip
 
 ```shell
 pip install pytest_richtrace
 ```
```

