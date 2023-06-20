# Comparing `tmp/logwrap-9.0.1.post0.tar.gz` & `tmp/logwrap-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\logwrap-9.0.1.post0.tar", last modified: Tue Oct 19 14:34:16 2021, max compression
+gzip compressed data, was "dist\logwrap-9.0.2.tar", last modified: Mon Nov  1 12:36:17 2021, max compression
```

## Comparing `logwrap-9.0.1.post0.tar` & `logwrap-9.0.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/
--rw-rw-rw-   0        0        0      288 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/.editorconfig
--rw-rw-rw-   0        0        0      313 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/.pydocstyle.ini
--rw-rw-rw-   0        0        0       21 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/CI_REQUIREMENTS.txt
--rw-rw-rw-   0        0        0    11567 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/LICENSE
--rw-rw-rw-   0        0        0      381 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/MANIFEST.in
--rw-rw-rw-   0        0        0    16188 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/PKG-INFO
--rw-rw-rw-   0        0        0    11628 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/README.rst
--rw-rw-rw-   0        0        0       77 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/build_requirements.txt
-drwxrwxrwx   0        0        0        0 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/doc/
--rw-rw-rw-   0        0        0     7844 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/Makefile
--rwxrwxrwx   0        0        0     7743 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/make.bat
-drwxrwxrwx   0        0        0        0 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/doc/source/
--rw-rw-rw-   0        0        0     4050 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/source/LogOnAccess.rst
--rw-rw-rw-   0        0        0     4270 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/source/PrettyFormat.rst
-drwxrwxrwx   0        0        0        0 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/doc/source/_static/
--rw-rw-rw-   0        0        0        0 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/source/_static/.gitkeep
--rw-rw-rw-   0        0        0    10380 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/source/conf.py
--rw-rw-rw-   0        0        0      450 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/source/index.rst
--rw-rw-rw-   0        0        0     7740 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/doc/source/logwrap.rst
--rw-rw-rw-   0        0        0       56 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/flake8_requirements.txt
-drwxrwxrwx   0        0        0        0 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap/
--rw-rw-rw-   0        0        0     2114 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/__init__.py
--rw-rw-rw-   0        0        0      153 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap/_version.py
--rw-rw-rw-   0        0        0      748 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/constants.py
--rw-rw-rw-   0        0        0    21506 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/log_on_access.py
--rw-rw-rw-   0        0        0     2067 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/log_wrap.pxd
--rw-rw-rw-   0        0        0    30125 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/log_wrap.py
--rw-rw-rw-   0        0        0    23388 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/log_wrap.pyx
--rw-rw-rw-   0        0        0        0 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/py.typed
--rw-rw-rw-   0        0        0     3433 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/repr_utils.pxd
--rw-rw-rw-   0        0        0    21988 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/repr_utils.py
--rw-rw-rw-   0        0        0    21648 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/logwrap/repr_utils.pyx
-drwxrwxrwx   0        0        0        0 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap.egg-info/
--rw-rw-rw-   0        0        0    16188 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      761 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/logwrap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1692 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/pyproject.toml
--rw-rw-rw-   0        0        0       97 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/pytest_requirements.txt
--rw-rw-rw-   0        0        0        0 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/requirements.txt
--rw-rw-rw-   0        0        0      893 2021-10-19 14:34:16.000000 logwrap-9.0.1.post0/setup.cfg
--rw-rw-rw-   0        0        0     9030 2021-10-19 14:33:50.000000 logwrap-9.0.1.post0/setup.py
+drwxrwxrwx   0        0        0        0 2021-11-01 12:36:17.000000 logwrap-9.0.2/
+-rw-rw-rw-   0        0        0      288 2021-11-01 12:35:51.000000 logwrap-9.0.2/.editorconfig
+-rw-rw-rw-   0        0        0     1473 2021-11-01 12:35:51.000000 logwrap-9.0.2/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      313 2021-11-01 12:35:51.000000 logwrap-9.0.2/.pydocstyle.ini
+-rw-rw-rw-   0        0        0       21 2021-11-01 12:35:51.000000 logwrap-9.0.2/CI_REQUIREMENTS.txt
+-rw-rw-rw-   0        0        0    11567 2021-11-01 12:35:51.000000 logwrap-9.0.2/LICENSE
+-rw-rw-rw-   0        0        0      381 2021-11-01 12:35:51.000000 logwrap-9.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    16182 2021-11-01 12:36:17.000000 logwrap-9.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11628 2021-11-01 12:35:51.000000 logwrap-9.0.2/README.rst
+-rw-rw-rw-   0        0        0       77 2021-11-01 12:35:51.000000 logwrap-9.0.2/build_requirements.txt
+drwxrwxrwx   0        0        0        0 2021-11-01 12:36:17.000000 logwrap-9.0.2/doc/
+-rw-rw-rw-   0        0        0     7844 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/Makefile
+-rwxrwxrwx   0        0        0     7743 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/make.bat
+drwxrwxrwx   0        0        0        0 2021-11-01 12:36:17.000000 logwrap-9.0.2/doc/source/
+-rw-rw-rw-   0        0        0     4050 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/source/LogOnAccess.rst
+-rw-rw-rw-   0        0        0     4270 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/source/PrettyFormat.rst
+drwxrwxrwx   0        0        0        0 2021-11-01 12:36:17.000000 logwrap-9.0.2/doc/source/_static/
+-rw-rw-rw-   0        0        0        0 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/source/_static/.gitkeep
+-rw-rw-rw-   0        0        0    10380 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/source/conf.py
+-rw-rw-rw-   0        0        0      450 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/source/index.rst
+-rw-rw-rw-   0        0        0     7630 2021-11-01 12:35:51.000000 logwrap-9.0.2/doc/source/logwrap.rst
+-rw-rw-rw-   0        0        0       56 2021-11-01 12:35:51.000000 logwrap-9.0.2/flake8_requirements.txt
+drwxrwxrwx   0        0        0        0 2021-11-01 12:36:17.000000 logwrap-9.0.2/logwrap/
+-rw-rw-rw-   0        0        0     2114 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/__init__.py
+-rw-rw-rw-   0        0        0      147 2021-11-01 12:36:16.000000 logwrap-9.0.2/logwrap/_version.py
+-rw-rw-rw-   0        0        0      748 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/constants.py
+-rw-rw-rw-   0        0        0    21121 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/log_on_access.py
+-rw-rw-rw-   0        0        0     2039 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/log_wrap.pxd
+-rw-rw-rw-   0        0        0    29707 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/log_wrap.py
+-rw-rw-rw-   0        0        0    23388 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/log_wrap.pyx
+-rw-rw-rw-   0        0        0        0 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/py.typed
+-rw-rw-rw-   0        0        0     3433 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/repr_utils.pxd
+-rw-rw-rw-   0        0        0    22020 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/repr_utils.py
+-rw-rw-rw-   0        0        0    21616 2021-11-01 12:35:51.000000 logwrap-9.0.2/logwrap/repr_utils.pyx
+drwxrwxrwx   0        0        0        0 2021-11-01 12:36:17.000000 logwrap-9.0.2/logwrap.egg-info/
+-rw-rw-rw-   0        0        0    16182 2021-11-01 12:36:16.000000 logwrap-9.0.2/logwrap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2021-11-01 12:36:16.000000 logwrap-9.0.2/logwrap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-11-01 12:36:16.000000 logwrap-9.0.2/logwrap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-11-01 12:36:16.000000 logwrap-9.0.2/logwrap.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2021-11-01 12:36:16.000000 logwrap-9.0.2/logwrap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1692 2021-11-01 12:35:51.000000 logwrap-9.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       97 2021-11-01 12:35:51.000000 logwrap-9.0.2/pytest_requirements.txt
+-rw-rw-rw-   0        0        0        0 2021-11-01 12:35:51.000000 logwrap-9.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      893 2021-11-01 12:36:17.000000 logwrap-9.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     7003 2021-11-01 12:35:51.000000 logwrap-9.0.2/setup.py
```

### Comparing `logwrap-9.0.1.post0/LICENSE` & `logwrap-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/PKG-INFO` & `logwrap-9.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logwrap
-Version: 9.0.1.post0
+Version: 9.0.2
 Summary: Decorator for logging function arguments and return value by human-readable way
 Home-page: https://github.com/python-useful-helpers/logwrap
 Author: Alexey Stepanov
 Author-email: penguinolog@gmail.com
 Maintainer: Alexey Stepanov <penguinolog@gmail.com>, Antonio Esposito <esposito.cloud@gmail.com>, Dennis Dmitriev <dis-xcom@gmail.com>
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/python-useful-helpers/logwrap/issues
```

### Comparing `logwrap-9.0.1.post0/README.rst` & `logwrap-9.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/doc/Makefile` & `logwrap-9.0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/doc/make.bat` & `logwrap-9.0.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/doc/source/LogOnAccess.rst` & `logwrap-9.0.2/doc/source/LogOnAccess.rst`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/doc/source/PrettyFormat.rst` & `logwrap-9.0.2/doc/source/PrettyFormat.rst`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/doc/source/conf.py` & `logwrap-9.0.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/doc/source/logwrap.rst` & `logwrap-9.0.2/doc/source/logwrap.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 API: Decorators: `LogWrap` class and `logwrap` function.
 ========================================================
 
 .. py:module:: logwrap
 .. py:currentmodule:: logwrap
 
