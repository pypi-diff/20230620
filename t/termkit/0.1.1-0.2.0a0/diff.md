# Comparing `tmp/termkit-0.1.1.tar.gz` & `tmp/termkit-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termkit-0.1.1.tar", max compression
+gzip compressed data, was "termkit-0.2.0a0.tar", max compression
```

## Comparing `termkit-0.1.1.tar` & `termkit-0.2.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.1.1/LICENSE
--rw-r--r--   0        0        0     2070 2023-06-12 22:04:59.369121 termkit-0.1.1/README.md
--rw-r--r--   0        0        0      618 2023-06-12 22:12:04.437179 termkit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      199 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/__init__.py
--rw-r--r--   0        0        0     3767 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/arguments.py
--rw-r--r--   0        0        0    10313 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/components.py
--rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/exceptions.py
--rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/formatters.py
--rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/groups.py
--rw-r--r--   0        0        0      330 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/helpers.py
--rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.1.1/termkit/tests.py
--rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 termkit-0.1.1/setup.py
--rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 termkit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.2.0a0/LICENSE
+-rw-r--r--   0        0        0     3170 2023-06-13 05:50:26.603066 termkit-0.2.0a0/README.md
+-rw-r--r--   0        0        0      620 2023-06-20 21:49:05.634333 termkit-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0      230 2023-06-20 21:44:13.937490 termkit-0.2.0a0/termkit/__init__.py
+-rw-r--r--   0        0        0     5594 2023-06-18 08:35:38.987150 termkit-0.2.0a0/termkit/arguments.py
+-rw-r--r--   0        0        0    10647 2023-06-20 20:44:25.213962 termkit-0.2.0a0/termkit/components.py
+-rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.2.0a0/termkit/exceptions.py
+-rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.2.0a0/termkit/formatters.py
+-rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.2.0a0/termkit/groups.py
+-rw-r--r--   0        0        0     1178 2023-06-20 21:41:07.832952 termkit-0.2.0a0/termkit/helpers.py
+-rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.2.0a0/termkit/tests.py
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 termkit-0.2.0a0/setup.py
+-rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 termkit-0.2.0a0/PKG-INFO
```

### Comparing `termkit-0.1.1/LICENSE` & `termkit-0.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `termkit-0.1.1/pyproject.toml` & `termkit-0.2.0a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "termkit"
-version = "0.1.1"
+version = "0.2.0a0"
 description = "Command Line Tools with ease"
 authors = ["Thomas Mahé <contact@tmahe.dev>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `termkit-0.1.1/termkit/components.py` & `termkit-0.2.0a0/termkit/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # SPDX-FileCopyrightText: 2023 Thomas Mahé <contact@tmahe.dev>
 
 import argparse
+import contextlib
+import getpass
 import inspect
+import io
 import os
 import sys
 import typing
+import unittest.mock
 from abc import ABC
 from typing import Optional, Callable, Union, Dict, Any
 
 from termkit.helpers import get_callback_arguments
 from termkit.groups import ArgumentGroup, MutuallyExclusiveGroup
 
 from termkit.formatters import TermkitDefaultFormatter
@@ -46,14 +50,15 @@
         else:
             self.help = description.splitlines()[0]
 
         self.name = name
 
         self._callback = callback
         self._childs = list()
+        self._secrets = set()
 
     def add(self, app_or_command: typing.Union[Component, Callable]):
         # Adding sub-app
         if isinstance(app_or_command, Termkit):
             if app_or_command.name == os.path.basename(sys.argv[0]):
                 raise TermkitError('cannot add unnamed Termkit application')
             self._childs.append(app_or_command)
@@ -179,43 +184,46 @@
                 self.description += f"\n\n{command.description}"
             self._populate_command(command)
 
         if len(app._childs) > 0:
             p = self.add_subparsers(title="Commands")
 
             for child in app._childs:
