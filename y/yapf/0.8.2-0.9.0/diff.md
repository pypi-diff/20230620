# Comparing `tmp/yapf-0.8.2.tar.gz` & `tmp/yapf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yapf-0.8.2.tar", last modified: Sat May 21 07:41:58 2016, max compression
+gzip compressed data, was "dist/yapf-0.9.0.tar", last modified: Sun May 29 23:14:06 2016, max compression
```

## Comparing `yapf-0.8.2.tar` & `yapf-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-21 07:41:58.000000 yapf-0.8.2/
--rw-r--r--   0 morbo    (218952)     5000    22659 2016-05-21 07:41:58.000000 yapf-0.8.2/PKG-INFO
--rw-r--r--   0 morbo    (218952)     5000    17495 2016-05-18 08:50:36.000000 yapf-0.8.2/README.rst
--rw-r--r--   0 morbo    (218952)     5000       88 2016-05-21 07:41:58.000000 yapf-0.8.2/setup.cfg
--rw-r--r--   0 morbo    (218952)     5000     2359 2016-03-07 04:47:12.000000 yapf-0.8.2/setup.py
-drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf/
--rw-r--r--   0 morbo    (218952)     5000     9559 2016-05-21 07:39:32.000000 yapf-0.8.2/yapf/__init__.py
--rw-r--r--   0 morbo    (218952)     5000      625 2015-10-21 03:44:07.000000 yapf-0.8.2/yapf/__main__.py
-drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf/yapflib/
--rw-r--r--   0 morbo    (218952)     5000      596 2015-10-21 03:44:07.000000 yapf-0.8.2/yapf/yapflib/__init__.py
--rw-r--r--   0 morbo    (218952)     5000     6492 2016-05-20 04:40:31.000000 yapf-0.8.2/yapf/yapflib/blank_line_calculator.py
--rw-r--r--   0 morbo    (218952)     5000    13790 2016-03-20 09:19:13.000000 yapf-0.8.2/yapf/yapflib/comment_splicer.py
--rw-r--r--   0 morbo    (218952)     5000     1738 2015-10-21 03:44:08.000000 yapf-0.8.2/yapf/yapflib/continuation_splicer.py
--rw-r--r--   0 morbo    (218952)     5000      818 2015-10-21 03:44:08.000000 yapf-0.8.2/yapf/yapflib/errors.py
--rw-r--r--   0 morbo    (218952)     5000     4764 2015-10-25 17:25:58.000000 yapf-0.8.2/yapf/yapflib/file_resources.py
--rw-r--r--   0 morbo    (218952)     5000    20105 2016-05-21 07:31:34.000000 yapf-0.8.2/yapf/yapflib/format_decision_state.py
--rw-r--r--   0 morbo    (218952)     5000     8400 2016-05-21 07:10:33.000000 yapf-0.8.2/yapf/yapflib/format_token.py
--rw-r--r--   0 morbo    (218952)     5000     3924 2015-10-21 03:44:09.000000 yapf-0.8.2/yapf/yapflib/line_joiner.py
--rw-r--r--   0 morbo    (218952)     5000     2404 2015-10-21 03:44:09.000000 yapf-0.8.2/yapf/yapflib/py3compat.py
--rw-r--r--   0 morbo    (218952)     5000    12303 2016-03-07 05:48:49.000000 yapf-0.8.2/yapf/yapflib/pytree_unwrapper.py
--rw-r--r--   0 morbo    (218952)     5000     9876 2016-03-20 10:27:08.000000 yapf-0.8.2/yapf/yapflib/pytree_utils.py
--rw-r--r--   0 morbo    (218952)     5000     4528 2016-03-07 05:39:11.000000 yapf-0.8.2/yapf/yapflib/pytree_visitor.py
--rw-r--r--   0 morbo    (218952)     5000    20163 2016-05-21 07:28:13.000000 yapf-0.8.2/yapf/yapflib/reformatter.py
--rw-r--r--   0 morbo    (218952)     5000    15543 2016-05-19 18:30:49.000000 yapf-0.8.2/yapf/yapflib/split_penalty.py
--rw-r--r--   0 morbo    (218952)     5000    14188 2016-05-18 08:49:58.000000 yapf-0.8.2/yapf/yapflib/style.py
--rw-r--r--   0 morbo    (218952)     5000    14064 2016-05-18 08:38:30.000000 yapf-0.8.2/yapf/yapflib/subtype_assigner.py
--rw-r--r--   0 morbo    (218952)     5000    18300 2016-05-19 08:47:35.000000 yapf-0.8.2/yapf/yapflib/unwrapped_line.py
--rw-r--r--   0 morbo    (218952)     5000     3030 2015-10-21 03:44:16.000000 yapf-0.8.2/yapf/yapflib/verifier.py
--rw-r--r--   0 morbo    (218952)     5000     8879 2016-04-12 12:09:40.000000 yapf-0.8.2/yapf/yapflib/yapf_api.py
-drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf.egg-info/
--rw-r--r--   0 morbo    (218952)     5000        1 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf.egg-info/dependency_links.txt
--rw-r--r--   0 morbo    (218952)     5000       40 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf.egg-info/entry_points.txt
--rw-r--r--   0 morbo    (218952)     5000    22659 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf.egg-info/PKG-INFO
--rw-r--r--   0 morbo    (218952)     5000     1329 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf.egg-info/SOURCES.txt
--rw-r--r--   0 morbo    (218952)     5000       15 2016-05-21 07:41:58.000000 yapf-0.8.2/yapf.egg-info/top_level.txt
-drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-21 07:41:58.000000 yapf-0.8.2/yapftests/
--rw-r--r--   0 morbo    (218952)     5000        1 2015-10-21 03:44:17.000000 yapf-0.8.2/yapftests/__init__.py
--rw-r--r--   0 morbo    (218952)     5000     8019 2016-05-20 04:43:58.000000 yapf-0.8.2/yapftests/blank_line_calculator_test.py
--rw-r--r--   0 morbo    (218952)     5000    10029 2015-10-21 03:44:17.000000 yapf-0.8.2/yapftests/comment_splicer_test.py
--rw-r--r--   0 morbo    (218952)     5000     8070 2015-10-21 03:44:17.000000 yapf-0.8.2/yapftests/file_resources_test.py
--rw-r--r--   0 morbo    (218952)     5000     5064 2015-10-21 03:44:17.000000 yapf-0.8.2/yapftests/format_decision_state_test.py
--rw-r--r--   0 morbo    (218952)     5000     1250 2015-10-21 03:44:17.000000 yapf-0.8.2/yapftests/format_token_test.py
--rw-r--r--   0 morbo    (218952)     5000     3181 2015-10-21 03:44:17.000000 yapf-0.8.2/yapftests/line_joiner_test.py
--rw-r--r--   0 morbo    (218952)     5000     3718 2015-10-21 03:44:18.000000 yapf-0.8.2/yapftests/main_test.py
--rw-r--r--   0 morbo    (218952)     5000    10765 2015-10-21 03:44:18.000000 yapf-0.8.2/yapftests/pytree_unwrapper_test.py
--rw-r--r--   0 morbo    (218952)     5000     7818 2015-10-21 03:46:40.000000 yapf-0.8.2/yapftests/pytree_utils_test.py
--rw-r--r--   0 morbo    (218952)     5000     4056 2016-03-20 10:27:08.000000 yapf-0.8.2/yapftests/pytree_visitor_test.py
--rw-r--r--   0 morbo    (218952)     5000   117032 2016-05-21 07:35:39.000000 yapf-0.8.2/yapftests/reformatter_test.py
--rw-r--r--   0 morbo    (218952)     5000     6748 2016-03-13 09:02:06.000000 yapf-0.8.2/yapftests/split_penalty_test.py
--rw-r--r--   0 morbo    (218952)     5000     8213 2015-10-21 03:44:20.000000 yapf-0.8.2/yapftests/style_test.py
--rw-r--r--   0 morbo    (218952)     5000     8559 2016-05-18 08:44:58.000000 yapf-0.8.2/yapftests/subtype_assigner_test.py
--rw-r--r--   0 morbo    (218952)     5000     3835 2015-10-21 03:44:21.000000 yapf-0.8.2/yapftests/unwrapped_line_test.py
--rw-r--r--   0 morbo    (218952)     5000    35194 2016-04-10 05:19:53.000000 yapf-0.8.2/yapftests/yapf_test.py
+drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-29 23:14:06.000000 yapf-0.9.0/
+-rw-r--r--   0 morbo    (218952)     5000    22999 2016-05-29 23:14:06.000000 yapf-0.9.0/PKG-INFO
+-rw-r--r--   0 morbo    (218952)     5000    17827 2016-05-26 07:03:42.000000 yapf-0.9.0/README.rst
+-rw-r--r--   0 morbo    (218952)     5000       88 2016-05-29 23:14:06.000000 yapf-0.9.0/setup.cfg
+-rw-r--r--   0 morbo    (218952)     5000     2365 2016-05-24 03:20:29.000000 yapf-0.9.0/setup.py
+drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf/
+-rw-r--r--   0 morbo    (218952)     5000     9409 2016-05-29 23:12:53.000000 yapf-0.9.0/yapf/__init__.py
+-rw-r--r--   0 morbo    (218952)     5000      630 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/__main__.py
+drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf/yapflib/
+-rw-r--r--   0 morbo    (218952)     5000      601 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/__init__.py
+-rw-r--r--   0 morbo    (218952)     5000     6497 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/blank_line_calculator.py
+-rw-r--r--   0 morbo    (218952)     5000    13886 2016-05-24 03:20:32.000000 yapf-0.9.0/yapf/yapflib/comment_splicer.py
+-rw-r--r--   0 morbo    (218952)     5000     1743 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/continuation_splicer.py
+-rw-r--r--   0 morbo    (218952)     5000      823 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/errors.py
+-rw-r--r--   0 morbo    (218952)     5000     4804 2016-05-24 03:20:32.000000 yapf-0.9.0/yapf/yapflib/file_resources.py
+-rw-r--r--   0 morbo    (218952)     5000    20727 2016-05-26 07:19:03.000000 yapf-0.9.0/yapf/yapflib/format_decision_state.py
+-rw-r--r--   0 morbo    (218952)     5000     8637 2016-05-24 07:41:54.000000 yapf-0.9.0/yapf/yapflib/format_token.py
+-rw-r--r--   0 morbo    (218952)     5000     3929 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/line_joiner.py
+-rw-r--r--   0 morbo    (218952)     5000     2409 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/py3compat.py
+-rw-r--r--   0 morbo    (218952)     5000    12554 2016-05-26 04:54:50.000000 yapf-0.9.0/yapf/yapflib/pytree_unwrapper.py
+-rw-r--r--   0 morbo    (218952)     5000     9869 2016-05-27 04:58:45.000000 yapf-0.9.0/yapf/yapflib/pytree_utils.py
+-rw-r--r--   0 morbo    (218952)     5000     4533 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/pytree_visitor.py
+-rw-r--r--   0 morbo    (218952)     5000    20497 2016-05-26 04:48:48.000000 yapf-0.9.0/yapf/yapflib/reformatter.py
+-rw-r--r--   0 morbo    (218952)     5000    15780 2016-05-24 06:06:10.000000 yapf-0.9.0/yapf/yapflib/split_penalty.py
+-rw-r--r--   0 morbo    (218952)     5000    15420 2016-05-26 07:03:42.000000 yapf-0.9.0/yapf/yapflib/style.py
+-rw-r--r--   0 morbo    (218952)     5000    14069 2016-05-24 06:41:16.000000 yapf-0.9.0/yapf/yapflib/subtype_assigner.py
+-rw-r--r--   0 morbo    (218952)     5000    18304 2016-05-26 04:46:44.000000 yapf-0.9.0/yapf/yapflib/unwrapped_line.py
+-rw-r--r--   0 morbo    (218952)     5000     3035 2016-05-21 07:45:41.000000 yapf-0.9.0/yapf/yapflib/verifier.py
+-rw-r--r--   0 morbo    (218952)     5000     9016 2016-05-24 03:20:40.000000 yapf-0.9.0/yapf/yapflib/yapf_api.py
+drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf.egg-info/
+-rw-r--r--   0 morbo    (218952)     5000        1 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf.egg-info/dependency_links.txt
+-rw-r--r--   0 morbo    (218952)     5000       40 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf.egg-info/entry_points.txt
+-rw-r--r--   0 morbo    (218952)     5000    22999 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf.egg-info/PKG-INFO
+-rw-r--r--   0 morbo    (218952)     5000     1329 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf.egg-info/SOURCES.txt
+-rw-r--r--   0 morbo    (218952)     5000       15 2016-05-29 23:14:06.000000 yapf-0.9.0/yapf.egg-info/top_level.txt
+drwxr-xr-x   0 morbo    (218952)     5000        0 2016-05-29 23:14:06.000000 yapf-0.9.0/yapftests/
+-rw-r--r--   0 morbo    (218952)     5000        1 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/__init__.py
+-rw-r--r--   0 morbo    (218952)     5000     8024 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/blank_line_calculator_test.py
+-rw-r--r--   0 morbo    (218952)     5000    10034 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/comment_splicer_test.py
+-rw-r--r--   0 morbo    (218952)     5000     8286 2016-05-24 03:20:40.000000 yapf-0.9.0/yapftests/file_resources_test.py
+-rw-r--r--   0 morbo    (218952)     5000     5057 2016-05-24 03:20:41.000000 yapf-0.9.0/yapftests/format_decision_state_test.py
+-rw-r--r--   0 morbo    (218952)     5000     1255 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/format_token_test.py
+-rw-r--r--   0 morbo    (218952)     5000     3186 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/line_joiner_test.py
+-rw-r--r--   0 morbo    (218952)     5000     3723 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/main_test.py
+-rw-r--r--   0 morbo    (218952)     5000    10720 2016-05-24 03:20:41.000000 yapf-0.9.0/yapftests/pytree_unwrapper_test.py
+-rw-r--r--   0 morbo    (218952)     5000     8179 2016-05-27 04:58:45.000000 yapf-0.9.0/yapftests/pytree_utils_test.py
+-rw-r--r--   0 morbo    (218952)     5000     4061 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/pytree_visitor_test.py
+-rw-r--r--   0 morbo    (218952)     5000   125347 2016-05-26 04:54:38.000000 yapf-0.9.0/yapftests/reformatter_test.py
+-rw-r--r--   0 morbo    (218952)     5000     6793 2016-05-24 02:05:21.000000 yapf-0.9.0/yapftests/split_penalty_test.py
+-rw-r--r--   0 morbo    (218952)     5000     8218 2016-05-21 07:45:41.000000 yapf-0.9.0/yapftests/style_test.py
+-rw-r--r--   0 morbo    (218952)     5000     8539 2016-05-24 03:20:44.000000 yapf-0.9.0/yapftests/subtype_assigner_test.py
+-rw-r--r--   0 morbo    (218952)     5000     3863 2016-05-24 03:20:44.000000 yapf-0.9.0/yapftests/unwrapped_line_test.py
+-rw-r--r--   0 morbo    (218952)     5000    35246 2016-05-24 07:44:50.000000 yapf-0.9.0/yapftests/yapf_test.py
```

### Comparing `yapf-0.8.2/PKG-INFO` & `yapf-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: yapf
-Version: 0.8.2
+Version: 0.9.0
 Summary: A formatter for Python code.
 Home-page: UNKNOWN
 Author: Bill Wendling
 Author-email: morbo@google.com
 License: Apache License, Version 2.0
 Description: ====
         YAPF
@@ -88,15 +88,14 @@
         Usage
         =====
         
         Options::
         
             usage: yapf [-h] [-v] [-d | -i] [-r | -l START-END] [-e PATTERN]
                         [--style STYLE] [--style-help] [--no-local-style]
-                        [--verify]
                         [files [files ...]]
         
             Formatter for Python code.
         
             positional arguments:
               files
         
@@ -114,15 +113,14 @@
                                     example "pep8" or "google"), or the name of a file
                                     with style settings. The default is pep8 unless a
                                     .style.yapf or setup.cfg file located in one of the
                                     parent directories of the source file (or current
                                     directory for stdin)
               --style-help          show style settings and exit
               --no-local-style      don't search for local style definition (.style.yapf)