-.. py:class:: LogWrap(object)
+.. py:class:: LogWrap
 
     Log function calls and return values.
 
     .. versionadded:: 2.2.0
 
     .. py:method:: __init__(*, log=None, log_level=logging.DEBUG, exc_level=logging.ERROR, max_indent=20, blacklisted_names=None, blacklisted_exceptions=None, log_call_args=True, log_call_args_on_exc=True, log_traceback=True, log_result_obj=True, )
 
         :param log: logger object for decorator, by default trying to use logger from target module. Fallback: 'logwrap'
-        :type log: typing.Optional[logging.Logger]
+        :type log: logging.Logger | None
         :param log_level: log level for successful calls
         :type log_level: int
         :param exc_level: log level for exception cases
         :type exc_level: int
         :param max_indent: maximum indent before classic `repr()` call.
         :type max_indent: int
         :param blacklisted_names: Blacklisted argument names.
                                   Arguments with this names will be skipped in log.
-        :type blacklisted_names: typing.Optional[typing.Iterable[str]]
+        :type blacklisted_names: Iterable[str] | None
         :param blacklisted_exceptions: list of exception,
                                        which should be re-raised without
                                        producing traceback and text log record.
-        :type blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]]
+        :type blacklisted_exceptions: Iterable[type[Exception]] | None
         :param log_call_args: log call arguments before executing wrapped function.
         :type log_call_args: bool
         :param log_call_args_on_exc: log call arguments if exception raised.
         :type log_call_args_on_exc: bool
         :param log_traceback: log traceback on exception in addition to failure info
         :type log_traceback: bool
         :param log_result_obj: log result of function call.
@@ -101,26 +101,26 @@
 .. py:function:: logwrap(func=None, *, log=None, log_level=logging.DEBUG, exc_level=logging.ERROR, max_indent=20, blacklisted_names=None, blacklisted_exceptions=None, log_call_args=True, log_call_args_on_exc=True, log_traceback=True, log_result_obj=True, )
 
     Log function calls and return values.
 
     :param func: function to wrap
     :type func: typing.Optional[typing.Callable]
     :param log: logger object for decorator, by default trying to use logger from target module. Fallback: 'logwrap'
-    :type log: typing.Optional[logging.Logger]
+    :type log: logging.Logger | None
     :param log_level: log level for successful calls
     :type log_level: int
     :param exc_level: log level for exception cases
     :type exc_level: int
     :param max_indent: maximum indent before classic `repr()` call.
     :type max_indent: int
     :param blacklisted_names: Blacklisted argument names. Arguments with this names will be skipped in log.
-    :type blacklisted_names: typing.Optional[typing.Iterable[str]]
+    :type blacklisted_names: Iterable[str] | None
     :param blacklisted_exceptions: list of exceptions, which should be re-raised
                                    without producing traceback and text log record.
-    :type blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]]
+    :type blacklisted_exceptions: Iterable[type[Exception]] | None
     :param log_call_args: log call arguments before executing wrapped function.
     :type log_call_args: bool
     :param log_call_args_on_exc: log call arguments if exception raised.
     :type log_call_args_on_exc: bool
     :param log_traceback: log traceback on exception in addition to failure info
     :type log_traceback: bool
     :param log_result_obj: log result of function call.
```

### Comparing `logwrap-9.0.1.post0/logwrap/__init__.py` & `logwrap-9.0.2/logwrap/__init__.py`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/logwrap/constants.py` & `logwrap-9.0.2/logwrap/constants.py`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/logwrap/log_on_access.py` & `logwrap-9.0.2/logwrap/log_on_access.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,33 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 """Property with logging on successful get/set/delete or failure."""
 
+from __future__ import annotations
+
 # Standard Library
 import inspect
 import logging
 import os
 import sys
 import time
 import traceback
 import typing
 
 # Package Implementation
 from logwrap import constants
 from logwrap import repr_utils
 
+if typing.TYPE_CHECKING:
+    # Standard Library
+    from collections.abc import Callable
+
 __all__ = ("LogOnAccess",)
 
 _LOGGER: logging.Logger = logging.getLogger(__name__)
 _CURRENT_FILE = os.path.abspath(__file__)
 _OwnerT = typing.TypeVar("_OwnerT")
 _ReturnT = typing.TypeVar("_ReturnT")
 
@@ -133,43 +139,43 @@
     'Traceback (most recent call last):'
 
     .. versionadded:: 6.1.0
     """
 
     def __init__(
         self,
-        fget: typing.Optional[typing.Callable[[_OwnerT], _ReturnT]] = None,
-        fset: typing.Optional[typing.Callable[[_OwnerT, _ReturnT], None]] = None,
-        fdel: typing.Optional[typing.Callable[[_OwnerT], None]] = None,
-        doc: typing.Optional[str] = None,
+        fget: Callable[[_OwnerT], _ReturnT] | None = None,
+        fset: Callable[[_OwnerT, _ReturnT], None] | None = None,
+        fdel: Callable[[_OwnerT], None] | None = None,
+        doc: str | None = None,
         *,
         # Extended settings start
-        logger: typing.Optional[typing.Union[logging.Logger, str]] = None,
+        logger: logging.Logger | str | None = None,
         log_object_repr: bool = True,
         log_level: int = logging.DEBUG,
         exc_level: int = logging.DEBUG,
         log_before: bool = True,
         log_success: bool = True,
         log_failure: bool = True,
         log_traceback: bool = True,
-        override_name: typing.Optional[str] = None,
+        override_name: str | None = None,
         max_indent: int = 20,
     ) -> None:
         """Advanced property main entry point.
 
         :param fget: normal getter.
