# Comparing `tmp/panel-jstree-0.1.0.tar.gz` & `tmp/panel-jstree-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panel-jstree-0.1.0.tar", last modified: Tue Jun 20 00:36:05 2023, max compression
+gzip compressed data, was "panel-jstree-0.1.1.tar", last modified: Tue Jun 20 16:19:27 2023, max compression
```

## Comparing `panel-jstree-0.1.0.tar` & `panel-jstree-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.538312 panel-jstree-0.1.0/
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     1073 2023-06-20 00:35:04.000000 panel-jstree-0.1.0/LICENSE
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      287 2023-06-20 00:33:52.000000 panel-jstree-0.1.0/MANIFEST.in
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     5308 2023-06-20 00:36:05.537961 panel-jstree-0.1.0/PKG-INFO
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     2473 2023-06-13 22:08:30.000000 panel-jstree-0.1.0/README.md
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     3363 2023-06-20 00:31:50.000000 panel-jstree-0.1.0/pyproject.toml
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       38 2023-06-20 00:36:05.538417 panel-jstree-0.1.0/setup.cfg
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.515340 panel-jstree-0.1.0/src/
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.521451 panel-jstree-0.1.0/src/panel_jstree/
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       99 2023-06-19 22:39:17.000000 panel-jstree-0.1.0/src/panel_jstree/__init__.py
--rw-r--r--   0 madelinescyphers   (501) staff       (20)        3 2023-05-17 19:36:32.000000 panel-jstree-0.1.0/src/panel_jstree/bokeh.ext.json
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.525628 panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/
--rw-r--r--   0 madelinescyphers   (501) staff       (20)        0 2023-05-17 19:36:32.000000 panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/__init__.py
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      129 2023-06-13 18:13:34.000000 panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/index.ts
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     1407 2023-06-19 21:22:06.000000 panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/jstree.py
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     6325 2023-06-19 21:25:46.000000 panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/jstree.ts
--rw-r--r--   0 madelinescyphers   (501) staff       (20)        0 2023-05-17 19:36:32.000000 panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/layout.py
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     4407 2023-06-14 21:15:44.000000 panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/layout.ts
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.527878 panel-jstree-0.1.0/src/panel_jstree/dist/
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.529520 panel-jstree-0.1.0/src/panel_jstree/dist/lib/
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.535555 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       55 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/index.d.ts
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      162 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/index.js
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      257 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/index.js.map
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     1435 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     5476 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     6100 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     1106 2023-06-20 00:35:21.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     4650 2023-06-20 00:35:21.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     4486 2023-06-20 00:35:21.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       76 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/index.d.ts
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      321 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/index.js
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      280 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/lib/index.js.map
--rw-r--r--   0 madelinescyphers   (501) staff       (20)    14815 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.js
--rw-r--r--   0 madelinescyphers   (501) staff       (20)    14835 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.js.map
--rw-r--r--   0 madelinescyphers   (501) staff       (20)    43519 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.json
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     8654 2023-06-20 00:35:22.000000 panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.min.js
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      289 2023-05-17 19:36:32.000000 panel-jstree-0.1.0/src/panel_jstree/index.ts
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     6419 2023-06-19 22:14:35.000000 panel-jstree-0.1.0/src/panel_jstree/package-lock.json
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      320 2023-06-19 21:48:57.000000 panel-jstree-0.1.0/src/panel_jstree/package.json
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       63 2023-05-17 19:36:32.000000 panel-jstree-0.1.0/src/panel_jstree/py.typed
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     1054 2023-06-13 18:13:34.000000 panel-jstree-0.1.0/src/panel_jstree/tsconfig.json
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.536720 panel-jstree-0.1.0/src/panel_jstree/widgets/
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       28 2023-05-17 19:36:32.000000 panel-jstree-0.1.0/src/panel_jstree/widgets/__init__.py
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     7587 2023-06-19 21:25:29.000000 panel-jstree-0.1.0/src/panel_jstree/widgets/jstree.py
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.523217 panel-jstree-0.1.0/src/panel_jstree.egg-info/
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     5308 2023-06-20 00:36:05.000000 panel-jstree-0.1.0/src/panel_jstree.egg-info/PKG-INFO
--rw-r--r--   0 madelinescyphers   (501) staff       (20)     1574 2023-06-20 00:36:05.000000 panel-jstree-0.1.0/src/panel_jstree.egg-info/SOURCES.txt
--rw-r--r--   0 madelinescyphers   (501) staff       (20)        1 2023-06-20 00:36:05.000000 panel-jstree-0.1.0/src/panel_jstree.egg-info/dependency_links.txt
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       68 2023-06-20 00:36:05.000000 panel-jstree-0.1.0/src/panel_jstree.egg-info/requires.txt
--rw-r--r--   0 madelinescyphers   (501) staff       (20)       13 2023-06-20 00:36:05.000000 panel-jstree-0.1.0/src/panel_jstree.egg-info/top_level.txt
-drwxr-xr-x   0 madelinescyphers   (501) staff       (20)        0 2023-06-20 00:36:05.537255 panel-jstree-0.1.0/tests/
--rw-r--r--   0 madelinescyphers   (501) staff       (20)      191 2023-06-13 22:08:30.000000 panel-jstree-0.1.0/tests/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.739536 panel-jstree-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.743536 panel-jstree-0.1.1/src/panel_jstree/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/bokeh.ext.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.743536 panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/jstree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/jstree.ts
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/layout.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/src/panel_jstree/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/src/panel_jstree/dist/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/layout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/lib/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    43332 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-20 16:19:20.000000 panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-20 16:19:18.000000 panel-jstree-0.1.1/src/panel_jstree/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/src/panel_jstree/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/src/panel_jstree/widgets/jstree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.743536 panel-jstree-0.1.1/src/panel_jstree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-20 16:19:27.000000 panel-jstree-0.1.1/src/panel_jstree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-20 16:19:27.000000 panel-jstree-0.1.1/src/panel_jstree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:19:27.000000 panel-jstree-0.1.1/src/panel_jstree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 16:19:27.000000 panel-jstree-0.1.1/src/panel_jstree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 16:19:27.000000 panel-jstree-0.1.1/src/panel_jstree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:19:27.747536 panel-jstree-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-20 16:18:40.000000 panel-jstree-0.1.1/tests/test_hello.py
```

### Comparing `panel-jstree-0.1.0/LICENSE` & `panel-jstree-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/PKG-INFO` & `panel-jstree-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panel-jstree
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: madeline-scyphers
 License: MIT License
         
         Copyright (c) 2023 Madeline Scyphers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,47 +67,28 @@
 You can install and use the package as simple as.
 
 ```bash
 pip install panel-jstree
 ```
 
 ```python
-import panel_jstree
-INSERT A SHORT EXAMPLE
+import panel as pn
+from panel_jstree import FileTree
+
+pn.Column(FileTree())
 ```
 
 ![Project Intro](assets/videos/project-intro.gif)
 
-REPLACE THE INTRO VIDEO
-
 ## 🚀 Get started in under a minute
 
-Install `panel-jstree` including the *`examples` dependencies*.
-
-```bash
-pip install  panel-jstree[examples]
-```
-
-Explore the sample apps
-
 ```bash
-pn hello panel-jstree
+pip install  panel-jstree
 ```
 