-              --verify              try to verify reformatted code for syntax errors
         
         
         Formatting style
         ================
         
         The formatting style used by YAPF is configurable and there are many "knobs"
         that can be used to tune how YAPF does formatting. See the ``style.py`` module
@@ -285,21 +283,22 @@
         
         Knobs
         =====
         
         ``ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT``
             Align closing bracket with visual indentation.
         
-        ``BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF``
-            Insert a blank line before a 'def' or 'class' immediately nested
-            within another 'def' or 'class'.
+        ``ALLOW_MULTILINE_LAMBDAS``
+            Allow lambdas to be formatted on more than one line.
         
-            For example:
+        ``BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF``
+            Insert a blank line before a ``def`` or ``class`` immediately nested within
+            another ``def`` or ``class``. For example:
         
-        .. code-block:: python
+            .. code-block:: python
         
                 class Foo:
                                    # <------ this blank line
                     def method():
                         pass
         
         ``COLUMN_LIMIT``
@@ -307,124 +306,126 @@
         
         ``CONTINUATION_INDENT_WIDTH``
             Indent width used for line continuations.
         
         ``DEDENT_CLOSING_BRACKETS``
             Put closing brackets on a separate line, dedented, if the bracketed
             expression can't fit in a single line. Applies to all kinds of brackets,
-            including function definitions and calls.
+            including function definitions and calls. For example:
         
-            For example:
-        
-        .. code-block:: python
+            .. code-block:: python
         
                 config = {
                     'key1': 'value1',
                     'key2': 'value2',
-                }        # <--- this bracket is dedented and on a separate line
+                }  # <--- this bracket is dedented and on a separate line
         
                 time_series = self.remote_client.query_entity_counters(
-                  entity='dev3246.region1',
-                  key='dns.query_latency_tcp',
-                  transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
-                  start_ts=now()-timedelta(days=3),
-                  end_ts=now(),
-                )        # <--- this bracket is dedented and on a separate line
+                    entity='dev3246.region1',
+                    key='dns.query_latency_tcp',
+                    transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
+                    start_ts=now()-timedelta(days=3),
+                    end_ts=now(),
+                )  # <--- this bracket is dedented and on a separate line
         
         ``I18N_COMMENT``
             The regex for an internationalization comment. The presence of this comment
             stops reformatting of that line, because the comments are required to be
             next to the string they translate.
         
         ``I18N_FUNCTION_CALL``
-            The internationalization function call names. The presence of this
-            function stops reformattting on that line, because the string it has
-            cannot be moved away from the i18n comment.
+            The internationalization function call names. The presence of this function
+            stops reformattting on that line, because the string it has cannot be moved
+            away from the i18n comment.
         
         ``INDENT_DICTIONARY_VALUE``
             Indent the dictionary value if it cannot fit on the same line as the
-            dictionary key.
+            dictionary key. For example:
         
-            For example:
-        
-        .. code-block:: python
+            .. code-block:: python
         
                 config = {
                     'key1':
                         'value1',
                     'key2': value1 +
                             value2,
                 }
         
         ``INDENT_WIDTH``
             The number of columns to use for indentation.
         
         ``JOIN_MULTIPLE_LINES``
             Join short lines into one line. E.g., single line ``if`` statements.
         
-        ``SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET``
-            Insert a space between the ending comma and closing bracket of a list,
-            etc.
-        
         ``SPACES_AROUND_POWER_OPERATOR``
             Set to ``True`` to prefer using spaces around ``**``.
         
         ``SPACES_BEFORE_COMMENT``
             The number of spaces required before a trailing comment.
         
+        ``SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET``
+            Insert a space between the ending comma and closing bracket of a list, etc.
+        
+        ``SPLIT_ARGUMENTS_WHEN_COMMA_TERMINATED``
+            Split before arguments if the argument list is terminated by a comma.
+        
         ``SPLIT_BEFORE_BITWISE_OPERATOR``
             Set to ``True`` to prefer splitting before ``&``, ``|`` or ``^`` rather
             than after.
         
+        ``SPLIT_BEFORE_FIRST_ARGUMENT``
+            If an argument / parameter list is going to be split, then split before the
+            first argument.
+        
         ``SPLIT_BEFORE_LOGICAL_OPERATOR``
             Set to ``True`` to prefer splitting before ``and`` or ``or`` rather than
             after.
         
         ``SPLIT_BEFORE_NAMED_ASSIGNS``
             Split named assignments onto individual lines.
         
         ``SPLIT_PENALTY_AFTER_OPENING_BRACKET``
             The penalty for splitting right after the opening bracket.
         
         ``SPLIT_PENALTY_AFTER_UNARY_OPERATOR``
             The penalty for splitting the line after a unary operator.
         
+        ``SPLIT_PENALTY_BEFORE_IF_EXPR``
+            The penalty for splitting right before an ``if`` expression.
+        
         ``SPLIT_PENALTY_BITWISE_OPERATOR``
             The penalty of splitting the line around the ``&``, ``|``, and ``^``
             operators.
         
         ``SPLIT_PENALTY_EXCESS_CHARACTER``
             The penalty for characters over the column limit.
         
         ``SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT``
-            The penalty incurred by adding a line split to the unwrapped line. The
-            more line splits added the higher the penalty.
+            The penalty incurred by adding a line split to the unwrapped line. The more
+            line splits added the higher the penalty.
         
         ``SPLIT_PENALTY_IMPORT_NAMES``
-            The penalty of splitting a list of ``import as`` names.
+            The penalty of splitting a list of ``import as`` names. For example:
         
-            For example:
-        
-        .. code-block:: python
+            .. code-block:: python
         
               from a_very_long_or_indented_module_name_yada_yad import (long_argument_1,
                                                                         long_argument_2,
                                                                         long_argument_3)
         
             would reformat to something like:
         
-        .. code-block:: python
+            .. code-block:: python
         
               from a_very_long_or_indented_module_name_yada_yad import (
                   long_argument_1, long_argument_2, long_argument_3)
         
         ``SPLIT_PENALTY_LOGICAL_OPERATOR``
             The penalty of splitting the line around the ``and`` and ``or`` operators.
         
-        
         (Potentially) Frequently Asked Questions
         ========================================
         
         Why does YAPF destroy my awesome formatting?
         --------------------------------------------
         
         YAPF tries very hard to get the formatting correct. But for some code, it won't
```

### Comparing `yapf-0.8.2/README.rst` & `yapf-0.9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 Usage
 =====
 
 Options::
 
     usage: yapf [-h] [-v] [-d | -i] [-r | -l START-END] [-e PATTERN]
                 [--style STYLE] [--style-help] [--no-local-style]
-                [--verify]
                 [files [files ...]]
 
     Formatter for Python code.
 
     positional arguments:
       files
 
@@ -106,15 +105,14 @@
                             example "pep8" or "google"), or the name of a file
                             with style settings. The default is pep8 unless a
                             .style.yapf or setup.cfg file located in one of the
                             parent directories of the source file (or current
                             directory for stdin)
       --style-help          show style settings and exit
       --no-local-style      don't search for local style definition (.style.yapf)
-      --verify              try to verify reformatted code for syntax errors
 
 
 Formatting style
 ================
 
 The formatting style used by YAPF is configurable and there are many "knobs"
 that can be used to tune how YAPF does formatting. See the ``style.py`` module
@@ -277,21 +275,22 @@
 
 Knobs
 =====
 
 ``ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT``
     Align closing bracket with visual indentation.
 
-``BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF``
-    Insert a blank line before a 'def' or 'class' immediately nested
-    within another 'def' or 'class'.
+``ALLOW_MULTILINE_LAMBDAS``
+    Allow lambdas to be formatted on more than one line.
 
-    For example:
+``BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF``
+    Insert a blank line before a ``def`` or ``class`` immediately nested within
+    another ``def`` or ``class``. For example:
 
-.. code-block:: python
+    .. code-block:: python
 
         class Foo:
                            # <------ this blank line
             def method():
                 pass
 
 ``COLUMN_LIMIT``
@@ -299,124 +298,126 @@
 
 ``CONTINUATION_INDENT_WIDTH``
     Indent width used for line continuations.
 
 ``DEDENT_CLOSING_BRACKETS``
     Put closing brackets on a separate line, dedented, if the bracketed
     expression can't fit in a single line. Applies to all kinds of brackets,
-    including function definitions and calls.
+    including function definitions and calls. For example:
 
-    For example:
-
-.. code-block:: python
+    .. code-block:: python
 
         config = {
             'key1': 'value1',
             'key2': 'value2',
-        }        # <--- this bracket is dedented and on a separate line
+        }  # <--- this bracket is dedented and on a separate line
 
         time_series = self.remote_client.query_entity_counters(
-          entity='dev3246.region1',
-          key='dns.query_latency_tcp',
-          transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
-          start_ts=now()-timedelta(days=3),
-          end_ts=now(),
-        )        # <--- this bracket is dedented and on a separate line
+            entity='dev3246.region1',
+            key='dns.query_latency_tcp',
+            transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
+            start_ts=now()-timedelta(days=3),
+            end_ts=now(),
+        )  # <--- this bracket is dedented and on a separate line
 
 ``I18N_COMMENT``
     The regex for an internationalization comment. The presence of this comment
     stops reformatting of that line, because the comments are required to be
     next to the string they translate.
 
 ``I18N_FUNCTION_CALL``
-    The internationalization function call names. The presence of this
-    function stops reformattting on that line, because the string it has
-    cannot be moved away from the i18n comment.
+    The internationalization function call names. The presence of this function
+    stops reformattting on that line, because the string it has cannot be moved
+    away from the i18n comment.
 
 ``INDENT_DICTIONARY_VALUE``
     Indent the dictionary value if it cannot fit on the same line as the
-    dictionary key.
+    dictionary key. For example:
 
-    For example:
-
-.. code-block:: python
+    .. code-block:: python
 
         config = {
             'key1':
                 'value1',
             'key2': value1 +
                     value2,
         }
 
 ``INDENT_WIDTH``
     The number of columns to use for indentation.
 
 ``JOIN_MULTIPLE_LINES``
     Join short lines into one line. E.g., single line ``if`` statements.
 
-``SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET``
-    Insert a space between the ending comma and closing bracket of a list,
-    etc.
-
 ``SPACES_AROUND_POWER_OPERATOR``
     Set to ``True`` to prefer using spaces around ``**``.
 
 ``SPACES_BEFORE_COMMENT``
     The number of spaces required before a trailing comment.
 
+``SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET``
+    Insert a space between the ending comma and closing bracket of a list, etc.
+
+``SPLIT_ARGUMENTS_WHEN_COMMA_TERMINATED``
+    Split before arguments if the argument list is terminated by a comma.
+
 ``SPLIT_BEFORE_BITWISE_OPERATOR``
     Set to ``True`` to prefer splitting before ``&``, ``|`` or ``^`` rather
     than after.
 
+``SPLIT_BEFORE_FIRST_ARGUMENT``
+    If an argument / parameter list is going to be split, then split before the
+    first argument.
+
 ``SPLIT_BEFORE_LOGICAL_OPERATOR``
     Set to ``True`` to prefer splitting before ``and`` or ``or`` rather than
     after.
 
 ``SPLIT_BEFORE_NAMED_ASSIGNS``
     Split named assignments onto individual lines.
 
 ``SPLIT_PENALTY_AFTER_OPENING_BRACKET``
     The penalty for splitting right after the opening bracket.
 
 ``SPLIT_PENALTY_AFTER_UNARY_OPERATOR``
     The penalty for splitting the line after a unary operator.
 
+``SPLIT_PENALTY_BEFORE_IF_EXPR``
+    The penalty for splitting right before an ``if`` expression.
+
 ``SPLIT_PENALTY_BITWISE_OPERATOR``
     The penalty of splitting the line around the ``&``, ``|``, and ``^``
     operators.
 
 ``SPLIT_PENALTY_EXCESS_CHARACTER``
     The penalty for characters over the column limit.
 
 ``SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT``
-    The penalty incurred by adding a line split to the unwrapped line. The
-    more line splits added the higher the penalty.
+    The penalty incurred by adding a line split to the unwrapped line. The more
+    line splits added the higher the penalty.
 
 ``SPLIT_PENALTY_IMPORT_NAMES``
-    The penalty of splitting a list of ``import as`` names.
+    The penalty of splitting a list of ``import as`` names. For example:
 
-    For example:
-
-.. code-block:: python
+    .. code-block:: python
 
       from a_very_long_or_indented_module_name_yada_yad import (long_argument_1,
                                                                 long_argument_2,
                                                                 long_argument_3)
 
     would reformat to something like:
 
-.. code-block:: python
+    .. code-block:: python
 
       from a_very_long_or_indented_module_name_yada_yad import (
           long_argument_1, long_argument_2, long_argument_3)
 
 ``SPLIT_PENALTY_LOGICAL_OPERATOR``
     The penalty of splitting the line around the ``and`` and ``or`` operators.
 
-
 (Potentially) Frequently Asked Questions
 ========================================
 
 Why does YAPF destroy my awesome formatting?
 --------------------------------------------
 
 YAPF tries very hard to get the formatting correct. But for some code, it won't
```

### Comparing `yapf-0.8.2/setup.py` & `yapf-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,14 +34,15 @@
   def run(self):
     loader = unittest.TestLoader()
     tests = loader.discover('yapftests', pattern='*_test.py', top_level_dir='.')
     runner = unittest.TextTestRunner()
     results = runner.run(tests)
     sys.exit(0 if results.wasSuccessful() else 1)
 