-        :type fget: typing.Optional[typing.Callable[[typing.Any, ], typing.Any]]
+        :type fget: Callable[[_OwnerT], _ReturnT] | None
         :param fset: normal setter.
-        :type fset: typing.Optional[typing.Callable[[typing.Any, typing.Any], None]]
+        :type fset: Callable[[_OwnerT, _ReturnT], None] | None
         :param fdel: normal deleter.
-        :type fdel: typing.Optional[typing.Callable[[typing.Any, ], None]]
+        :type fdel: Callable[[_OwnerT], None] | None
         :param doc: docstring override
-        :type doc: typing.Optional[str]
+        :type doc: str | None
         :param logger: logger instance or name to use as override
-        :type logger: typing.Optional[typing.Union[logging.Logger, str]]
+        :type logger: logging.Logger | str | None
         :param log_object_repr: use `repr` over object to describe owner if True else owner class name and id
         :type log_object_repr: bool
         :param log_level: log level for successful operations
         :type log_level: int
         :param exc_level: log level for exceptions
         :type exc_level: int
         :param log_before: log before operation
@@ -177,81 +183,81 @@
         :param log_success: log successful operations
         :type log_success: bool
         :param log_failure: log exceptions
         :type log_failure: bool
         :param log_traceback: Log traceback on exceptions
         :type log_traceback: bool
         :param override_name: override property name if not None else use getter/setter/deleter name
-        :type override_name: typing.Optional[str]
+        :type override_name: str | None
         :param max_indent: maximal indent before classic repr() call
         :type max_indent: int
         """
         super().__init__(fget=fget, fset=fset, fdel=fdel, doc=doc)
 
         if logger is None or isinstance(logger, logging.Logger):
-            self.__logger: typing.Optional[logging.Logger] = logger
+            self.__logger: logging.Logger | None = logger
         else:
             self.__logger = logging.getLogger(logger)
 
         self.__log_object_repr: bool = log_object_repr
         self.__log_level: int = log_level
         self.__exc_level: int = exc_level
         self.__log_before: bool = log_before
         self.__log_success: bool = log_success
         self.__log_failure: bool = log_failure
         self.__log_traceback: bool = log_traceback
-        self.__override_name: typing.Optional[str] = override_name
+        self.__override_name: str | None = override_name
         self.__max_indent: int = max_indent
         self.__name: str = ""
-        self.__owner: typing.Optional[typing.Type[_OwnerT]] = None
+        self.__owner: type[_OwnerT] | None = None
 
-    def __set_name__(self, owner: typing.Optional[typing.Type[_OwnerT]], name: str) -> None:
+    def __set_name__(self, owner: type[_OwnerT] | None, name: str) -> None:
         """Set __name__ and __objclass__ property.
 
         :param owner: owner class, where descriptor applied
-        :type owner: typing.Optional[type]
+        :type owner: type[_OwnerT] | None
         :param name: descriptor name
         :type name: str
         """
         self.__owner = owner
         self.__name = name
 
     @property
-    def __objclass__(self) -> typing.Optional[typing.Type[_OwnerT]]:  # pragma: no cover
+    def __objclass__(self) -> type[_OwnerT] | None:  # pragma: no cover
         """Read-only owner.
 
         :return: property owner class
-        :rtype: typing.Optional[type]
+        :rtype: type[_OwnerT] | None
         """
         return self.__owner
 
     @property
     def __traceback(self) -> str:
         """Get outer traceback text for logging.
 
         :return: traceback without decorator internals if traceback logging enabled else empty line
         :rtype: str
         """
         if not self.log_traceback:
             return ""
         exc_info = sys.exc_info()
         stack: traceback.StackSummary = traceback.extract_stack()
-        full_tb: typing.List[traceback.FrameSummary] = [elem for elem in stack if elem.filename != _CURRENT_FILE]
-        exc_line: typing.List[str] = traceback.format_exception_only(*exc_info[:2])
+        full_tb: list[traceback.FrameSummary] = [elem for elem in stack if elem.filename != _CURRENT_FILE]
+        exc_line: list[str] = traceback.format_exception_only(*exc_info[:2])
         # Make standard traceback string
         tb_text = "\nTraceback (most recent call last):\n" + "".join(traceback.format_list(full_tb)) + "".join(exc_line)
         return tb_text
 
-    def __get_obj_source(self, instance: _OwnerT, owner: typing.Optional[typing.Type[_OwnerT]] = None) -> str:
+    def __get_obj_source(self, instance: _OwnerT, owner: type[_OwnerT] | None = None) -> str:
         """Get object repr block.
 
         :param instance: object instance
         :type instance: typing.Any
         :param owner: object class (available for getter usage only)
-        :type owner: typing.Optional[type]
+        :type owner: type[_OwnerT] | None
         :return: repr of object if it not disabled else repr placeholder
         :rtype: str
         """
         if self.log_object_repr:
             return repr_utils.pretty_repr(instance, max_indent=self.max_indent)
         if owner is not None:
             return f"<{owner.__name__}() at 0x{id(instance):X}>"
@@ -259,15 +265,15 @@
             return f"<{self.__objclass__.__name__}() at 0x{id(instance):X}>"
         return f"<{instance.__class__.__name__}() at 0x{id(instance):X}>"
 
     def _get_logger_for_instance(self, instance: _OwnerT) -> logging.Logger:
         """Get logger for log calls.
 
         :param instance: Owner class instance. Filled only if instance created, else None.
-        :type instance: typing.Optional[owner]
+        :type instance: _OwnerT | None
         :return: logger instance
         :rtype: logging.Logger
         """
         if self.logger is not None:
             return self.logger
         for logger_name in constants.VALID_LOGGER_NAMES:
             logger_candidate = getattr(instance, logger_name, None)
@@ -280,53 +286,53 @@
                 return logger_candidate
         return _LOGGER
 
     @typing.overload
     def __get__(
         self,
         instance: None,
-        owner: typing.Optional[typing.Type[_OwnerT]] = None,
+        owner: type[_OwnerT] | None = None,
     ) -> typing.NoReturn:
         """Get descriptor.
 
         :param instance: Owner class instance. Filled only if instance created, else None.
-        :type instance: typing.Optional[owner]
+        :type instance: _OwnerT | None
         :param owner: Owner class for property.
         :return: getter call result if getter presents
         :rtype: typing.Any
         :raises AttributeError: Getter is not available
         :raises Exception: Something goes wrong
         """
 
     @typing.overload
     def __get__(
         self,
         instance: _OwnerT,
-        owner: typing.Optional[typing.Type[_OwnerT]] = None,
-    ) -> _ReturnT:  # noqa: F811
+        owner: type[_OwnerT] | None = None,
+    ) -> _ReturnT:
         """Get descriptor.
 
         :param instance: Owner class instance. Filled only if instance created, else None.
-        :type instance: typing.Optional[owner]
+        :type instance: _OwnerT | None
         :param owner: Owner class for property.
         :return: getter call result if getter presents
         :rtype: typing.Any
         :raises AttributeError: Getter is not available
         :raises Exception: Something goes wrong
         """
 
     def __get__(
         self,
-        instance: typing.Optional[_OwnerT],
-        owner: typing.Optional[typing.Type[_OwnerT]] = None,
-    ) -> _ReturnT:  # noqa: F811
+        instance: _OwnerT | None,
+        owner: type[_OwnerT] | None = None,
+    ) -> _ReturnT:
         """Get descriptor.
 
         :param instance: Owner class instance. Filled only if instance created, else None.