-                p.add_parser(app=child, name=child.name, help=child.help, description=child.description, depth=self._depth+1)
+                p.add_parser(app=child, name=child.name, help=child.help, description=child.description,
+                             depth=self._depth + 1)
 
     def _populate_command(self, command: Command):
         self.add_argument(f'__TERMKIT_CALLBACK_{self._depth}', action="store_const", const=command._callback,
                           help=argparse.SUPPRESS)
         if sys.version_info >= (3, 9):
             type_hints = typing.get_type_hints(command._callback, include_extras=True)
         else:
             type_hints = typing.get_type_hints(command._callback)  # pragma: nocover
 
         for arg_name, arg_spec in inspect.signature(command._callback).parameters.items():
 
-            if sys.version_info >= (3, 9) and isinstance(typing.get_origin(type_hints.get(arg_name, None)), typing.Annotated.__class__):
+            if sys.version_info >= (3, 9) and isinstance(typing.get_origin(type_hints.get(arg_name, None)),
+                                                         typing.Annotated.__class__):
                 annotated_type, argument = typing.get_args(type_hints.get(arg_name, None))
                 if issubclass(type(argument), Argument):
                     if argument.type is not None and annotated_type != argument.type:
                         raise InconsistentTypingError(arg_name, command._callback, annotated_type, argument.type)
                     argument._populate(self, arg_name, annotated_type)
                 else:
                     raise TermkitError(f"incompatible object for Termkit command: "
                                        f"'{arg_name}: Annotated[{annotated_type.__name__}, {argument.__class__.__name__}]'")
 
             elif isinstance(type_hints.get(arg_name, None), Argument):
                 type_hints.get(arg_name)._populate(self, arg_name, None)
 
             elif isinstance(arg_spec.default, Argument):
                 type_hint = type_hints.get(arg_name, None)
-                if None not in [type_hint, arg_spec.default.type] and arg_spec.default.type != type_hint:
-                    raise InconsistentTypingError(arg_name, command._callback, type_hint, arg_spec.default.type)
+                if hasattr(arg_spec.default, "type"):
+                    if None not in [type_hint, arg_spec.default.type] and arg_spec.default.type != type_hint:
+                        raise InconsistentTypingError(arg_name, command._callback, type_hint, arg_spec.default.type)
                 arg_spec.default._populate(self, arg_name, type_hints.get(arg_name, None))
 
             elif arg_spec.default is inspect.Parameter.empty:
                 # implicit positional
                 _type = type_hints.get(arg_name, str)
                 self.positionals.add_argument(arg_name, metavar=arg_name.upper(), type=_type, help="(%(type)s)")
             else:
@@ -243,15 +251,16 @@
         if isinstance(group, MutuallyExclusiveGroup) and group.parent is not None:
             parent_group = self.add_argument_group(group=group.parent)
 
         if isinstance(group, MutuallyExclusiveGroup):
             self._argument_groups[group] = parent_group.add_mutually_exclusive_group(required=group.required)
 
         if isinstance(group, ArgumentGroup):
-            self._argument_groups[group] = super(self.__class__, self).add_argument_group(title=group.title, description=group.description)
+            self._argument_groups[group] = super(self.__class__, self).add_argument_group(title=group.title,
+                                                                                          description=group.description)
 
         return self._argument_groups[group]
 
 
 def run(func_or_app: Union[Callable, Termkit]):
     if inspect.isfunction(func_or_app):
         Termkit(name=func_or_app.__name__, callback=func_or_app)()
```

### Comparing `termkit-0.1.1/termkit/exceptions.py` & `termkit-0.2.0a0/termkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `termkit-0.1.1/termkit/formatters.py` & `termkit-0.2.0a0/termkit/formatters.py`

 * *Files identical despite different names*

### Comparing `termkit-0.1.1/termkit/groups.py` & `termkit-0.2.0a0/termkit/groups.py`

 * *Files identical despite different names*

### Comparing `termkit-0.1.1/termkit/tests.py` & `termkit-0.2.0a0/termkit/tests.py`

 * *Files identical despite different names*