+
 with codecs.open('README.rst', 'r', 'utf-8') as fd:
   setup(name='yapf',
         version=yapf.__version__,
         description='A formatter for Python code.',
         long_description=fd.read(),
         license='Apache License, Version 2.0',
         author='Google Inc.',
```

### Comparing `yapf-0.8.2/yapf/__init__.py` & `yapf-0.9.0/yapf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,15 +34,15 @@
 
 from yapf.yapflib import errors
 from yapf.yapflib import file_resources
 from yapf.yapflib import py3compat
 from yapf.yapflib import style
 from yapf.yapflib import yapf_api
 
-__version__ = '0.8.2'
+__version__ = '0.9.0'
 
 
 def main(argv):
   """Main program.
 
   Arguments:
     argv: command-line arguments, such as sys.argv (including the program name
@@ -99,18 +99,15 @@
             'stdin)' % (style.LOCAL_STYLE, style.SETUP_CONFIG)))
   parser.add_argument('--style-help',
                       action='store_true',
                       help='show style settings and exit')
   parser.add_argument('--no-local-style',
                       action='store_true',
                       help="don't search for local style definition")
-  parser.add_argument('--verify',
-                      action='store_true',
-                      help=('try to verify reformatted code for syntax errors. '
-                            'This option is for debugging purposes only.'))
+  parser.add_argument('--verify', action='store_true', help=argparse.SUPPRESS)
 
   parser.add_argument('files', nargs='*')
   args = parser.parse_args(argv[1:])
 
   if args.version:
     print('yapf {}'.format(__version__))
     return 0
```

### Comparing `yapf-0.8.2/yapf/__main__.py` & `yapf-0.9.0/yapf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/__init__.py` & `yapf-0.9.0/yapf/yapflib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/blank_line_calculator.py` & `yapf-0.9.0/yapf/yapflib/blank_line_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/comment_splicer.py` & `yapf-0.9.0/yapf/yapflib/comment_splicer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -143,17 +143,16 @@
                       context=('', (comment_lineno, comment_column)))
                   pytree_utils.InsertNodesAfter([comment_leaf], prev_leaf[0])
                   comment_prefix = '\n'.join(comment_lines[1:])
                   comment_lineno += 1
 
                 rindex = (0 if '\n' not in comment_prefix.rstrip() else
                           comment_prefix.rstrip().rindex('\n') + 1)
-                comment_column = (
-                    len(comment_prefix[rindex:]) -
-                    len(comment_prefix[rindex:].lstrip()))
+                comment_column = (len(comment_prefix[rindex:]) -
+                                  len(comment_prefix[rindex:].lstrip()))
                 comments = _CreateCommentsFromPrefix(comment_prefix,
                                                      comment_lineno,
                                                      comment_column,
                                                      standalone=False)
                 pytree_utils.InsertNodesBefore(comments, child)
                 break
 
@@ -215,17 +214,18 @@
 # *eventually*, and we'll modify it with time as we discover more corner cases
 # in the parse tree.
 #
 # When splicing a standalone comment (i.e. a comment that appears on its own
 # line, not on the same line with other code), it's important to insert it into
 # an appropriate parent of the node it's attached to. An appropriate parent
 # is the first "standaline line node" in the parent chain of a node.
-_STANDALONE_LINE_NODES = frozenset(
-    ['suite', 'if_stmt', 'while_stmt', 'for_stmt', 'try_stmt', 'with_stmt',
-     'funcdef', 'classdef', 'decorated', 'file_input'])
+_STANDALONE_LINE_NODES = frozenset(['suite', 'if_stmt', 'while_stmt',
+                                    'for_stmt', 'try_stmt', 'with_stmt',
+                                    'funcdef', 'classdef', 'decorated',
+                                    'file_input'])
 
 
 def _FindNodeWithStandaloneLineParent(node):
   """Find a node whose parent is a 'standalone line' node.
 
   See the comment above _STANDALONE_LINE_NODES for more details.
```

### Comparing `yapf-0.8.2/yapf/yapflib/continuation_splicer.py` & `yapf-0.9.0/yapf/yapflib/continuation_splicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/errors.py` & `yapf-0.9.0/yapf/yapflib/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/file_resources.py` & `yapf-0.9.0/yapf/yapflib/file_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -96,27 +96,26 @@
 def _FindPythonFiles(filenames, recursive, exclude):
   """Find all Python files."""
   python_files = []
   for filename in filenames:
     if os.path.isdir(filename):
       if recursive:
         # TODO(morbo): Look into a version of os.walk that can handle recursion.
-        python_files.extend(
-            os.path.join(dirpath, f)
-            for dirpath, _, filelist in os.walk(filename) for f in filelist
-            if IsPythonFile(os.path.join(dirpath, f)))
+        python_files.extend(os.path.join(dirpath, f)
+                            for dirpath, _, filelist in os.walk(filename)
+                            for f in filelist
+                            if IsPythonFile(os.path.join(dirpath, f)))
       else:
         raise errors.YapfError(
             "directory specified without '--recursive' flag: %s" % filename)
     elif os.path.isfile(filename):
       python_files.append(filename)
 
   if exclude:
-    return [f
-            for f in python_files
+    return [f for f in python_files
             if not any(fnmatch.fnmatch(f, p) for p in exclude)]
 
   return python_files
 
 
 def IsPythonFile(filename):
   """Return True if filename is a Python file."""
```

### Comparing `yapf-0.8.2/yapf/yapflib/format_decision_state.py` & `yapf-0.9.0/yapf/yapflib/format_decision_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,14 +28,15 @@
 
 import copy
 
 from yapf.yapflib import format_token
 from yapf.yapflib import pytree_utils
 from yapf.yapflib import split_penalty
 from yapf.yapflib import style
+from yapf.yapflib import unwrapped_line
 
 _COMPOUND_STMTS = frozenset({'for', 'while', 'if', 'elif', 'with', 'except',
                              'def', 'class'})
 
 
 class FormatDecisionState(object):
   """The current state when indenting an unwrapped line.
@@ -79,28 +80,28 @@
     self.first_indent = first_indent
     self.newline = False
     self.previous = None
     self._MoveStateToNextToken()
 
   def Clone(self):
     new = copy.copy(self)
-    new.stack = copy.deepcopy(self.stack)
+    new.stack = [copy.copy(state) for state in self.stack]
     return new
 
   def __eq__(self, other):
     # Note: 'first_indent' is implicit in the stack. Also, we ignore 'previous',
     # because it shouldn't have a bearing on this comparison. (I.e., it will
     # report equal if 'next_token' does.)
     return (self.next_token == other.next_token and
             self.column == other.column and
             self.paren_level == other.paren_level and
             self.start_of_line_level == other.start_of_line_level and
-            self.lowest_level_on_line == other.lowest_level_on_line and (
-                self.ignore_stack_for_comparison or
-                other.ignore_stack_for_comparison or self.stack == other.stack))
+            self.lowest_level_on_line == other.lowest_level_on_line and
+            (self.ignore_stack_for_comparison or
+             other.ignore_stack_for_comparison or self.stack == other.stack))
 
   def __ne__(self, other):
     return not self == other
 
   def __hash__(self):
     return hash((self.next_token, self.column, self.paren_level,
                  self.start_of_line_level, self.lowest_level_on_line))
@@ -124,43 +125,35 @@
     current = self.next_token
     previous = current.previous_token
     column_limit = style.Get('COLUMN_LIMIT')
 
     if current.must_break_before:
       return True
 
-    if style.Get('DEDENT_CLOSING_BRACKETS'):
+    if (previous and (style.Get('DEDENT_CLOSING_BRACKETS') or
+                      style.Get('SPLIT_BEFORE_FIRST_ARGUMENT'))):
       bracket = current if current.ClosesScope() else previous
-      if ((bracket.OpensScope() or bracket.ClosesScope()) and
-          format_token.Subtype.SUBSCRIPT_BRACKET not in bracket.subtypes):
-        if previous and previous.OpensScope():
-          length = (previous.matching_bracket.total_length -
-                    previous.total_length)
-          if _IsLastScopeInLine(previous.matching_bracket):
-            last_token = _LastTokenInLine(previous.matching_bracket)
-            length = last_token.total_length - previous.total_length
-
-          if length + previous.column >= column_limit:
+      if format_token.Subtype.SUBSCRIPT_BRACKET not in bracket.subtypes:
+        if bracket.OpensScope():
+          if (unwrapped_line.IsSurroundedByBrackets(bracket) or
+              not _IsLastScopeInLine(bracket)):
+            last_token = bracket.matching_bracket
+          else:
+            last_token = _LastTokenInLine(bracket.matching_bracket)
+
+          length = last_token.total_length - bracket.total_length
+          if length + self.column >= column_limit:
+            self.stack[-1].split_before_closing_bracket = True
             return True
-        elif current.ClosesScope():
-          opening = current.matching_bracket
-          length = current.total_length - opening.total_length
-          if _IsLastScopeInLine(current):
-            last_token = _LastTokenInLine(current)
-            length = last_token.total_length - opening.total_length
 
-          if length + opening.column >= column_limit:
-            return True
+        elif style.Get('DEDENT_CLOSING_BRACKETS') and current.ClosesScope():
+          return self.stack[-1].split_before_closing_bracket
 
-    if (self.stack[-1].split_before_closing_bracket and
-        # FIXME(morbo): Use the 'matching_bracket' instead of this.
-        # FIXME(morbo): Don't forget about tuples!
-        current.value in ']}'):
-      # Split if we need to split before the closing bracket and the next
-      # token is a closing bracket.
+    if self.stack[-1].split_before_closing_bracket and current.value in '}]':
+      # Split if we need to split before the closing bracket.
       return current.node_split_penalty != split_penalty.UNBREAKABLE
 
     if not previous:
       return False
 
     # TODO(morbo): This should be controlled with a knob.
     if (format_token.Subtype.DICTIONARY_KEY in current.subtypes and
@@ -175,44 +168,55 @@
     if (style.Get('SPLIT_BEFORE_NAMED_ASSIGNS') and
         format_token.Subtype.DEFAULT_OR_NAMED_ASSIGN_ARG_LIST in
         current.subtypes):
       if (previous.value not in {'(', '=', '*', '**'} and
           current.value not in '=,)'):
         opening = _GetOpeningParen(current)
         if opening:
-          arglist_length = (
-              opening.matching_bracket.total_length - opening.total_length +
-              self.column)
+          arglist_length = (opening.matching_bracket.total_length -
+                            opening.total_length + self.column)
           return arglist_length > column_limit
 
+    if style.Get('SPLIT_ARGUMENTS_WHEN_COMMA_TERMINATED'):
+      # Split before arguments in a function call or definition if the
+      # arguments are terminated by a comma.
+      opening = _GetOpeningParen(current)
+      if opening and opening.previous_token and opening.previous_token.is_name:
+        if previous.value in '(,':
+          if opening.matching_bracket.previous_token.value == ',':
+            return True
+
     if (previous.value in '{[' and current.lineno != previous.lineno and
         format_token.Subtype.SUBSCRIPT_BRACKET not in previous.subtypes):
+      # Retain the split after the container opening.
       return True
 
     if (previous.value == ':' and _IsDictionaryValue(current) and
         current.lineno != previous.lineno):
       # Retain the split between the dictionary key and value.
       return True
 
     if (format_token.Subtype.COMP_FOR in current.subtypes and
         format_token.Subtype.COMP_FOR not in previous.subtypes):
+      # Split at the beginning of a list comprehension.
       length = _GetLengthOfSubtype(current, format_token.Subtype.COMP_FOR,
                                    format_token.Subtype.COMP_IF)
       if length + self.column > column_limit:
         return True
 
     if (format_token.Subtype.COMP_IF in current.subtypes and
         format_token.Subtype.COMP_IF not in previous.subtypes):
+      # Split at the beginning of an if expression.
       length = _GetLengthOfSubtype(current, format_token.Subtype.COMP_IF)
       if length + self.column > column_limit:
         return True
 
     previous_previous_token = previous.previous_token
-    if (previous_previous_token and previous_previous_token.name == 'NAME' and
-        not previous_previous_token.is_keyword and previous.value == '('):
+    if (current.is_name and previous_previous_token and
+        previous_previous_token.is_name and previous.value == '('):
       sibling = previous.node.next_sibling
       if pytree_utils.NodeName(sibling) == 'arglist':
         arglist = previous.node.next_sibling
         if len(arglist.children) > 2:
           if _IsFunctionCallWithArguments(current):
             # There is a function call, with more than 1 argument, where
             # the first argument is itself a function call with arguments.
@@ -224,16 +228,17 @@
           elif (current.OpensScope() and
                 current.matching_bracket.total_length + self.column >
                 column_limit):
             # There is a data literal that will need to be split and could mess
             # up the formatting.
             return True
 
-    if (style.Get('SPLIT_BEFORE_BITWISE_OPERATOR') and
-        current.value in '&|' and previous.lineno < current.lineno):
+    if (style.Get('SPLIT_BEFORE_BITWISE_OPERATOR') and current.value in '&|' and
+        previous.lineno < current.lineno):
+      # Retain the split before a bitwise operator.
       return True
 
     if (current.is_comment and
         previous.lineno < current.lineno - current.value.count('\n')):
       # If a comment comes in the middle of an unwrapped line (like an if
       # conditional with comments interspersed), then we want to split if the
       # original comments were on a separate line.
@@ -329,36 +334,39 @@
     for paren_state in self.stack:
       paren_state.split_before_parameter = True
 
     if (previous.value != ',' and not previous.is_binary_op and
         not current.is_binary_op and not previous.OpensScope()):
       self.stack[-1].split_before_parameter = True
 
-    if (previous.OpensScope() or
-        (previous.is_comment and previous.previous_token is not None and
-         previous.previous_token.OpensScope())):
+    if (previous.OpensScope() or (previous.is_comment and
+                                  previous.previous_token is not None and
+                                  previous.previous_token.OpensScope())):
       self.stack[-1].closing_scope_indent = max(
           0, self.stack[-1].indent - style.Get('CONTINUATION_INDENT_WIDTH'))
       self.stack[-1].split_before_closing_bracket = True
 
     # Calculate the split penalty.
     penalty = current.split_penalty
 
+    if must_split:
+      # Don't penalize for a must split.
+      return penalty
+
     if previous.is_pseudo_paren and previous.value == '(':
       # Small penalty for splitting after a pseudo paren.
       penalty += 50
 
-    # Add a penalty for each increasing newline we add.
-    last = self.stack[-1]
-    penalty += (style.Get('SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT') *
-                last.num_line_splits)
+    # Add a penalty for each increasing newline we add, but don't penalize for
+    # splitting before an if-expression or list comprehension.
     if not must_split and current.value not in {'if', 'for'}:
-      # Don't penalize for a must split or for splitting before an
-      # if-expression or list comprehension.
+      last = self.stack[-1]
       last.num_line_splits += 1
+      penalty += (style.Get('SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT') *
+                  last.num_line_splits)
 
     return penalty + 10
 
   def _GetNewlineColumn(self):
     """Return the new column on the newline."""
     current = self.next_token
     previous = current.previous_token
@@ -367,32 +375,33 @@
     if current.spaces_required_before > 2 or self.line.disable:
       return current.spaces_required_before
 
     if current.OpensScope():
       return top_of_stack.indent if self.paren_level else self.first_indent
 
     if current.ClosesScope():
-      if (previous.OpensScope() or
-          (previous.is_comment and previous.previous_token is not None and
-           previous.previous_token.OpensScope())):
+      if (previous.OpensScope() or (previous.is_comment and
+                                    previous.previous_token is not None and
+                                    previous.previous_token.OpensScope())):
         return max(0,
                    top_of_stack.indent - style.Get('CONTINUATION_INDENT_WIDTH'))
       return top_of_stack.closing_scope_indent
 
     if (previous and previous.is_string and current.is_string and
         _IsDictionaryValue(current)):
       return previous.column
 
     if style.Get('INDENT_DICTIONARY_VALUE'):
       if _IsDictionaryValue(current):
         if previous and (previous.value == ':' or previous.is_pseudo_paren):
           return top_of_stack.indent
 
     if (self.line.first.value in _COMPOUND_STMTS and
-        not style.Get('DEDENT_CLOSING_BRACKETS')):
+        (not style.Get('DEDENT_CLOSING_BRACKETS') or
+         style.Get('SPLIT_BEFORE_FIRST_ARGUMENT'))):
       token_indent = (len(self.line.first.whitespace_prefix.split('\n')[-1]) +
                       style.Get('INDENT_WIDTH'))
       if token_indent == top_of_stack.indent:
         return top_of_stack.indent + style.Get('CONTINUATION_INDENT_WIDTH')
 
     return top_of_stack.indent
 
@@ -414,15 +423,14 @@
     # If we encounter an opening bracket, we add a level to our stack to prepare
     # for the subsequent tokens.
     if current.OpensScope():
       last = self.stack[-1]
       new_indent = style.Get('CONTINUATION_INDENT_WIDTH') + last.last_space
 
       self.stack.append(_ParenState(new_indent, self.stack[-1].last_space))
-      self.stack[-1].break_before_paremeter = False
       self.paren_level += 1
 
     # If we encounter a closing bracket, we can remove a level from our
     # parenthesis stack.
     if len(self.stack) > 1 and current.ClosesScope():
       self.stack[-2].last_space = self.stack[-1].last_space
       self.stack.pop()
@@ -476,23 +484,27 @@
          (exclude is None or exclude not in current.subtypes)):
     current = current.next_token
   return current.total_length - token.total_length + 1
 
 
 def _GetOpeningParen(current):
   previous = current
+  if previous and previous.matching_bracket:
+    return previous.matching_bracket
   while previous is not None and previous.matching_bracket is None:
     previous = previous.previous_token
+    if not previous:
+      break
     if previous.ClosesScope():
       previous = previous.matching_bracket.previous_token
   return previous
 
 
 def _LastTokenInLine(current):
-  while current.next_token:
+  while not current.is_comment and current.next_token:
     current = current.next_token
   return current
 
 
 def _IsLastScopeInLine(current):
   while current:
     current = current.next_token
```

### Comparing `yapf-0.8.2/yapf/yapflib/format_token.py` & `yapf-0.9.0/yapf/yapflib/format_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -194,14 +194,20 @@
   @property
   def newlines(self):
     """The number of newlines needed before this token."""
     return pytree_utils.GetNodeAnnotation(self._node,
                                           pytree_utils.Annotation.NEWLINES)
 
   @property
+  def must_split(self):
+    """Return true if the token requires a split before it."""
+    return pytree_utils.GetNodeAnnotation(self._node,
+                                          pytree_utils.Annotation.MUST_SPLIT)
+
+  @property
   def column(self):
     """The original column number of the node in the source."""
     return self._node.column
 
   @property
   def lineno(self):
     """The original line number of the node in the source."""
```

### Comparing `yapf-0.8.2/yapf/yapflib/line_joiner.py` & `yapf-0.9.0/yapf/yapflib/line_joiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/py3compat.py` & `yapf-0.9.0/yapf/yapflib/py3compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/pytree_unwrapper.py` & `yapf-0.9.0/yapf/yapflib/pytree_unwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -116,16 +116,22 @@
     # can leave it in the tree directly without creating a suite. But we have
     # to increase depth in these cases as well. However, don't increase the
     # depth of we have a simple_stmt that's a comment node. This represents a
     # standalone comment and in the case of it coming directly after the
     # funcdef, it is a "top" comment for the whole function.
     # TODO(eliben): add more relevant compound statements here.
     single_stmt_suite = (node.parent and pytree_utils.NodeName(node.parent) in {
-        'if_stmt', 'while_stmt', 'for_stmt', 'try_stmt', 'expect_clause',
-        'with_stmt', 'funcdef', 'classdef',
+        'if_stmt',
+        'while_stmt',
+        'for_stmt',
+        'try_stmt',
+        'expect_clause',
+        'with_stmt',
+        'funcdef',
+        'classdef',
     })
     is_comment_stmt = pytree_utils.NodeName(node.children[0]) == 'COMMENT'
     if single_stmt_suite and not is_comment_stmt:
       self._cur_depth += 1
     self._StartNewLine()
     self.DefaultNodeVisit(node)
     if single_stmt_suite and not is_comment_stmt:
@@ -167,14 +173,20 @@
 
   def Visit_except_clause(self, node):  # pylint: disable=invalid-name
     self._VisitCompoundStatement(node, {'except'})
 
   def Visit_funcdef(self, node):  # pylint: disable=invalid-name
     self._VisitCompoundStatement(node, {'def'})
 
+  def Visit_async_funcdef(self, node):  # pylint: disable=invalid-name
+    self._StartNewLine()
+    self.Visit(node.children[0])
+    for child in node.children[1].children:
+      self.Visit(child)
+
   def Visit_classdef(self, node):  # pylint: disable=invalid-name
     self._VisitCompoundStatement(node, {'class'})
 
   def Visit_async_stmt(self, node):  # pylint: disable=invalid-name
     self._StartNewLine()
     self.Visit(node.children[0])
     for child in node.children[1].children:
```

### Comparing `yapf-0.8.2/yapf/yapflib/pytree_utils.py` & `yapf-0.9.0/yapf/yapflib/pytree_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -72,14 +72,15 @@
 # context where a keyword is disallowed).
 # It forgets to do the same for 'exec' though. Luckily, Python is amenable to
 # monkey-patching.
 _GRAMMAR_FOR_PY3 = pygram.python_grammar_no_print_statement.copy()
 del _GRAMMAR_FOR_PY3.keywords['exec']
 
 _GRAMMAR_FOR_PY2 = pygram.python_grammar.copy()
+del _GRAMMAR_FOR_PY2.keywords['nonlocal']
 
 
 def ParseCodeToTree(code):
   """Parse the given code to a lib2to3 pytree.
 
   Arguments:
     code: a string with the code to parse.
@@ -277,20 +278,18 @@
                       len=len(node.children),
                       indent=GetNodeAnnotation(node, Annotation.CHILD_INDENT))
 
 
 def _PytreeNodeRepr(node):
   """Like pytree.Node.__repr__, but names instead of numbers for tokens."""
   if isinstance(node, pytree.Node):
-    return '%s(%s, %r)' % (node.__class__.__name__,
-                           NodeName(node),
+    return '%s(%s, %r)' % (node.__class__.__name__, NodeName(node),
                            [_PytreeNodeRepr(c) for c in node.children])
   if isinstance(node, pytree.Leaf):
-    return '%s(%s, %r)' % (node.__class__.__name__,
-                           NodeName(node), node.value)
+    return '%s(%s, %r)' % (node.__class__.__name__, NodeName(node), node.value)
   # Throw an exception if it's not an expected type:
   assert isinstance(node, (pytree.Node, pytree.Leaf)), type(node)
 
 
 def IsCommentStatement(node):
   return (NodeName(node) == 'simple_stmt' and
           NodeName(node.children[0]) == 'COMMENT')
```

### Comparing `yapf-0.8.2/yapf/yapflib/pytree_visitor.py` & `yapf-0.9.0/yapf/yapflib/pytree_visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/reformatter.py` & `yapf-0.9.0/yapf/yapflib/reformatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -69,49 +69,31 @@
         _RetainVerticalSpacingBeforeComments(uwline)
 
     if (_LineContainsI18n(uwline) or uwline.disable or
         _LineHasContinuationMarkers(uwline)):
       _RetainHorizontalSpacing(uwline)
       _RetainVerticalSpacing(uwline, prev_uwline)
       _EmitLineUnformatted(state)
-    elif _CanPlaceOnSingleLine(uwline):
+    elif (_CanPlaceOnSingleLine(uwline) and not any(tok.must_split
+                                                    for tok in uwline.tokens)):
       # The unwrapped line fits on one line.
       while state.next_token:
         state.AddTokenToState(newline=False, dry_run=False)
     else:
       if not _AnalyzeSolutionSpace(state, dry_run=False):
         # Failsafe mode. If there isn't a solution to the line, then just emit
         # it as is.
         state = format_decision_state.FormatDecisionState(uwline, indent_amt)
         _RetainHorizontalSpacing(uwline)
         _RetainVerticalSpacing(uwline, prev_uwline)
         _EmitLineUnformatted(state)
 
     final_lines.append(uwline)
     prev_uwline = uwline
-
-  formatted_code = []
-  for line in final_lines:
-    formatted_line = []
-    for tok in line.tokens:
-      if not tok.is_pseudo_paren:
-        formatted_line.append(tok.whitespace_prefix)
-        formatted_line.append(tok.value)
-      else:
-        if (not tok.next_token.whitespace_prefix.startswith('\n') and
-            not tok.next_token.whitespace_prefix.startswith(' ')):
-          if (tok.previous_token.value == ':' or
-              tok.next_token.value not in ',}])'):
-            formatted_line.append(' ')
-
-    formatted_code.append(''.join(formatted_line))
-    if verify:
-      verifier.VerifyCode(formatted_code[-1])
-
-  return ''.join(formatted_code) + '\n'
+  return _FormatFinalLines(final_lines, verify)
 
 
 def _RetainHorizontalSpacing(uwline):
   """Retain all horizontal spacing between tokens."""
   for tok in uwline.tokens:
     tok.RetainHorizontalSpacing(uwline.first.column, uwline.depth)
 
@@ -231,14 +213,36 @@
     True if the line can or should be added to a single line. False otherwise.
   """
   indent_amt = style.Get('INDENT_WIDTH') * uwline.depth
   return (uwline.last.total_length + indent_amt <= style.Get('COLUMN_LIMIT') and
           not any(tok.is_comment for tok in uwline.tokens[:-1]))
 
 
+def _FormatFinalLines(final_lines, verify):
+  formatted_code = []
+  for line in final_lines:
+    formatted_line = []
+    for tok in line.tokens:
+      if not tok.is_pseudo_paren:
+        formatted_line.append(tok.whitespace_prefix)
+        formatted_line.append(tok.value)
+      else:
+        if (not tok.next_token.whitespace_prefix.startswith('\n') and
+            not tok.next_token.whitespace_prefix.startswith(' ')):
+          if (tok.previous_token.value == ':' or
+              tok.next_token.value not in ',}])'):
+            formatted_line.append(' ')
+
+    formatted_code.append(''.join(formatted_line))
+    if verify:
+      verifier.VerifyCode(formatted_code[-1])
+
+  return ''.join(formatted_code) + '\n'
+
+
 class _StateNode(object):
   """An edge in the solution space from 'previous.state' to 'state'.
 
   Attributes:
     state: (format_decision_state.FormatDecisionState) The format decision state
       for this node.
     newline: If True, then on the edge from 'previous.state' to 'state' a
@@ -345,20 +349,23 @@
 
   Returns:
     The updated number of elements in the queue.
   """
   if newline and not previous_node.state.CanSplit():
     # Don't add a newline if the token cannot be split.
     return count
-  if not newline and previous_node.state.MustSplit():
+  must_split = previous_node.state.MustSplit()
+  if not newline and must_split:
     # Don't add a token we must split but where we aren't splitting.
     return count
 
   node = _StateNode(previous_node.state, newline, previous_node)
-  penalty += node.state.AddTokenToState(newline=newline, dry_run=True)
+  penalty += node.state.AddTokenToState(newline=newline,
+                                        dry_run=True,
+                                        must_split=must_split)
   heapq.heappush(p_queue, _QueueItem(_OrderedPenalty(penalty, count), node))
   return count + 1
 
 
 def _ReconstructPath(initial_state, current):
   """Reconstruct the path through the queue with lowest penalty.
```

### Comparing `yapf-0.8.2/yapf/yapflib/split_penalty.py` & `yapf-0.9.0/yapf/yapflib/split_penalty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -99,15 +99,16 @@
 
   def Visit_parameters(self, node):  # pylint: disable=invalid-name
     # parameters ::= '(' [typedargslist] ')'
     self.DefaultNodeVisit(node)
 
     # Can't break before the opening paren of a parameter list.
     self._SetUnbreakable(node.children[0])
-    self._SetStronglyConnected(node.children[-1])
+    if not style.Get('DEDENT_CLOSING_BRACKETS'):
+      self._SetStronglyConnected(node.children[-1])
 
   def Visit_argument(self, node):  # pylint: disable=invalid-name
     # argument ::= test [comp_for] | test '=' test  # Really [keyword '='] test
     self.DefaultNodeVisit(node)
 
     index = 0
     while index < len(node.children) - 1:
@@ -133,23 +134,25 @@
         self._SetStronglyConnected(child)
 
   def Visit_trailer(self, node):  # pylint: disable=invalid-name
     # trailer ::= '(' [arglist] ')' | '[' subscriptlist ']' | '.' NAME
     self.DefaultNodeVisit(node)
     if node.children[0].value == '.':
       self._SetUnbreakableOnChildren(node)
-      pytree_utils.SetNodeAnnotation(
-          node.children[1], pytree_utils.Annotation.SPLIT_PENALTY,
-          DOTTED_NAME)
+      pytree_utils.SetNodeAnnotation(node.children[1],
+                                     pytree_utils.Annotation.SPLIT_PENALTY,
+                                     DOTTED_NAME)
     elif len(node.children) == 2:
       # Don't split an empty argument list if at all possible.
       self._SetStronglyConnected(node.children[1])
     elif len(node.children) == 3:
-      if (pytree_utils.NodeName(node.children[1]) not in
-          {'arglist', 'argument', 'term', 'or_test', 'and_test', 'comparison'}):
+      if pytree_utils.NodeName(node.children[1]) not in {
+          'arglist', 'argument', 'term', 'or_test', 'and_test', 'comparison',
+          'atom'
+      }:
         # Don't split an argument list with one element if at all possible.
         self._SetStronglyConnected(node.children[1], node.children[2])
       if pytree_utils.NodeName(node.children[-1]) == 'RSQB':
         # Don't split the ending bracket of a subscript list.
         self._SetStronglyConnected(node.children[-1])
 
   def Visit_power(self, node):  # pylint: disable=invalid-name,missing-docstring
@@ -225,23 +228,24 @@
   def Visit_subscript(self, node):  # pylint: disable=invalid-name
     # subscript ::= test | [test] ':' [test] [sliceop]
     self._SetStronglyConnected(*node.children)
     self.DefaultNodeVisit(node)
 
   def Visit_comp_for(self, node):  # pylint: disable=invalid-name
     # comp_for ::= 'for' exprlist 'in' testlist_safe [comp_iter]
-    pytree_utils.SetNodeAnnotation(_FirstChildNode(node),
-                                   pytree_utils.Annotation.SPLIT_PENALTY, 0)
+    pytree_utils.SetNodeAnnotation(
+        _FirstChildNode(node), pytree_utils.Annotation.SPLIT_PENALTY, 0)
     self._SetStronglyConnected(*node.children[1:])
     self.DefaultNodeVisit(node)
 
   def Visit_comp_if(self, node):  # pylint: disable=invalid-name
     # comp_if ::= 'if' old_test [comp_iter]
     pytree_utils.SetNodeAnnotation(node.children[0],
-                                   pytree_utils.Annotation.SPLIT_PENALTY, 0)
+                                   pytree_utils.Annotation.SPLIT_PENALTY,
+                                   style.Get('SPLIT_PENALTY_BEFORE_IF_EXPR'))
     self._SetStronglyConnected(*node.children[1:])
     self.DefaultNodeVisit(node)
 
   def Visit_not_test(self, node):  # pylint: disable=invalid-name
     # not_test ::= 'not' not_test | comparison
     self.DefaultNodeVisit(node)
     self._SetExpressionPenalty(node, NOT_TEST)
@@ -268,25 +272,25 @@
         if pytree_utils.NodeName(node.parent) == 'if_stmt':
           pytree_utils.SetNodeAnnotation(node.children[-1],
                                          pytree_utils.Annotation.SPLIT_PENALTY,
                                          UNBREAKABLE)
         else:
           pytree_utils.SetNodeAnnotation(node.children[-1],
                                          pytree_utils.Annotation.SPLIT_PENALTY,
-                                         STRONGLY_CONNECTED)
+                                         COMPARISON_EXPRESSION)
     elif node.children[0].value in '[{':
       # Keep empty containers together if we can.
       lbracket = node.children[0]
       rbracket = node.children[-1]
       if len(node.children) == 2:
         self._SetUnbreakable(node.children[-1])
       elif (rbracket.value in ']}' and
             lbracket.get_lineno() == rbracket.get_lineno() and
             rbracket.column - lbracket.column < style.Get('COLUMN_LIMIT')):