-        :type instance: typing.Optional[owner]
+        :type instance: _OwnerT | None
         :param owner: Owner class for property.
         :return: getter call result if getter presents
         :rtype: typing.Any
         :raises AttributeError: Getter is not available
         :raises Exception: Something goes wrong
         """
         if instance is None or self.fget is None:
@@ -356,15 +362,15 @@
                 )
             raise
 
     def __set__(self, instance: _OwnerT, value: _ReturnT) -> None:
         """Set descriptor.
 
         :param instance: Owner class instance. Filled only if instance created, else None.
-        :type instance: typing.Optional
+        :type instance: _OwnerT | None
         :param value: Value for setter
         :raises AttributeError: Setter is not available
         :raises Exception: Something goes wrong
         """
         if self.fset is None:
             raise AttributeError()
 
@@ -392,15 +398,15 @@
                 )
             raise
 
     def __delete__(self, instance: _OwnerT) -> None:
         """Delete descriptor.
 
         :param instance: Owner class instance. Filled only if instance created, else None.
-        :type instance: typing.Optional
+        :type instance: _OwnerT | None
         :raises AttributeError: Deleter is not available
         :raises Exception: Something goes wrong
         """
         if self.fdel is None:
             raise AttributeError()
 
         source: str = self.__get_obj_source(instance)
@@ -419,28 +425,28 @@
                     self.exc_level,
                     f"Failed after {time.time() - timestamp:.03f}s: del {source}.{self.__name__}{self.__traceback}",
                     exc_info=False,
                 )
             raise
 
     @property
-    def logger(self) -> typing.Optional[logging.Logger]:
+    def logger(self) -> logging.Logger | None:
         """Logger instance to use as override.
 
         :return: logger instance if set
-        :rtype: typing.Optional[logging.Logger]
+        :rtype: logging.Logger | None
         """
         return self.__logger
 
     @logger.setter
-    def logger(self, logger: typing.Union[logging.Logger, str, None]) -> None:
+    def logger(self, logger: logging.Logger | str | None) -> None:
         """Logger instance to use as override.
 
         :param logger: logger instance, logger name or None if override disable required
-        :type logger: typing.Union[logging.Logger, str, None]
+        :type logger: logging.Logger | str | None
         """
         if logger is None or isinstance(logger, logging.Logger):
             self.__logger = logger
         else:
             self.__logger = logging.getLogger(logger)
 
     @property
@@ -566,28 +572,28 @@
 
         :param value: switch state
         :type value: bool
         """
         self.__log_traceback = value
 
     @property
-    def override_name(self) -> typing.Optional[str]:
+    def override_name(self) -> str | None:
         """Override property name if not None else use getter/setter/deleter name.
 
         :return: property name override
-        :rtype: typing.Optional[str]
+        :rtype: str | None
         """
         return self.__override_name
 
     @override_name.setter
-    def override_name(self, name: typing.Optional[str]) -> None:
+    def override_name(self, name: str | None) -> None:
         """Override property name if not None else use getter/setter/deleter name.
 
         :param name: property name override
-        :type name: typing.Optional[str]
+        :type name: str | None
         """
         self.__override_name = name
 
     @property
     def max_indent(self) -> int:
         """Max indent during repr.
```

### Comparing `logwrap-9.0.1.post0/logwrap/log_wrap.pxd` & `logwrap-9.0.2/logwrap/log_wrap.pxd`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 """log_wrap shared code module."""
 
 # Standard Library
 import inspect
 import logging
 import typing
 
-# Package Implementation
-
 cdef:
     unsigned long indent
 
 
     class LogWrap:
         """Base class for LogWrap implementation."""
```

### Comparing `logwrap-9.0.1.post0/logwrap/log_wrap.py` & `logwrap-9.0.2/logwrap/log_wrap.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 import types
 import typing
 
 # Package Implementation
 from logwrap import constants
 from logwrap import repr_utils
 
+if typing.TYPE_CHECKING:
+    # Standard Library
+    from collections.abc import Iterable
+    from collections.abc import MutableMapping
+
 __all__ = ("LogWrap", "logwrap", "BoundParameter", "bind_args_kwargs")
 
 LOGGER: logging.Logger = logging.getLogger("logwrap")
 INDENT = 4
 _CURRENT_FILE = os.path.abspath(__file__)
 
 _WrappedT = typing.TypeVar("_WrappedT", bound=typing.Callable[..., typing.Any])
@@ -127,31 +132,31 @@
 
         :return: representation for logging/debug purposes
         :rtype: str
         """
         return f'<{self.__class__.__name__} "{self}">'
 
 
-def bind_args_kwargs(sig: inspect.Signature, *args: typing.Any, **kwargs: typing.Any) -> typing.List[BoundParameter]:
+def bind_args_kwargs(sig: inspect.Signature, *args: typing.Any, **kwargs: typing.Any) -> list[BoundParameter]:
     """Bind *args and **kwargs to signature and get Bound Parameters.
 
     :param sig: source signature
     :type sig: inspect.Signature
     :param args: positional arguments
     :type args: typing.Any
     :param kwargs: keyword arguments
     :type kwargs: typing.Any
     :return: Iterator for bound parameters with all information about it
     :rtype: typing.List[BoundParameter]
 
     .. versionadded:: 3.3.0
     .. versionchanged:: 5.3.1 return list
     """
-    result: typing.List[BoundParameter] = []
-    bound: typing.MutableMapping[str, inspect.Parameter] = sig.bind(*args, **kwargs).arguments
+    result: list[BoundParameter] = []
+    bound: MutableMapping[str, inspect.Parameter] = sig.bind(*args, **kwargs).arguments
     for param in sig.parameters.values():
         result.append(BoundParameter(parameter=param, value=bound.get(param.name, param.default)))
     return result
 
 
 class LogWrap:
     """Base class for LogWrap implementation."""
@@ -167,20 +172,20 @@
         "__log_call_args_on_exc",
         "__log_traceback",
         "__log_result_obj",
     )
 
     def __init__(
         self,
-        log: typing.Optional[logging.Logger] = None,
+        log: logging.Logger | None = None,
         log_level: int = logging.DEBUG,
         exc_level: int = logging.ERROR,
         max_indent: int = 20,
-        blacklisted_names: typing.Optional[typing.Iterable[str]] = None,
-        blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]] = None,
+        blacklisted_names: Iterable[str] | None = None,
+        blacklisted_exceptions: Iterable[type[Exception]] | None = None,
         log_call_args: bool = True,
         log_call_args_on_exc: bool = True,
         log_traceback: bool = True,
         log_result_obj: bool = True,
     ) -> None:
         """Log function calls and return values.
 
@@ -189,18 +194,18 @@
         :param log_level: log level for successful calls
         :type log_level: int
         :param exc_level: log level for exception cases
         :type exc_level: int
         :param max_indent: maximum indent before classic `repr()` call.
         :type max_indent: int
         :param blacklisted_names: Blacklisted argument names. Arguments with this names will be skipped in log.
-        :type blacklisted_names: typing.Optional[typing.Iterable[str]]
+        :type blacklisted_names: Iterable[str] | None
         :param blacklisted_exceptions: list of exception, which should be re-raised
                without producing traceback and text log record.
-        :type blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]]
+        :type blacklisted_exceptions: Iterable[type[Exception]]
         :param log_call_args: log call arguments before executing wrapped function.
         :type log_call_args: bool
         :param log_call_args_on_exc: log call arguments if exception raised.
         :type log_call_args_on_exc: bool
         :param log_traceback: log traceback on exception in addition to failure info
         :type log_traceback: bool
         :param log_result_obj: log result of function call.
@@ -209,24 +214,24 @@
         .. versionchanged:: 3.3.0 Extract func from log and do not use Union.
         .. versionchanged:: 5.1.0 log_traceback parameter
         .. versionchanged:: 8.0.0 pick up logger from target module if possible
         .. versionchanged:: 9.0.0 Only LogWrap instance act as decorator
         """
         # Typing fix:
         if blacklisted_names is None:
-            self.__blacklisted_names: typing.List[str] = []
+            self.__blacklisted_names: list[str] = []
         else:
             self.__blacklisted_names = list(blacklisted_names)
         if blacklisted_exceptions is None:
-            self.__blacklisted_exceptions: typing.List[typing.Type[Exception]] = []
+            self.__blacklisted_exceptions: list[type[Exception]] = []
         else:
             self.__blacklisted_exceptions = list(blacklisted_exceptions)
 
         if isinstance(log, logging.Logger):
-            self.__logger: typing.Optional[logging.Logger] = log
+            self.__logger: logging.Logger | None = log
         else:
             self.__logger = None
 
         self.__log_level: int = log_level
         self.__exc_level: int = exc_level
         self.__max_indent: int = max_indent
         self.__log_call_args: bool = log_call_args
@@ -314,24 +319,24 @@
         :raises TypeError: indent is not integer
         """
         if not isinstance(val, int):
             raise TypeError(f"Unexpected type: {val.__class__.__name__}. Should be {int.__name__}.")
         self.__max_indent = val
 
     @property
-    def blacklisted_names(self) -> typing.List[str]:
+    def blacklisted_names(self) -> list[str]:
         """List of arguments names to ignore in log.
 
         :return: list of arguments to ignore in log
         :rtype: typing.List[str]
         """
         return self.__blacklisted_names
 
     @property
-    def blacklisted_exceptions(self) -> typing.List[typing.Type[Exception]]:
+    def blacklisted_exceptions(self) -> list[type[Exception]]:
         """List of exceptions to re-raise without log traceback and text.
 
         :return: list of exceptions to re-raise silent
         :rtype: typing.List[typing.Type[Exception]]
         """
         return self.__blacklisted_exceptions
 
@@ -416,15 +421,15 @@
         :raises TypeError: Value is not bool
         """
         if not isinstance(val, bool):
             raise TypeError(f"Unexpected type: {val.__class__.__name__}. Should be {bool.__name__}.")
         self.__log_result_obj = val
 
     @property
-    def _logger(self) -> typing.Optional[logging.Logger]:
+    def _logger(self) -> logging.Logger | None:
         """Logger instance.
 
         :return: logger instance if configured
         :rtype: typing.Optional[logging.Logger]
         """
         return self.__logger
 
@@ -447,15 +452,15 @@
             f"log_result_obj={self.log_result_obj}, )"
         )
 
     # noinspection PyMethodMayBeStatic
     def pre_process_param(  # pylint: disable=no-self-use
         self,
         arg: BoundParameter,
-    ) -> typing.Union[BoundParameter, typing.Tuple[BoundParameter, typing.Any], None]:
+    ) -> BoundParameter | tuple[BoundParameter, typing.Any] | None:
         """Process parameter for the future logging.
 
         :param arg: bound parameter
         :type arg: BoundParameter
         :return: value, value override for logging or None if argument should not be logged.
         :rtype: typing.Union[BoundParameter, typing.Tuple[BoundParameter, typing.Any], None]
 
@@ -509,16 +514,16 @@
             if isinstance(value, types.MethodType):  # pragma: no cover
                 return f"<method {base_name} {base_details}>"
             return f"<object {base_name} {base_details}>"
 
     def _get_func_args_repr(
         self,
         sig: inspect.Signature,
-        args: typing.Tuple[typing.Any, ...],
-        kwargs: typing.Dict[str, typing.Any],
+        args: tuple[typing.Any, ...],
+        kwargs: dict[str, typing.Any],
     ) -> str:
         """Internal helper for reducing complexity of decorator code.
 
         :param sig: function signature
         :type sig: inspect.Signature
         :param args: positional arguments
         :type args: typing.Tuple
@@ -535,17 +540,15 @@
         param_str: str = ""
 
         last_kind = None
         for param in bind_args_kwargs(sig, *args, **kwargs):
             if param.name in self.blacklisted_names:
                 continue
 
-            preprocessed: typing.Union[
-                BoundParameter, typing.Tuple[BoundParameter, typing.Any], None
-            ] = self.pre_process_param(param)
+            preprocessed: (BoundParameter | tuple[BoundParameter, typing.Any] | None) = self.pre_process_param(param)
             if preprocessed is None:
                 continue
 
             if isinstance(preprocessed, (tuple, list)):
                 param, value = preprocessed
             else:
                 value = param.value
