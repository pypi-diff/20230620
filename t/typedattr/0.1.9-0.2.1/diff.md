# Comparing `tmp/typedattr-0.1.9.tar.gz` & `tmp/typedattr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedattr-0.1.9.tar", last modified: Wed Mar 29 15:23:03 2023, max compression
+gzip compressed data, was "typedattr-0.2.1.tar", last modified: Tue Jun 20 09:53:58 2023, max compression
```

## Comparing `typedattr-0.1.9.tar` & `typedattr-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 15:23:03.859237 typedattr-0.1.9/
--rw-rw-rw-   0        0        0    11336 2023-03-29 13:28:06.000000 typedattr-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     3875 2023-03-29 15:23:03.858238 typedattr-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-03-29 15:22:14.000000 typedattr-0.1.9/README.md
--rw-rw-rw-   0        0        0     2268 2023-03-29 15:20:31.000000 typedattr-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 15:23:03.859237 typedattr-0.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-29 15:23:03.828925 typedattr-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-03-29 15:23:03.836937 typedattr-0.1.9/src/typedattr/
--rw-rw-rw-   0        0        0      121 2023-03-29 15:22:14.000000 typedattr-0.1.9/src/typedattr/__init__.py
--rw-rw-rw-   0        0        0    11027 2023-03-29 15:22:14.000000 typedattr-0.1.9/src/typedattr/_typedattr.py
--rw-rw-rw-   0        0        0      243 2023-03-29 15:22:14.000000 typedattr-0.1.9/src/typedattr/attrutils.py
--rw-rw-rw-   0        0        0     3090 2023-03-29 15:22:14.000000 typedattr-0.1.9/src/typedattr/cacheutils.py
--rw-rw-rw-   0        0        0     8799 2023-03-29 15:22:14.000000 typedattr-0.1.9/src/typedattr/objutils.py
--rw-rw-rw-   0        0        0      192 2023-03-29 15:22:14.000000 typedattr-0.1.9/src/typedattr/typeutils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 15:23:03.857230 typedattr-0.1.9/src/typedattr.egg-info/
--rw-rw-rw-   0        0        0     3875 2023-03-29 15:23:03.000000 typedattr-0.1.9/src/typedattr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-03-29 15:23:03.000000 typedattr-0.1.9/src/typedattr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 15:23:03.000000 typedattr-0.1.9/src/typedattr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-29 15:23:03.000000 typedattr-0.1.9/src/typedattr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-29 14:51:16.000000 typedattr-0.1.9/src/typedattr.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:53:58.733937 typedattr-0.2.1/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-03-30 08:00:06.000000 typedattr-0.2.1/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5007 2023-06-20 09:53:58.729937 typedattr-0.2.1/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4207 2023-06-20 09:37:24.000000 typedattr-0.2.1/README.md
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2330 2023-03-30 10:16:34.000000 typedattr-0.2.1/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       39 2023-06-20 09:37:24.000000 typedattr-0.2.1/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-20 09:53:58.733937 typedattr-0.2.1/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:53:58.633935 typedattr-0.2.1/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:53:58.657936 typedattr-0.2.1/src/typedattr/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      209 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    12187 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/_typedattr.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/const.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      715 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:53:58.725937 typedattr-0.2.1/src/typedattr/utils/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)       40 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/utils/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3090 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/utils/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/utils/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/utils/dtime.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     4229 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/utils/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     9298 2023-06-20 09:37:24.000000 typedattr-0.2.1/src/typedattr/utils/objects.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:53:58.701937 typedattr-0.2.1/src/typedattr.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5007 2023-06-20 09:53:58.000000 typedattr-0.2.1/src/typedattr.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      549 2023-06-20 09:53:58.000000 typedattr-0.2.1/src/typedattr.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 09:53:58.000000 typedattr-0.2.1/src/typedattr.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       39 2023-06-20 09:53:58.000000 typedattr-0.2.1/src/typedattr.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-06-20 09:53:58.000000 typedattr-0.2.1/src/typedattr.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 09:35:51.000000 typedattr-0.2.1/src/typedattr.egg-info/zip-safe
```

### Comparing `typedattr-0.1.9/LICENSE` & `typedattr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typedattr-0.1.9/PKG-INFO` & `typedattr-0.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,131 @@
-Metadata-Version: 2.1
-Name: typedattr
-Version: 0.1.9
-Summary: Typed conversion of dictionaries to attrs instances
-Author: gingsi
-License: Apache-2.0
-Project-URL: Project-URL, https://github.com/gingsi/typedattr
-Keywords: attrs,typing,dict,attr
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# typedattr
-
-Typechecking and conversion utility for [attrs](https://www.attrs.org/en/stable/).
-
-Parses a dictionary into an attrs instance. Contains other generic object, type and cache utilities.
-
-## Install
-
-Requires python 3.7 or higher.
-
-```bash
-pip install typedattr
-```
-
-## Quickstart
-
-Define class hierarchy and parse the input.
-
-~~~python
-from attrs import define
-from typing import Optional
-from typedattr import attrs_from_dict
-
-@define
-class Cfg:
-    foo: int = 12
-    bar: Optional[int] = None
-
-print(attrs_from_dict(Cfg, {"foo": 1, "bar": 2}))
-# Cfg(foo=1, bar=2)
-
-
-@define
-class CfgNested:
-    sub_cfg: Cfg = None
-
-print(attrs_from_dict(CfgNested, {"sub_cfg": {"foo": 1, "bar": 2}}))
-# CfgNested(sub_cfg=Cfg(foo=1, bar=2))
-~~~
-
-## Features
-
-* Nested checking and conversion of python standard types.
-* `@definenumpy` decorator for equality check if the instances contains numpy arrays.
-* Supports old and new style typing (e.g. `typing.List` and `list`)
-* Supports positional and keyword arguments in classes.
-* Can typecheck existing attrs instances.
-* Allows custom conversions, by default converts source type `str` to target type `Path` and
-  `int` to `float`.
-* Allows to redefine which objects will be recursed into, by default recurses into standard
-  containers (list, dict, etc.) 
-
-### Strict mode (default)
-
-* Convert everything to the target type, e.g. if the input is a list and the annotation is a tuple,
-  the output will be a tuple.
-* Raise errors if types cannot be matched, there are unknown fields in the input or
-  abstract annotation types are used (e.g. Sequence).
-
-### Non-strict mode
-
-Enabled by calling `attrs_from_dict` with `strict=False`
-
-* No conversion except for creating the attrs instance from the dict.
-* Ignore silently if types cannot be matched or abstract annotation types are used.
-* Warn about unknown fields in the input.
-
-### Hints
-
-The following behaviour stems from the `attrs` package:
-
-* New attributes cannot to be added after class definition to an attrs instance,
-  unless it is created with `@define(slots=False)`. 
-  [Explanation](https://www.attrs.org/en/21.2.0/glossary.html#term-slotted-classes)
-* Untyped fields or "ClassVar" typed fields will be ignored by @attrs.define
-  and therefore also by this library.
-
-### Possible improvements
-
-* Supports Callable but does not typecheck the signature
-* Not tested for NewType, Literal
-
-## Install locally and run tests
-
-Clone repository and cd into, then:
-
-~~~bash
-pip install -e .
-pip install pytest pytest-cov pylint
-pylint typedattr
-
-# run tests for python>=3.7
-python -m pytest --cov
-pylint tests
-
-# run tests for python>=3.9
-python -m pytest tests_py39 --cov
-pylint tests_py39
-
-~~~
-
-## Alternatives
-
-This library should be useful for off-the-shelf typechecking and conversion of dicts to
-attrs instances.
-
-For more complex use cases there are many alternatives: 
-`cattrs`, `attrs-strict`, `pydantic`, `dataconf` to name a few.
+# typedattr
+
+<p align="center">
+<a href="https://github.com/gingsi/typedattr/actions/workflows/build_py37.yml">
+  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py37.yml?branch=main&label=build%203.7" />
+</a>
+<a href="https://github.com/gingsi/typedattr/actions/workflows/build_py39.yml">
+  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py39.yml?branch=main&label=build%203.9" />
+</a>
+<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/typedattr/main/docs/coverage.svg" />
+<a href="https://pypi.org/project/typedattr/">
+  <img alt="version" title="version" src="https://img.shields.io/pypi/v/typedattr?color=success" />
+</a>
+</p>
+
+Typechecking and conversion utility for [attrs](https://www.attrs.org/en/stable/)
+
+Parses a dictionary into an attrs instance.
+Contains other generic object, type and cache utilities.
+
+## Install
+
+Requires `python>=3.7`
+
+Note: `0.2` breaks some backwards compatibility. Use `0.1` or update your code. 
+
+```bash
+pip install typedattr
+```
+
+## Quickstart
+
+Define the class hierarchy and parse the input using `attrs_from_dict`:
+
+~~~python
+from attrs import define
+from typing import Optional
+from typedattr import attrs_from_dict
+
+@define
+class Cfg:
+    foo: int = 12
+    bar: Optional[int] = None
+
+print(attrs_from_dict(Cfg, {"foo": 1, "bar": 2}))
+# Cfg(foo=1, bar=2)
+
+
+@define
+class CfgNested:
+    sub_cfg: Cfg = None
+
+print(attrs_from_dict(CfgNested, {"sub_cfg": {"foo": 1, "bar": 2}}))
+# CfgNested(sub_cfg=Cfg(foo=1, bar=2))
+~~~
+
+## Features
+
+* Nested checking and conversion of python standard types
+* Supports old and new style typing (e.g. `typing.List` and `list`)
+* Supports positional and keyword arguments in classes
+* Can also typecheck existing attrs instances
+* Allows custom conversions, by default converts source type `str` to target type `Path` and
+  `int` to `float`
+* Allows to redefine which objects will be recursed into, by default recurses into standard
+  containers (list, dict, etc.)
+* `@definenumpy` decorator for equality check if the instances contains numpy arrays
+
+### Strict mode (default)
+
+* Convert everything to the target type, e.g. if the input is a list and the annotation is a tuple,
+  the output will be a tuple
+* Raise errors if types cannot be matched, there are unknown fields in the input or
+  abstract annotation types are used (e.g. Sequence)
+
+### Non-strict mode
+
+Enabled by calling `attrs_from_dict` with `strict=False`
+
+* No conversion except for creating the attrs instance from the dict
+* Ignore silently if types cannot be matched or abstract annotation types are used
+* Unknown fields in the input will be added to the attrs instance if possible
+  (see the hint below about slots)
+
+### Skip unknowns
+
+Set `skip_unknowns=True` to ignore all unknown input fields.
+
+### Hints
+
+The following behaviour stems from the `attrs` package:
+
+* New attributes cannot to be added after class definition to an attrs instance,
+  unless it is created with `@define(slots=False)`
+  [Explanation](https://www.attrs.org/en/21.2.0/glossary.html#term-slotted-classes)
+* Untyped fields or "ClassVar" typed fields will be ignored by @attrs.define
+  and therefore also by this library.
+
+### Other utilities in the package 
+
+* `Const`: An alternative to `enum.Enum` for defining constants
+* `cacheutils`: Cache objects to disk / to memory
+* `objutils`: Various utilities like nested modification of dicts
+* Type definitions and other utilities
+
+## Install locally and run tests
+
+Clone repository and cd into, then:
+
+~~~bash
+pip install -e .
+pip install -U pytest pytest-cov pylint
+pylint typedattr
+
+# run tests for python>=3.7
+python -m pytest --cov
+pylint tests
+
+# run tests for python>=3.9
+python -m pytest tests tests_py39 --cov
+pylint tests 
+pylint tests_py39
+~~~
+
+## Alternatives
+
+This library should be useful for off-the-shelf typechecking and conversion of dicts to
+attrs instances.
+
+For more complex or other related use cases there are many alternatives:
+`cattrs`, `attrs-strict`, `pydantic`, `dataconf`, `omegaconf` to name a few.
```

### Comparing `typedattr-0.1.9/pyproject.toml` & `typedattr-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Version Control :: Git"
 ]
-dynamic = ["version"]
+dynamic = ["version", "dependencies"]
 
 [project.urls]
 Project-URL = "https://github.com/gingsi/typedattr"
 
 [tool.setuptools]
 zip-safe = true
 platforms = ["any"]
@@ -59,14 +59,15 @@
 enable = "all"
 
 disable = [
     'suppressed-message', 'locally-disabled', 'line-too-long', 'missing-module-docstring',
     'missing-class-docstring', 'missing-function-docstring', 'fixme',
     'f-string-without-interpolation', 'invalid-name',
     'logging-fstring-interpolation', 'consider-iterating-dictionary',
+    'use-implicit-booleaness-not-comparison',
     'attribute-defined-outside-init', 'consider-using-with', 'global-statement',
     'import-outside-toplevel', 'super-init-not-called', 'broad-exception-caught',
     'disallowed-name', 'redefined-outer-name', ]
 
 [tool.pylint.format]
 max-line-length = 99999
 max-module-lines = 99999
```

### Comparing `typedattr-0.1.9/src/typedattr/_typedattr.py` & `typedattr-0.2.1/src/typedattr/_typedattr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import collections
-import logging
 from functools import partial
 from inspect import isclass
 from pathlib import Path
 from typing import (
     Tuple, Union, Dict, AbstractSet, Iterable, Mapping, Collection, Type, Any, List, Optional)
 
 import attrs
 from attr import has, AttrsInstance
 from attrs import define, fields_dict, fields, Attribute
+from typedattr.typext import AttrsClass
+from typedattr.utils.objects import check_object_equality, RecursorInterface, StrictRecursor
 
 try:
     # python>=3.8
     from typing import get_origin, get_args
 except ImportError:
     # python<3.8
     from typing_extensions import get_origin, get_args
 
-from typedattr.typeutils import AttrsClass
-from typedattr.objutils import check_object_equality, RecursorInterface, StrictRecursor
-
 # default conversions allow to convert instead of raising errors in case of matching types
 # e.g. create Path given str, or create float given int
 conversion_type = List[Tuple[Tuple[Type, ...], Type]]
 default_conversions: conversion_type = [
     ((str,), Path),
     ((int,), float),
 ]
 
 
-def print_fn(*args, **kwargs):  # pylint: disable=unused-argument  # noqa
+def _print_fn(*args, **kwargs):  # pylint: disable=unused-argument  # noqa
     # print(*args, **kwargs)  # uncomment for debugging
     pass
 
 
 def definenumpy(maybe_cls: Union[bool, Type] = False, **kwargs):
     """
     @attrs.define decorator with added numpy equality check
@@ -49,52 +47,60 @@
         attrs_cls.__eq__ = check_object_equality
         return attrs_cls
 
     return wrap
 
 
 def attrs_from_dict(
-        cls: AttrsClass, input_dict_or_attrs_inst: Union[Dict, AttrsInstance], strict: bool = True,
+        cls: AttrsClass, input_dict_or_attrs_inst: Union[Dict, AttrsInstance],
+        strict: bool = True, skip_unknowns: bool = False,
         recursor_class: Type[RecursorInterface] = StrictRecursor,
         conversions: Optional[conversion_type] = None) -> AttrsInstance:
     """
     Create typechecked attrs instance from dictionary or existing attrs instance.
 
     Args:
         cls: class decorated with @attrs.define or @definetyped
         input_dict_or_attrs_inst: data source, dict or attrs instance.
         strict: whether to do type checking and conversion
+        skip_unknowns: whether to skip input fields that are not defined in cls
         recursor_class: recursor definition to find nested content
         conversions: custom conversions, e.g. if target is annotated as Path and value
             is given as str, then convert to Path instead of raising a TypeError.
             default converts int to float and str to Path.
             pass empty list to disable all conversions.
 
     Returns:
         Instance of cls with values from input_dict_or_attrs_inst
     """
     recursor = recursor_class()
-    return _attrs_from_dict(recursor, cls, input_dict_or_attrs_inst, strict=strict,
-                            conversions=conversions)
+    try:
+        return _attrs_from_dict(recursor, cls, input_dict_or_attrs_inst, strict=strict,
+                                skip_unknowns=skip_unknowns, conversions=conversions)
+    except TypeError as e:
+        raise TypeError(f"Error parsing {cls} from {input_dict_or_attrs_inst}, see the original "
+                        f"error above.") from e
 
 
 def _attrs_from_dict(
         recursor: RecursorInterface, cls: AttrsClass, input_dict_or_attrs: Union[Dict, object],
-        strict: bool = False, conversions: Optional[conversion_type] = None):
-    print_fn(f"Parsing {cls} from {input_dict_or_attrs}")
-    if has(input_dict_or_attrs):
+        strict: bool = False, skip_unknowns: bool = False,
+        conversions: Optional[conversion_type] = None):
+    _print_fn(f"Parsing {cls} from {input_dict_or_attrs}")
+    input_cls = type(input_dict_or_attrs)
+    if has(input_cls):
         # if given an attrs instance, convert it to dict and then
         # parse it for conversions and typechecking
-        input_cls = type(input_dict_or_attrs)
         assert input_cls == cls, (
             f"Mismatch: Trying to parse input of type {input_cls} as type {cls}")
         input_fields_dict = fields_dict(type(input_dict_or_attrs))
         input_dict: Dict[str, Any] = {k: getattr(input_dict_or_attrs, k) for k in input_fields_dict}
         return _attrs_from_dict(
-            recursor, input_cls, input_dict, strict=strict, conversions=conversions)
+            recursor, input_cls, input_dict, strict=strict, skip_unknowns=skip_unknowns,
+            conversions=conversions)
 
     input_dict: Dict[str, Any] = input_dict_or_attrs
     if input_dict is None:
         if strict:
             raise TypeError(f"Cannot parse None into {cls}")
         return None
 
@@ -104,21 +110,14 @@
     matching_input, nonmatching_input = {}, {}
     for key, value in input_dict.items():
         if key in all_att_names:
             matching_input[key] = value
         else:
             nonmatching_input[key] = value
 
-    if len(nonmatching_input) > 0:
-        err_msg = (f"Keys in input {list(nonmatching_input.keys())} not defined "
-                   f"for class {cls} with attributes {sorted(all_att_names)}")
-        if strict:
-            raise TypeError(err_msg)
-        logging.getLogger(__name__).warning(f"Skipped some keys from the input: {err_msg}")
-
     # split into positional and keyword arguments
     in_args, in_kwargs = [], {}
     cls_fields_dict = fields_dict(cls)
     for field_name, field_value in matching_input.items():
         field_att = cls_fields_dict[field_name]
         try:
             is_positional = bool(field_att.default == attrs.NOTHING)
@@ -134,50 +133,68 @@
     # create an attrs instance from the dict
     # the instance will be flat (nested dicts are not resolved yet) and not typechecked.
     attrs_inst = attrs.evolve(cls(*in_args), **in_kwargs)  # noqa
 
     # typecheck and unfold nested values in the attrs instance
     for att in all_atts:
         name = att.name
-        if name in nonmatching_input:
-            # skip adding illegal keys
-            continue
         value = getattr(attrs_inst, name)
         typ = att.type
         new_value = _parse_nested(recursor, name, value, typ, strict=strict,
-                                  conversions=conversions)
+                                  skip_unknowns=skip_unknowns, conversions=conversions)
         setattr(attrs_inst, name, new_value)
-    print_fn(f"Output of _attrs_from_dict: {attrs_inst}")
+
+    # handle unknown fields
+    if len(nonmatching_input) > 0 and not skip_unknowns:
+        if strict:
+            raise TypeError(f"Keys in input {list(nonmatching_input.keys())} not defined "
+                            f"for class {cls} with attributes {sorted(all_att_names)}")
+        for key, value in nonmatching_input.items():
+            if skip_unknowns:
+                break
+            # non-strict mode and keep unknowns: try to add it to the class
+            try:
+                setattr(attrs_inst, key, value)
+            except AttributeError as e:
+                raise AttributeError(
+                    f"Field {key} is missing from configuration {cls}. Either add it to the "
+                    f"configuration or decorate with @attrs.define(slots=False) to allow adding "
+                    f"unknown fields or set skip_unknowns=True to ignore them.") from e
+
+    _print_fn(f"Output of _attrs_from_dict: {attrs_inst}")
     return attrs_inst
 
 
-def _parse_nested(parser: RecursorInterface, name, value, typ, strict: bool = True,
+def _parse_nested(recursor: RecursorInterface, name, value, typ,
+                  strict: bool = True, skip_unknowns: bool = False,
                   conversions: conversion_type = None, depth: int = 0):
     conversions = default_conversions if conversions is None else conversions
-    parse_recursive = partial(_parse_nested, parser, depth=depth + 1)
+    parse_recursive = partial(_parse_nested, recursor, depth=depth + 1, skip_unknowns=skip_unknowns)
 
     origin = get_origin(typ)
     args = get_args(typ)
 
     target_type_name = typ.__name__ if hasattr(typ, "__name__") else str(typ)
     value_type = type(value)
     value_type_name = value_type.__name__ if hasattr(value_type, "__name__") else str(value_type)
     err_msg = (f"Could not parse {name}={value} (type {value_type_name}) as type "
-               f"{target_type_name} with strict={strict} depth={depth} "
-               f"type annotation origin={origin} args={args}")
+               f"{target_type_name} with strict={strict} "
+               # f"depth={depth} type annotation origin={origin} args={args}"
+               )
 
     def maybe_raise_typeerorr(full_err_msg):
         if strict:
             raise TypeError(full_err_msg)
-        print_fn(f"Caught: {full_err_msg}. Returning as is.")
+        _print_fn(f"Caught: {full_err_msg}. Returning as is.")
         return value
 
     # resolve nested attrclass
     if has(typ):
-        return _attrs_from_dict(parser, typ, value, strict=strict, conversions=conversions)
+        return _attrs_from_dict(recursor, typ, value, strict=strict, skip_unknowns=skip_unknowns,
+                                conversions=conversions)
 
     # resolve any
     if typ == Any:
         return value
 
     # resolve unions (mostly "optional")
     if origin == Union:
@@ -192,30 +209,30 @@
 
     final_list_type = None
 
     # check tuples
     if origin == tuple:
         if not (len(args) == 2 and args[1] == Ellipsis):
             # resolve fixed tuple
-            if not parser.is_iterable_fn(value):
+            if not recursor.is_iterable_fn(value):
                 return maybe_raise_typeerorr(f"{err_msg}. Expect a sequence, got {type(value)}")
             if len(value) != len(args):
                 return maybe_raise_typeerorr(
                     f"{err_msg}. Expect a sequence with length {len(args)}, got length {len(value)}")
             new_tuple = []
             for item, item_type in zip(value, args):
                 new_tuple.append(parse_recursive(name, item, item_type, strict=strict))
             return tuple(new_tuple)
         if len(args) == 0:
             # undefined tuple can be anything
             args = [Any, Ellipsis]
 
     # check dict
     if origin in (dict, collections.defaultdict):
-        if not parser.is_mapping_fn(value):
+        if not recursor.is_mapping_fn(value):
             return maybe_raise_typeerorr(f"{err_msg}. Expect a mapping, got {type(value)}")
         if len(args) == 0:
             args = [Any, Any]
         dict_keytype, dict_valuetype = args
 
         if origin == collections.defaultdict:
             # must keep the default factory if exists
@@ -234,15 +251,15 @@
         origin, final_list_type = list, origin
         if len(args) == 0:
             args = [Any]
         args = [args[0]]
 
     # resolve list
     if origin == list:
-        if not parser.is_iterable_fn(value):
+        if not recursor.is_iterable_fn(value):
             return maybe_raise_typeerorr(f"{err_msg}. Expect iterable, got {type(value)}")
         list_arg_type = args[0]
         list_output = []
         for item in value:
             list_item = parse_recursive(name, item, list_arg_type, strict=strict)
             list_output.append(list_item)
         if not strict:
@@ -253,18 +270,18 @@
         return list_output
 
     # try to parse as a regular type (float, etc), this also parses Callable and any other types
     # but only non-nested parsing and no further inspection.
     try:
         if isinstance(value, typ):
             return value
-        print_fn(f"Not compatible: {value} as {typ}, {err_msg}")
+        _print_fn(f"Not compatible: {value} as {typ}, {err_msg}")
 
     except TypeError as e:
-        print_fn(f"Caught {e} while trying to parse {value} as {typ}, {err_msg}")
+        _print_fn(f"Caught {e} while trying to parse {value} as {typ}, {err_msg}")
 
     # show better error message for abstract types
     try:
         is_sc = issubclass(origin, (AbstractSet, Mapping, Collection, Iterable))
     except TypeError:
         is_sc = False
     if is_sc:
@@ -274,10 +291,13 @@
     for convert_source, convert_target in conversions:
         if not isclass(typ):
             continue
         if issubclass(typ, convert_target) and isinstance(value, convert_source):
             return convert_target(value)
 
     if strict:
-        raise TypeError(f"{err_msg}. Wrong type or type not supported.")
-    print_fn(f"{err_msg}. Returning value {value} as-is")
+        add_info = ""
+        if typ is None:
+            add_info = "Untyped fields not allowed in strict mode. "
+        raise TypeError(f"{add_info}{err_msg}. Wrong type or type not supported.")
+    _print_fn(f"{err_msg}. Returning value {value} as-is")
     return value
```

### Comparing `typedattr-0.1.9/src/typedattr/cacheutils.py` & `typedattr-0.2.1/src/typedattr/utils/caching.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.1.9/src/typedattr/objutils.py` & `typedattr-0.2.1/src/typedattr/utils/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from copy import deepcopy
 from functools import partial
 from typing import Any, Callable, Type, List
 
 import numpy as np
 from attr import has
 
-from .attrutils import get_attr_names
+from typedattr.typext import get_attr_names
 
 
 def get_all_base_classes(klass: type) -> List[type]:
     for base in klass.__bases__:
         yield base
         yield from get_all_base_classes(base)
 
@@ -255,7 +255,26 @@
         recursor_class: recursor definition to find nested content
 
     Returns:
         List of strings describing the differences between the two objects.
         Empty list means the objects are identical.
     """
     return len(compare_nested_objects(d1, d2, recursor_class)) == 0
+
+
+def big_obj_to_short_str(d: Any) -> str:
+    """
+    Args:
+        d: any big object e.g. a dict or a numpy array
+
+    Returns:
+        A hopefully short and representative string representation of the object.
+    """
+    if d is None:
+        return str(None)
+    class_name = type(d).__name__
+    if hasattr(d, "shape"):
+        return f"{class_name} shape {d.shape}"
+    try:
+        return f"{class_name} len {len(d)}"
+    except TypeError:
+        return f"Object of type {class_name}"
```

### Comparing `typedattr-0.1.9/src/typedattr.egg-info/PKG-INFO` & `typedattr-0.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,130 +1,153 @@
-Metadata-Version: 2.1
-Name: typedattr
-Version: 0.1.9
-Summary: Typed conversion of dictionaries to attrs instances
-Author: gingsi
-License: Apache-2.0
-Project-URL: Project-URL, https://github.com/gingsi/typedattr
-Keywords: attrs,typing,dict,attr
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# typedattr
-
-Typechecking and conversion utility for [attrs](https://www.attrs.org/en/stable/).
-
-Parses a dictionary into an attrs instance. Contains other generic object, type and cache utilities.
-
-## Install
-
-Requires python 3.7 or higher.
-
-```bash
-pip install typedattr
-```
-
-## Quickstart
-
-Define class hierarchy and parse the input.
-
-~~~python
-from attrs import define
-from typing import Optional
-from typedattr import attrs_from_dict
-
-@define
-class Cfg:
-    foo: int = 12
-    bar: Optional[int] = None
-
-print(attrs_from_dict(Cfg, {"foo": 1, "bar": 2}))
-# Cfg(foo=1, bar=2)
-
-
-@define
-class CfgNested:
-    sub_cfg: Cfg = None
-
-print(attrs_from_dict(CfgNested, {"sub_cfg": {"foo": 1, "bar": 2}}))
-# CfgNested(sub_cfg=Cfg(foo=1, bar=2))
-~~~
-
-## Features
-
-* Nested checking and conversion of python standard types.
-* `@definenumpy` decorator for equality check if the instances contains numpy arrays.
-* Supports old and new style typing (e.g. `typing.List` and `list`)
-* Supports positional and keyword arguments in classes.
-* Can typecheck existing attrs instances.
-* Allows custom conversions, by default converts source type `str` to target type `Path` and
-  `int` to `float`.
-* Allows to redefine which objects will be recursed into, by default recurses into standard
-  containers (list, dict, etc.) 
-
-### Strict mode (default)
-
-* Convert everything to the target type, e.g. if the input is a list and the annotation is a tuple,
-  the output will be a tuple.
-* Raise errors if types cannot be matched, there are unknown fields in the input or
-  abstract annotation types are used (e.g. Sequence).
-
-### Non-strict mode
-
-Enabled by calling `attrs_from_dict` with `strict=False`
-
-* No conversion except for creating the attrs instance from the dict.
-* Ignore silently if types cannot be matched or abstract annotation types are used.
-* Warn about unknown fields in the input.
-
-### Hints
-
-The following behaviour stems from the `attrs` package:
-
-* New attributes cannot to be added after class definition to an attrs instance,
-  unless it is created with `@define(slots=False)`. 
-  [Explanation](https://www.attrs.org/en/21.2.0/glossary.html#term-slotted-classes)
-* Untyped fields or "ClassVar" typed fields will be ignored by @attrs.define
-  and therefore also by this library.
-
-### Possible improvements
-
-* Supports Callable but does not typecheck the signature
-* Not tested for NewType, Literal
-
-## Install locally and run tests
-
-Clone repository and cd into, then:
-
-~~~bash
-pip install -e .
-pip install pytest pytest-cov pylint
-pylint typedattr
-
-# run tests for python>=3.7
-python -m pytest --cov
-pylint tests
-
-# run tests for python>=3.9
-python -m pytest tests_py39 --cov
-pylint tests_py39
-
-~~~
-
-## Alternatives
-
-This library should be useful for off-the-shelf typechecking and conversion of dicts to
-attrs instances.
-
-For more complex use cases there are many alternatives: 
-`cattrs`, `attrs-strict`, `pydantic`, `dataconf` to name a few.
+Metadata-Version: 2.1
+Name: typedattr
+Version: 0.2.1
+Summary: Typed conversion of dictionaries to attrs instances
+Author: gingsi
+License: Apache-2.0
+Project-URL: Project-URL, https://github.com/gingsi/typedattr
+Keywords: attrs,typing,dict,attr
+Platform: any
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Version Control :: Git
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# typedattr
+
+<p align="center">
+<a href="https://github.com/gingsi/typedattr/actions/workflows/build_py37.yml">
+  <img alt="build 3.7 status" title="build 3.7 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py37.yml?branch=main&label=build%203.7" />
+</a>
+<a href="https://github.com/gingsi/typedattr/actions/workflows/build_py39.yml">
+  <img alt="build 3.9 status" title="build 3.9 status" src="https://img.shields.io/github/actions/workflow/status/gingsi/typedattr/build_py39.yml?branch=main&label=build%203.9" />
+</a>
+<img alt="coverage" title="coverage" src="https://raw.githubusercontent.com/gingsi/typedattr/main/docs/coverage.svg" />
+<a href="https://pypi.org/project/typedattr/">
+  <img alt="version" title="version" src="https://img.shields.io/pypi/v/typedattr?color=success" />
+</a>
+</p>
+
+Typechecking and conversion utility for [attrs](https://www.attrs.org/en/stable/)
+
+Parses a dictionary into an attrs instance.
+Contains other generic object, type and cache utilities.
+
+## Install
+
+Requires `python>=3.7`
+
+Note: `0.2` breaks some backwards compatibility. Use `0.1` or update your code. 
+
+```bash
+pip install typedattr
+```
+
+## Quickstart
+
+Define the class hierarchy and parse the input using `attrs_from_dict`:
+
+~~~python
+from attrs import define
+from typing import Optional
+from typedattr import attrs_from_dict
+
+@define
+class Cfg:
+    foo: int = 12
+    bar: Optional[int] = None
+
+print(attrs_from_dict(Cfg, {"foo": 1, "bar": 2}))
+# Cfg(foo=1, bar=2)
+
+
+@define
+class CfgNested:
+    sub_cfg: Cfg = None
+
+print(attrs_from_dict(CfgNested, {"sub_cfg": {"foo": 1, "bar": 2}}))
+# CfgNested(sub_cfg=Cfg(foo=1, bar=2))
+~~~
+
+## Features
+
+* Nested checking and conversion of python standard types
+* Supports old and new style typing (e.g. `typing.List` and `list`)
+* Supports positional and keyword arguments in classes
+* Can also typecheck existing attrs instances
+* Allows custom conversions, by default converts source type `str` to target type `Path` and
+  `int` to `float`
+* Allows to redefine which objects will be recursed into, by default recurses into standard
+  containers (list, dict, etc.)
+* `@definenumpy` decorator for equality check if the instances contains numpy arrays
+
+### Strict mode (default)
+
+* Convert everything to the target type, e.g. if the input is a list and the annotation is a tuple,
+  the output will be a tuple
+* Raise errors if types cannot be matched, there are unknown fields in the input or
+  abstract annotation types are used (e.g. Sequence)
+
+### Non-strict mode
+
+Enabled by calling `attrs_from_dict` with `strict=False`
+
+* No conversion except for creating the attrs instance from the dict
+* Ignore silently if types cannot be matched or abstract annotation types are used
+* Unknown fields in the input will be added to the attrs instance if possible
+  (see the hint below about slots)
+
+### Skip unknowns
+
+Set `skip_unknowns=True` to ignore all unknown input fields.
+
+### Hints
+
+The following behaviour stems from the `attrs` package:
+
+* New attributes cannot to be added after class definition to an attrs instance,
+  unless it is created with `@define(slots=False)`
+  [Explanation](https://www.attrs.org/en/21.2.0/glossary.html#term-slotted-classes)
+* Untyped fields or "ClassVar" typed fields will be ignored by @attrs.define
+  and therefore also by this library.
+
+### Other utilities in the package 
+
+* `Const`: An alternative to `enum.Enum` for defining constants
+* `cacheutils`: Cache objects to disk / to memory
+* `objutils`: Various utilities like nested modification of dicts
+* Type definitions and other utilities
+
+## Install locally and run tests
+
+Clone repository and cd into, then:
+
+~~~bash
+pip install -e .
+pip install -U pytest pytest-cov pylint
+pylint typedattr
+
+# run tests for python>=3.7
+python -m pytest --cov
+pylint tests
+
+# run tests for python>=3.9
+python -m pytest tests tests_py39 --cov
+pylint tests 
+pylint tests_py39
+~~~
+
+## Alternatives
+
+This library should be useful for off-the-shelf typechecking and conversion of dicts to
+attrs instances.
+
+For more complex or other related use cases there are many alternatives:
+`cattrs`, `attrs-strict`, `pydantic`, `dataconf`, `omegaconf` to name a few.
```