-        self._SetExpressionPenalty(node, CONTIGUOUS_LIST)
+        self._SetStronglyConnected(*node.children[1:])
 
   ############################################################################
   # Helper methods that set the annotations.
 
   def _SetUnbreakable(self, node):
     """Set an UNBREAKABLE penalty annotation for the given node."""
     _RecAnnotate(node, pytree_utils.Annotation.SPLIT_PENALTY, UNBREAKABLE)
@@ -312,20 +316,20 @@
       if node is first_child_leaf:
         return
 
       if isinstance(node, pytree.Leaf):
         if node.value in {'(', 'for', 'if'}:
           return
         penalty_annotation = pytree_utils.GetNodeAnnotation(
-            node,
-            pytree_utils.Annotation.SPLIT_PENALTY,
+            node, pytree_utils.Annotation.SPLIT_PENALTY,
             default=0)
         if penalty_annotation < penalty:
-          pytree_utils.SetNodeAnnotation(
-              node, pytree_utils.Annotation.SPLIT_PENALTY, penalty)
+          pytree_utils.SetNodeAnnotation(node,
+                                         pytree_utils.Annotation.SPLIT_PENALTY,
+                                         penalty)
       else:
         for child in node.children:
           RecArithmeticExpression(child, first_child_leaf)
 
     RecArithmeticExpression(node, _FirstChildNode(node))
