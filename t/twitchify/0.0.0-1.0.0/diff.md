# Comparing `tmp/twitchify-0.0.0.tar.gz` & `tmp/twitchify-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-0.0.0.tar", last modified: Fri Jun  9 12:59:24 2023, max compression
+gzip compressed data, was "twitchify-1.0.0.tar", last modified: Tue Jun 20 16:49:16 2023, max compression
```

## Comparing `twitchify-0.0.0.tar` & `twitchify-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 12:59:24.492510 twitchify-0.0.0/
--rw-rw-rw-   0        0        0      202 2023-06-09 12:59:24.491511 twitchify-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 12:59:24.492510 twitchify-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-06-09 12:53:04.000000 twitchify-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:59:24.475521 twitchify-0.0.0/twitch/
--rw-rw-rw-   0        0        0     1247 2023-06-09 12:35:49.000000 twitchify-0.0.0/twitch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 12:59:24.490514 twitchify-0.0.0/twitchify.egg-info/
--rw-rw-rw-   0        0        0      202 2023-06-09 12:59:24.000000 twitchify-0.0.0/twitchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-06-09 12:59:24.000000 twitchify-0.0.0/twitchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 12:59:24.000000 twitchify-0.0.0/twitchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 12:59:24.000000 twitchify-0.0.0/twitchify.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 16:49:16.239256 twitchify-1.0.0/
+-rw-rw-rw-   0        0        0      260 2023-06-20 16:49:16.238256 twitchify-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-06-20 16:26:45.000000 twitchify-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:49:16.239256 twitchify-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-06-20 16:37:33.000000 twitchify-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:49:16.167300 twitchify-1.0.0/twitch/
+-rw-rw-rw-   0        0        0     1328 2023-06-20 15:33:19.000000 twitchify-1.0.0/twitch/__init__.py
+-rw-rw-rw-   0        0        0     5241 2023-06-20 15:29:57.000000 twitchify-1.0.0/twitch/channel.py
+-rw-rw-rw-   0        0        0     7468 2023-06-20 15:19:57.000000 twitchify-1.0.0/twitch/client.py
+-rw-rw-rw-   0        0        0     3352 2023-06-20 15:24:23.000000 twitchify-1.0.0/twitch/errors.py
+-rw-rw-rw-   0        0        0    11170 2023-06-20 15:27:41.000000 twitchify-1.0.0/twitch/gateway.py
+-rw-rw-rw-   0        0        0     7491 2023-06-20 00:35:39.000000 twitchify-1.0.0/twitch/goals.py
+-rw-rw-rw-   0        0        0    15095 2023-06-20 15:27:41.000000 twitchify-1.0.0/twitch/http.py
+-rw-rw-rw-   0        0        0     2171 2023-06-20 00:12:07.000000 twitchify-1.0.0/twitch/message.py
+-rw-rw-rw-   0        0        0     3729 2023-06-20 00:35:40.000000 twitchify-1.0.0/twitch/moderation.py
+-rw-rw-rw-   0        0        0     6566 2023-06-20 00:35:39.000000 twitchify-1.0.0/twitch/reward.py
+-rw-rw-rw-   0        0        0    13751 2023-06-20 01:23:10.000000 twitchify-1.0.0/twitch/state.py
+-rw-rw-rw-   0        0        0     3970 2023-06-20 00:35:40.000000 twitchify-1.0.0/twitch/stream.py
+-rw-rw-rw-   0        0        0     7761 2023-06-20 00:35:40.000000 twitchify-1.0.0/twitch/survey.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:49:16.203277 twitchify-1.0.0/twitch/types/
+-rw-rw-rw-   0        0        0     2137 2023-06-20 00:12:07.000000 twitchify-1.0.0/twitch/types/gateway.py
+-rw-rw-rw-   0        0        0     1414 2023-06-20 00:12:07.000000 twitchify-1.0.0/twitch/types/http.py
+-rw-rw-rw-   0        0        0     1306 2023-06-20 00:12:07.000000 twitchify-1.0.0/twitch/types/message.py
+-rw-rw-rw-   0        0        0     2701 2023-06-20 00:12:07.000000 twitchify-1.0.0/twitch/types/user.py
+-rw-rw-rw-   0        0        0     5701 2023-06-20 00:35:40.000000 twitchify-1.0.0/twitch/user.py
+-rw-rw-rw-   0        0        0     5432 2023-06-20 01:19:01.000000 twitchify-1.0.0/twitch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:49:16.236257 twitchify-1.0.0/twitchify.egg-info/
+-rw-rw-rw-   0        0        0      260 2023-06-20 16:49:16.000000 twitchify-1.0.0/twitchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-06-20 16:49:16.000000 twitchify-1.0.0/twitchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:49:16.000000 twitchify-1.0.0/twitchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-20 16:49:16.000000 twitchify-1.0.0/twitchify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 16:49:16.000000 twitchify-1.0.0/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-0.0.0/twitch/__init__.py` & `twitchify-1.0.0/twitch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
 The MIT License (MIT)
 
-Copyright (c) 2023-present Snifo
+Copyright (c) 2023-present MrSniFo
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
-Software is furnishegiotd to do so, subject to the following conditions:
+Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in
 all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-__title__ = "Twitchify"
-__version__ = "0.0.0"
-__license__ = "MIT License"
-__author__ = "Snifo"
-__email__ = "Snifo@mail.com"
+__title__ = 'Twitchify'
+__version__ = '1.0.0'
+__license__ = 'MIT License'
+__author__ = 'Snifo'
+__email__ = 'Snifo@mail.com'
+__github__ = 'https://github.com/mrsnifo/twitchify'
+
+from .client import Client
```

