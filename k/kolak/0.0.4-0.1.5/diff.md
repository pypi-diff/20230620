# Comparing `tmp/kolak-0.0.4.tar.gz` & `tmp/kolak-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolak-0.0.4.tar", last modified: Thu Nov 17 06:31:54 2022, max compression
+gzip compressed data, was "kolak-0.1.5.tar", last modified: Tue Jun 20 18:43:06 2023, max compression
```

## Comparing `kolak-0.0.4.tar` & `kolak-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 06:31:54.202902 kolak-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1521 2022-11-17 06:31:54.202902 kolak-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1254 2022-11-17 06:31:43.000000 kolak-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 06:31:54.200902 kolak-0.0.4/kolak/
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-11-17 06:31:53.000000 kolak-0.0.4/kolak/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11820 2022-11-17 06:31:53.000000 kolak-0.0.4/kolak/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2022-11-17 06:31:53.000000 kolak-0.0.4/kolak/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 06:31:54.201902 kolak-0.0.4/kolak.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1521 2022-11-17 06:31:54.000000 kolak-0.0.4/kolak.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-11-17 06:31:54.000000 kolak-0.0.4/kolak.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-17 06:31:54.000000 kolak-0.0.4/kolak.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-11-17 06:31:54.000000 kolak-0.0.4/kolak.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-17 06:31:54.202902 kolak-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      615 2022-11-17 06:31:53.000000 kolak-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 18:43:06.933394 kolak-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-06-20 18:43:06.932394 kolak-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2023-06-20 18:42:57.000000 kolak-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 18:43:06.931394 kolak-0.1.5/kolak/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12997 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3448 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 18:43:06.932394 kolak-0.1.5/kolak.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-20 18:43:06.000000 kolak-0.1.5/kolak.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 18:43:06.933394 kolak-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-06-20 18:43:06.000000 kolak-0.1.5/setup.py
```

### Comparing `kolak-0.0.4/PKG-INFO` & `kolak-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: kolak
-Version: 0.0.4
-Summary: universal rss parser with AI
-Home-page: https://github.com/guangrei/Kolak
+Version: 0.1.5
+Summary: universal rss parser
+Home-page: https://gitlab.com/guangrei/Kolak
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: rss feed parser podcast xml
 Description-Content-Type: text/markdown
 
-Universal RSS Parser with AI.
+Universal RSS Parser.
 
 extra features:
 
 - work with any rss and atom feed format.
 - smart cache
 - multiple rss support
 - parallel parser
-- parse podcast
+- parse rss podcast.
 
 ## Installation
 
 ```
 pip install kolak
 ```
```

### Comparing `kolak-0.0.4/README.md` & `kolak-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Universal RSS Parser with AI.
+Universal RSS Parser.
 
 extra features:
 
 - work with any rss and atom feed format.
 - smart cache
 - multiple rss support
 - parallel parser
-- parse podcast
+- parse rss podcast.
 
 ## Installation
 
 ```
 pip install kolak
 ```
```

### Comparing `kolak-0.0.4/kolak/parser.py` & `kolak-0.1.5/kolak/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,45 @@
 # -*-coding:utf8;-*-
+"""
+The MIT License (MIT)
+
+Copyright (c) 2023 kolak https://pypi.org/project/kolak
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+"""
+
 import re
 import os
 import sys
 from zcache import Cache
 from urllib import parse
 from .util import util
 from multiprocessing import Process, Queue
 
 
 class Parser(object):
 
     def __init__(self, uri, cache_time=600):
+        self.isValid = False
         self.title = ""
         self.description = ""
         self.permalink = ""
         self.updated = ""
         self.author = ""
         self.items = []
         cache = Cache()
@@ -102,14 +127,15 @@
         models.append(re.compile('<item.*?>(.*?)<\/item>', re.S))
         models.append(re.compile('<entry.*?>(.*?)<\/entry>', re.S))
         for model in models:
 
             mytry = model.findall(txml)
             if len(mytry) != 0:
                 self.__matcItems = model
+                self.isValid = True
                 return mytry
             else:
                 pass
         if self.__debug:
             util.log_file(
                 self.__log_path, "parse_items: no model is matching!\n---\n%s" % txml, "critical")
         return []
```

### Comparing `kolak-0.0.4/kolak.egg-info/PKG-INFO` & `kolak-0.1.5/kolak.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: kolak
-Version: 0.0.4
-Summary: universal rss parser with AI
-Home-page: https://github.com/guangrei/Kolak
+Version: 0.1.5
+Summary: universal rss parser
+Home-page: https://gitlab.com/guangrei/Kolak
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: rss feed parser podcast xml
 Description-Content-Type: text/markdown
 
-Universal RSS Parser with AI.
+Universal RSS Parser.
 
 extra features:
 
 - work with any rss and atom feed format.
 - smart cache
 - multiple rss support
 - parallel parser
-- parse podcast
+- parse rss podcast.
 
 ## Installation
 
 ```
 pip install kolak
 ```
```