```

### Comparing `yapf-0.8.2/yapf/yapflib/style.py` & `yapf-0.9.0/yapf/yapflib/style.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -39,112 +39,119 @@
 def SetGlobalStyle(style):
   """Set a style dict."""
   global _style
   _style = style
 
 
 _STYLE_HELP = dict(
-    ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT=
-    'Align closing bracket with visual indentation.',
-    ALLOW_MULTILINE_LAMBDAS=
-    'Allow lambdas to be formatted on more than one line.',
-    COLUMN_LIMIT='The column limit.',
+    ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT=textwrap.dedent("""\
+      Align closing bracket with visual indentation."""),
+    ALLOW_MULTILINE_LAMBDAS=textwrap.dedent("""\
+      Allow lambdas to be formatted on more than one line."""),
+    BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF=textwrap.dedent("""\
+      Insert a blank line before a 'def' or 'class' immediately nested
+      within another 'def' or 'class'. For example:
+
+        class Foo:
+                           # <------ this blank line
+          def method():
+            ..."""),
+    COLUMN_LIMIT=textwrap.dedent("""\
+      The column limit."""),
+    CONTINUATION_INDENT_WIDTH=textwrap.dedent("""\
+      Indent width used for line continuations."""),
+    DEDENT_CLOSING_BRACKETS=textwrap.dedent("""\
+      Put closing brackets on a separate line, dedented, if the bracketed
+      expression can't fit in a single line. Applies to all kinds of brackets,
+      including function definitions and calls. For example:
+
+        config = {
+            'key1': 'value1',
+            'key2': 'value2',
+        }        # <--- this bracket is dedented and on a separate line
+
+        time_series = self.remote_client.query_entity_counters(
+            entity='dev3246.region1',
+            key='dns.query_latency_tcp',
+            transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
+            start_ts=now()-timedelta(days=3),
+            end_ts=now(),
+        )        # <--- this bracket is dedented and on a separate line"""),
     I18N_COMMENT=textwrap.dedent("""\
       The regex for an i18n comment. The presence of this comment stops
       reformatting of that line, because the comments are required to be
       next to the string they translate."""),
     I18N_FUNCTION_CALL=textwrap.dedent("""\
       The i18n function call names. The presence of this function stops
       reformattting on that line, because the string it has cannot be moved
       away from the i18n comment."""),
     INDENT_DICTIONARY_VALUE=textwrap.dedent("""\
       Indent the dictionary value if it cannot fit on the same line as the
-      dictionary key.
+      dictionary key. For example:
 
-      For example:
-
-      config = {
-          'key1':
-              'value1',
-          'key2': value1 +
-                  value2,
-      }"""),
-    INDENT_WIDTH='The number of columns to use for indentation.',
-    CONTINUATION_INDENT_WIDTH='Indent width used for line continuations.',
-    BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF=textwrap.dedent("""\
-      Insert a blank line before a 'def' or 'class' immediately nested
-      within another 'def' or 'class'.
-
-      For example:
-
-      class Foo:
-                         # <------ this blank line
-        def method():
-          ..."""),
-    DEDENT_CLOSING_BRACKETS=textwrap.dedent("""\
-      Put closing brackets on a separate line, dedented, if the bracketed
-      expression can't fit in a single line. Applies to all kinds of brackets,
-      including function definitions and calls.
-
-      For example:
-
-      config = {
-          'key1': 'value1',
-          'key2': 'value2',
-      }        # <--- this bracket is dedented and on a separate line
-
-      time_series = self.remote_client.query_entity_counters(
-        entity='dev3246.region1',
-        key='dns.query_latency_tcp',
-        transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
-        start_ts=now()-timedelta(days=3),
-        end_ts=now(),
-      )        # <--- this bracket is dedented and on a separate line
-      """),
-    JOIN_MULTIPLE_LINES=
-    "Join short lines into one line. E.g., single line 'if' statements.",
+        config = {
+            'key1':
+                'value1',
+            'key2': value1 +
+                    value2,
+        }"""),
+    INDENT_WIDTH=textwrap.dedent("""\
+      The number of columns to use for indentation."""),
+    JOIN_MULTIPLE_LINES=textwrap.dedent("""\
+      Join short lines into one line. E.g., single line 'if' statements."""),
+    SPACES_AROUND_POWER_OPERATOR=textwrap.dedent("""\
+      Use spaces around the power operator."""),
+    SPACES_BEFORE_COMMENT=textwrap.dedent("""\
+      The number of spaces required before a trailing comment."""),
     SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET=textwrap.dedent("""\
       Insert a space between the ending comma and closing bracket of a list,
       etc."""),
-    SPACES_AROUND_POWER_OPERATOR=
-    'Use spaces around the power operator.',
-    SPACES_BEFORE_COMMENT=
-    'The number of spaces required before a trailing comment.',
-    SPLIT_BEFORE_BITWISE_OPERATOR=
-    "Set to True to prefer splitting before '&', '|' or '^' rather than after.",
-    SPLIT_BEFORE_LOGICAL_OPERATOR=
-    "Set to True to prefer splitting before 'and' or 'or' rather than after.",
-    SPLIT_BEFORE_NAMED_ASSIGNS='Split named assignments onto individual lines.',
-    SPLIT_PENALTY_AFTER_UNARY_OPERATOR=
-    'The penalty for splitting the line after a unary operator.',
-    SPLIT_PENALTY_EXCESS_CHARACTER=
-    'The penalty for characters over the column limit.',
-    SPLIT_PENALTY_BITWISE_OPERATOR=
-    "The penalty of splitting the line around the '&', '|', and '^' operators.",
-    SPLIT_PENALTY_IMPORT_NAMES=textwrap.dedent("""\
-    The penalty of splitting a list of "import as" names.
-
-    For example:
-
-      from a_very_long_or_indented_module_name_yada_yad import (long_argument_1,
-                                                                long_argument_2,
-                                                                long_argument_3)
-
-    would reformat to something like:
-
-      from a_very_long_or_indented_module_name_yada_yad import (
-          long_argument_1, long_argument_2, long_argument_3)
-    """),
-    SPLIT_PENALTY_LOGICAL_OPERATOR=
-    "The penalty of splitting the line around the 'and' and 'or' operators.",
-    SPLIT_PENALTY_AFTER_OPENING_BRACKET=
-    'The penalty for splitting right after the opening bracket.',
+    SPLIT_ARGUMENTS_WHEN_COMMA_TERMINATED=textwrap.dedent("""\
+      Split before arguments if the argument list is terminated by a
+      comma."""),
+    SPLIT_BEFORE_BITWISE_OPERATOR=textwrap.dedent("""\
+      Set to True to prefer splitting before '&', '|' or '^' rather than
+      after."""),
+    SPLIT_BEFORE_FIRST_ARGUMENT=textwrap.dedent("""\
+      If an argument / parameter list is going to be split, then split before
+      the first argument."""),
+    SPLIT_BEFORE_LOGICAL_OPERATOR=textwrap.dedent("""\
+      Set to True to prefer splitting before 'and' or 'or' rather than
+      after."""),
+    SPLIT_BEFORE_NAMED_ASSIGNS=textwrap.dedent("""\
+      Split named assignments onto individual lines."""),
+    SPLIT_PENALTY_AFTER_OPENING_BRACKET=textwrap.dedent("""\
+      The penalty for splitting right after the opening bracket."""),
+    SPLIT_PENALTY_AFTER_UNARY_OPERATOR=textwrap.dedent("""\
+      The penalty for splitting the line after a unary operator."""),
+    SPLIT_PENALTY_BEFORE_IF_EXPR=textwrap.dedent("""\
+      The penalty for splitting right before an if expression."""),
+    SPLIT_PENALTY_BITWISE_OPERATOR=textwrap.dedent("""\
+      The penalty of splitting the line around the '&', '|', and '^'
+      operators."""),
+    SPLIT_PENALTY_EXCESS_CHARACTER=textwrap.dedent("""\
+      The penalty for characters over the column limit."""),
     SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT=textwrap.dedent("""\
       The penalty incurred by adding a line split to the unwrapped line. The
       more line splits added the higher the penalty."""),
+    SPLIT_PENALTY_IMPORT_NAMES=textwrap.dedent("""\
+      The penalty of splitting a list of "import as" names. For example:
+
+        from a_very_long_or_indented_module_name_yada_yad import (long_argument_1,
+                                                                  long_argument_2,
+                                                                  long_argument_3)
+
+      would reformat to something like:
+
+        from a_very_long_or_indented_module_name_yada_yad import (
+            long_argument_1, long_argument_2, long_argument_3)
+      """),
+    SPLIT_PENALTY_LOGICAL_OPERATOR=textwrap.dedent("""\
+      The penalty of splitting the line around the 'and' and 'or'
+      operators."""),
     # BASED_ON_STYLE='Which predefined style this style is based on',
 )
 
 
 def CreatePEP8Style():
   return dict(
       ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT=True,
@@ -157,24 +164,27 @@
       INDENT_WIDTH=4,
       CONTINUATION_INDENT_WIDTH=4,
       BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF=False,
       JOIN_MULTIPLE_LINES=True,
       SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET=True,
       SPACES_AROUND_POWER_OPERATOR=False,
       SPACES_BEFORE_COMMENT=2,
+      SPLIT_ARGUMENTS_WHEN_COMMA_TERMINATED=False,
       SPLIT_BEFORE_BITWISE_OPERATOR=False,
+      SPLIT_BEFORE_FIRST_ARGUMENT=False,
       SPLIT_BEFORE_LOGICAL_OPERATOR=False,
       SPLIT_BEFORE_NAMED_ASSIGNS=True,
       SPLIT_PENALTY_AFTER_UNARY_OPERATOR=10000,
       SPLIT_PENALTY_EXCESS_CHARACTER=2500,
       SPLIT_PENALTY_BITWISE_OPERATOR=300,
       SPLIT_PENALTY_IMPORT_NAMES=0,
       SPLIT_PENALTY_LOGICAL_OPERATOR=300,
       SPLIT_PENALTY_AFTER_OPENING_BRACKET=30,
       SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT=30,
+      SPLIT_PENALTY_BEFORE_IF_EXPR=0,
   )  # yapf: disable
 
 
 def CreateGoogleStyle():
   style = CreatePEP8Style()
   style['ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT'] = False
   style['COLUMN_LIMIT'] = 80
@@ -201,14 +211,15 @@
   style['ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT'] = False
   style['COLUMN_LIMIT'] = 80
   style['DEDENT_CLOSING_BRACKETS'] = True
   style['JOIN_MULTIPLE_LINES'] = False
   style['SPACES_BEFORE_COMMENT'] = 2
   style['SPLIT_PENALTY_AFTER_OPENING_BRACKET'] = 0
   style['SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT'] = 30
+  style['SPLIT_PENALTY_BEFORE_IF_EXPR'] = 30
   return style
 
 
 _STYLE_NAME_TO_FACTORY = dict(
     pep8=CreatePEP8Style,
     chromium=CreateChromiumStyle,
     google=CreateGoogleStyle,
@@ -243,24 +254,28 @@
     INDENT_WIDTH=int,
     CONTINUATION_INDENT_WIDTH=int,
     BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF=_BoolConverter,
     JOIN_MULTIPLE_LINES=_BoolConverter,
     SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET=_BoolConverter,
     SPACES_AROUND_POWER_OPERATOR=_BoolConverter,
     SPACES_BEFORE_COMMENT=int,
+    SPLIT_ARGUMENTS_WHEN_COMMA_TERMINATED=_BoolConverter,
     SPLIT_BEFORE_BITWISE_OPERATOR=_BoolConverter,
+    SPLIT_BEFORE_FIRST_ARGUMENT=_BoolConverter,
     SPLIT_BEFORE_LOGICAL_OPERATOR=_BoolConverter,
     SPLIT_BEFORE_NAMED_ASSIGNS=_BoolConverter,
     SPLIT_PENALTY_AFTER_UNARY_OPERATOR=int,
     SPLIT_PENALTY_EXCESS_CHARACTER=int,
     SPLIT_PENALTY_BITWISE_OPERATOR=int,
     SPLIT_PENALTY_IMPORT_NAMES=int,
     SPLIT_PENALTY_LOGICAL_OPERATOR=int,
     SPLIT_PENALTY_AFTER_OPENING_BRACKET=int,
-    SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT=int,)
+    SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT=int,
+    SPLIT_PENALTY_BEFORE_IF_EXPR=int,
+)  # yapf: disable
 
 
 def CreateStyleFromConfig(style_config):
   """Create a style dict from the given config.
 
   Arguments:
     style_config: either a style name or a file name. The file is expected to
@@ -367,16 +382,17 @@
 
 # The default style - used if yapf is not invoked without specifically
 # requesting a formatting style.
 DEFAULT_STYLE = 'pep8'
 DEFAULT_STYLE_FACTORY = CreatePEP8Style
 
 # The name of the file to use for global style definition.
-GLOBAL_STYLE = (os.path.join(os.getenv('XDG_CONFIG_HOME') or
-                os.path.expanduser('~/.config'), 'yapf', 'style'))
+GLOBAL_STYLE = (os.path.join(
+    os.getenv('XDG_CONFIG_HOME') or os.path.expanduser('~/.config'), 'yapf',
+    'style'))
 
 # The name of the file to use for directory-local style definition.
 LOCAL_STYLE = '.style.yapf'
 
 # Alternative place for directory-local style definition. Style should be
 # specified in the '[yapf]' section.
 SETUP_CONFIG = 'setup.cfg'
```

### Comparing `yapf-0.8.2/yapf/yapflib/subtype_assigner.py` & `yapf-0.9.0/yapf/yapflib/subtype_assigner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/unwrapped_line.py` & `yapf-0.9.0/yapf/yapflib/unwrapped_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -317,15 +317,15 @@
 
 
 def _MustBreakBefore(prev_token, cur_token):
   """Return True if a line break is required before the current token."""
   if prev_token.is_comment:
     # Must break if the previous token was a comment.
     return True
-  if (_IsSurroundedByBrackets(cur_token) and cur_token.is_string and
+  if (IsSurroundedByBrackets(cur_token) and cur_token.is_string and
       prev_token.is_string):
     # We want consecutive strings to be on separate lines. This is a
     # reasonable assumption, because otherwise they should have written them
     # all on the same line, or with a '+'.
     return True
   return pytree_utils.GetNodeAnnotation(cur_token.node,
                                         pytree_utils.Annotation.MUST_SPLIT,
@@ -367,15 +367,15 @@
     return False
   if format_token.Subtype.UNARY_OPERATOR in prev_token.subtypes:
     # Don't break after a unary token.
     return False
   return True
 
 
-def _IsSurroundedByBrackets(tok):
+def IsSurroundedByBrackets(tok):
   """Return True if the token is surrounded by brackets."""
   paren_count = 0
   brace_count = 0
   sq_bracket_count = 0
   previous_token = tok.previous_token
   while previous_token:
     if previous_token.value == ')':
@@ -454,15 +454,15 @@
   if prev_token.is_binary_op:
     # We would rather not split after an equality operator.
     return 20
   if (format_token.Subtype.VARARGS_STAR in prev_token.subtypes or
       format_token.Subtype.KWARGS_STAR_STAR in prev_token.subtypes):
     # Don't split after a varargs * or kwargs **.
     return split_penalty.UNBREAKABLE
-  if prev_token.value in pytree_utils.OPENING_BRACKETS:
+  if prev_token.OpensScope() and cur_token.value != '(':
     # Slightly prefer
     return style.Get('SPLIT_PENALTY_AFTER_OPENING_BRACKET')
   if cur_token.value == ':':
     # Don't split before a colon.
     return split_penalty.UNBREAKABLE
   if cur_token.value == '=':
     # Don't split before an assignment.
```

### Comparing `yapf-0.8.2/yapf/yapflib/verifier.py` & `yapf-0.9.0/yapf/yapflib/verifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapf/yapflib/yapf_api.py` & `yapf-0.9.0/yapf/yapflib/yapf_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -228,24 +228,24 @@
     elif re.search(DISABLE_PATTERN, uwline.last.value.strip(), re.IGNORECASE):
       uwline.disable = True
     index += 1
 
 
 def _DisableYAPF(line):
   return (re.search(DISABLE_PATTERN, line.split('\n')[0].strip(),
-                    re.IGNORECASE) or
-          re.search(DISABLE_PATTERN, line.split('\n')[-1].strip(),
-                    re.IGNORECASE))
+                    re.IGNORECASE) or re.search(DISABLE_PATTERN,
+                                                line.split('\n')[-1].strip(),
+                                                re.IGNORECASE))
 
 
 def _EnableYAPF(line):
   return (re.search(ENABLE_PATTERN, line.split('\n')[0].strip(),
-                    re.IGNORECASE) or
-          re.search(ENABLE_PATTERN, line.split('\n')[-1].strip(),
-                    re.IGNORECASE))
+                    re.IGNORECASE) or re.search(ENABLE_PATTERN,
+                                                line.split('\n')[-1].strip(),
+                                                re.IGNORECASE))
 
 
 def _GetUnifiedDiff(before, after, filename='code'):
   """Get a unified diff of the changes.
 
   Arguments:
     before: (unicode) The original source code.
```

### Comparing `yapf-0.8.2/yapf.egg-info/PKG-INFO` & `yapf-0.9.0/yapf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: yapf
-Version: 0.8.2
+Version: 0.9.0
 Summary: A formatter for Python code.
 Home-page: UNKNOWN
 Author: Bill Wendling
 Author-email: morbo@google.com
 License: Apache License, Version 2.0
 Description: ====
         YAPF
@@ -88,15 +88,14 @@
         Usage
         =====
         
         Options::
         
             usage: yapf [-h] [-v] [-d | -i] [-r | -l START-END] [-e PATTERN]
                         [--style STYLE] [--style-help] [--no-local-style]
-                        [--verify]
                         [files [files ...]]
         
             Formatter for Python code.
         
             positional arguments:
               files
         
@@ -114,15 +113,14 @@
                                     example "pep8" or "google"), or the name of a file
                                     with style settings. The default is pep8 unless a
                                     .style.yapf or setup.cfg file located in one of the
                                     parent directories of the source file (or current
                                     directory for stdin)
               --style-help          show style settings and exit
               --no-local-style      don't search for local style definition (.style.yapf)
-              --verify              try to verify reformatted code for syntax errors
         
         
         Formatting style
         ================
         
         The formatting style used by YAPF is configurable and there are many "knobs"
         that can be used to tune how YAPF does formatting. See the ``style.py`` module
@@ -285,21 +283,22 @@
         
         Knobs
         =====
         
         ``ALIGN_CLOSING_BRACKET_WITH_VISUAL_INDENT``
             Align closing bracket with visual indentation.
         
-        ``BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF``
-            Insert a blank line before a 'def' or 'class' immediately nested
-            within another 'def' or 'class'.
+        ``ALLOW_MULTILINE_LAMBDAS``
+            Allow lambdas to be formatted on more than one line.
         
-            For example:
+        ``BLANK_LINE_BEFORE_NESTED_CLASS_OR_DEF``
+            Insert a blank line before a ``def`` or ``class`` immediately nested within
+            another ``def`` or ``class``. For example:
         
-        .. code-block:: python
+            .. code-block:: python
         
                 class Foo:
                                    # <------ this blank line
                     def method():
                         pass
         
         ``COLUMN_LIMIT``
@@ -307,124 +306,126 @@
         
         ``CONTINUATION_INDENT_WIDTH``
             Indent width used for line continuations.
         
         ``DEDENT_CLOSING_BRACKETS``
             Put closing brackets on a separate line, dedented, if the bracketed
             expression can't fit in a single line. Applies to all kinds of brackets,
-            including function definitions and calls.
+            including function definitions and calls. For example:
         
-            For example:
-        
-        .. code-block:: python
+            .. code-block:: python
         
                 config = {
                     'key1': 'value1',
                     'key2': 'value2',
-                }        # <--- this bracket is dedented and on a separate line
+                }  # <--- this bracket is dedented and on a separate line
         
                 time_series = self.remote_client.query_entity_counters(
-                  entity='dev3246.region1',
-                  key='dns.query_latency_tcp',
-                  transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
-                  start_ts=now()-timedelta(days=3),
-                  end_ts=now(),
-                )        # <--- this bracket is dedented and on a separate line
+                    entity='dev3246.region1',
+                    key='dns.query_latency_tcp',
+                    transform=Transformation.AVERAGE(window=timedelta(seconds=60)),
+                    start_ts=now()-timedelta(days=3),
+                    end_ts=now(),
+                )  # <--- this bracket is dedented and on a separate line
         
         ``I18N_COMMENT``
             The regex for an internationalization comment. The presence of this comment
             stops reformatting of that line, because the comments are required to be
             next to the string they translate.
         
         ``I18N_FUNCTION_CALL``
-            The internationalization function call names. The presence of this
-            function stops reformattting on that line, because the string it has
-            cannot be moved away from the i18n comment.
+            The internationalization function call names. The presence of this function
+            stops reformattting on that line, because the string it has cannot be moved
+            away from the i18n comment.
         
         ``INDENT_DICTIONARY_VALUE``
             Indent the dictionary value if it cannot fit on the same line as the
-            dictionary key.
+            dictionary key. For example:
         
-            For example:
-        
-        .. code-block:: python
+            .. code-block:: python
         
                 config = {
                     'key1':
                         'value1',
                     'key2': value1 +
                             value2,
                 }
         
         ``INDENT_WIDTH``
             The number of columns to use for indentation.
         
         ``JOIN_MULTIPLE_LINES``
             Join short lines into one line. E.g., single line ``if`` statements.
         
-        ``SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET``
-            Insert a space between the ending comma and closing bracket of a list,
-            etc.
-        
         ``SPACES_AROUND_POWER_OPERATOR``
             Set to ``True`` to prefer using spaces around ``**``.
         
         ``SPACES_BEFORE_COMMENT``
             The number of spaces required before a trailing comment.
         
+        ``SPACE_BETWEEN_ENDING_COMMA_AND_CLOSING_BRACKET``
+            Insert a space between the ending comma and closing bracket of a list, etc.
+        
+        ``SPLIT_ARGUMENTS_WHEN_COMMA_TERMINATED``
+            Split before arguments if the argument list is terminated by a comma.
+        
         ``SPLIT_BEFORE_BITWISE_OPERATOR``
             Set to ``True`` to prefer splitting before ``&``, ``|`` or ``^`` rather
             than after.
         
+        ``SPLIT_BEFORE_FIRST_ARGUMENT``
+            If an argument / parameter list is going to be split, then split before the
+            first argument.
+        
         ``SPLIT_BEFORE_LOGICAL_OPERATOR``
             Set to ``True`` to prefer splitting before ``and`` or ``or`` rather than
             after.
         
         ``SPLIT_BEFORE_NAMED_ASSIGNS``
             Split named assignments onto individual lines.
         
         ``SPLIT_PENALTY_AFTER_OPENING_BRACKET``
             The penalty for splitting right after the opening bracket.
         
         ``SPLIT_PENALTY_AFTER_UNARY_OPERATOR``
             The penalty for splitting the line after a unary operator.
         
+        ``SPLIT_PENALTY_BEFORE_IF_EXPR``
+            The penalty for splitting right before an ``if`` expression.
+        
         ``SPLIT_PENALTY_BITWISE_OPERATOR``
             The penalty of splitting the line around the ``&``, ``|``, and ``^``
             operators.
         
         ``SPLIT_PENALTY_EXCESS_CHARACTER``
             The penalty for characters over the column limit.
         
         ``SPLIT_PENALTY_FOR_ADDED_LINE_SPLIT``
-            The penalty incurred by adding a line split to the unwrapped line. The
-            more line splits added the higher the penalty.
+            The penalty incurred by adding a line split to the unwrapped line. The more
+            line splits added the higher the penalty.
         
         ``SPLIT_PENALTY_IMPORT_NAMES``
-            The penalty of splitting a list of ``import as`` names.
+            The penalty of splitting a list of ``import as`` names. For example:
         
-            For example:
-        
-        .. code-block:: python
+            .. code-block:: python
         
               from a_very_long_or_indented_module_name_yada_yad import (long_argument_1,
                                                                         long_argument_2,
                                                                         long_argument_3)
         
             would reformat to something like:
         
-        .. code-block:: python
+            .. code-block:: python
         
               from a_very_long_or_indented_module_name_yada_yad import (
                   long_argument_1, long_argument_2, long_argument_3)
         
         ``SPLIT_PENALTY_LOGICAL_OPERATOR``
             The penalty of splitting the line around the ``and`` and ``or`` operators.
         
-        
         (Potentially) Frequently Asked Questions
         ========================================
         
         Why does YAPF destroy my awesome formatting?
         --------------------------------------------
         
         YAPF tries very hard to get the formatting correct. But for some code, it won't
```

### Comparing `yapf-0.8.2/yapf.egg-info/SOURCES.txt` & `yapf-0.9.0/yapf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yapf-0.8.2/yapftests/blank_line_calculator_test.py` & `yapf-0.9.0/yapftests/blank_line_calculator_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapftests/comment_splicer_test.py` & `yapf-0.9.0/yapftests/comment_splicer_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapftests/file_resources_test.py` & `yapf-0.9.0/yapftests/file_resources_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -85,25 +85,21 @@
     tdir1 = self._make_test_dir('test1')
     tdir2 = self._make_test_dir('test2')
     file1 = os.path.join(tdir1, 'testfile1.py')
     file2 = os.path.join(tdir2, 'testfile2.py')
     _touch_files([file1, file2])
 
     self.assertEqual(
-        file_resources.GetCommandLineFiles(
-            [file1, file2],
-            recursive=False,
-            exclude=None),
-        [file1, file2])
+        file_resources.GetCommandLineFiles([file1, file2],
+                                           recursive=False,
+                                           exclude=None), [file1, file2])
     self.assertEqual(
-        file_resources.GetCommandLineFiles(
-            [file1, file2],
-            recursive=True,
-            exclude=None),
-        [file1, file2])
+        file_resources.GetCommandLineFiles([file1, file2],
+                                           recursive=True,
+                                           exclude=None), [file1, file2])
 
   def test_nonrecursive_find_in_dir(self):
     tdir1 = self._make_test_dir('test1')
     tdir2 = self._make_test_dir('test1/foo')
     file1 = os.path.join(tdir1, 'testfile1.py')
     file2 = os.path.join(tdir2, 'testfile2.py')
     _touch_files([file1, file2])
@@ -120,36 +116,34 @@
     tdir3 = self._make_test_dir('test3/foo/bar/bas/xxx')
     files = [os.path.join(tdir1, 'testfile1.py'),
              os.path.join(tdir2, 'testfile2.py'),
              os.path.join(tdir3, 'testfile3.py')]
     _touch_files(files)
 
     self.assertEqual(
-        sorted(file_resources.GetCommandLineFiles(
-            [self.test_tmpdir],
-            recursive=True,
-            exclude=None)),
+        sorted(file_resources.GetCommandLineFiles([self.test_tmpdir],
+                                                  recursive=True,
+                                                  exclude=None)),
         sorted(files))
 
   def test_recursive_find_in_dir_with_exclude(self):
     tdir1 = self._make_test_dir('test1')
     tdir2 = self._make_test_dir('test2/testinner/')
     tdir3 = self._make_test_dir('test3/foo/bar/bas/xxx')
     files = [os.path.join(tdir1, 'testfile1.py'),
              os.path.join(tdir2, 'testfile2.py'),
              os.path.join(tdir3, 'testfile3.py')]
     _touch_files(files)
 
     self.assertEqual(
-        sorted(file_resources.GetCommandLineFiles(
-            [self.test_tmpdir],
-            recursive=True,
-            exclude=['*test*3.py'])),
-        sorted([os.path.join(tdir1, 'testfile1.py'), os.path.join(
-            tdir2, 'testfile2.py')]))
+        sorted(file_resources.GetCommandLineFiles([self.test_tmpdir],
+                                                  recursive=True,
+                                                  exclude=['*test*3.py'])),
+        sorted([os.path.join(tdir1, 'testfile1.py'),
+                os.path.join(tdir2, 'testfile2.py')]))
 
 
 class IsPythonFileTest(unittest.TestCase):
 
   def setUp(self):
     self.test_tmpdir = tempfile.mkdtemp()
```

### Comparing `yapf-0.8.2/yapftests/format_decision_state_test.py` & `yapf-0.9.0/yapftests/format_decision_state_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -51,16 +51,15 @@
     if dumptree:
       pytree_visitor.DumpPyTree(tree, target_stream=sys.stderr)
 
     return pytree_unwrapper.UnwrapPyTree(tree)
 
   def _FilterLine(self, uwline):
     """Filter out nonsemantic tokens from the UnwrappedLines."""
-    return [ft
-            for ft in uwline.tokens
+    return [ft for ft in uwline.tokens
             if ft.name not in pytree_utils.NONSEMANTIC_TOKENS]
 
   def testSimpleFunctionDefWithNoSplitting(self):
     code = textwrap.dedent(r"""
       def f(a, b):
         pass
       """)
```

### Comparing `yapf-0.8.2/yapftests/format_token_test.py` & `yapf-0.9.0/yapftests/format_token_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapftests/line_joiner_test.py` & `yapf-0.9.0/yapftests/line_joiner_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapftests/main_test.py` & `yapf-0.9.0/yapftests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapftests/pytree_unwrapper_test.py` & `yapf-0.9.0/yapftests/pytree_unwrapper_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -53,16 +53,15 @@
     Args:
       uwlines: list of UnwrappedLine
       list_of_expected: list of (depth, values) pairs. Non-semantic tokens are
         filtered out from the expected values.
     """
     actual = []
     for uwl in uwlines:
