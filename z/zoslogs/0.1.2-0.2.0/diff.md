# Comparing `tmp/zoslogs-0.1.2.tar.gz` & `tmp/zoslogs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kdm/src/zoslogs/dist/tmpou7ug8xn/zoslogs-0.1.2.tar", last modified: Tue Mar 29 19:10:57 2022, max compression
+gzip compressed data, was "zoslogs-0.2.0.tar", last modified: Tue Jun 20 20:05:14 2023, max compression
```

## Comparing `zoslogs-0.1.2.tar` & `zoslogs-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 kdm        (501) staff       (20)        0 2022-03-29 19:10:57.000000 zoslogs-0.1.2/
--rw-r--r--   0 kdm        (501) staff       (20)     2605 2022-03-29 19:10:57.000000 zoslogs-0.1.2/PKG-INFO
--rw-r--r--   0 kdm        (501) staff       (20)      575 2022-03-04 19:04:14.000000 zoslogs-0.1.2/LICENSE
--rw-r--r--   0 kdm        (501) staff       (20)     3452 2022-03-29 18:38:31.000000 zoslogs-0.1.2/CONTRIBUTING.rst
-drwxr-xr-x   0 kdm        (501) staff       (20)        0 2022-03-29 19:10:57.000000 zoslogs-0.1.2/tests/
--rw-r--r--   0 kdm        (501) staff       (20)      739 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_utils.py
--rw-r--r--   0 kdm        (501) staff       (20)     9459 2022-03-17 14:47:39.000000 zoslogs-0.1.2/tests/test_zoslogs.py
-drwxr-xr-x   0 kdm        (501) staff       (20)        0 2022-03-29 19:10:57.000000 zoslogs-0.1.2/tests/test_data/
--rw-r--r--   0 kdm        (501) staff       (20)     4569 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/multiple_messages.txt
--rw-r--r--   0 kdm        (501) staff       (20)     2197 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/multi_line_with_no_message_header.txt
--rw-r--r--   0 kdm        (501) staff       (20)      276 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/multi_line_with_continuation.txt
--rw-r--r--   0 kdm        (501) staff       (20)     2095 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/multi_line_no_messagenum.txt
--rw-r--r--   0 kdm        (501) staff       (20)       96 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/syslog_initialization_message.txt
--rw-r--r--   0 kdm        (501) staff       (20)     2099 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/multi_line.txt
--rw-r--r--   0 kdm        (501) staff       (20)     2159 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/multi_line_response_IEE932I.txt
--rw-r--r--   0 kdm        (501) staff       (20)       73 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/single_line_internal.txt
--rw-r--r--   0 kdm        (501) staff       (20)      206 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/single_line_with_continuation.txt
--rw-r--r--   0 kdm        (501) staff       (20)       55 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/empty_multi_line.txt
--rw-r--r--   0 kdm        (501) staff       (20)       81 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/single_line_command.txt
--rw-r--r--   0 kdm        (501) staff       (20)       55 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/empty_line.txt
--rw-r--r--   0 kdm        (501) staff       (20)       82 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/new_syslog_page.txt
--rw-r--r--   0 kdm        (501) staff       (20)      121 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_data/single_line_message.txt
--rw-r--r--   0 kdm        (501) staff       (20)       37 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/__init__.py
--rw-r--r--   0 kdm        (501) staff       (20)     8689 2022-03-04 19:04:14.000000 zoslogs-0.1.2/tests/test_zosmessage.py
--rw-r--r--   0 kdm        (501) staff       (20)      262 2022-03-04 19:04:14.000000 zoslogs-0.1.2/MANIFEST.in
-drwxr-xr-x   0 kdm        (501) staff       (20)        0 2022-03-29 19:10:57.000000 zoslogs-0.1.2/docs/
--rw-r--r--   0 kdm        (501) staff       (20)      304 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/index.rst
--rw-r--r--   0 kdm        (501) staff       (20)       33 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/contributing.rst
--rw-r--r--   0 kdm        (501) staff       (20)      608 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/Makefile
--rwxr-xr-x   0 kdm        (501) staff       (20)     4793 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/conf.py
--rw-r--r--   0 kdm        (501) staff       (20)       69 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/usage.rst
--rw-r--r--   0 kdm        (501) staff       (20)      769 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/make.bat
--rw-r--r--   0 kdm        (501) staff       (20)       28 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/history.rst
--rw-r--r--   0 kdm        (501) staff       (20)     1110 2022-03-21 18:30:54.000000 zoslogs-0.1.2/docs/installation.rst
--rw-r--r--   0 kdm        (501) staff       (20)       28 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/authors.rst
--rw-r--r--   0 kdm        (501) staff       (20)       27 2022-03-04 19:04:14.000000 zoslogs-0.1.2/docs/readme.rst
--rw-r--r--   0 kdm        (501) staff       (20)     1996 2022-03-29 19:10:20.000000 zoslogs-0.1.2/setup.py
--rw-r--r--   0 kdm        (501) staff       (20)      159 2022-03-29 18:40:27.000000 zoslogs-0.1.2/HISTORY.rst
--rw-r--r--   0 kdm        (501) staff       (20)      159 2022-03-04 19:04:14.000000 zoslogs-0.1.2/AUTHORS.rst
--rw-r--r--   0 kdm        (501) staff       (20)      463 2022-03-29 19:10:57.000000 zoslogs-0.1.2/setup.cfg
--rw-r--r--   0 kdm        (501) staff       (20)     1576 2022-03-29 18:38:31.000000 zoslogs-0.1.2/README.rst
-drwxr-xr-x   0 kdm        (501) staff       (20)        0 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/
--rw-r--r--   0 kdm        (501) staff       (20)        0 2022-03-04 19:04:14.000000 zoslogs-0.1.2/src/__init__.py
-drwxr-xr-x   0 kdm        (501) staff       (20)        0 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs.egg-info/
--rw-r--r--   0 kdm        (501) staff       (20)     2605 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs.egg-info/PKG-INFO
--rw-r--r--   0 kdm        (501) staff       (20)        1 2022-03-03 20:49:29.000000 zoslogs-0.1.2/src/zoslogs.egg-info/not-zip-safe
--rw-r--r--   0 kdm        (501) staff       (20)     1286 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs.egg-info/SOURCES.txt
--rw-r--r--   0 kdm        (501) staff       (20)       53 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs.egg-info/entry_points.txt
--rw-r--r--   0 kdm        (501) staff       (20)        5 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs.egg-info/requires.txt
--rw-r--r--   0 kdm        (501) staff       (20)       17 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs.egg-info/top_level.txt
--rw-r--r--   0 kdm        (501) staff       (20)        1 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs.egg-info/dependency_links.txt
-drwxr-xr-x   0 kdm        (501) staff       (20)        0 2022-03-29 19:10:57.000000 zoslogs-0.1.2/src/zoslogs/
--rw-r--r--   0 kdm        (501) staff       (20)     6973 2022-03-17 14:47:39.000000 zoslogs-0.1.2/src/zoslogs/zoslogs.py
--rw-r--r--   0 kdm        (501) staff       (20)      128 2022-03-29 19:10:20.000000 zoslogs-0.1.2/src/zoslogs/__init__.py
--rw-r--r--   0 kdm        (501) staff       (20)      546 2022-03-04 19:04:14.000000 zoslogs-0.1.2/src/zoslogs/utils.py
--rw-r--r--   0 kdm        (501) staff       (20)     4132 2022-03-04 19:04:14.000000 zoslogs-0.1.2/src/zoslogs/zosmessage.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-20 20:05:14.852385 zoslogs-0.2.0/
+-rw-r--r--   0 kdm        (501) staff       (20)      159 2022-03-04 19:04:14.000000 zoslogs-0.2.0/AUTHORS.rst
+-rw-r--r--   0 kdm        (501) staff       (20)     3456 2022-04-21 18:18:13.000000 zoslogs-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      371 2022-04-20 15:41:19.000000 zoslogs-0.2.0/HISTORY.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      575 2022-03-04 19:04:14.000000 zoslogs-0.2.0/LICENSE
+-rw-r--r--   0 kdm        (501) staff       (20)      262 2022-03-04 19:04:14.000000 zoslogs-0.2.0/MANIFEST.in
+-rw-r--r--   0 kdm        (501) staff       (20)     2797 2023-06-20 20:05:14.852476 zoslogs-0.2.0/PKG-INFO
+-rw-r--r--   0 kdm        (501) staff       (20)     1576 2022-03-29 18:38:31.000000 zoslogs-0.2.0/README.rst
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-20 20:05:14.845018 zoslogs-0.2.0/docs/
+-rw-r--r--   0 kdm        (501) staff       (20)      608 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/Makefile
+-rw-r--r--   0 kdm        (501) staff       (20)       28 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 kdm        (501) staff       (20)     4793 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/conf.py
+-rw-r--r--   0 kdm        (501) staff       (20)       33 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/contributing.rst
+-rw-r--r--   0 kdm        (501) staff       (20)       28 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/history.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      304 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/index.rst
+-rw-r--r--   0 kdm        (501) staff       (20)     1110 2022-03-21 18:30:54.000000 zoslogs-0.2.0/docs/installation.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      769 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/make.bat
+-rw-r--r--   0 kdm        (501) staff       (20)       27 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/readme.rst
+-rw-r--r--   0 kdm        (501) staff       (20)       69 2022-03-04 19:04:14.000000 zoslogs-0.2.0/docs/usage.rst
+-rw-r--r--   0 kdm        (501) staff       (20)      463 2023-06-20 20:05:14.852818 zoslogs-0.2.0/setup.cfg
+-rw-r--r--   0 kdm        (501) staff       (20)     1996 2023-06-20 19:55:08.000000 zoslogs-0.2.0/setup.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-20 20:05:14.845218 zoslogs-0.2.0/src/
+-rw-r--r--   0 kdm        (501) staff       (20)        0 2022-03-04 19:04:14.000000 zoslogs-0.2.0/src/__init__.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-20 20:05:14.846255 zoslogs-0.2.0/src/zoslogs/
+-rw-r--r--   0 kdm        (501) staff       (20)      128 2023-06-20 19:55:08.000000 zoslogs-0.2.0/src/zoslogs/__init__.py
+-rw-r--r--   0 kdm        (501) staff       (20)      546 2022-03-04 19:04:14.000000 zoslogs-0.2.0/src/zoslogs/utils.py
+-rw-r--r--   0 kdm        (501) staff       (20)     6973 2022-03-17 14:47:39.000000 zoslogs-0.2.0/src/zoslogs/zoslogs.py
+-rw-r--r--   0 kdm        (501) staff       (20)     4132 2022-03-04 19:04:14.000000 zoslogs-0.2.0/src/zoslogs/zosmessage.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-20 20:05:14.847717 zoslogs-0.2.0/src/zoslogs.egg-info/
+-rw-r--r--   0 kdm        (501) staff       (20)     2797 2023-06-20 20:05:14.000000 zoslogs-0.2.0/src/zoslogs.egg-info/PKG-INFO
+-rw-r--r--   0 kdm        (501) staff       (20)     1286 2023-06-20 20:05:14.000000 zoslogs-0.2.0/src/zoslogs.egg-info/SOURCES.txt
+-rw-r--r--   0 kdm        (501) staff       (20)        1 2023-06-20 20:05:14.000000 zoslogs-0.2.0/src/zoslogs.egg-info/dependency_links.txt
+-rw-r--r--   0 kdm        (501) staff       (20)       52 2023-06-20 20:05:14.000000 zoslogs-0.2.0/src/zoslogs.egg-info/entry_points.txt
+-rw-r--r--   0 kdm        (501) staff       (20)        1 2022-03-03 20:49:29.000000 zoslogs-0.2.0/src/zoslogs.egg-info/not-zip-safe
+-rw-r--r--   0 kdm        (501) staff       (20)        5 2023-06-20 20:05:14.000000 zoslogs-0.2.0/src/zoslogs.egg-info/requires.txt
+-rw-r--r--   0 kdm        (501) staff       (20)       17 2023-06-20 20:05:14.000000 zoslogs-0.2.0/src/zoslogs.egg-info/top_level.txt
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-20 20:05:14.848508 zoslogs-0.2.0/tests/
+-rw-r--r--   0 kdm        (501) staff       (20)       37 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/__init__.py
+drwxr-xr-x   0 kdm        (501) staff       (20)        0 2023-06-20 20:05:14.852205 zoslogs-0.2.0/tests/test_data/
+-rw-r--r--   0 kdm        (501) staff       (20)       55 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/empty_line.txt
+-rw-r--r--   0 kdm        (501) staff       (20)       55 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/empty_multi_line.txt
+-rw-r--r--   0 kdm        (501) staff       (20)     2099 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/multi_line.txt
+-rw-r--r--   0 kdm        (501) staff       (20)     2095 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/multi_line_no_messagenum.txt
+-rw-r--r--   0 kdm        (501) staff       (20)     2159 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/multi_line_response_IEE932I.txt
+-rw-r--r--   0 kdm        (501) staff       (20)      276 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/multi_line_with_continuation.txt
+-rw-r--r--   0 kdm        (501) staff       (20)     2197 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/multi_line_with_no_message_header.txt
+-rw-r--r--   0 kdm        (501) staff       (20)     4569 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/multiple_messages.txt
+-rw-r--r--   0 kdm        (501) staff       (20)       82 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/new_syslog_page.txt
+-rw-r--r--   0 kdm        (501) staff       (20)       81 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/single_line_command.txt
+-rw-r--r--   0 kdm        (501) staff       (20)       73 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/single_line_internal.txt
+-rw-r--r--   0 kdm        (501) staff       (20)      121 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/single_line_message.txt
+-rw-r--r--   0 kdm        (501) staff       (20)      206 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/single_line_with_continuation.txt
+-rw-r--r--   0 kdm        (501) staff       (20)       96 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_data/syslog_initialization_message.txt
+-rw-r--r--   0 kdm        (501) staff       (20)      739 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_utils.py
+-rw-r--r--   0 kdm        (501) staff       (20)     9459 2022-03-17 14:47:39.000000 zoslogs-0.2.0/tests/test_zoslogs.py
+-rw-r--r--   0 kdm        (501) staff       (20)     8689 2022-03-04 19:04:14.000000 zoslogs-0.2.0/tests/test_zosmessage.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zoslogs-0.1.2/PKG-INFO` & `zoslogs-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: zoslogs
-Version: 0.1.2
+Version: 0.2.0
 Summary: Library for breaking z/OS log files up into individual messages
 Home-page: https://github.com/Tam-Lin/zoslogs
 Author: Kevin McKenzie
 Author-email: kmckenzi@us.ibm.com
 License: Apache Software License 2.0
 Keywords: zoslogs
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -73,19 +72,27 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.1.1 (2022-03-04)
+0.1.3 (2022-0x-04)
+------------------
+
+* Include history update for version 0.1.2, and other cleanup to doc
+
+0.1.2 (2022-03-29)
+------------------
+
+* Point source code location in setup.py to the correct place.
+
+0.1.1 (2022-03-29)
 ------------------
 
 * Move CI to Github actions.
 
 
 0.1.0 (2022-03-04)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `zoslogs-0.1.2/LICENSE` & `zoslogs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/CONTRIBUTING.rst` & `zoslogs-0.2.0/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/kmckenzi/zoslogs/issues.
+Report bugs at https://github.com/Tam-Lin/zoslogs/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -41,15 +41,15 @@
 zoslogs could always use more documentation, whether as part of the
 official zoslogs docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/kmckenzi/zoslogs/issues.
+The best way to send feedback is to file an issue at https://github.com/Tam-Lin/zoslogs/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -99,15 +99,15 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
 3. The pull request should work for Python 3.6, 3.7, 3.8, 3.9 and 3.10. Check
-   https://travis-ci.com/kmckenzi/zoslogs/pull_requests
+   https://github.com/Tam-Lin/zoslogs/workflows/check_pr.yaml
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `zoslogs-0.1.2/tests/test_utils.py` & `zoslogs-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/tests/test_zoslogs.py` & `zoslogs-0.2.0/tests/test_zoslogs.py`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/tests/test_data/multiple_messages.txt` & `zoslogs-0.2.0/tests/test_data/multiple_messages.txt`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/tests/test_data/multi_line_with_no_message_header.txt` & `zoslogs-0.2.0/tests/test_data/multi_line_with_no_message_header.txt`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/tests/test_data/multi_line_no_messagenum.txt` & `zoslogs-0.2.0/tests/test_data/multi_line_no_messagenum.txt`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/tests/test_data/multi_line.txt` & `zoslogs-0.2.0/tests/test_data/multi_line.txt`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/tests/test_data/multi_line_response_IEE932I.txt` & `zoslogs-0.2.0/tests/test_data/multi_line_response_IEE932I.txt`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/tests/test_zosmessage.py` & `zoslogs-0.2.0/tests/test_zosmessage.py`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/docs/Makefile` & `zoslogs-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/docs/conf.py` & `zoslogs-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/docs/make.bat` & `zoslogs-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/docs/installation.rst` & `zoslogs-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/setup.py` & `zoslogs-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,10 +63,10 @@
     name='zoslogs',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Tam-Lin/zoslogs',
-    version='0.1.2',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `zoslogs-0.1.2/README.rst` & `zoslogs-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/src/zoslogs.egg-info/PKG-INFO` & `zoslogs-0.2.0/src/zoslogs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: zoslogs
-Version: 0.1.2
+Version: 0.2.0
 Summary: Library for breaking z/OS log files up into individual messages
 Home-page: https://github.com/Tam-Lin/zoslogs
 Author: Kevin McKenzie
 Author-email: kmckenzi@us.ibm.com
 License: Apache Software License 2.0
 Keywords: zoslogs
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -73,19 +72,27 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
-0.1.1 (2022-03-04)
+0.1.3 (2022-0x-04)
+------------------
+
+* Include history update for version 0.1.2, and other cleanup to doc
+
+0.1.2 (2022-03-29)
+------------------
+
+* Point source code location in setup.py to the correct place.
+
+0.1.1 (2022-03-29)
 ------------------
 
 * Move CI to Github actions.
 
 
 0.1.0 (2022-03-04)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `zoslogs-0.1.2/src/zoslogs.egg-info/SOURCES.txt` & `zoslogs-0.2.0/src/zoslogs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/src/zoslogs/zoslogs.py` & `zoslogs-0.2.0/src/zoslogs/zoslogs.py`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/src/zoslogs/utils.py` & `zoslogs-0.2.0/src/zoslogs/utils.py`

 * *Files identical despite different names*

### Comparing `zoslogs-0.1.2/src/zoslogs/zosmessage.py` & `zoslogs-0.2.0/src/zoslogs/zosmessage.py`

 * *Files identical despite different names*

