# Comparing `tmp/maxgradient-0.1.0.tar.gz` & `tmp/maxgradient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxgradient-0.1.0.tar", last modified: Mon Jun 19 04:10:43 2023, max compression
+gzip compressed data, was "maxgradient-0.1.1.tar", last modified: Tue Jun 20 03:48:40 2023, max compression
```

## Comparing `maxgradient-0.1.0.tar` & `maxgradient-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1066 2023-05-20 01:18:06.237490 maxgradient-0.1.0/LICENSE
--rw-r--r--   0        0        0       13 2023-05-20 01:18:06.237623 maxgradient-0.1.0/README.md
--rw-r--r--   0        0        0      750 2023-06-17 03:14:06.061956 maxgradient-0.1.0/maxgradient/__init__.py
--rw-r--r--   0        0        0    10879 2023-06-18 19:16:19.295760 maxgradient-0.1.0/maxgradient/_gradient_substring.py
--rw-r--r--   0        0        0     1886 2023-06-14 20:46:22.513323 maxgradient-0.1.0/maxgradient/_mode.py
--rw-r--r--   0        0        0    16154 2023-06-16 21:20:44.170100 maxgradient-0.1.0/maxgradient/_rich.py
--rw-r--r--   0        0        0    12225 2023-06-16 21:17:22.440850 maxgradient-0.1.0/maxgradient/_x11.py
--rw-r--r--   0        0        0     2395 2023-06-19 03:17:45.252021 maxgradient-0.1.0/maxgradient/cli.py
--rw-r--r--   0        0        0    19133 2023-06-19 01:34:58.510343 maxgradient-0.1.0/maxgradient/color.py
--rw-r--r--   0        0        0     3294 2023-06-16 21:20:58.780049 maxgradient-0.1.0/maxgradient/color_list.py
--rw-r--r--   0        0        0    10462 2023-06-19 00:24:10.378696 maxgradient-0.1.0/maxgradient/console.py
--rw-r--r--   0        0        0    30263 2023-06-16 16:09:50.267902 maxgradient-0.1.0/maxgradient/default_styles.py
--rw-r--r--   0        0        0    20228 2023-06-19 03:17:18.349630 maxgradient-0.1.0/maxgradient/gradient.py
--rw-r--r--   0        0        0    13231 2023-06-18 15:30:08.337049 maxgradient-0.1.0/maxgradient/log.py
--rw-r--r--   0        0        0     2649 2023-06-18 18:22:16.438034 maxgradient-0.1.0/maxgradient/theme.py
--rw-r--r--   0        0        0      856 2023-06-19 04:10:43.315036 maxgradient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 maxgradient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-20 01:18:06.237490 maxgradient-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4054 2023-06-20 03:46:31.450409 maxgradient-0.1.1/README.md
+-rw-r--r--   0        0        0      735 2023-06-19 17:15:40.456613 maxgradient-0.1.1/maxgradient/__init__.py
+-rw-r--r--   0        0        0    10879 2023-06-18 19:16:19.295760 maxgradient-0.1.1/maxgradient/_gradient_substring.py
+-rw-r--r--   0        0        0     1886 2023-06-14 20:46:22.513323 maxgradient-0.1.1/maxgradient/_mode.py
+-rw-r--r--   0        0        0    16154 2023-06-16 21:20:44.170100 maxgradient-0.1.1/maxgradient/_rich.py
+-rw-r--r--   0        0        0    12225 2023-06-16 21:17:22.440850 maxgradient-0.1.1/maxgradient/_x11.py
+-rw-r--r--   0        0        0     2395 2023-06-20 03:47:24.996801 maxgradient-0.1.1/maxgradient/cli.py
+-rw-r--r--   0        0        0    19133 2023-06-19 01:34:58.510343 maxgradient-0.1.1/maxgradient/color.py
+-rw-r--r--   0        0        0     3294 2023-06-16 21:20:58.780049 maxgradient-0.1.1/maxgradient/color_list.py
+-rw-r--r--   0        0        0    10462 2023-06-19 00:24:10.378696 maxgradient-0.1.1/maxgradient/console.py
+-rw-r--r--   0        0        0    30263 2023-06-16 16:09:50.267902 maxgradient-0.1.1/maxgradient/default_styles.py
+-rw-r--r--   0        0        0    20228 2023-06-19 03:17:18.349630 maxgradient-0.1.1/maxgradient/gradient.py
+-rw-r--r--   0        0        0    13231 2023-06-18 15:30:08.337049 maxgradient-0.1.1/maxgradient/log.py
+-rw-r--r--   0        0        0     1473 2023-06-19 17:26:36.354259 maxgradient-0.1.1/maxgradient/logs/debug.log
+-rw-r--r--   0        0        0       87 2023-06-19 17:26:36.354163 maxgradient-0.1.1/maxgradient/logs/info.log
+-rw-r--r--   0        0        0     2649 2023-06-18 18:22:16.438034 maxgradient-0.1.1/maxgradient/theme.py
+-rw-r--r--   0        0        0      856 2023-06-20 03:48:40.128596 maxgradient-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-06-20 02:00:32.188634 maxgradient-0.1.1/tests/_x11_tests.py
+-rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 maxgradient-0.1.1/PKG-INFO
```

### Comparing `maxgradient-0.1.0/LICENSE` & `maxgradient-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/__init__.py` & `maxgradient-0.1.1/maxgradient/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """MaxGradient is a Python library for styling and coloring terminal text with gradient color.\
     It is built on top of Rich, and is designed to work seamlessly with it.\
     It is a global singleton class that can be imported and used anywhere in the project and \
     used as a drop in replacement for [italic bold #00ffff]rich.console.Console[/].
     """
+# pylint: disable=W0604
 from maxgradient.color import Color
+from maxgradient.console import Console
 from maxgradient.gradient import Gradient
-
-# pylint: disable=W0604
 from maxgradient.log import Log, LogConsole
 
-# from maxgradient.console import Console
 
 __all__ = [
     "_gradient_substring",
     "_mode",
     "_rich",
     "_x11",
     "color_list",
     "color",
     "console",
     "default_styles",
     "gradient",
     "log",
-    "panel",
-    "theme"
+    "theme",
 ]
```

### Comparing `maxgradient-0.1.0/maxgradient/_gradient_substring.py` & `maxgradient-0.1.1/maxgradient/_gradient_substring.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/_mode.py` & `maxgradient-0.1.1/maxgradient/_mode.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/_rich.py` & `maxgradient-0.1.1/maxgradient/_rich.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/_x11.py` & `maxgradient-0.1.1/maxgradient/_x11.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/cli.py` & `maxgradient-0.1.1/maxgradient/cli.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/color.py` & `maxgradient-0.1.1/maxgradient/color.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/color_list.py` & `maxgradient-0.1.1/maxgradient/color_list.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/console.py` & `maxgradient-0.1.1/maxgradient/console.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/default_styles.py` & `maxgradient-0.1.1/maxgradient/default_styles.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/gradient.py` & `maxgradient-0.1.1/maxgradient/gradient.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/log.py` & `maxgradient-0.1.1/maxgradient/log.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/maxgradient/theme.py` & `maxgradient-0.1.1/maxgradient/theme.py`

 * *Files identical despite different names*

### Comparing `maxgradient-0.1.0/pyproject.toml` & `maxgradient-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "MaxGradient"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library to make printing gradient color to the terminal a lot easier. Think `lolcat` but utilizing python's `rich` library so you can use it anywhere."
 authors = [
     { name = "maxludden", email = "dev@maxludden.com" },
 ]
 dependencies = [
     "rich>=13.3.5",
     "lorem-text>=2.1",
```