-      filtered_values = [ft.value
-                         for ft in uwl.tokens
+      filtered_values = [ft.value for ft in uwl.tokens
                          if ft.name not in pytree_utils.NONSEMANTIC_TOKENS]
       actual.append((uwl.depth, filtered_values))
 
     self.assertEqual(list_of_expected, actual)
 
   def testSimpleFileScope(self):
     code = textwrap.dedent(r"""
@@ -324,16 +323,15 @@
       uwlines: list of UnwrappedLine.
       list_of_expected: list of (index, index) pairs. The matching brackets at
         the indexes need to match. Non-semantic tokens are filtered out from the
         expected values.
     """
     actual = []
     for uwl in uwlines:
-      filtered_values = [(ft, ft.matching_bracket)
-                         for ft in uwl.tokens
+      filtered_values = [(ft, ft.matching_bracket) for ft in uwl.tokens
                          if ft.name not in pytree_utils.NONSEMANTIC_TOKENS]
       if filtered_values:
         actual.append(filtered_values)
 
     for index, bracket_list in enumerate(list_of_expected):
       uwline = actual[index]
       if not bracket_list:
```

### Comparing `yapf-0.8.2/yapftests/pytree_utils_test.py` & `yapf-0.9.0/yapftests/pytree_utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -64,14 +64,20 @@
 
   def testPrintStatementToTree(self):
     tree = pytree_utils.ParseCodeToTree('print "hello world"\n')
     self.assertEqual('file_input', pytree_utils.NodeName(tree))
     self.assertEqual(2, len(tree.children))
     self.assertEqual('simple_stmt', pytree_utils.NodeName(tree.children[0]))
 
+  def testClassNotLocal(self):
+    tree = pytree_utils.ParseCodeToTree('class nonlocal: pass\n')
+    self.assertEqual('file_input', pytree_utils.NodeName(tree))
+    self.assertEqual(2, len(tree.children))
+    self.assertEqual('classdef', pytree_utils.NodeName(tree.children[0]))
+
 
 class InsertNodesBeforeAfterTest(unittest.TestCase):
 
   def _BuildSimpleTree(self):
     # Builds a simple tree we can play with in the tests.
     # The tree looks like this:
     #
@@ -92,16 +98,16 @@
     return pytree.Leaf(token.RPAR, ')')
 
   def setUp(self):
     self._simple_tree = self._BuildSimpleTree()
 
   def testInsertNodesBefore(self):
     # Insert before simple_stmt and make sure it went to the right place
-    pytree_utils.InsertNodesBefore(
-        [self._MakeNewNodeRPAR()], self._simple_tree.children[2])
+    pytree_utils.InsertNodesBefore([self._MakeNewNodeRPAR()],
+                                   self._simple_tree.children[2])
     self.assertEqual(4, len(self._simple_tree.children))
     self.assertEqual('RPAR',
                      pytree_utils.NodeName(self._simple_tree.children[2]))
     self.assertEqual('simple_stmt',
                      pytree_utils.NodeName(self._simple_tree.children[3]))
 
   def testInsertNodesBeforeFirstChild(self):
@@ -112,16 +118,16 @@
     self.assertEqual(3, len(self._simple_tree.children))
     self.assertEqual(2, len(simple_stmt.children))
     self.assertEqual('RPAR', pytree_utils.NodeName(simple_stmt.children[0]))
     self.assertEqual('NAME', pytree_utils.NodeName(simple_stmt.children[1]))
 
   def testInsertNodesAfter(self):
     # Insert after and make sure it went to the right place
-    pytree_utils.InsertNodesAfter(
-        [self._MakeNewNodeRPAR()], self._simple_tree.children[2])
+    pytree_utils.InsertNodesAfter([self._MakeNewNodeRPAR()],
+                                  self._simple_tree.children[2])
     self.assertEqual(4, len(self._simple_tree.children))
     self.assertEqual('simple_stmt',
                      pytree_utils.NodeName(self._simple_tree.children[2]))
     self.assertEqual('RPAR',
                      pytree_utils.NodeName(self._simple_tree.children[3]))
 
   def testInsertNodesAfterLastChild(self):
@@ -133,16 +139,16 @@
     self.assertEqual(2, len(simple_stmt.children))
     self.assertEqual('NAME', pytree_utils.NodeName(simple_stmt.children[0]))
     self.assertEqual('RPAR', pytree_utils.NodeName(simple_stmt.children[1]))
 
   def testInsertNodesWhichHasParent(self):
     # Try to insert an existing tree node into another place and fail.
     with self.assertRaises(RuntimeError):
-      pytree_utils.InsertNodesAfter(
-          [self._simple_tree.children[1]], self._simple_tree.children[0])
+      pytree_utils.InsertNodesAfter([self._simple_tree.children[1]],
+                                    self._simple_tree.children[0])
 
 
 class AnnotationsTest(unittest.TestCase):
 
   def setUp(self):
     self._leaf = pytree.Leaf(token.LPAR, '(')
     self._node = pytree.Node(_GRAMMAR_SYMBOL2NUMBER['simple_stmt'],
```

### Comparing `yapf-0.8.2/yapftests/pytree_visitor_test.py` & `yapf-0.9.0/yapftests/pytree_visitor_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapftests/reformatter_test.py` & `yapf-0.9.0/yapftests/reformatter_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -483,15 +483,17 @@
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
   def testOpeningAndClosingBrackets(self):
     unformatted_code = textwrap.dedent("""\
         foo( ( 1, 2, 3, ) )
         """)
     expected_formatted_code = textwrap.dedent("""\
-        foo((1, 2, 3,))
+        foo((1,
+             2,
+             3,))
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
   def testSingleLineFunctions(self):
     unformatted_code = textwrap.dedent("""\
         def foo():  return 42
@@ -1409,16 +1411,16 @@
           def __repr__(self):
             tokens_repr = ','.join(['{0}({1!r})'.format(tok.name, tok.value) for tok in self._tokens])
         """)
     expected_formatted_code = textwrap.dedent("""\
         class f:
 
           def __repr__(self):
-            tokens_repr = ','.join(['{0}({1!r})'.format(tok.name, tok.value)
-                                    for tok in self._tokens])
+            tokens_repr = ','.join(
+                ['{0}({1!r})'.format(tok.name, tok.value) for tok in self._tokens])
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
   def testFunctionCallArguments(self):
     unformatted_code = textwrap.dedent("""\
         def f():
@@ -1619,53 +1621,116 @@
 
       uwlines = _ParseAndUnwrap(reformatted_code)
       reformatted_code = reformatter.Reformat(uwlines)
       self.assertCodeEqual(code, reformatted_code)
     finally:
       style.SetGlobalStyle(style.CreateChromiumStyle())
 
-  def testDedentingInnerScope(self):
-    try:
-      style.SetGlobalStyle(style.CreateStyleFromConfig(
-          '{based_on_style: pep8, column_limit: 100, '
-          'dedent_closing_brackets: True}'))
-      code = textwrap.dedent("""\
-          class Foo():
-              @classmethod
-              def _pack_results_for_constraint_or(cls, combination, constraints):
-                  return cls._create_investigation_result(
-                      (
-                          clue for clue in combination if not clue == Verifier.UNMATCHED
-                      ), constraints, InvestigationResult.OR
-                  )
-          """)
-      uwlines = _ParseAndUnwrap(code)
-      reformatted_code = reformatter.Reformat(uwlines)
-      self.assertCodeEqual(code, reformatted_code)
-
-      uwlines = _ParseAndUnwrap(reformatted_code)
-      reformatted_code = reformatter.Reformat(uwlines)
-      self.assertCodeEqual(code, reformatted_code)
-    finally:
-      style.SetGlobalStyle(style.CreateChromiumStyle())
-
   def testNotSplittingAfterSubscript(self):
     unformatted_code = textwrap.dedent("""\
         if not aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa.b(c == d[
                 'eeeeee']).ffffff():
           pass
         """)
     expected_formatted_code = textwrap.dedent("""\
         if not aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa.b(
             c == d['eeeeee']).ffffff():
           pass
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
+  def testSplittingOneArgumentList(self):
+    unformatted_code = textwrap.dedent("""\
+        def _():
+          if True:
+            if True:
+              if True:
+                if True:
+                  if True:
+                    boxes[id_] = np.concatenate((points.min(axis=0), qoints.max(axis=0)))
+        """)
+    expected_formatted_code = textwrap.dedent("""\
+        def _():
+          if True:
+            if True:
+              if True:
+                if True:
+                  if True:
+                    boxes[id_] = np.concatenate(
+                        (points.min(axis=0), qoints.max(axis=0)))
+        """)
+    uwlines = _ParseAndUnwrap(unformatted_code)
+    self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
+
+  def testSplittingBeforeFirstElementListArgument(self):
+    unformatted_code = textwrap.dedent("""\
+        class _():
+          @classmethod
+          def _pack_results_for_constraint_or(cls, combination, constraints):
+            if True:
+              if True:
+                if True:
+                  return cls._create_investigation_result(
+                          (
+                                  clue for clue in combination if not clue == Verifier.UNMATCHED
+                          ), constraints, InvestigationResult.OR
+                  )
+        """)
+    expected_formatted_code = textwrap.dedent("""\
+        class _():
+
+          @classmethod
+          def _pack_results_for_constraint_or(cls, combination, constraints):
+            if True:
+              if True:
+                if True:
+                  return cls._create_investigation_result(
+                      (clue for clue in combination if not clue == Verifier.UNMATCHED),
+                      constraints, InvestigationResult.OR)
+        """)
+    uwlines = _ParseAndUnwrap(unformatted_code)
+    self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
+
+  def testSplittingArgumentsTerminatedByComma(self):
+    try:
+      style.SetGlobalStyle(style.CreateStyleFromConfig(
+          '{based_on_style: chromium, '
+          'split_arguments_when_comma_terminated: True}'))
+      code = textwrap.dedent("""\
+          function_name(argument_name_1=1, argument_name_2=2, argument_name_3=3)
+
+          function_name(
+              argument_name_1=1,
+              argument_name_2=2,
+              argument_name_3=3,
+          )
+
+          a_very_long_function_name(long_argument_name_1=1,
+                                    long_argument_name_2=2,
+                                    long_argument_name_3=3,
+                                    long_argument_name_4=4)
+
+          a_very_long_function_name(
+              long_argument_name_1,
+              long_argument_name_2,
+              long_argument_name_3,
+              long_argument_name_4,
+          )
+          """)
+      uwlines = _ParseAndUnwrap(code)
+      reformatted_code = reformatter.Reformat(uwlines)
+      self.assertCodeEqual(code, reformatted_code)
+
+      uwlines = _ParseAndUnwrap(reformatted_code)
+      reformatted_code = reformatter.Reformat(uwlines)
+      self.assertCodeEqual(code, reformatted_code)
+    finally:
+      style.SetGlobalStyle(style.CreateChromiumStyle())
+
 
 class BuganizerFixes(ReformatterTest):
 
   @classmethod
   def setUpClass(cls):
     style.SetGlobalStyle(style.CreateChromiumStyle())
 
@@ -1784,17 +1849,16 @@
         """)
     uwlines = _ParseAndUnwrap(code)
     self.assertCodeEqual(code, reformatter.Reformat(uwlines))
 
   def testB25157123(self):
     code = textwrap.dedent("""\
         def ListArgs():
-          FairlyLongMethodName(
-              [relatively_long_identifier_for_a_list],
-              another_argument_with_a_long_identifier)
+          FairlyLongMethodName([relatively_long_identifier_for_a_list],
+                               another_argument_with_a_long_identifier)
         """)
     uwlines = _ParseAndUnwrap(code)
     self.assertCodeEqual(code, reformatter.Reformat(uwlines))
 
   def testB25136820(self):
     unformatted_code = textwrap.dedent("""\
         def foo():
@@ -1963,32 +2027,33 @@
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
   def testB28414371(self):
     code = textwrap.dedent("""\
         def _():
-          return ((m.fffff(
-              m.rrr('mmmmmmmmmmmmmmmm', 'ssssssssssssssssssssssssss'), ffffffffffffffff)
-                   | m.wwwwww(m.ddddd('1h'))
-                   | m.ggggggg(bbbbbbbbbbbbbbb)
-                   | m.ppppp(
-                       (1 - m.ffffffffffffffff(llllllllllllllllllllll * 1000000, m.vvv))
-                       * m.ddddddddddddddddd(m.vvv)),
-                   m.fffff(
+          return (
+              (m.fffff(
+                  m.rrr('mmmmmmmmmmmmmmmm', 'ssssssssssssssssssssssssss'),
+                  ffffffffffffffff)
+               | m.wwwwww(m.ddddd('1h'))
+               | m.ggggggg(bbbbbbbbbbbbbbb)
+               | m.ppppp(
+                   (1 - m.ffffffffffffffff(llllllllllllllllllllll * 1000000, m.vvv)) *
+                   m.ddddddddddddddddd(m.vvv)), m.fffff(
                        m.rrr('mmmmmmmmmmmmmmmm', 'sssssssssssssssssssssss'),
                        dict(ffffffffffffffff,
                             **{
                                 'mmmmmm:ssssss': m.rrrrrrrrrrr('|'.join(iiiiiiiiiiiiii),
                                                                iiiiii=True)
                             }))
-                   | m.wwwwww(m.rrrr('1h'))
-                   | m.ggggggg(bbbbbbbbbbbbbbb))
-                  | m.jjjj()
-                  | m.ppppp(m.vvv[0] + m.vvv[1]))
+               | m.wwwwww(m.rrrr('1h'))
+               | m.ggggggg(bbbbbbbbbbbbbbb))
+              | m.jjjj()
+              | m.ppppp(m.vvv[0] + m.vvv[1]))
         """)
     uwlines = _ParseAndUnwrap(code)
     self.assertCodeEqual(code, reformatter.Reformat(uwlines))
 
   def testB20127686(self):
     code = textwrap.dedent("""\
         def f():
@@ -2220,19 +2285,19 @@
             lambda arg2=0.5: arg2)
         """)
     uwlines = _ParseAndUnwrap(code)
     self.assertCodeEqual(code, reformatter.Reformat(uwlines))
 
   def testB19073499(self):
     code = textwrap.dedent("""\
-        instance = (aaaaaaa.bbbbbbb().ccccccccccccccccc().ddddddddddd(
-            {'aa': 'context!'}).eeeeeeeeeeeeeeeeeee(
-                {  # Inline comment about why fnord has the value 6.
-                    'fnord': 6
-                }))
+        instance = (aaaaaaa.bbbbbbb().ccccccccccccccccc().ddddddddddd({
+            'aa': 'context!'
+        }).eeeeeeeeeeeeeeeeeee({  # Inline comment about why fnord has the value 6.
+            'fnord': 6
+        }))
         """)
     uwlines = _ParseAndUnwrap(code)
     self.assertCodeEqual(code, reformatter.Reformat(uwlines))
 
   def testB18257115(self):
     code = textwrap.dedent("""\
         if True:
@@ -2313,16 +2378,16 @@
               return aaaa.bbbbbbbbb(ccccccc=dddddddddddddd({('eeee', \
 'ffffffff'): str(j)}))
         """)
     expected_formatted_code = textwrap.dedent("""\
         def f():
           if True:
             if True:
-              return aaaa.bbbbbbbbb(
-                  ccccccc=dddddddddddddd({('eeee', 'ffffffff'): str(j)}))
+              return aaaa.bbbbbbbbb(ccccccc=dddddddddddddd(
+                  {('eeee', 'ffffffff'): str(j)}))
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
   def testB17133019(self):
     unformatted_code = textwrap.dedent("""\
         class aaaaaaaaaaaaaa(object):
@@ -2523,15 +2588,16 @@
   def testB14468247(self):
     unformatted_code = textwrap.dedent("""\
         call(a=1,
             b=2,
         )
         """)
     expected_formatted_code = textwrap.dedent("""\
-        call(a=1, b=2,)
+        call(a=1,
+             b=2,)
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
   def testB14406499(self):
     unformatted_code = textwrap.dedent("""\
         def foo1(parameter_1, parameter_2, parameter_3, parameter_4, \
@@ -2875,14 +2941,35 @@
             if True:
                 keys.append(
                     aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa)  # may be unassigned.
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
+  def testSplittingBeforeFirstArgument(self):
+    try:
+      style.SetGlobalStyle(style.CreateStyleFromConfig(
+          '{based_on_style: pep8, split_before_first_argument: True}'))
+      unformatted_code = textwrap.dedent("""\
+          a_very_long_function_name(long_argument_name_1=1, long_argument_name_2=2,
+                                    long_argument_name_3=3, long_argument_name_4=4)
+          """)
+      expected_formatted_code = textwrap.dedent("""\
+          a_very_long_function_name(
+              long_argument_name_1=1,
+              long_argument_name_2=2,
+              long_argument_name_3=3,
+              long_argument_name_4=4)
+          """)
+      uwlines = _ParseAndUnwrap(unformatted_code)
+      self.assertCodeEqual(expected_formatted_code,
+                           reformatter.Reformat(uwlines))
+    finally:
+      style.SetGlobalStyle(style.CreatePEP8Style())
+
 
 class TestingNotInParameters(unittest.TestCase):
 
   def testNotInParams(self):
     unformatted_code = textwrap.dedent("""\
       list("a long line to break the line. a long line to break the brk a long lin", not True)
       """)
@@ -2922,16 +3009,15 @@
         """)
     expected_formatted_code = textwrap.dedent("""\
         class ABC(metaclass=type):
             pass
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code,
-                         reformatter.Reformat(uwlines,
-                                              verify=False))
+                         reformatter.Reformat(uwlines, verify=False))
 
   def testVerifyFutureImport(self):
     unformatted_code = textwrap.dedent("""\
         from __future__ import print_function
 
         def call_my_function(the_function):
           the_function("hi")
@@ -2952,16 +3038,15 @@
 
 
         if __name__ == "__main__":
             call_my_function(print)
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code,
-                         reformatter.Reformat(uwlines,
-                                              verify=False))
+                         reformatter.Reformat(uwlines, verify=False))
 
   def testContinuationLineShouldBeDistinguished(self):
     unformatted_code = textwrap.dedent("""\
         class Foo(object):
 
             def bar(self):
                 if self.solo_generator_that_is_long is None and len(
@@ -2973,16 +3058,15 @@
             def bar(self):
                 if self.solo_generator_that_is_long is None and len(
                         self.generators + self.next_batch) == 1:
                     pass
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code,
-                         reformatter.Reformat(uwlines,
-                                              verify=False))
+                         reformatter.Reformat(uwlines, verify=False))
 
 
 @unittest.skipUnless(py3compat.PY3, 'Requires Python 3')
 class TestsForPython3Code(ReformatterTest):
   """Test a few constructs that are new Python 3 syntax."""
 
   @classmethod
@@ -3023,14 +3107,15 @@
     if sys.version_info[1] < 5:
       return
     code = textwrap.dedent("""\
         import asyncio
         import time
 
 
+        @print_args
         async def slow_operation():
             await asyncio.sleep(1)
             # print("Slow operation {} complete".format(n))
 
 
         async def main():
             start = time.time()
@@ -3081,16 +3166,15 @@
         def overly_long_function_name(
           first_argument_on_the_same_line,
           second_argument_makes_the_line_too_long):
           pass
         """)
     expected_formatted_code = textwrap.dedent("""\
         def overly_long_function_name(
-            first_argument_on_the_same_line, \
-second_argument_makes_the_line_too_long
+            first_argument_on_the_same_line, second_argument_makes_the_line_too_long
         ):
             pass
         """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
   def testBreakAfterOpeningBracketIfContentsTooBig(self):
@@ -3254,14 +3338,163 @@
                     return cls.single_constraint_not(
                         clues_lists, effect, constraints[0], constraint_manager
                     )
     """)
     uwlines = _ParseAndUnwrap(unformatted_code)
     self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
 
+  def testDedentingCallsWithInnerLists(self):
+    unformatted_code = textwrap.dedent("""\
+    class _():
+        def _():
+            cls.effect_clues = {
+                'effect': Clue((cls.effect_time, 'apache_host'), effect_line, 40)
+            }
+    """)
+    uwlines = _ParseAndUnwrap(unformatted_code)
+    self.assertCodeEqual(unformatted_code, reformatter.Reformat(uwlines))
+
+  def testDedentingListComprehension(self):
+    unformatted_code = textwrap.dedent("""\
+    class Foo():
+        def _pack_results_for_constraint_or():
+            self.param_groups = dict(
+                (
+                    key + 1, ParamGroup(groups[key], default_converter)
+                ) for key in six.moves.range(len(groups))
+            )
+
+            for combination in cls._clues_combinations(clues_lists):
+                if all(
+                    cls._verify_constraint(combination, effect, constraint)
+                    for constraint in constraints
+                ):
+                    pass
+
+            guessed_dict = dict(
+                (
+                    key, guessed_pattern_matches[key]
+                ) for key in six.moves.range(len(guessed_pattern_matches))
+            )
+
+            content = "".join(
+                itertools.chain(
+                    (first_line_fragment, ), lines_between, (last_line_fragment, )
+                )
+            )
+
+            rule = Rule(
+                [self.cause1, self.cause2, self.cause1, self.cause2], self.effect, constraints1,
+                Rule.LINKAGE_AND
+            )
+
+            assert sorted(log_type.files_to_parse) == [
+                ('localhost', os.path.join(path, 'node_1.log'), super_parser),
+                ('localhost', os.path.join(path, 'node_2.log'), super_parser)
+            ]
+    """)
+    expected_formatted_code = textwrap.dedent("""\
+    class Foo():
+        def _pack_results_for_constraint_or():
+            self.param_groups = dict(
+                (key + 1, ParamGroup(groups[key], default_converter))
+                for key in six.moves.range(len(groups))
+            )
+
+            for combination in cls._clues_combinations(clues_lists):
+                if all(
+                    cls._verify_constraint(combination, effect, constraint)
+                    for constraint in constraints
+                ):
+                    pass
+
+            guessed_dict = dict(
+                (key, guessed_pattern_matches[key])
+                for key in six.moves.range(len(guessed_pattern_matches))
+            )
+
+            content = "".join(
+                itertools.chain(
+                    (first_line_fragment, ), lines_between, (last_line_fragment, )
+                )
+            )
+
+            rule = Rule(
+                [self.cause1, self.cause2, self.cause1, self.cause2], self.effect,
+                constraints1, Rule.LINKAGE_AND
+            )
+
+            assert sorted(log_type.files_to_parse) == [
+                ('localhost', os.path.join(path, 'node_1.log'), super_parser),
+                ('localhost', os.path.join(path, 'node_2.log'), super_parser)
+            ]
+    """)
+    uwlines = _ParseAndUnwrap(unformatted_code)
+    self.assertCodeEqual(expected_formatted_code, reformatter.Reformat(uwlines))
+
+  def testMustSplitDedenting(self):
+    unformatted_code = textwrap.dedent("""\
+    class _():
+        def _():
+            effect_line = FrontInput(
+                effect_line_offset, line_content,
+                LineSource('localhost', xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx)
+            )
+    """)
+    uwlines = _ParseAndUnwrap(unformatted_code)
+    self.assertCodeEqual(unformatted_code, reformatter.Reformat(uwlines))
+
+  def testDedentIfConditional(self):
+    unformatted_code = textwrap.dedent("""\
+    class _():
+        def _():
+            if True:
+                if not self.frobbies and (
+                    self.foobars.counters['db.cheeses'] != 1 or
+                    self.foobars.counters['db.marshmellow_skins'] != 1
+                ):
+                    pass
+    """)
+    uwlines = _ParseAndUnwrap(unformatted_code)
+    self.assertCodeEqual(unformatted_code, reformatter.Reformat(uwlines))
+
+  def testDedentSet(self):
+    unformatted_code = textwrap.dedent("""\
+    class _():
+        def _():
+            assert set(self.constraint_links.get_links()) == set(
+                [
+                    (2, 10, 100),
+                    (2, 10, 200),
+                    (2, 20, 100),
+                    (2, 20, 200),
+                ]
+            )
+    """)
+    uwlines = _ParseAndUnwrap(unformatted_code)
+    self.assertCodeEqual(unformatted_code, reformatter.Reformat(uwlines))
+
+  def testDedentingInnerScope(self):
+    code = textwrap.dedent("""\
+        class Foo():
+            @classmethod
+            def _pack_results_for_constraint_or(cls, combination, constraints):
+                return cls._create_investigation_result(
+                    (clue for clue in combination if not clue == Verifier.UNMATCHED),
+                    constraints, InvestigationResult.OR
+                )
+        """)
+    uwlines = _ParseAndUnwrap(code)
+    reformatted_code = reformatter.Reformat(uwlines)
+    self.assertCodeEqual(code, reformatted_code)
+
+    uwlines = _ParseAndUnwrap(reformatted_code)
+    reformatted_code = reformatter.Reformat(uwlines)
+    self.assertCodeEqual(code, reformatted_code)
+
 
 def _ParseAndUnwrap(code, dumptree=False):
   """Produces unwrapped lines from the given code.
 
   Parses the code into a tree, performs comment splicing and runs the
   unwrapper.
```

### Comparing `yapf-0.8.2/yapftests/split_penalty_test.py` & `yapf-0.9.0/yapftests/split_penalty_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -184,26 +184,26 @@
     # Test list comprehension.
     code = textwrap.dedent(r"""
       [a for a in foo if a.x == 37]
       """)
     tree = self._ParseAndComputePenalties(code)
     self._CheckPenalties(tree, [
         ('[', None),
-        ('a', CONTIGUOUS_LIST),
-        ('for', 0),
+        ('a', STRONGLY_CONNECTED),
+        ('for', STRONGLY_CONNECTED),
         ('a', STRONGLY_CONNECTED),
         ('in', STRONGLY_CONNECTED),
         ('foo', STRONGLY_CONNECTED),
-        ('if', 0),
+        ('if', STRONGLY_CONNECTED),
         ('a', STRONGLY_CONNECTED),
         ('.', UNBREAKABLE),
         ('x', DOTTED_NAME),
         ('==', STRONGLY_CONNECTED),
         ('37', STRONGLY_CONNECTED),
-        (']', CONTIGUOUS_LIST),
+        (']', STRONGLY_CONNECTED),
     ])  # yapf: disable
 
   def testFuncCalls(self):
     code = 'foo(1, 2, 3)\n'
     tree = self._ParseAndComputePenalties(code)
     self._CheckPenalties(tree, [
         ('foo', None),
```

### Comparing `yapf-0.8.2/yapftests/style_test.py` & `yapf-0.9.0/yapftests/style_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `yapf-0.8.2/yapftests/subtype_assigner_test.py` & `yapf-0.9.0/yapftests/subtype_assigner_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -53,16 +53,15 @@
     Args:
       uwlines: list of UnwrappedLine.
       list_of_expected: list of (name, subtype) pairs. Non-semantic tokens are
         filtered out from the expected values.
     """
     actual = []
     for uwl in uwlines:
-      filtered_values = [(ft.value, ft.subtypes)
-                         for ft in uwl.tokens
+      filtered_values = [(ft.value, ft.subtypes) for ft in uwl.tokens
                          if ft.name not in pytree_utils.NONSEMANTIC_TOKENS]
       if filtered_values:
         actual.append(filtered_values)
 
     self.assertEqual(list_of_expected, actual)
 
   def testFuncDefDefaultAssign(self):
```

### Comparing `yapf-0.8.2/yapftests/unwrapped_line_test.py` & `yapf-0.9.0/yapftests/unwrapped_line_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,24 +42,24 @@
   def testConstruction(self):
     toks = _MakeFormatTokenList([(token.DOT, '.'), (token.VBAR, '|')])
     uwl = unwrapped_line.UnwrappedLine(20, toks)
     self.assertEqual(20, uwl.depth)
     self.assertEqual(['DOT', 'VBAR'], [tok.name for tok in uwl.tokens])
 
   def testFirstLast(self):
-    toks = _MakeFormatTokenList([(token.DOT, '.'), (token.LPAR, '('), (
-        token.VBAR, '|')])
+    toks = _MakeFormatTokenList([(token.DOT, '.'), (token.LPAR, '('),
+                                 (token.VBAR, '|')])
     uwl = unwrapped_line.UnwrappedLine(20, toks)
     self.assertEqual(20, uwl.depth)
     self.assertEqual('DOT', uwl.first.name)
     self.assertEqual('VBAR', uwl.last.name)
 
   def testAsCode(self):
-    toks = _MakeFormatTokenList([(token.DOT, '.'), (token.LPAR, '('), (
-        token.VBAR, '|')])
+    toks = _MakeFormatTokenList([(token.DOT, '.'), (token.LPAR, '('),
+                                 (token.VBAR, '|')])
     uwl = unwrapped_line.UnwrappedLine(2, toks)
     self.assertEqual('    . ( |', uwl.AsCode())
 
   def testAppendToken(self):
     uwl = unwrapped_line.UnwrappedLine(0)
     uwl.AppendToken(_MakeFormatTokenLeaf(token.LPAR, '('))
     uwl.AppendToken(_MakeFormatTokenLeaf(token.RPAR, ')'))
@@ -79,16 +79,15 @@
     comment_splicer.SpliceComments(tree)
     subtype_assigner.AssignSubtypes(tree)
     split_penalty.ComputeSplitPenalties(tree)
 
     uwlines = pytree_unwrapper.UnwrapPyTree(tree)
     for i, uwline in enumerate(uwlines):
       uwlines[i] = unwrapped_line.UnwrappedLine(
-          uwline.depth, [ft
-                         for ft in uwline.tokens
+          uwline.depth, [ft for ft in uwline.tokens
                          if ft.name not in pytree_utils.NONSEMANTIC_TOKENS])
     return uwlines
 
   def testFuncDef(self):
     code = textwrap.dedent(r'''
       def f(a, b):
         pass
```

### Comparing `yapf-0.8.2/yapftests/yapf_test.py` & `yapf-0.9.0/yapftests/yapf_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2015 Google Inc. All Rights Reserved.
+# Copyright 2015-2016 Google Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -812,15 +812,15 @@
 
         def still_horrible():
             oh_god()
             why_would_you()
             [
                 'do',
 
-                'that',
+                'that'
             ]
         """)
     expected_formatted_code = textwrap.dedent(u"""\
         def horrible():
             oh_god()
             why_would_you()
             [
@@ -828,15 +828,15 @@
 
                 'that',
             ]
 
         def still_horrible():
             oh_god()
             why_would_you()
-            ['do', 'that', ]
+            ['do', 'that']
         """)
     self.assertYapfReformats(unformatted_code,
                              expected_formatted_code,
                              extra_options=['--lines', '14-15'])
 
   def testRetainVerticalFormattingBetweenDisabledAndEnabledLines(self):
     unformatted_code = textwrap.dedent(u"""\
@@ -850,17 +850,17 @@
              gggggggggggg.hhhhhhhhh(c, c.ffffffffffff))
                 iiiii = jjjjjjjjjjjjjj.iiiii
         """)
     expected_formatted_code = textwrap.dedent(u"""\
         class A(object):
             def aaaaaaaaaaaaa(self):
                 c = bbbbbbbbb.ccccccccc('challenge', 0, 1, 10)
-                self.assertEqual(
-                    ('ddddddddddddddddddddddddd', 'eeeeeeeeeeeeeeeeeeeeeeeee.%s' %
-                     c.ffffffffffff), gggggggggggg.hhhhhhhhh(c, c.ffffffffffff))
+                self.assertEqual(('ddddddddddddddddddddddddd',
+                                  'eeeeeeeeeeeeeeeeeeeeeeeee.%s' % c.ffffffffffff),
+                                 gggggggggggg.hhhhhhhhh(c, c.ffffffffffff))
                 iiiii = jjjjjjjjjjjjjj.iiiii
         """)
     self.assertYapfReformats(unformatted_code,
                              expected_formatted_code,
                              extra_options=['--lines', '4-7'])
 
   def testFormatLinesSpecifiedInMiddleOfExpression(self):
@@ -875,17 +875,17 @@
              gggggggggggg.hhhhhhhhh(c, c.ffffffffffff))
                 iiiii = jjjjjjjjjjjjjj.iiiii
         """)
     expected_formatted_code = textwrap.dedent(u"""\
         class A(object):
             def aaaaaaaaaaaaa(self):
                 c = bbbbbbbbb.ccccccccc('challenge', 0, 1, 10)
-                self.assertEqual(
-                    ('ddddddddddddddddddddddddd', 'eeeeeeeeeeeeeeeeeeeeeeeee.%s' %
-                     c.ffffffffffff), gggggggggggg.hhhhhhhhh(c, c.ffffffffffff))
+                self.assertEqual(('ddddddddddddddddddddddddd',
+                                  'eeeeeeeeeeeeeeeeeeeeeeeee.%s' % c.ffffffffffff),
+                                 gggggggggggg.hhhhhhhhh(c, c.ffffffffffff))
                 iiiii = jjjjjjjjjjjjjj.iiiii
         """)
     self.assertYapfReformats(unformatted_code,
                              expected_formatted_code,
                              extra_options=['--lines', '5-6'])
 
   def testCommentFollowingMultilineString(self):
@@ -970,16 +970,16 @@
     expected_formatted_code = textwrap.dedent(u"""\
         def foo():
           def bar():
             return {msg_id: author for author, msg_id in reader}
         """)
     self.assertYapfReformats(unformatted_code,
                              expected_formatted_code,
-                             extra_options=['--lines', '1-1',
-                                            '--style', 'chromium'])
+                             extra_options=['--lines', '1-1', '--style',
+                                            'chromium'])
 
   def testMultilineCommentFormattingDisabled(self):
     unformatted_code = textwrap.dedent(u"""\
         # This is a comment
         FOO = {
             aaaaaaaa.ZZZ: [
                 bbbbbbbbbb.Pop(),
@@ -1004,16 +1004,16 @@
             'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx':
                 ('yyyyy', zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz),
             '#': lambda x: x  # do nothing
         }
         """)
     self.assertYapfReformats(unformatted_code,
                              expected_formatted_code,
-                             extra_options=['--lines', '1-1',
-                                            '--style', 'chromium'])
+                             extra_options=['--lines', '1-1', '--style',
+                                            'chromium'])
 
   def testTrailingCommentsWithDisabledFormatting(self):
     unformatted_code = textwrap.dedent(u"""\
         import os
 
         SCOPES = [
             'hello world'  # This is a comment.
@@ -1024,16 +1024,16 @@
 
         SCOPES = [
             'hello world'  # This is a comment.
         ]
         """)
     self.assertYapfReformats(unformatted_code,
                              expected_formatted_code,
-                             extra_options=['--lines', '1-1',
-                                            '--style', 'chromium'])
+                             extra_options=['--lines', '1-1', '--style',
+                                            'chromium'])
 
 
 class BadInputTest(unittest.TestCase):
   """Test yapf's behaviour when passed bad input."""
 
   def testBadSyntax(self):
     code = '  a = 1\n'
```