@@ -614,16 +617,16 @@
         :param arguments: function arguments repr
         :type arguments: str
         :param exception: exception captured
         :type exception: Exception
         """
         exc_info = sys.exc_info()
         stack: traceback.StackSummary = traceback.extract_stack()
-        full_tb: typing.List[traceback.FrameSummary] = [elem for elem in stack if elem.filename != _CURRENT_FILE]
-        exc_line: typing.List[str] = traceback.format_exception_only(*exc_info[:2])
+        full_tb: list[traceback.FrameSummary] = [elem for elem in stack if elem.filename != _CURRENT_FILE]
+        exc_line: list[str] = traceback.format_exception_only(*exc_info[:2])
         # Make standard traceback string
         tb_text: str = (
             f"Traceback (most recent call last):\n{''.join(traceback.format_list(full_tb))}{''.join(exc_line)}"
             if self.log_traceback and not isinstance(exception, tuple(self.blacklisted_exceptions))
             else exception.__class__.__name__
         )
 
@@ -680,109 +683,109 @@
                 result = func(*args, **kwargs)
                 self._make_done_record(logger=logger, func_name=func.__name__, result=result)
             except Exception as e:
                 self._make_exc_record(logger=logger, name=func.__name__, arguments=args_repr, exception=e)
                 raise
             return result
 
-        return async_wrapper if asyncio.iscoroutinefunction(func) else wrapper  # type: ignore
+        return async_wrapper if asyncio.iscoroutinefunction(func) else wrapper  # type: ignore[return-value]
 
     def __call__(self, func: _WrappedT) -> _WrappedT:
         """Callable instance.
 
         :return: decorated function
         :rtype: typing.Callable[..., FuncResultType]
         """
         return self._get_function_wrapper(func)
 
 
 @typing.overload
 def logwrap(
     *,
-    log: typing.Optional[logging.Logger] = None,
+    log: logging.Logger | None = None,
     log_level: int = logging.DEBUG,
     exc_level: int = logging.ERROR,
     max_indent: int = 20,
-    blacklisted_names: typing.Optional[typing.Iterable[str]] = None,
-    blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]] = None,
+    blacklisted_names: Iterable[str] | None = None,
+    blacklisted_exceptions: Iterable[type[Exception]] | None = None,
     log_call_args: bool = True,
     log_call_args_on_exc: bool = True,
     log_traceback: bool = True,
     log_result_obj: bool = True,
 ) -> LogWrap:
     """Overload: with no func."""
 
 
 @typing.overload
 def logwrap(
     func: None = None,
     *,
-    log: typing.Optional[logging.Logger] = None,
+    log: logging.Logger | None = None,
     log_level: int = logging.DEBUG,
     exc_level: int = logging.ERROR,
     max_indent: int = 20,
-    blacklisted_names: typing.Optional[typing.Iterable[str]] = None,
-    blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]] = None,
+    blacklisted_names: Iterable[str] | None = None,
+    blacklisted_exceptions: Iterable[type[Exception]] | None = None,
     log_call_args: bool = True,
     log_call_args_on_exc: bool = True,
     log_traceback: bool = True,
     log_result_obj: bool = True,
 ) -> LogWrap:
     """Overload: with no func."""
 
 
-@typing.overload  # noqa: F811
+@typing.overload
 def logwrap(
     func: _WrappedT,
     *,
-    log: typing.Optional[logging.Logger] = None,
+    log: logging.Logger | None = None,
     log_level: int = logging.DEBUG,
     exc_level: int = logging.ERROR,
     max_indent: int = 20,
-    blacklisted_names: typing.Optional[typing.Iterable[str]] = None,
-    blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]] = None,
+    blacklisted_names: Iterable[str] | None = None,
+    blacklisted_exceptions: Iterable[type[Exception]] | None = None,
     log_call_args: bool = True,
     log_call_args_on_exc: bool = True,
     log_traceback: bool = True,
     log_result_obj: bool = True,
 ) -> _WrappedT:
     """Overload: func provided."""
 
 
-def logwrap(  # noqa: F811
-    func: typing.Optional[_WrappedT] = None,
+def logwrap(
+    func: _WrappedT | None = None,
     *,
-    log: typing.Optional[logging.Logger] = None,
+    log: logging.Logger | None = None,
     log_level: int = logging.DEBUG,
     exc_level: int = logging.ERROR,
     max_indent: int = 20,
-    blacklisted_names: typing.Optional[typing.Iterable[str]] = None,
-    blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]] = None,
+    blacklisted_names: Iterable[str] | None = None,
+    blacklisted_exceptions: Iterable[type[Exception]] | None = None,
     log_call_args: bool = True,
     log_call_args_on_exc: bool = True,
     log_traceback: bool = True,
     log_result_obj: bool = True,
-) -> typing.Union[LogWrap, _WrappedT]:
+) -> LogWrap | _WrappedT:
     """Log function calls and return values.
 
     :param func: function to wrap
     :type func: typing.Optional[typing.Callable]
     :param log: logger object for decorator, by default trying to use logger from target module. Fallback: 'logwrap'
     :type log: typing.Optional[logging.Logger]
     :param log_level: log level for successful calls
     :type log_level: int
     :param exc_level: log level for exception cases
     :type exc_level: int
     :param max_indent: maximum indent before classic `repr()` call.
     :type max_indent: int
     :param blacklisted_names: Blacklisted argument names. Arguments with this names will be skipped in log.
-    :type blacklisted_names: typing.Optional[typing.Iterable[str]]
+    :type blacklisted_names: Iterable[str] | None
     :param blacklisted_exceptions: list of exceptions, which should be re-raised
                                    without producing traceback and text log record.
-    :type blacklisted_exceptions: typing.Optional[typing.Iterable[typing.Type[Exception]]]
+    :type blacklisted_exceptions: Iterable[type[Exception]] | None
     :param log_call_args: log call arguments before executing wrapped function.
     :type log_call_args: bool
     :param log_call_args_on_exc: log call arguments if exception raised.
     :type log_call_args_on_exc: bool
     :param log_traceback: log traceback on exception in addition to failure info
     :type log_traceback: bool
     :param log_result_obj: log result of function call.
```

### Comparing `logwrap-9.0.1.post0/logwrap/log_wrap.pyx` & `logwrap-9.0.2/logwrap/log_wrap.pyx`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/logwrap/repr_utils.pxd` & `logwrap-9.0.2/logwrap/repr_utils.pxd`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/logwrap/repr_utils.py` & `logwrap-9.0.2/logwrap/repr_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 # Standard Library
 import abc
 import inspect
 import types
 import typing
 
+if typing.TYPE_CHECKING:
+    # Standard Library
+    from collections.abc import Callable
+    from collections.abc import Iterable
+
 __all__ = ("PrettyFormat", "PrettyRepr", "PrettyStr", "pretty_repr", "pretty_str")
 
 
 def _known_callable(item: typing.Any) -> bool:
     """Check for possibility to parse callable.
 
     :param item:  item to check for repr() way
@@ -83,19 +88,19 @@
 
         :return: original inspect.Parameter object
         :rtype: inspect.Parameter
         """
         return self._parameter
 
     @property
-    def name(self) -> typing.Union[None, str]:
+    def name(self) -> None | str:
         """Parameter name.
 
         :return: parameter name. For `*args` and `**kwargs` add corresponding prefixes
-        :rtype: typing.Union[None, str]
+        :rtype: None | str
         """
         if self.kind == inspect.Parameter.VAR_POSITIONAL:
             return "*" + self.parameter.name
         if self.kind == inspect.Parameter.VAR_KEYWORD:
             return "**" + self.parameter.name
         return self.parameter.name
 
@@ -105,19 +110,19 @@
 
         :return: If function is bound to class -> value is class instance else default value.
         :rtype: typing.Any
         """
         return self._value
 
     @property
-    def annotation(self) -> typing.Union[inspect.Parameter.empty, str]:
+    def annotation(self) -> inspect.Parameter.empty | str:
         """Parameter annotation.
 
         :return: parameter annotation from signature
-        :rtype: typing.Union[inspect.Parameter.empty, str]
+        :rtype: inspect.Parameter.empty | str
         """
         return self.parameter.annotation
 
     @property
     def kind(self) -> int:
         """Parameter kind.
 
@@ -140,33 +145,33 @@
 
         :return: parameter repr for debug purposes
         :rtype: str
         """
         return f'<{self.__class__.__name__} "{self}">'
 
 
-def _prepare_repr(func: typing.Union[types.FunctionType, types.MethodType]) -> typing.List[ReprParameter]:
+def _prepare_repr(func: types.FunctionType | types.MethodType) -> list[ReprParameter]:
     """Get arguments lists with defaults.
 
     :param func: Callable object to process
-    :type func: typing.Union[types.FunctionType, types.MethodType]
+    :type func: types.FunctionType | types.MethodType
     :return: repr of callable parameter from signature
