# Comparing `tmp/PlexLabExchange-0.8.3.tar.gz` & `tmp/PlexLabExchange-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexLabExchange-0.8.3.tar", last modified: Tue Jun 20 18:05:49 2023, max compression
+gzip compressed data, was "PlexLabExchange-0.8.4.tar", last modified: Tue Jun 20 19:04:51 2023, max compression
```

## Comparing `PlexLabExchange-0.8.3.tar` & `PlexLabExchange-0.8.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 18:05:49.543394 PlexLabExchange-0.8.3/
--rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 18:05:49.543261 PlexLabExchange-0.8.3/PKG-INFO
-drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 18:05:49.543095 PlexLabExchange-0.8.3/PlexLabExchange.egg-info/
--rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 18:05:49.000000 PlexLabExchange-0.8.3/PlexLabExchange.egg-info/PKG-INFO
--rw-r--r--   0 mcmenemy   (501) staff       (20)      174 2023-06-20 18:05:49.000000 PlexLabExchange-0.8.3/PlexLabExchange.egg-info/SOURCES.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 18:05:49.000000 PlexLabExchange-0.8.3/PlexLabExchange.egg-info/dependency_links.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 18:05:49.000000 PlexLabExchange-0.8.3/PlexLabExchange.egg-info/top_level.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)        0 2023-06-20 18:05:22.000000 PlexLabExchange-0.8.3/README.md
--rw-r--r--   0 mcmenemy   (501) staff       (20)       38 2023-06-20 18:05:49.543434 PlexLabExchange-0.8.3/setup.cfg
--rw-r--r--   0 mcmenemy   (501) staff       (20)     3036 2023-06-20 18:04:33.000000 PlexLabExchange-0.8.3/setup.py
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 19:04:51.772650 PlexLabExchange-0.8.4/
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 19:04:51.772508 PlexLabExchange-0.8.4/PKG-INFO
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 19:04:51.772329 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/PKG-INFO
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      174 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/SOURCES.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/dependency_links.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/top_level.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      117 2023-06-20 18:06:34.000000 PlexLabExchange-0.8.4/README.md
+-rw-r--r--   0 mcmenemy   (501) staff       (20)       38 2023-06-20 19:04:51.772689 PlexLabExchange-0.8.4/setup.cfg
+-rw-r--r--   0 mcmenemy   (501) staff       (20)     3980 2023-06-20 19:04:45.000000 PlexLabExchange-0.8.4/setup.py
```

### Comparing `PlexLabExchange-0.8.3/PKG-INFO` & `PlexLabExchange-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexLabExchange
-Version: 0.8.3
+Version: 0.8.4
 Summary: A Python interface to the Plex Go CLI.
 Home-page: https://github.com/labdao/plex
 Author: LabDAO
 Author-email: media@labdao.xyz
 License: MIT
 Keywords: plex golang cli wrapper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `PlexLabExchange-0.8.3/PlexLabExchange.egg-info/PKG-INFO` & `PlexLabExchange-0.8.4/PlexLabExchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexLabExchange
-Version: 0.8.3
+Version: 0.8.4
 Summary: A Python interface to the Plex Go CLI.
 Home-page: https://github.com/labdao/plex
 Author: LabDAO
 Author-email: media@labdao.xyz
 License: MIT
 Keywords: plex golang cli wrapper
 Classifier: Development Status :: 3 - Alpha
```

