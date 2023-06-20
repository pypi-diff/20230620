# Comparing `tmp/gorilla-cli-0.0.4.tar.gz` & `tmp/gorilla-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gorilla-cli-0.0.4.tar", last modified: Sat Jun 17 17:36:50 2023, max compression
+gzip compressed data, was "gorilla-cli-0.0.5.tar", last modified: Tue Jun 20 08:41:20 2023, max compression
```

## Comparing `gorilla-cli-0.0.4.tar` & `gorilla-cli-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 17:36:50.290624 gorilla-cli-0.0.4/
--rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/LICENSE
--rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-17 17:36:50.290424 gorilla-cli-0.0.4/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)     1656 2023-06-17 09:55:31.000000 gorilla-cli-0.0.4/README.md
--rw-r--r--   0 shishir    (501) staff       (20)     2623 2023-06-17 17:29:39.000000 gorilla-cli-0.0.4/go_cli.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 17:36:50.287275 gorilla-cli-0.0.4/go_questionary/
--rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/constants.py
--rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/form.py
--rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompt.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 17:36:50.289230 gorilla-cli-0.0.4/go_questionary/prompts/
--rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/autocomplete.py
--rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/checkbox.py
--rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/common.py
--rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/confirm.py
--rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/password.py
--rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/path.py
--rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/rawselect.py
--rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/select.py
--rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/prompts/text.py
--rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/question.py
--rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/utils.py
--rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-17 09:51:12.000000 gorilla-cli-0.0.4/go_questionary/version.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 17:36:50.290166 gorilla-cli-0.0.4/gorilla_cli.egg-info/
--rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-17 17:36:50.000000 gorilla-cli-0.0.4/gorilla_cli.egg-info/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-17 17:36:50.000000 gorilla-cli-0.0.4/gorilla_cli.egg-info/SOURCES.txt
--rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-17 17:36:50.000000 gorilla-cli-0.0.4/gorilla_cli.egg-info/dependency_links.txt
--rw-r--r--   0 shishir    (501) staff       (20)       36 2023-06-17 17:36:50.000000 gorilla-cli-0.0.4/gorilla_cli.egg-info/entry_points.txt
--rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-17 17:36:50.000000 gorilla-cli-0.0.4/gorilla_cli.egg-info/requires.txt
--rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-17 17:36:50.000000 gorilla-cli-0.0.4/gorilla_cli.egg-info/top_level.txt
--rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-17 17:36:50.290678 gorilla-cli-0.0.4/setup.cfg
--rw-r--r--   0 shishir    (501) staff       (20)      905 2023-06-17 17:29:29.000000 gorilla-cli-0.0.4/setup.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.366309 gorilla-cli-0.0.5/
+-rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/LICENSE
+-rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-20 08:41:20.366065 gorilla-cli-0.0.5/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)     1656 2023-06-17 09:55:31.000000 gorilla-cli-0.0.5/README.md
+-rw-r--r--   0 shishir    (501) staff       (20)     4301 2023-06-20 08:34:03.000000 gorilla-cli-0.0.5/go_cli.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.362827 gorilla-cli-0.0.5/go_questionary/
+-rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/constants.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/form.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompt.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.365176 gorilla-cli-0.0.5/go_questionary/prompts/
+-rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/autocomplete.py
+-rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/checkbox.py
+-rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/common.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/confirm.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/password.py
+-rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/path.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/rawselect.py
+-rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/select.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/text.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/question.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/utils.py
+-rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/version.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.365887 gorilla-cli-0.0.5/gorilla_cli.egg-info/
+-rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       36 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/entry_points.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/requires.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/top_level.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-20 08:41:20.366351 gorilla-cli-0.0.5/setup.cfg
+-rw-r--r--   0 shishir    (501) staff       (20)     1502 2023-06-20 08:32:13.000000 gorilla-cli-0.0.5/setup.py
```

### Comparing `gorilla-cli-0.0.4/LICENSE` & `gorilla-cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/PKG-INFO` & `gorilla-cli-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gorilla-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: LLMs for CLI
 Home-page: https://github.com/gorilla-llm/gorilla-cli
 Author: Shishir Patil, Tianjun Zhang
 Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gorilla-cli-0.0.4/README.md` & `gorilla-cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/__init__.py` & `gorilla-cli-0.0.5/go_questionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/constants.py` & `gorilla-cli-0.0.5/go_questionary/constants.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/form.py` & `gorilla-cli-0.0.5/go_questionary/form.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompt.py` & `gorilla-cli-0.0.5/go_questionary/prompt.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/__init__.py` & `gorilla-cli-0.0.5/go_questionary/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/autocomplete.py` & `gorilla-cli-0.0.5/go_questionary/prompts/autocomplete.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/checkbox.py` & `gorilla-cli-0.0.5/go_questionary/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/common.py` & `gorilla-cli-0.0.5/go_questionary/prompts/common.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/confirm.py` & `gorilla-cli-0.0.5/go_questionary/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/password.py` & `gorilla-cli-0.0.5/go_questionary/prompts/password.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/path.py` & `gorilla-cli-0.0.5/go_questionary/prompts/path.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/rawselect.py` & `gorilla-cli-0.0.5/go_questionary/prompts/rawselect.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/select.py` & `gorilla-cli-0.0.5/go_questionary/prompts/select.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/prompts/text.py` & `gorilla-cli-0.0.5/go_questionary/prompts/text.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/question.py` & `gorilla-cli-0.0.5/go_questionary/question.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/go_questionary/utils.py` & `gorilla-cli-0.0.5/go_questionary/utils.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.4/gorilla_cli.egg-info/PKG-INFO` & `gorilla-cli-0.0.5/gorilla_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gorilla-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: LLMs for CLI
 Home-page: https://github.com/gorilla-llm/gorilla-cli
 Author: Shishir Patil, Tianjun Zhang
 Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gorilla-cli-0.0.4/gorilla_cli.egg-info/SOURCES.txt` & `gorilla-cli-0.0.5/gorilla_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