-    :rtype: typing.List[ReprParameter]
+    :rtype: list[ReprParameter]
     """
     ismethod: bool = isinstance(func, types.MethodType)
     self_processed: bool = False
-    result: typing.List[ReprParameter] = []
+    result: list[ReprParameter] = []
     if not ismethod:
-        real_func: typing.Callable[..., typing.Any] = func
+        real_func: Callable[..., typing.Any] = func
     else:
-        real_func = func.__func__  # type: ignore
+        real_func = func.__func__  # type: ignore[union-attr]
 
     for param in inspect.signature(real_func).parameters.values():
-        if not self_processed and ismethod and func.__self__ is not None:  # type: ignore
-            result.append(ReprParameter(param, value=func.__self__))  # type: ignore
+        if not self_processed and ismethod and func.__self__ is not None:  # type: ignore[union-attr]
+            result.append(ReprParameter(param, value=func.__self__))  # type: ignore[union-attr]
             self_processed = True
         else:
             result.append(ReprParameter(param))
 
     return result
 
 
@@ -217,21 +222,21 @@
         :return: next indentation value
         :rtype: int
         """
         return indent + multiplier * self.indent_step
 
     def _repr_callable(
         self,
-        src: typing.Union[types.FunctionType, types.MethodType],
+        src: types.FunctionType | types.MethodType,
         indent: int = 0,
     ) -> str:
         """Repr callable object (function or method).
 
         :param src: Callable to process
-        :type src: typing.Union[types.FunctionType, types.MethodType]
+        :type src: types.FunctionType | types.MethodType
         :param indent: start indentation
         :type indent: int
         :return: Repr of function or method with signature.
         :rtype: str
         """
         param_str: str = ""
         prefix: str = "\n" + " " * self.next_indent(indent)
@@ -279,21 +284,21 @@
         :return: simple repr() over object
         :rtype: str
         """
 
     @abc.abstractmethod
     def _repr_dict_items(
         self,
-        src: typing.Dict[typing.Any, typing.Any],
+        src: dict[typing.Any, typing.Any],
         indent: int = 0,
     ) -> str:
         """Repr dict items.
 
         :param src: object to process
-        :type src: typing.Dict
+        :type src: dict[typing.Any, typing.Any]
         :param indent: start indentation
         :type indent: int
         :return: repr of key/value pairs from dict
         :rtype: str
         """
 
     @staticmethod
@@ -322,28 +327,28 @@
         :type suffix: str
         :return: formatted repr of "result" with prefix and suffix to explain type.
         :rtype: str
         """
 
     def _repr_iterable_items(
         self,
-        src: typing.Iterable[typing.Any],
+        src: Iterable[typing.Any],
         indent: int = 0,
     ) -> str:
         """Repr iterable items (not designed for dicts).
 
         :param src: object to process
-        :type src: typing.Iterable
+        :type src: Iterable[typing.Any]
         :param indent: start indentation
         :type indent: int
         :return: repr of elements in iterable item
         :rtype: str
         """
         next_indent: int = self.next_indent(indent)
-        buf: typing.List[str] = []
+        buf: list[str] = []
         for elem in src:
             buf.append("\n")
             buf.append(self.process_element(src=elem, indent=next_indent))
             buf.append(",")
         return "".join(buf)
 
     @property
@@ -370,15 +375,15 @@
         :param no_indent_start: do not indent open bracket and simple parameters
         :type no_indent_start: bool
         :return: formatted string
         :rtype: str
         """
         if hasattr(src, self._magic_method_name):
             result = getattr(src, self._magic_method_name)(self, indent=indent, no_indent_start=no_indent_start)
-            return result  # type: ignore
+            return result  # type: ignore[no-any-return]
 
         if _known_callable(src):
             return self._repr_callable(src=src, indent=indent)
 
         if _simple(src) or indent >= self.max_indent or not src:
             return self._repr_simple(src=src, indent=indent, no_indent_start=no_indent_start)
 
@@ -459,30 +464,30 @@
         :return: simple repr() over object, except strings (add prefix) and set (uniform py2/py3)
         :rtype: str
         """
         return f"{'':<{0 if no_indent_start else indent}}{src!r}"
 
     def _repr_dict_items(
         self,
-        src: typing.Dict[typing.Any, typing.Any],
+        src: dict[typing.Any, typing.Any],
         indent: int = 0,
     ) -> str:
         """Repr dict items.
 
         :param src: object to process
-        :type src: typing.Dict
+        :type src: dict[typing.Any, typing.Any]
         :param indent: start indentation
         :type indent: int
         :return: repr of key/value pairs from dict
         :rtype: str
         """
-        max_len: int = max((len(repr(key)) for key in src)) if src else 0
+        max_len: int = max(len(repr(key)) for key in src) if src else 0
         next_indent: int = self.next_indent(indent)
         prefix: str = "\n" + " " * next_indent
-        buf: typing.List[str] = []
+        buf: list[str] = []
         for key, val in src.items():
             buf.append(prefix)
             buf.append(f"{key!r:{max_len}}: ")
             buf.append(self.process_element(val, indent=next_indent, no_indent_start=True))
             buf.append(",")
         return "".join(buf)
 
@@ -530,22 +535,22 @@
         :rtype: str
         """
         return "__pretty_str__"
 
     @staticmethod
     def _strings_str(
         indent: int,
-        val: typing.Union[bytes, str],
+        val: bytes | str,
     ) -> str:
         """Custom str for strings and binary strings.
 
         :param indent: result indent
         :type indent: int
         :param val: value for repr
-        :type val: typing.Union[bytes, str]
+        :type val: bytes | str
         :return: indented string as `str`
         :rtype: str
         """
         if isinstance(val, bytes):
             string: str = val.decode(encoding="utf-8", errors="backslashreplace")
         else:
             string = val
@@ -571,30 +576,30 @@
         indent = 0 if no_indent_start else indent
         if isinstance(src, (bytes, str)):
             return self._strings_str(indent=indent, val=src)
         return f"{'':<{indent}}{src!s}"
 
     def _repr_dict_items(
         self,
-        src: typing.Dict[typing.Any, typing.Any],
+        src: dict[typing.Any, typing.Any],
         indent: int = 0,
     ) -> str:
         """Repr dict items.
 
         :param src: object to process