-![Project Intro](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/pn-hello-panel-jstree.gif)
-
-You can now find the *reference* and *gallery* notebooks in the `examples/madeline-scyphers/panel-jstree` folder. Check them out by running `jupyter lab`.
-
-## 📒 Explore the examples online
-
-Click one of the buttons
-
-[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/madeline-scyphers/panel-jstree/tree/main/examples/)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/madeline-scyphers/panel-jstree/HEAD)
-
 ## ⭐ Support
 
 Please support [Panel](https://panel.holoviz.org) and
 [awesome-panel](https://awesome-panel.org) by giving the projects a star on Github:
 
 - [holoviz/panel](https://github.com/holoviz/panel).
 - [awesome-panel/awesome-panel](https://github.com/awesome-panel/awesome-panel).
@@ -121,11 +102,10 @@
 I would love to support and receive your contributions. Thanks.
 
 [![Hacktober Fest](https://github.blog/wp-content/uploads/2022/10/hacktoberfestbanner.jpeg?fit=1200%2C630)](https://github.com/madeline-scyphers/panel-jstree/issues).
 
 ## Monitor
 
 [![PyPI version](https://badge.fury.io/py/panel-jstree.svg)](https://pypi.org/project/panel-jstree/)
-[![Downloads](https://pepy.tech/badge/panel-jstree/month)](https://pepy.tech/project/panel-jstree)
-![Python Versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
 [![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIT)
-![Test Results](https://github.com/madeline-scyphers/panel-jstree/actions/workflows/tests.yaml/badge.svg?branch=main)
+
```

### Comparing `panel-jstree-0.1.0/pyproject.toml` & `panel-jstree-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,20 @@
 
 authors = [
     {name = "madeline-scyphers"}
 ]
 
 [project.optional-dependencies]
 dev = [
-    "awesome-panel-cli[dev]"
+    "pytest",
+    "black",
+    "isort"
 ]
 examples = [
-    "awesome-panel-cli",
+    "notebook",   
 ]
 
 [project.urls]
 repository = "https://github.com/madeline-scyphers/panel-jstree"
 
 [tool.setuptools.dynamic]
 version = {attr = "panel_jstree.VERSION"}
```

### Comparing `panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/jstree.py` & `panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/jstree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Defines custom jsTree bokeh model to render Ace editor.
 """
 from __future__ import absolute_import, division, unicode_literals
 
-from bokeh.core.properties import String, Override, Dict, Any, List, Bool, Enum, JSON
-# from .layout import HTMLBox
-from bokeh.util.compiler import TypeScript
+import pathlib
+
+from bokeh.core.properties import JSON, Any, Bool, Dict, Enum, List, Override, String
 from bokeh.models.layouts import LayoutDOM
 
-from panel.io.resources import bundled_files, JS_URLS
+# from .layout import HTMLBox
+from bokeh.util.compiler import TypeScript
+from panel import extension
+from panel.io.resources import JS_URLS, bundled_files
 from panel.util import classproperty
 
-import pathlib
-
-from panel import extension
 # pylint: disable=protected-access
 
 extension._imports["tree"] = "panel_jstree.bokeh_extensions.jstree"
 # pylint: enable=protected-access
 
 
 class HTMLBox(LayoutDOM):
@@ -26,21 +26,19 @@
 
 class jsTreePlot(HTMLBox):
     """
     A Bokeh model that wraps around a jsTree editor and renders it inside
     a Bokeh plot.
     """
 
-    __css__ = [
-        'https://cdnjs.cloudflare.com/ajax/libs/jstree/3.2.1/themes/default/style.min.css'
-    ]
+    __css__ = ["https://cdnjs.cloudflare.com/ajax/libs/jstree/3.2.1/themes/default/style.min.css"]
 
     __javascript__ = [
-        'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js',
-        'https://cdnjs.cloudflare.com/ajax/libs/jstree/3.3.12/jstree.min.js'
+        "https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js",
+        "https://cdnjs.cloudflare.com/ajax/libs/jstree/3.3.12/jstree.min.js",
     ]
 
     plugins = List(Any)
     multiple = Bool(default=True)
     show_icons = Bool(default=True)
     show_dots = Bool(default=True)
     _last_opened = Any()
```

### Comparing `panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/jstree.ts` & `panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/jstree.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/bokeh_extensions/layout.ts` & `panel-jstree-0.1.1/src/panel_jstree/bokeh_extensions/layout.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts` & `panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/jstree.d.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js` & `panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map` & `panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js.map`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts` & `panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/layout.d.ts`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js` & `panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/layout.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map` & `panel-jstree-0.1.1/src/panel_jstree/dist/lib/bokeh_extensions/layout.js.map`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.js` & `panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.js.map` & `panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.js.map`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.json` & `panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944196428571428%*

 * *Differences: {"'artifacts'": "{0: {'module': {'file': "*

 * *                "'/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/index.js', "*

 * *                "'base': '/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib', "*

 * *                "'dependency_paths': {0: {insert: [(1, "*

 * *                "'/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/index.js')], "*

 * *                "delete: [1]}}}}, 1: {'module': {'file': "*

 * *                "'/home/runner/w […]*

```diff
@@ -3,27 +3,27 @@
         {
             "code": {
                 "min_map": "{\"version\":3,\"file\":\"index.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"PaneljsTree\",\"__importStar\",\"register_models\"],\"sources\":[\"0\"],\"mappings\":\"AAAe,SAASA,EAAEC,EAASC,EAAQC,EAASC,EAAYC,GAC5DD,IACA,MAIME,EAJUL,EAAQ,SAIIM,aAAaN,EAAQ,eACjDE,EAAQG,YAAcA,GAEtB,EADeL,EAAQ,iBACZO,iBAAiBF,EAChC\"}",
                 "min_source": "function _(e,s,t,o,r){o();const a=e(\"tslib\").__importStar(e(\"ef403b5ad2\"));t.PaneljsTree=a;(0,e(\"@bokehjs/base\").register_models)(a)}\n//# sourceMappingURL=index.min.js.map",
                 "source": "/* index.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const tslib_1 = require(\"tslib\");\n    // export {jsTreePlot} from \"./models/jstree\"\n    // import {register_models} from \"@bokehjs/base\"\n    // register_models(jsTreePlot as any)\n    const PaneljsTree = tslib_1.__importStar(require(\"ef403b5ad2\") /* ./bokeh_extensions/ */);\n    exports.PaneljsTree = PaneljsTree;\n    const base_1 = require(\"@bokehjs/base\");\n    (0, base_1.register_models)(PaneljsTree);\n}\n"
             },
             "module": {
-                "base": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib",
+                "base": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib",
                 "base_path": "index.js",
                 "canonical": "index",
                 "dependency_map": [],
                 "dependency_paths": [
                     [
                         "./bokeh_extensions/",
-                        "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/index.js"
+                        "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/index.js"
                     ]
                 ],
                 "exported": [],
                 "externals": [],
-                "file": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib/index.js",
+                "file": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/index.js",
                 "hash": "ecf49f9c64208508db8dd2906850a0d3457930667d111e4a7b9931fdf24b2b0c",
                 "id": "ecf49f9c64",
                 "resolution": "ESM",
                 "shims": [],
                 "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.PaneljsTree = void 0;\nconst tslib_1 = require(\"tslib\");\n// export {jsTreePlot} from \"./models/jstree\"\n// import {register_models} from \"@bokehjs/base\"\n// register_models(jsTreePlot as any)\nconst PaneljsTree = tslib_1.__importStar(require(\"./bokeh_extensions/\"));\nexports.PaneljsTree = PaneljsTree;\nconst base_1 = require(\"@bokehjs/base\");\n(0, base_1.register_models)(PaneljsTree);\n//# sourceMappingURL=index.js.map\n",
                 "type": "js"
             }
@@ -31,27 +31,27 @@
         {
             "code": {
                 "min_map": "{\"version\":3,\"file\":\"index.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"jsTree\",\"__importStar\",\"register_models\"],\"sources\":[\"0\"],\"mappings\":\"AAAgC,SAASA,EAAEC,EAASC,EAAQC,EAASC,EAAYC,GAC7ED,IACA,MACME,EADUL,EAAQ,SACDM,aAAaN,EAAQ,eAC5CE,EAAQG,OAASA,GAEjB,EADeL,EAAQ,iBACZO,iBAAiBF,EAChC\"}",
                 "min_source": "function _(e,s,t,c,o){c();const r=e(\"tslib\").__importStar(e(\"e4c337fccb\"));t.jsTree=r;(0,e(\"@bokehjs/base\").register_models)(r)}\n//# sourceMappingURL=index.min.js.map",
                 "source": "/* bokeh_extensions/index.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const tslib_1 = require(\"tslib\");\n    const jsTree = tslib_1.__importStar(require(\"e4c337fccb\") /* ./jstree */);\n    exports.jsTree = jsTree;\n    const base_1 = require(\"@bokehjs/base\");\n    (0, base_1.register_models)(jsTree);\n}\n"
             },
             "module": {
-                "base": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib",
+                "base": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib",
                 "base_path": "bokeh_extensions/index.js",
                 "canonical": "bokeh_extensions/index",
                 "dependency_map": [],
                 "dependency_paths": [
                     [
                         "./jstree",
-                        "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js"
+                        "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js"
                     ]
                 ],
                 "exported": [],
                 "externals": [],
-                "file": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/index.js",
+                "file": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/index.js",
                 "hash": "ef403b5ad2ae2ff463f17aebd2c0750540ffbffad4e2956e5aeac3b4d101823c",
                 "id": "ef403b5ad2",
                 "resolution": "ESM",
                 "shims": [],
                 "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.jsTree = void 0;\nconst tslib_1 = require(\"tslib\");\nconst jsTree = tslib_1.__importStar(require(\"./jstree\"));\nexports.jsTree = jsTree;\nconst base_1 = require(\"@bokehjs/base\");\n(0, base_1.register_models)(jsTree);\n//# sourceMappingURL=index.js.map\n",
                 "type": "js"
             }
@@ -59,36 +59,36 @@
         {
             "code": {
                 "min_map": "{\"version\":3,\"file\":\"jstree.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"_a\",\"dom_1\",\"layout_1\",\"jsTreePlotView\",\"HTMLBoxView\",\"initialize\",\"super\",\"this\",\"_last_selected\",\"connect_signals\",\"console\",\"log\",\"connect\",\"model\",\"properties\",\"data\",\"change\",\"_update_tree_from_data\",\"value\",\"_update_selection_from_value\",\"_new_nodes\",\"_update_tree_from_new_nodes\",\"show_icons\",\"_setShowIcons\",\"show_dots\",\"_setShowDots\",\"multiple\",\"_setMultiple\",\"render\",\"_id\",\"Math\",\"random\",\"toString\",\"substr\",\"_container\",\"div\",\"id\",\"style\",\"set_size\",\"shadow_el\",\"appendChild\",\"_jstree\",\"jQuery\",\"jstree\",\"Object\",\"assign\",\"core\",\"check_callback\",\"themes\",\"dots\",\"icons\",\"plugins\",\"checkbox\",\"three_state\",\"cascade\",\"init_callbacks\",\"on\",\"e\",\"_update_code_from_editor\",\"_listen_for_node_open\",\"instance\",\"get_selected\",\"deselected\",\"filter\",\"x\",\"includes\",\"select_node\",\"deselect_node\",\"node\",\"create_node\",\"settings\",\"get_json\",\"no_li_attr\",\"no_a_attr\",\"no_data\",\"_flat_tree\",\"flat\",\"hide_icons\",\"hide_dots\",\"_update_tree_theme_from_model\",\"refresh\",\"_last_opened\",\"__name__\",\"jsTreePlot\",\"HTMLBox\",\"constructor\",\"attrs\",\"__module__\",\"prototype\",\"default_view\",\"define\",\"Array\",\"Any\",\"Boolean\"],\"sources\":[\"0\"],\"mappings\":\"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\"}",
                 "min_source": "function _(e,t,s,o,i){var _;o();const n=e(\"@bokehjs/core/dom\"),l=e(\"bfe8e8c0eb\");class r extends l.HTMLBoxView{initialize(){super.initialize(),this._last_selected=[]}connect_signals(){console.log(\"connect\"),super.connect_signals(),this.connect(this.model.properties.data.change,(()=>this._update_tree_from_data())),this.connect(this.model.properties.value.change,(()=>this._update_selection_from_value())),this.connect(this.model.properties._new_nodes.change,(()=>this._update_tree_from_new_nodes())),this.connect(this.model.properties.show_icons.change,(()=>this._setShowIcons())),this.connect(this.model.properties.show_dots.change,(()=>this._setShowDots())),this.connect(this.model.properties.multiple.change,(()=>this._setMultiple())),console.log(this.model.show_dots),console.log(this.model.show_icons)}render(){super.render(),this._id=\"_\"+Math.random().toString(36).substr(2,9),console.log(this._id),this._container=(0,n.div)({id:this._id,style:\"overflow: auto; minHeight: 200px; minWidth: 200px;\"}),(0,l.set_size)(this._container,this.model),this.shadow_el.appendChild(this._container),console.log(this._container);this._jstree=jQuery(this._container).jstree(Object.assign({core:{data:this.model.data,check_callback:!0,multiple:this.model.multiple,themes:{dots:this.model.show_dots,icons:this.model.show_icons}},plugins:this.model.plugins},{checkbox:{three_state:!1,cascade:\"undetermined\"}})),this.init_callbacks()}init_callbacks(){this._jstree.on(\"refresh.jstree\",(({},{})=>this._update_selection_from_value())),this._jstree.on(\"changed.jstree\",((e,t)=>this._update_code_from_editor(e,t))),this._jstree.on(\"before_open.jstree\",((e,t)=>this._listen_for_node_open(e,t)))}_update_code_from_editor({},e){this.model.value=e.instance.get_selected()}_update_selection_from_value(){console.log(\"last selected: \",this._last_selected);let e=this._last_selected.filter((e=>!this.model.value.includes(e)));console.log(\"values: \",this.model.value),this._jstree.jstree(!0).select_node(this.model.value),console.log(\"deselected: \",e),this._jstree.jstree(!0).deselect_node(e),this._last_selected=this.model.value}_update_tree_from_new_nodes(){console.log(\"new nodes: \",this.model._new_nodes);for(let e of this.model._new_nodes)this._jstree.jstree(!0).create_node(e.parent,e,\"first\");this._jstree.jstree(!0).settings.core.data=this._jstree.jstree(!0).get_json(null,{no_li_attr:!0,no_a_attr:!0,no_data:!0}),this.model.data=this._jstree.jstree(!0).settings.core.data}_update_tree_from_data(){console.log(\"updating data\"),this._jstree.jstree(!0).settings.core.data=this.model.data,console.log(\"flat tree: \",this.model._flat_tree),this.model._flat_tree=this._jstree.jstree(!0).get_json(null,{flat:!0})}_setShowIcons(){this.model.show_icons?this._jstree.jstree(!0).show_icons():this._jstree.jstree(!0).hide_icons()}_setShowDots(){this.model.show_dots?this._jstree.jstree(!0).show_dots():this._jstree.jstree(!0).hide_dots()}_setMultiple(){this._jstree.jstree(!0).settings.core.multiple=this.model.multiple}_update_tree_theme_from_model(){this._jstree.jstree(!0).refresh(!1,!0)}_listen_for_node_open({},e){console.log(\"node opened\"),console.log(\"openeing node: \",e.node),this.model._last_opened=e.node}}s.jsTreePlotView=r,r.__name__=\"jsTreePlotView\";class d extends l.HTMLBox{constructor(e){super(e)}}s.jsTreePlot=d,_=d,d.__name__=\"jsTreePlot\",d.__module__=\"panel_jstree.bokeh_extensions.jstree\",_.prototype.default_view=r,_.define((({Array:e,Any:t,Boolean:s})=>({value:[e(t),[]],data:[e(t),[]],plugins:[e(t),[]],multiple:[s,!0],show_icons:[s,!0],show_dots:[s,!0],_last_opened:[t,{}],_new_nodes:[t,{}],_flat_tree:[e(t),[]]})))}\n//# sourceMappingURL=jstree.min.js.map",
                 "source": "/* bokeh_extensions/jstree.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    var _a;\n    const dom_1 = require(\"@bokehjs/core/dom\");\n    const layout_1 = require(\"bfe8e8c0eb\") /* ./layout */;\n    function ID() {\n        // Math.random should be unique because of its seeding algorithm.\n        // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n        // after the decimal.\n        return '_' + Math.random().toString(36).substr(2, 9);\n    }\n    class jsTreePlotView extends layout_1.HTMLBoxView {\n        initialize() {\n            super.initialize();\n            this._last_selected = [];\n        }\n        connect_signals() {\n            console.log(\"connect\");\n            super.connect_signals();\n            this.connect(this.model.properties.data.change, () => this._update_tree_from_data());\n            this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n            this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n            this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n            this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n            this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n            console.log(this.model.show_dots);\n            console.log(this.model.show_icons);\n        }\n        //\n        render() {\n            super.render();\n            this._id = ID();\n            console.log(this._id);\n            this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n            (0, layout_1.set_size)(this._container, this.model);\n            this.shadow_el.appendChild(this._container);\n            console.log(this._container);\n            let kw = { \"checkbox\": {\n                    \"three_state\": false,\n                    \"cascade\": \"undetermined\"\n                } };\n            this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model.data, \"check_callback\": true,\n                    \"multiple\": this.model.multiple,\n                    \"themes\": {\n                        \"dots\": this.model.show_dots,\n                        \"icons\": this.model.show_icons\n                    }\n                }, \"plugins\": this.model.plugins }, kw));\n            this.init_callbacks();\n        }\n        init_callbacks() {\n            // Rendering callbacks\n            // TODO: do I need both of these?\n            this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n            // Sync state with model\n            this._jstree.on('changed.jstree', (e, data) => this._update_code_from_editor(e, data));\n            this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n        }\n        _update_code_from_editor({}, data) {\n            this.model.value = data.instance.get_selected();\n        }\n        _update_selection_from_value() {\n            console.log(\"last selected: \", this._last_selected);\n            let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n            console.log(\"values: \", this.model.value);\n            this._jstree.jstree(true).select_node(this.model.value);\n            console.log(\"deselected: \", deselected);\n            this._jstree.jstree(true).deselect_node(deselected);\n            this._last_selected = this.model.value;\n        }\n        _update_tree_from_new_nodes() {\n            console.log(\"new nodes: \", this.model._new_nodes);\n            for (let node of this.model._new_nodes) {\n                this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n            }\n            this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n            this.model.data = this._jstree.jstree(true).settings.core.data;\n            // this._update_selection_from_value()\n        }\n        _update_tree_from_data() {\n            console.log(\"updating data\");\n            this._jstree.jstree(true).settings.core.data = this.model.data;\n            console.log(\"flat tree: \", this.model._flat_tree);\n            this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n        }\n        _setShowIcons() {\n            if (this.model.show_icons) {\n                this._jstree.jstree(true).show_icons();\n            }\n            else {\n                this._jstree.jstree(true).hide_icons();\n            }\n        }\n        _setShowDots() {\n            if (this.model.show_dots) {\n                this._jstree.jstree(true).show_dots();\n            }\n            else {\n                this._jstree.jstree(true).hide_dots();\n            }\n        }\n        _setMultiple() {\n            this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n        }\n        _update_tree_theme_from_model() {\n            this._jstree.jstree(true).refresh(false, true);\n        }\n        _listen_for_node_open({}, data) {\n            console.log(\"node opened\");\n            console.log(\"openeing node: \", data.node);\n            this.model._last_opened = data.node;\n        }\n    }\n    exports.jsTreePlotView = jsTreePlotView;\n    jsTreePlotView.__name__ = \"jsTreePlotView\";\n    class jsTreePlot extends layout_1.HTMLBox {\n        constructor(attrs) {\n            super(attrs);\n        }\n    }\n    exports.jsTreePlot = jsTreePlot;\n    _a = jsTreePlot;\n    jsTreePlot.__name__ = \"jsTreePlot\";\n    jsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n    (() => {\n        _a.prototype.default_view = jsTreePlotView;\n        _a.define(({ Array, Any, Boolean }) => ({\n            value: [Array(Any), []],\n            data: [Array(Any), []],\n            plugins: [Array(Any), []],\n            multiple: [Boolean, true],\n            show_icons: [Boolean, true],\n            show_dots: [Boolean, true],\n            _last_opened: [Any, {}],\n            _new_nodes: [Any, {}],\n            _flat_tree: [Array(Any), []],\n        }));\n    })();\n}\n"
             },
             "module": {
-                "base": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib",
+                "base": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib",
                 "base_path": "bokeh_extensions/jstree.js",
                 "canonical": "bokeh_extensions/jstree",
                 "dependency_map": [],
                 "dependency_paths": [
                     [
                         "./layout",
-                        "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/layout.js"
+                        "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/layout.js"
                     ]
                 ],
                 "exported": [
                     {
                         "name": "jsTreePlotView",
                         "type": "named"
                     },
                     {
                         "name": "jsTreePlot",
                         "type": "named"
                     }
                 ],
                 "externals": [],
-                "file": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js",
+                "file": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/jstree.js",
                 "hash": "e4c337fccb4f7ae60392cd3547c911306f99ec980eb489b689270f46039545eb",
                 "id": "e4c337fccb",
                 "resolution": "ESM",
                 "shims": [],
                 "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.jsTreePlot = exports.jsTreePlotView = void 0;\nvar _a;\nconst dom_1 = require(\"@bokehjs/core/dom\");\nconst layout_1 = require(\"./layout\");\nfunction ID() {\n    // Math.random should be unique because of its seeding algorithm.\n    // Convert it to base 36 (numbers + letters), and grab the first 9 characters\n    // after the decimal.\n    return '_' + Math.random().toString(36).substr(2, 9);\n}\nclass jsTreePlotView extends layout_1.HTMLBoxView {\n    initialize() {\n        super.initialize();\n        this._last_selected = [];\n    }\n    connect_signals() {\n        console.log(\"connect\");\n        super.connect_signals();\n        this.connect(this.model.properties.data.change, () => this._update_tree_from_data());\n        this.connect(this.model.properties.value.change, () => this._update_selection_from_value());\n        this.connect(this.model.properties._new_nodes.change, () => this._update_tree_from_new_nodes());\n        this.connect(this.model.properties.show_icons.change, () => this._setShowIcons());\n        this.connect(this.model.properties.show_dots.change, () => this._setShowDots());\n        this.connect(this.model.properties.multiple.change, () => this._setMultiple());\n        console.log(this.model.show_dots);\n        console.log(this.model.show_icons);\n    }\n    //\n    render() {\n        super.render();\n        this._id = ID();\n        console.log(this._id);\n        this._container = (0, dom_1.div)({ id: this._id, style: \"overflow: auto; minHeight: 200px; minWidth: 200px;\" });\n        (0, layout_1.set_size)(this._container, this.model);\n        this.shadow_el.appendChild(this._container);\n        console.log(this._container);\n        let kw = { \"checkbox\": {\n                \"three_state\": false,\n                \"cascade\": \"undetermined\"\n            } };\n        this._jstree = jQuery(this._container).jstree(Object.assign({ \"core\": { \"data\": this.model.data, \"check_callback\": true,\n                \"multiple\": this.model.multiple,\n                \"themes\": {\n                    \"dots\": this.model.show_dots,\n                    \"icons\": this.model.show_icons\n                }\n            }, \"plugins\": this.model.plugins }, kw));\n        this.init_callbacks();\n    }\n    init_callbacks() {\n        // Rendering callbacks\n        // TODO: do I need both of these?\n        this._jstree.on('refresh.jstree', ({}, {}) => this._update_selection_from_value());\n        // Sync state with model\n        this._jstree.on('changed.jstree', (e, data) => this._update_code_from_editor(e, data));\n        this._jstree.on('before_open.jstree', (e, data) => this._listen_for_node_open(e, data));\n    }\n    _update_code_from_editor({}, data) {\n        this.model.value = data.instance.get_selected();\n    }\n    _update_selection_from_value() {\n        console.log(\"last selected: \", this._last_selected);\n        let deselected = this._last_selected.filter(x => !this.model.value.includes(x));\n        console.log(\"values: \", this.model.value);\n        this._jstree.jstree(true).select_node(this.model.value);\n        console.log(\"deselected: \", deselected);\n        this._jstree.jstree(true).deselect_node(deselected);\n        this._last_selected = this.model.value;\n    }\n    _update_tree_from_new_nodes() {\n        console.log(\"new nodes: \", this.model._new_nodes);\n        for (let node of this.model._new_nodes) {\n            this._jstree.jstree(true).create_node(node[\"parent\"], node, \"first\");\n        }\n        this._jstree.jstree(true).settings.core.data = this._jstree.jstree(true).get_json(null, { no_li_attr: true, no_a_attr: true, no_data: true });\n        this.model.data = this._jstree.jstree(true).settings.core.data;\n        // this._update_selection_from_value()\n    }\n    _update_tree_from_data() {\n        console.log(\"updating data\");\n        this._jstree.jstree(true).settings.core.data = this.model.data;\n        console.log(\"flat tree: \", this.model._flat_tree);\n        this.model._flat_tree = this._jstree.jstree(true).get_json(null, { \"flat\": true });\n    }\n    _setShowIcons() {\n        if (this.model.show_icons) {\n            this._jstree.jstree(true).show_icons();\n        }\n        else {\n            this._jstree.jstree(true).hide_icons();\n        }\n    }\n    _setShowDots() {\n        if (this.model.show_dots) {\n            this._jstree.jstree(true).show_dots();\n        }\n        else {\n            this._jstree.jstree(true).hide_dots();\n        }\n    }\n    _setMultiple() {\n        this._jstree.jstree(true).settings.core.multiple = this.model.multiple;\n    }\n    _update_tree_theme_from_model() {\n        this._jstree.jstree(true).refresh(false, true);\n    }\n    _listen_for_node_open({}, data) {\n        console.log(\"node opened\");\n        console.log(\"openeing node: \", data.node);\n        this.model._last_opened = data.node;\n    }\n}\nexports.jsTreePlotView = jsTreePlotView;\njsTreePlotView.__name__ = \"jsTreePlotView\";\nclass jsTreePlot extends layout_1.HTMLBox {\n    constructor(attrs) {\n        super(attrs);\n    }\n}\nexports.jsTreePlot = jsTreePlot;\n_a = jsTreePlot;\njsTreePlot.__name__ = \"jsTreePlot\";\njsTreePlot.__module__ = \"panel_jstree.bokeh_extensions.jstree\";\n(() => {\n    _a.prototype.default_view = jsTreePlotView;\n    _a.define(({ Array, Any, Boolean }) => ({\n        value: [Array(Any), []],\n        data: [Array(Any), []],\n        plugins: [Array(Any), []],\n        multiple: [Boolean, true],\n        show_icons: [Boolean, true],\n        show_dots: [Boolean, true],\n        _last_opened: [Any, {}],\n        _new_nodes: [Any, {}],\n        _flat_tree: [Array(Any), []],\n    }));\n})();\n//# sourceMappingURL=jstree.js.map\n",
                 "type": "js"
             }
@@ -96,15 +96,15 @@
         {
             "code": {
                 "min_map": "{\"version\":3,\"file\":\"layout.min.js\",\"names\":[\"_\",\"require\",\"module\",\"exports\",\"__esModule\",\"__esExport\",\"dom_1\",\"types_1\",\"widget_1\",\"layout_dom_1\",\"PanelMarkupView\",\"WidgetView\",\"async\",\"super\",\"lazy_initialize\",\"this\",\"provider\",\"status\",\"ready\",\"connect\",\"contains_tex_string\",\"model\",\"text\",\"render\",\"connect_signals\",\"change\",\"has_math_disabled\",\"disable_math\",\"set_size\",\"el\",\"container\",\"div\",\"shadow_el\",\"appendChild\",\"_has_finished\",\"adjustMargin\",\"width_policy\",\"width\",\"height_policy\",\"height\",\"sizing_mode\",\"margin\",\"Error\",\"wm\",\"hm\",\"isArray\",\"length\",\"style\",\"min_width\",\"minWidth\",\"max_width\",\"maxWidth\",\"min_height\",\"minHeight\",\"maxHeight\",\"max_height\",\"__name__\",\"HTMLBoxView\",\"LayoutDOMView\",\"watch_stylesheets\",\"_initialized_stylesheets\",\"sts\",\"_applied_stylesheets\",\"style_el\",\"HTMLLinkElement\",\"href\",\"addEventListener\",\"Object\",\"values\",\"every\",\"Boolean\",\"style_redraw\",\"child_models\",\"HTMLBox\",\"LayoutDOM\",\"constructor\",\"attrs\"],\"sources\":[\"0\"],\"mappings\":\"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\"}",
                 "min_source": "function _(e,t,i,s,h){s();const a=e(\"@bokehjs/core/dom\"),l=e(\"@bokehjs/core/util/types\"),n=e(\"@bokehjs/models/widgets/widget\"),d=e(\"@bokehjs/models/layouts/layout_dom\");class r extends n.WidgetView{async lazy_initialize(){await super.lazy_initialize(),\"not_started\"!=this.provider.status&&\"loading\"!=this.provider.status||this.provider.ready.connect((()=>{this.contains_tex_string(this.model.text)&&this.render()}))}connect_signals(){super.connect_signals(),this.connect(this.model.change,(()=>{this.render()}))}has_math_disabled(){return this.model.disable_math||!this.contains_tex_string(this.model.text)}render(){super.render(),o(this.el,this.model),this.container=(0,a.div)(),o(this.container,this.model,!1),this.shadow_el.appendChild(this.container),\"failed\"!=this.provider.status&&\"loaded\"!=this.provider.status||(this._has_finished=!0)}}function o(e,t,i=!0){let s=null!=t.width?\"fixed\":\"fit\",h=null!=t.height?\"fixed\":\"fit\";const{sizing_mode:a,margin:n}=t;if(null!=a)if(\"fixed\"==a)s=h=\"fixed\";else if(\"stretch_both\"==a)s=h=\"max\";else if(\"stretch_width\"==a)s=\"max\";else if(\"stretch_height\"==a)h=\"max\";else switch(a){case\"scale_width\":s=\"max\",h=\"min\";break;case\"scale_height\":s=\"min\",h=\"max\";break;case\"scale_both\":s=\"max\",h=\"max\";break;default:throw new Error(\"unreachable\")}let d,r;i?(0,l.isArray)(n)?4===n.length?(r=n[0]+n[2],d=n[1]+n[3]):(r=2*n[0],d=2*n[1]):null==n?r=d=0:d=r=2*n:r=d=0,\"fixed\"==s&&t.width?e.style.width=t.width+\"px\":\"max\"==s&&(e.style.width=d?`calc(100% - ${d}px)`:\"100%\"),null!=t.min_width&&(e.style.minWidth=t.min_width+\"px\"),null!=t.max_width&&(e.style.maxWidth=t.max_width+\"px\"),\"fixed\"==h&&t.height?e.style.height=t.height+\"px\":\"max\"==h&&(e.style.height=r?`calc(100% - ${r}px)`:\"100%\"),null!=t.min_height&&(e.style.minHeight=t.min_height+\"px\"),null!=t.max_width&&(e.style.maxHeight=t.max_height+\"px\")}i.PanelMarkupView=r,r.__name__=\"PanelMarkupView\",i.set_size=o;class _ extends d.LayoutDOMView{render(){super.render(),o(this.el,this.model)}watch_stylesheets(){this._initialized_stylesheets={};for(const e of this._applied_stylesheets){const t=e.el;t instanceof HTMLLinkElement&&(this._initialized_stylesheets[t.href]=!1,t.addEventListener(\"load\",(()=>{this._initialized_stylesheets[t.href]=!0,Object.values(this._initialized_stylesheets).every(Boolean)&&this.style_redraw()})))}}style_redraw(){}get child_models(){return[]}}i.HTMLBoxView=_,_.__name__=\"HTMLBoxView\";class c extends d.LayoutDOM{constructor(e){super(e)}}i.HTMLBox=c,c.__name__=\"HTMLBox\"}\n//# sourceMappingURL=layout.min.js.map",
                 "source": "/* bokeh_extensions/layout.js */ function _(require, module, exports, __esModule, __esExport) {\n    __esModule();\n    const dom_1 = require(\"@bokehjs/core/dom\");\n    const types_1 = require(\"@bokehjs/core/util/types\");\n    const widget_1 = require(\"@bokehjs/models/widgets/widget\");\n    const layout_dom_1 = require(\"@bokehjs/models/layouts/layout_dom\");\n    class PanelMarkupView extends widget_1.WidgetView {\n        async lazy_initialize() {\n            await super.lazy_initialize();\n            if (this.provider.status == \"not_started\" || this.provider.status == \"loading\")\n                this.provider.ready.connect(() => {\n                    if (this.contains_tex_string(this.model.text))\n                        this.render();\n                });\n        }\n        connect_signals() {\n            super.connect_signals();\n            this.connect(this.model.change, () => {\n                this.render();\n            });\n        }\n        has_math_disabled() {\n            return this.model.disable_math || !this.contains_tex_string(this.model.text);\n        }\n        render() {\n            super.render();\n            set_size(this.el, this.model);\n            this.container = (0, dom_1.div)();\n            set_size(this.container, this.model, false);\n            this.shadow_el.appendChild(this.container);\n            if (this.provider.status == \"failed\" || this.provider.status == \"loaded\")\n                this._has_finished = true;\n        }\n    }\n    exports.PanelMarkupView = PanelMarkupView;\n    PanelMarkupView.__name__ = \"PanelMarkupView\";\n    function set_size(el, model, adjustMargin = true) {\n        let width_policy = model.width != null ? \"fixed\" : \"fit\";\n        let height_policy = model.height != null ? \"fixed\" : \"fit\";\n        const { sizing_mode, margin } = model;\n        if (sizing_mode != null) {\n            if (sizing_mode == \"fixed\")\n                width_policy = height_policy = \"fixed\";\n            else if (sizing_mode == \"stretch_both\")\n                width_policy = height_policy = \"max\";\n            else if (sizing_mode == \"stretch_width\")\n                width_policy = \"max\";\n            else if (sizing_mode == \"stretch_height\")\n                height_policy = \"max\";\n            else {\n                switch (sizing_mode) {\n                    case \"scale_width\":\n                        width_policy = \"max\";\n                        height_policy = \"min\";\n                        break;\n                    case \"scale_height\":\n                        width_policy = \"min\";\n                        height_policy = \"max\";\n                        break;\n                    case \"scale_both\":\n                        width_policy = \"max\";\n                        height_policy = \"max\";\n                        break;\n                    default:\n                        throw new Error(\"unreachable\");\n                }\n            }\n        }\n        let wm, hm;\n        if (!adjustMargin) {\n            hm = wm = 0;\n        }\n        else if ((0, types_1.isArray)(margin)) {\n            if (margin.length === 4) {\n                hm = margin[0] + margin[2];\n                wm = margin[1] + margin[3];\n            }\n            else {\n                hm = margin[0] * 2;\n                wm = margin[1] * 2;\n            }\n        }\n        else if (margin == null) {\n            hm = wm = 0;\n        }\n        else {\n            wm = hm = margin * 2;\n        }\n        if (width_policy == \"fixed\" && model.width)\n            el.style.width = model.width + \"px\";\n        else if (width_policy == \"max\")\n            el.style.width = wm ? `calc(100% - ${wm}px)` : \"100%\";\n        if (model.min_width != null)\n            el.style.minWidth = model.min_width + \"px\";\n        if (model.max_width != null)\n            el.style.maxWidth = model.max_width + \"px\";\n        if (height_policy == \"fixed\" && model.height)\n            el.style.height = model.height + \"px\";\n        else if (height_policy == \"max\")\n            el.style.height = hm ? `calc(100% - ${hm}px)` : \"100%\";\n        if (model.min_height != null)\n            el.style.minHeight = model.min_height + \"px\";\n        if (model.max_width != null)\n            el.style.maxHeight = model.max_height + \"px\";\n    }\n    exports.set_size = set_size;\n    class HTMLBoxView extends layout_dom_1.LayoutDOMView {\n        render() {\n            super.render();\n            set_size(this.el, this.model);\n        }\n        watch_stylesheets() {\n            this._initialized_stylesheets = {};\n            for (const sts of this._applied_stylesheets) {\n                const style_el = sts.el;\n                if (style_el instanceof HTMLLinkElement) {\n                    this._initialized_stylesheets[style_el.href] = false;\n                    style_el.addEventListener(\"load\", () => {\n                        this._initialized_stylesheets[style_el.href] = true;\n                        if (Object.values(this._initialized_stylesheets).every(Boolean))\n                            this.style_redraw();\n                    });\n                }\n            }\n        }\n        style_redraw() {\n        }\n        get child_models() {\n            return [];\n        }\n    }\n    exports.HTMLBoxView = HTMLBoxView;\n    HTMLBoxView.__name__ = \"HTMLBoxView\";\n    class HTMLBox extends layout_dom_1.LayoutDOM {\n        constructor(attrs) {\n            super(attrs);\n        }\n    }\n    exports.HTMLBox = HTMLBox;\n    HTMLBox.__name__ = \"HTMLBox\";\n}\n"
             },
             "module": {
-                "base": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib",
+                "base": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib",
                 "base_path": "bokeh_extensions/layout.js",
                 "canonical": "bokeh_extensions/layout",
                 "dependency_map": [],
                 "dependency_paths": [],
                 "exported": [
                     {
                         "name": "PanelMarkupView",
@@ -120,15 +120,15 @@
                     },
                     {
                         "name": "HTMLBox",
                         "type": "named"
                     }
                 ],
                 "externals": [],
-                "file": "/Users/madelinescyphers/Documents/projs_.nosync/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/layout.js",
+                "file": "/home/runner/work/panel-jstree/panel-jstree/src/panel_jstree/dist/lib/bokeh_extensions/layout.js",
                 "hash": "bfe8e8c0ebb8ecb1a28c475138f6dfae38a4e67878682cd23f1746d6f239897f",
                 "id": "bfe8e8c0eb",
                 "resolution": "ESM",
                 "shims": [],
                 "source": "\"use strict\";\nObject.defineProperty(exports, \"__esModule\", { value: true });\nexports.HTMLBox = exports.HTMLBoxView = exports.set_size = exports.PanelMarkupView = void 0;\nconst dom_1 = require(\"@bokehjs/core/dom\");\nconst types_1 = require(\"@bokehjs/core/util/types\");\nconst widget_1 = require(\"@bokehjs/models/widgets/widget\");\nconst layout_dom_1 = require(\"@bokehjs/models/layouts/layout_dom\");\nclass PanelMarkupView extends widget_1.WidgetView {\n    async lazy_initialize() {\n        await super.lazy_initialize();\n        if (this.provider.status == \"not_started\" || this.provider.status == \"loading\")\n            this.provider.ready.connect(() => {\n                if (this.contains_tex_string(this.model.text))\n                    this.render();\n            });\n    }\n    connect_signals() {\n        super.connect_signals();\n        this.connect(this.model.change, () => {\n            this.render();\n        });\n    }\n    has_math_disabled() {\n        return this.model.disable_math || !this.contains_tex_string(this.model.text);\n    }\n    render() {\n        super.render();\n        set_size(this.el, this.model);\n        this.container = (0, dom_1.div)();\n        set_size(this.container, this.model, false);\n        this.shadow_el.appendChild(this.container);\n        if (this.provider.status == \"failed\" || this.provider.status == \"loaded\")\n            this._has_finished = true;\n    }\n}\nexports.PanelMarkupView = PanelMarkupView;\nPanelMarkupView.__name__ = \"PanelMarkupView\";\nfunction set_size(el, model, adjustMargin = true) {\n    let width_policy = model.width != null ? \"fixed\" : \"fit\";\n    let height_policy = model.height != null ? \"fixed\" : \"fit\";\n    const { sizing_mode, margin } = model;\n    if (sizing_mode != null) {\n        if (sizing_mode == \"fixed\")\n            width_policy = height_policy = \"fixed\";\n        else if (sizing_mode == \"stretch_both\")\n            width_policy = height_policy = \"max\";\n        else if (sizing_mode == \"stretch_width\")\n            width_policy = \"max\";\n        else if (sizing_mode == \"stretch_height\")\n            height_policy = \"max\";\n        else {\n            switch (sizing_mode) {\n                case \"scale_width\":\n                    width_policy = \"max\";\n                    height_policy = \"min\";\n                    break;\n                case \"scale_height\":\n                    width_policy = \"min\";\n                    height_policy = \"max\";\n                    break;\n                case \"scale_both\":\n                    width_policy = \"max\";\n                    height_policy = \"max\";\n                    break;\n                default:\n                    throw new Error(\"unreachable\");\n            }\n        }\n    }\n    let wm, hm;\n    if (!adjustMargin) {\n        hm = wm = 0;\n    }\n    else if ((0, types_1.isArray)(margin)) {\n        if (margin.length === 4) {\n            hm = margin[0] + margin[2];\n            wm = margin[1] + margin[3];\n        }\n        else {\n            hm = margin[0] * 2;\n            wm = margin[1] * 2;\n        }\n    }\n    else if (margin == null) {\n        hm = wm = 0;\n    }\n    else {\n        wm = hm = margin * 2;\n    }\n    if (width_policy == \"fixed\" && model.width)\n        el.style.width = model.width + \"px\";\n    else if (width_policy == \"max\")\n        el.style.width = wm ? `calc(100% - ${wm}px)` : \"100%\";\n    if (model.min_width != null)\n        el.style.minWidth = model.min_width + \"px\";\n    if (model.max_width != null)\n        el.style.maxWidth = model.max_width + \"px\";\n    if (height_policy == \"fixed\" && model.height)\n        el.style.height = model.height + \"px\";\n    else if (height_policy == \"max\")\n        el.style.height = hm ? `calc(100% - ${hm}px)` : \"100%\";\n    if (model.min_height != null)\n        el.style.minHeight = model.min_height + \"px\";\n    if (model.max_width != null)\n        el.style.maxHeight = model.max_height + \"px\";\n}\nexports.set_size = set_size;\nclass HTMLBoxView extends layout_dom_1.LayoutDOMView {\n    render() {\n        super.render();\n        set_size(this.el, this.model);\n    }\n    watch_stylesheets() {\n        this._initialized_stylesheets = {};\n        for (const sts of this._applied_stylesheets) {\n            const style_el = sts.el;\n            if (style_el instanceof HTMLLinkElement) {\n                this._initialized_stylesheets[style_el.href] = false;\n                style_el.addEventListener(\"load\", () => {\n                    this._initialized_stylesheets[style_el.href] = true;\n                    if (Object.values(this._initialized_stylesheets).every(Boolean))\n                        this.style_redraw();\n                });\n            }\n        }\n    }\n    style_redraw() {\n    }\n    get child_models() {\n        return [];\n    }\n}\nexports.HTMLBoxView = HTMLBoxView;\nHTMLBoxView.__name__ = \"HTMLBoxView\";\nclass HTMLBox extends layout_dom_1.LayoutDOM {\n    constructor(attrs) {\n        super(attrs);\n    }\n}\nexports.HTMLBox = HTMLBox;\nHTMLBox.__name__ = \"HTMLBox\";\n//# sourceMappingURL=layout.js.map\n",
                 "type": "js"
             }
```

### Comparing `panel-jstree-0.1.0/src/panel_jstree/dist/panel_jstree.min.js` & `panel-jstree-0.1.1/src/panel_jstree/dist/panel_jstree.min.js`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/package-lock.json` & `panel-jstree-0.1.1/src/panel_jstree/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9161931818181818%*

 * *Differences: {"'packages'": "{'': {'version': '0.1.1'}}", "'version'": "'0.1.1'"}*

```diff
@@ -68,15 +68,15 @@
         "": {
             "dependencies": {
                 "@bokeh/bokehjs": "^3.1",
                 "@holoviz/panel": "^1"
             },
             "license": "MIT",
             "name": "panel_jstree",
-            "version": "0.1.0"
+            "version": "0.1.1"
         },
         "node_modules/@bokeh/bokehjs": {
             "engines": {
                 "node": ">=16.0",
                 "npm": ">=8.0"
             },
             "integrity": "sha512-+S3hqhIaOS17Xp0Oy7fB+hhOPe+v3jeIew40sWaH4/DEEMuUmhDZZMFowWhicuwTN9J6Bay9bp/62YJc5Na1Qg==",
@@ -141,9 +141,9 @@
             },
             "integrity": "sha512-4oh2sf208mKAdL5AQtzXxE387iSGNWMX/YjwMjH6m/XROILKAmx5Pbs2FsXrW7ixoVGGjpfYSBB833vOwYxNxw==",
             "resolved": "https://registry.npmjs.org/preact/-/preact-10.14.0.tgz",
             "version": "10.14.0"
         }
     },
     "requires": true,
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `panel-jstree-0.1.0/src/panel_jstree/tsconfig.json` & `panel-jstree-0.1.1/src/panel_jstree/tsconfig.json`

 * *Files identical despite different names*

### Comparing `panel-jstree-0.1.0/src/panel_jstree/widgets/jstree.py` & `panel-jstree-0.1.1/src/panel_jstree/widgets/jstree.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 from a list of options.
 """
 from __future__ import annotations
 
 import copy
 import logging
 import os
-
 from pathlib import Path
-from typing import (
-    AnyStr, TYPE_CHECKING, ClassVar, Type, Any, Optional
-)
+from typing import TYPE_CHECKING, Any, AnyStr, ClassVar, Optional, Type
 
 import param
-
-from panel.widgets.base import Widget
 from panel.util import fullpath
+from panel.widgets.base import Widget
 from panel.widgets.file_selector import _scan_path
+
 from ..bokeh_extensions.jstree import jsTreePlot
 
 if TYPE_CHECKING:
     from bokeh.model import Model
 
 logger = logging.getLogger(__file__)
 
@@ -29,30 +26,38 @@
 class _TreeBase(Widget):
     """
     jsTree widget allow editing a tree in an jsTree editor.
     """
 
     value = param.List(default=[], doc="List of currently selected leaves and nodes")
 
-    data = param.List(default=[], doc="Hierarchical tree structure of data. See "
-                                      " `jsTree <https://www.jstree.com>`_ for more"
-                                      " details on formatting")
-
-    select_multiple = param.Boolean(default=True, doc="Whether multiple nodes can be selected or not")
-
-    show_icons = param.Boolean(default=True, doc="""
-        Whether to use icons or not""")
-
-    show_dots = param.Boolean(default=True, doc="Whether to show dots on the left as part of the tree")
+    data = param.List(
+        default=[],
+        doc="Hierarchical tree structure of data. See "
+        " `jsTree <https://www.jstree.com>`_ for more"
+        " details on formatting",
+    )
+
+    select_multiple = param.Boolean(
+        default=True, doc="Whether multiple nodes can be selected or not"
+    )
+
+    show_icons = param.Boolean(default=True, doc="Whether to use icons or not")
+
+    show_dots = param.Boolean(
+        default=True, doc="Whether to show dots on the left as part of the tree"
+    )
 
     checkbox = param.Boolean(default=True, doc="Whether to to use checkboxes as selectables")
 
-    plugins = param.List(doc="Configure which additional plugins will be active. "
-                             "Should be an array of strings, where each element is a plugin name that are passed"
-                             "to jsTree.")
+    plugins = param.List(
+        doc="Configure which additional plugins will be active. "
+        "Should be an array of strings, where each element is a plugin name that are passed"
+        "to jsTree."
+    )
 
     _last_opened = param.Dict(doc="last opened node")
 
     _new_nodes = param.List(doc="Children to push to tree")
 
     _flat_tree = param.List(doc="Flat representation of tree")
 
@@ -75,30 +80,36 @@
         parameter value and bokeh model change. By default uses the
         _rename class level attribute to map between parameter and
         property names.
         """
         properties = super()._process_param_change(msg)
 
         properties.pop("title", None)
-        if not properties.get("height") and (self.sizing_mode is None or "width" in self.sizing_mode):
+        if not properties.get("height") and (
+            self.sizing_mode is None or "width" in self.sizing_mode
+        ):
             properties["height"] = 400
         if properties.get("height") and properties["height"] < 100:
             properties["height"] = 100
 
         if properties.pop("checkbox", None):
             properties.get("plugins", []).append("checkbox")
 
         properties["value"] = self._values
         return properties
 
 
 class FileTree(_TreeBase):
     """"""
-    directory = param.String(default=str(Path.cwd()), doc="""
-        The directory to explore.""")
+
+    directory = param.String(
+        default=str(Path.cwd()),
+        doc="""
+        The directory to explore.""",
+    )
 
     def _process_param_change(self, msg: dict[str, Any]) -> dict[str, Any]:
         """
         Transform parameter changes into bokeh model property updates.
         Should be overridden to provide appropriate mapping between
         parameter value and bokeh model change. By default uses the
         _rename class level attribute to map between parameter and
@@ -106,15 +117,15 @@
         """
         msg = super()._process_param_change(msg)
         msg.pop("directory", None)
         return msg
 
     def __init__(self, directory: AnyStr | os.PathLike | None = None, **params):
         if directory is not None:
-            params['directory'] = fullpath(directory)
+            params["directory"] = fullpath(directory)
         self._file_icon = "jstree-file"
         self._folder_icon = "jstree-folder"
         super().__init__(**params)
         self.data = self._get_child_json(self.directory, depth=1)
         self.param.watch(self._add_node_children, "_last_opened")
         self.param.watch(self._new_nodes_on_value_update, "value")
 
@@ -125,78 +136,96 @@
                 if Path(node["id"]) == Path(value):
                     break
                 if Path(node["id"]) in parents:
                     node.setdefault("state", {})["opened"] = True
                     if node.get("children"):
                         transverse(node["children"], value)
                     else:
-                        node["children"] = self._get_child_json(node["id"], add_parent=True, state={"opened": True}, depth=2)
-                        [transverse([n], value) for n in node["children"] if Path(n["id"]) in parents]
+                        node["children"] = self._get_child_json(
+                            node["id"], add_parent=True, state={"opened": True}, depth=2
+                        )
+                        [
+                            transverse([n], value)
+                            for n in node["children"]
+                            if Path(n["id"]) in parents
+                        ]
                     break
 
         ids = [node["id"] for node in self._flat_tree]
         values = [value for value in self._values if value not in ids]
         if values:
             data = copy.deepcopy(event.obj.data[:])
 
             for value in values:
                 transverse(data, value)
             self.data = data
 
-    def _add_node_children(self, event: param.parameterized.Event = None, dirs = None, **kwargs):
+    def _add_node_children(self, event: param.parameterized.Event = None, dirs=None, **kwargs):
         new_nodes = []
         kw = {}
         if not dirs:
             if event:
                 nodes_already_sent = event.new.get("children_d", [])
                 dirs = event.new["children"]
-                kw = dict(add_parent=True, children_to_skip=nodes_already_sent, )
+                kw = dict(
+                    add_parent=True,
+                    children_to_skip=nodes_already_sent,
+                )
             else:
                 dirs = [self.directory]
                 kw = dict(depth=1)
         for dir_ in dirs:
             children = self._get_child_json(dir_, **{**kwargs, **kw})
             if children:
                 new_nodes.extend(children)
         self._new_nodes = new_nodes
 
-
-    def _get_child_json(self, directory: str, add_parent=False, depth=0, children_to_skip=(), **kwargs):
+    def _get_child_json(
+        self, directory: str, add_parent=False, depth=0, children_to_skip=(), **kwargs
+    ):
         directory = str(directory)
         parent = directory if add_parent else None
         jsn = []
         if not os.path.isdir(directory):
             return []
         dirs, files = self._get_paths(directory, children_to_skip=children_to_skip)
         for dir in dirs:
             if depth > 0:
                 children = self._get_child_json(dir, add_parent=add_parent, depth=depth - 1)
             else:
                 children = None
-            jsn.append(self._get_json(dir, parent=parent, children=children, icon=self._folder_icon, **kwargs))
-        jsn.extend(self._get_json(file, parent=parent, icon=self._file_icon, **kwargs) for file in files)
+            jsn.append(
+                self._get_json(
+                    dir, parent=parent, children=children, icon=self._folder_icon, **kwargs
+                )
+            )
+        jsn.extend(
+            self._get_json(file, parent=parent, icon=self._file_icon, **kwargs) for file in files
+        )
         return jsn
 
     @staticmethod
     def _get_paths(directory, children_to_skip=()):
-        dirs_, files = _scan_path(directory, file_pattern='[!.]*')
+        dirs_, files = _scan_path(directory, file_pattern="[!.]*")
         dirs = []
         for d in dirs_:
             if not Path(d).name.startswith(".") and d not in children_to_skip:
                 try:
                     if os.listdir(d):
                         dirs.append(d)
                 except OSError as e:
                     print(repr(e), d)
 
         # dirs = [d for d in dirs if not Path(d).name.startswith(".") and d not in children_to_skip]
         files = [f for f in files if f not in children_to_skip]
         return dirs, files
 
-    def _get_json(self, txt, parent: str = None, children: Optional[list] = None, icon: str = None, **kwargs):
+    def _get_json(
+        self, txt, parent: str = None, children: Optional[list] = None, icon: str = None, **kwargs
+    ):
         jsn = dict(id=txt, text=Path(txt).name, **kwargs)
         if parent:
             jsn["parent"] = parent
         if children:
             jsn["children"] = children
         if icon:
             jsn["icon"] = icon
```

### Comparing `panel-jstree-0.1.0/src/panel_jstree.egg-info/PKG-INFO` & `panel-jstree-0.1.1/src/panel_jstree.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panel-jstree
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: madeline-scyphers
 License: MIT License
         
         Copyright (c) 2023 Madeline Scyphers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,47 +67,28 @@
 You can install and use the package as simple as.
 
 ```bash
 pip install panel-jstree
 ```
 
 ```python
-import panel_jstree
-INSERT A SHORT EXAMPLE
+import panel as pn
+from panel_jstree import FileTree
+
+pn.Column(FileTree())
 ```
 
 ![Project Intro](assets/videos/project-intro.gif)
 
-REPLACE THE INTRO VIDEO
-
 ## 🚀 Get started in under a minute
 
-Install `panel-jstree` including the *`examples` dependencies*.
-
-```bash
-pip install  panel-jstree[examples]
-```
-
-Explore the sample apps
-
 ```bash
-pn hello panel-jstree
+pip install  panel-jstree
 ```
 
-![Project Intro](https://raw.githubusercontent.com/madeline-scyphers/panel-jstree/main/assets/videos/pn-hello-panel-jstree.gif)
-
-You can now find the *reference* and *gallery* notebooks in the `examples/madeline-scyphers/panel-jstree` folder. Check them out by running `jupyter lab`.
-
-## 📒 Explore the examples online
-
-Click one of the buttons
-
-[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/madeline-scyphers/panel-jstree/tree/main/examples/)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/madeline-scyphers/panel-jstree/HEAD)
-
 ## ⭐ Support
 
 Please support [Panel](https://panel.holoviz.org) and
 [awesome-panel](https://awesome-panel.org) by giving the projects a star on Github:
 
 - [holoviz/panel](https://github.com/holoviz/panel).
 - [awesome-panel/awesome-panel](https://github.com/awesome-panel/awesome-panel).
@@ -121,11 +102,10 @@
 I would love to support and receive your contributions. Thanks.
 
 [![Hacktober Fest](https://github.blog/wp-content/uploads/2022/10/hacktoberfestbanner.jpeg?fit=1200%2C630)](https://github.com/madeline-scyphers/panel-jstree/issues).
 
 ## Monitor
 
 [![PyPI version](https://badge.fury.io/py/panel-jstree.svg)](https://pypi.org/project/panel-jstree/)
-[![Downloads](https://pepy.tech/badge/panel-jstree/month)](https://pepy.tech/project/panel-jstree)
-![Python Versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
+![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)
 [![License](https://img.shields.io/badge/License-MIT%202.0-blue.svg)](https://opensource.org/licenses/MIT)
-![Test Results](https://github.com/madeline-scyphers/panel-jstree/actions/workflows/tests.yaml/badge.svg?branch=main)
+
```

### Comparing `panel-jstree-0.1.0/src/panel_jstree.egg-info/SOURCES.txt` & `panel-jstree-0.1.1/src/panel_jstree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

