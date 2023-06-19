# Comparing `tmp/satori_playbook_validator-2.1.2.tar.gz` & `tmp/satori_playbook_validator-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-2.1.2.tar", last modified: Thu Jun 15 22:25:32 2023, max compression
+gzip compressed data, was "satori_playbook_validator-2.2.0.tar", last modified: Mon Jun 19 22:18:14 2023, max compression
```

## Comparing `satori_playbook_validator-2.1.2.tar` & `satori_playbook_validator-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       30 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/README.md
--rw-r--r--   0        0        0      474 2023-06-15 22:25:32.139214 satori_playbook_validator-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      176 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5141 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      223 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1049 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1888 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      874 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2469 2023-06-15 22:25:17.934955 satori_playbook_validator-2.1.2/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/README.md
+-rw-r--r--   0        0        0      474 2023-06-19 22:18:14.296859 satori_playbook_validator-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5171 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      284 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1049 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1888 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      874 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-06-19 22:17:54.508982 satori_playbook_validator-2.2.0/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.2.0/PKG-INFO
```

### Comparing `satori_playbook_validator-2.1.2/src/satorici/validator/_validator.py` & `satori_playbook_validator-2.2.0/src/satorici/validator/_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 import re
 from copy import deepcopy
 from pathlib import Path
 from urllib.parse import urlsplit
 
 from fastjsonschema import JsonSchemaValueException, compile
 
-from .exceptions import PlaybookValidationError, PlaybookVariableError
+from .exceptions import (
+    NoExecutionsError,
+    PlaybookValidationError,
+    PlaybookVariableError,
+)
 
 INPUT_REGEX = re.compile(r"\$\(([\w-]+)\)")
 
 SCHEMAS = Path(__file__).parent / "schemas"
 
 with (
     open(SCHEMAS / "command.json") as commands,
@@ -141,15 +145,15 @@
                 stack.append((path + (k,), v))
             elif validate_commands(v):
                 execution_found = True
                 if get_reference_names(v):
                     validate_references(current, k)
 
     if not execution_found:
-        raise PlaybookValidationError("No executions found.")
+        raise NoExecutionsError("No executions found.")
 
 
 def add_parent_info(d: dict):
     stack = [(d, None, None)]
 
     while stack:
         current, current_parent_key, current_parent_dict = stack.pop()
```

### Comparing `satori_playbook_validator-2.1.2/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-2.2.0/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.2/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-2.2.0/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.2/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-2.2.0/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.2/tests/test_playbook_validator.py` & `satori_playbook_validator-2.2.0/tests/test_playbook_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.1.2/tests/test_reference_finder.py` & `satori_playbook_validator-2.2.0/tests/test_reference_finder.py`

 * *Files identical despite different names*