-        :type src: typing.Dict
+        :type src: dict[typing.Any, typing.Any]
         :param indent: start indentation
         :type indent: int
         :return: repr of key/value pairs from dict
         :rtype: str
         """
-        max_len = max((len(str(key)) for key in src)) if src else 0
+        max_len = max(len(str(key)) for key in src) if src else 0
         next_indent: int = self.next_indent(indent)
         prefix: str = "\n" + " " * next_indent
-        buf: typing.List[str] = []
+        buf: list[str] = []
         for key, val in src.items():
             buf.append(prefix)
             buf.append(f"{key!s:{max_len}}: ")
             buf.append(self.process_element(val, indent=next_indent, no_indent_start=True))
             buf.append(",")
         return "".join(buf)
```

### Comparing `logwrap-9.0.1.post0/logwrap/repr_utils.pyx` & `logwrap-9.0.2/logwrap/repr_utils.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             bint ismethod = isinstance(func, types.MethodType)
             bint self_processed = False
             list result = []
 
         if not ismethod:
             real_func = func
         else:
-            real_func = func.__func__  # type: ignore
+            real_func = func.__func__
 
         for param in inspect.signature(real_func).parameters.values():
             if not self_processed and ismethod and func.__self__ is not None:
                 result.append(ReprParameter(param, value=func.__self__))
                 self_processed = True
             else:
                 result.append(ReprParameter(param))
@@ -309,15 +309,15 @@
             str prefix
             str suffix
             str result
             str new_line
 
         if hasattr(src, self._magic_method_name):
             result = getattr(src, self._magic_method_name)(self, indent=indent, no_indent_start=no_indent_start)
-            return result  # type: ignore
+            return result
 
         if _known_callable(src):
             return self._repr_callable(src=src, indent=indent)
 
         if _simple(src) or indent >= self.max_indent or not src:
             return self._repr_simple(src=src, indent=indent, no_indent_start=no_indent_start)
```

### Comparing `logwrap-9.0.1.post0/logwrap.egg-info/PKG-INFO` & `logwrap-9.0.2/logwrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logwrap
-Version: 9.0.1.post0
+Version: 9.0.2
 Summary: Decorator for logging function arguments and return value by human-readable way
 Home-page: https://github.com/python-useful-helpers/logwrap
 Author: Alexey Stepanov
 Author-email: penguinolog@gmail.com
 Maintainer: Alexey Stepanov <penguinolog@gmail.com>, Antonio Esposito <esposito.cloud@gmail.com>, Dennis Dmitriev <dis-xcom@gmail.com>
 License: Apache License, Version 2.0
 Project-URL: Bug Tracker, https://github.com/python-useful-helpers/logwrap/issues
```

### Comparing `logwrap-9.0.1.post0/logwrap.egg-info/SOURCES.txt` & `logwrap-9.0.2/logwrap.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .editorconfig
+.pre-commit-config.yaml
 .pydocstyle.ini
 CI_REQUIREMENTS.txt
 LICENSE
 MANIFEST.in
 README.rst
 build_requirements.txt
 flake8_requirements.txt
```

### Comparing `logwrap-9.0.1.post0/pyproject.toml` & `logwrap-9.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/setup.cfg` & `logwrap-9.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `logwrap-9.0.1.post0/setup.py` & `logwrap-9.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,40 +16,36 @@
 
 """logwrap decorator for human-readable logging of command arguments."""
 
 from __future__ import annotations
 
 # Standard Library
 import ast
-import distutils.errors
 import os.path
-import shutil
 import sys
-import typing
-from distutils.command import build_ext
 
 # External Dependencies
 import setuptools
 
 try:
     # noinspection PyPackageRequirements
     # External Dependencies
     from Cython.Build import cythonize
 except ImportError:
     cythonize = None
 
 PACKAGE_NAME = "logwrap"
 
-with open(os.path.join(os.path.dirname(__file__), PACKAGE_NAME, "__init__.py")) as f:
+with open(os.path.join(os.path.dirname(__file__), PACKAGE_NAME, "__init__.py"), encoding="utf-8") as f:
     SOURCE = f.read()
 
-with open("requirements.txt") as f:
+with open("requirements.txt", encoding="utf-8") as f:
     REQUIRED = f.read().splitlines()
 
-with open("README.rst") as f:
+with open("README.rst", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 
 # noinspection PyCallingNonCallable
 if cythonize is not None:
     if "win32" != sys.platform:
         REQUIRES_OPTIMIZATION = [
@@ -61,81 +57,33 @@
         REQUIRES_OPTIMIZATION = [
             setuptools.Extension("logwrap.repr_utils", ["logwrap/repr_utils.pyx"]),
         ]
         INTERFACES = ["repr_utils.pxd"]
 
     EXT_MODULES = cythonize(
         module_list=REQUIRES_OPTIMIZATION,
+        exclude_failures=True,
         compiler_directives={
             "always_allow_keywords": True,
             "binding": True,
             "embedsignature": True,
             "overflowcheck": True,
             "language_level": 3,
         },
     )
 else:
     REQUIRES_OPTIMIZATION = []
     INTERFACES = []
     EXT_MODULES = []
 
 
-class BuildFailed(Exception):
-    """For install clear scripts."""
-
-
-class AllowFailRepair(build_ext.build_ext):
-    """This class allows C extension building to fail and repairs init."""
-
-    def run(self) -> None:
-        """Run.
-
-        :raises BuildFailed: Build is failed and clean python code should be used.
-        """
-        try:
-            build_ext.build_ext.run(self)
-
-            # Copy __init__.py back to repair package.
-            build_dir = os.path.abspath(self.build_lib)
-            root_dir = os.path.abspath(os.path.join(__file__, ".."))
-            target_dir = build_dir if not self.inplace else root_dir
-
-            src_file = os.path.join(PACKAGE_NAME, "__init__.py")
-
-            src = os.path.join(root_dir, src_file)
-            dst = os.path.join(target_dir, src_file)
-
-            if src != dst:
-                shutil.copyfile(src, dst)
-        except (
-            distutils.errors.DistutilsPlatformError,
-            FileNotFoundError,
-        ) as exc:
-            raise BuildFailed() from exc
-
-    def build_extension(self, ext) -> None:
-        """build_extension.
-
-        :raises BuildFailed: Build is failed and clean python code should be used.
-        """
-        try:
-            build_ext.build_ext.build_extension(self, ext)
-        except (
-            distutils.errors.CCompilerError,
-            distutils.errors.DistutilsExecError,
-            distutils.errors.DistutilsPlatformError,
-            ValueError,
-        ) as exc:
-            raise BuildFailed() from exc
-
-
 # noinspection PyUnresolvedReferences
 def get_simple_vars_from_src(
     src: str,
-) -> typing.Dict[str, typing.Union[str, bytes, int, float, complex, list, set, dict, tuple, None, bool, Ellipsis]]:
+) -> dict[str, str | bytes | int | float | complex | list | set | dict | tuple | None | bool | Ellipsis]:
     """Get simple (string/number/boolean and None) assigned values from source.
 
     :param src: Source code
     :type src: str
     :return: OrderedDict with keys, values = variable names, values
     :rtype: typing.Dict[
                 str,
@@ -211,21 +159,19 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 KEYWORDS = ["logging", "debugging", "development"]
 
-SETUP_ARGS: typing.Dict[str, typing.Union[str, typing.List[str], typing.Dict[str, typing.List[str]]]] = dict(
+SETUP_ARGS: dict[str, str | list[str] | dict[str, list[str]]] = dict(
     name=PACKAGE_NAME,
     author=VARIABLES["__author__"],
     author_email=VARIABLES["__author_email__"],
-    maintainer=", ".join(
-        "{name} <{email}>".format(name=name, email=email) for name, email in VARIABLES["__maintainers__"].items()
-    ),
+    maintainer=", ".join(f"{name} <{email}>" for name, email in VARIABLES["__maintainers__"].items()),
     url=VARIABLES["__url__"],
     license=VARIABLES["__license__"],
     description=VARIABLES["__description__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     classifiers=CLASSIFIERS,
     keywords=KEYWORDS,
@@ -245,17 +191,10 @@
     ],
     use_scm_version={"write_to": f"{PACKAGE_NAME}/_version.py"},
     install_requires=REQUIRED,
     package_data={PACKAGE_NAME: INTERFACES + ["py.typed"]},
 )
 if cythonize is not None:
     SETUP_ARGS["ext_modules"] = EXT_MODULES
-    SETUP_ARGS["cmdclass"] = dict(build_ext=AllowFailRepair)
 
-try:
-    setuptools.setup(**SETUP_ARGS)
-except BuildFailed:
-    print("*" * 80 + "\n* Build Failed!\n* Use clear scripts version.\n" + "*" * 80 + "\n")
-    del SETUP_ARGS["ext_modules"]
-    del SETUP_ARGS["cmdclass"]
-    SETUP_ARGS["package_data"][PACKAGE_NAME] = ["py.typed"]
-    setuptools.setup(**SETUP_ARGS)
+
+setuptools.setup(**SETUP_ARGS)
```

