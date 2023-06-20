# Comparing `tmp/mypy-boto3-redshift-1.26.64.tar.gz` & `tmp/mypy-boto3-redshift-1.26.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-1.26.64.tar", last modified: Fri Feb  3 22:25:46 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
```

## Comparing `mypy-boto3-redshift-1.26.64.tar` & `mypy-boto3-redshift-1.26.79.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 22:25:46.271990 mypy-boto3-redshift-1.26.64/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-02-03 22:25:46.271990 mypy-boto3-redshift-1.26.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34736 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 22:25:46.271990 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   112008 2023-02-03 22:25:34.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   111846 2023-02-03 22:25:34.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-02-03 22:25:35.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-02-03 22:25:35.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42229 2023-02-03 22:25:34.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    42195 2023-02-03 22:25:34.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   130787 2023-02-03 22:25:37.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   130668 2023-02-03 22:25:36.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-02-03 22:25:34.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-02-03 22:25:34.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 22:25:46.271990 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-02-03 22:25:46.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-03 22:25:46.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 22:25:46.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 22:25:46.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-03 22:25:46.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-03 22:25:46.000000 mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 22:25:46.275990 mypy-boto3-redshift-1.26.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-03 22:25:33.000000 mypy-boto3-redshift-1.26.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34736 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112008 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111846 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-02-24 21:22:13.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42229 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42195 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   130787 2023-02-24 21:22:17.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130668 2023-02-24 21:22:15.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-02-24 21:22:12.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-24 21:22:49.000000 mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.737199 mypy-boto3-redshift-1.26.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-24 21:22:10.000000 mypy-boto3-redshift-1.26.79/setup.py
```

### Comparing `mypy-boto3-redshift-1.26.64/LICENSE` & `mypy-boto3-redshift-1.26.79/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/PKG-INFO` & `mypy-boto3-redshift-1.26.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.26.64
-Summary: Type annotations for boto3.Redshift 1.26.64 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.79
+Summary: Type annotations for boto3.Redshift 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.26.64](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-1.26.64/README.md` & `mypy-boto3-redshift-1.26.79/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.26.64](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/__init__.py` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/__init__.pyi` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/__main__.py` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Redshift 1.26.64\nVersion:         1.26.64\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Redshift 1.26.79\nVersion:         1.26.79\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.64")
+    print("1.26.79")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/client.py` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/client.pyi` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/literals.py` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,14 +494,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/literals.pyi` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -492,14 +492,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/paginator.py` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/paginator.pyi` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/type_defs.py` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/type_defs.pyi` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/waiter.py` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift/waiter.pyi` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/PKG-INFO` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.26.64
-Summary: Type annotations for boto3.Redshift 1.26.64 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.79
+Summary: Type annotations for boto3.Redshift 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.26.64](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-1.26.64/mypy_boto3_redshift.egg-info/SOURCES.txt` & `mypy-boto3-redshift-1.26.79/mypy_boto3_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.26.64/setup.py` & `mypy-boto3-redshift-1.26.79/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-redshift",
-    version="1.26.64",
+    version="1.26.79",
     packages=["mypy_boto3_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Redshift 1.26.64 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.Redshift 1.26.79 service generated with mypy-boto3-builder"
+        " 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

