# Comparing `tmp/nbsite-0.8.1a5.tar.gz` & `tmp/nbsite-0.8.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbsite-0.8.1a5.tar", last modified: Thu Jun 15 10:53:19 2023, max compression
+gzip compressed data, was "nbsite-0.8.1a6.tar", last modified: Tue Jun 20 16:35:15 2023, max compression
```

## Comparing `nbsite-0.8.1a5.tar` & `nbsite-0.8.1a6.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.039406 nbsite-0.8.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-15 10:53:19.039406 nbsite-0.8.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.031406 nbsite-0.8.1a5/nbsite/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 10:53:18.000000 nbsite-0.8.1a5/nbsite/.version
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.035406 nbsite-0.8.1a5/nbsite/_shared_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/alert.css
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/dataframe.css
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/gallery.css
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/holoviz-icon-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/mystnb.css
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/nbsite.css
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/notebook.css
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_static/scroller.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.035406 nbsite-0.8.1a5/nbsite/_shared_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_templates/copyright-last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/_shared_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.035406 nbsite-0.8.1a5/nbsite/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/gallery/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/gallery/thumbnailer.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/ipystartup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18133 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/nbbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/paramdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.035406 nbsite-0.8.1a5/nbsite/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/ServiceHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/ServiceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/WebWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/WorkerHandler.js
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.035406 nbsite-0.8.1a5/nbsite/pyodide/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/_static/run_cell.js
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/_static/runbutton.css
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/pyodide/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/shared_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.031406 nbsite-0.8.1a5/nbsite/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.039406 nbsite-0.8.1a5/nbsite/templates/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/templates/basic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/templates/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/templates/basic/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.039406 nbsite-0.8.1a5/nbsite/templates/holoviz/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/templates/holoviz/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/templates/holoviz/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/templates/holoviz/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/templates/holoviz/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.039406 nbsite-0.8.1a5/nbsite/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/nbsite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.035406 nbsite-0.8.1a5/nbsite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-15 10:53:18.000000 nbsite-0.8.1a5/nbsite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-15 10:53:19.000000 nbsite-0.8.1a5/nbsite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:53:18.000000 nbsite-0.8.1a5/nbsite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 10:53:18.000000 nbsite-0.8.1a5/nbsite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:53:18.000000 nbsite-0.8.1a5/nbsite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 10:53:18.000000 nbsite-0.8.1a5/nbsite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:53:19.039406 nbsite-0.8.1a5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/scripts/nbsite_cleandisthtml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/scripts/nbsite_fix_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/scripts/nbsite_from_tmplate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11126 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/scripts/nbsite_generate_modules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/scripts/nbsite_nbpagebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-15 10:53:19.039406 nbsite-0.8.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-15 10:52:24.000000 nbsite-0.8.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.251068 nbsite-0.8.1a6/nbsite/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite/_shared_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/alert.css
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/dataframe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/gallery.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/holoviz-icon-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/mystnb.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/nbsite.css
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/notebook.css
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_static/scroller.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite/_shared_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/copyright-last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/github-stars-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/_shared_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/gallery/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/gallery/thumbnailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/ipystartup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18133 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/nbbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/paramdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 16:34:08.000000 nbsite-0.8.1a6/nbsite/pyodide/ServiceHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/ServiceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/WebWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/WorkerHandler.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/pyodide/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/_static/run_cell.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/_static/runbutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/pyodide/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/shared_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.251068 nbsite-0.8.1a6/nbsite/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/templates/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/basic/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/templates/holoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/templates/holoviz/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.259068 nbsite-0.8.1a6/nbsite/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/nbsite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.255068 nbsite-0.8.1a6/nbsite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:35:15.000000 nbsite-0.8.1a6/nbsite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_cleandisthtml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5851 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_fix_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_from_tmplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11126 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_generate_modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/scripts/nbsite_nbpagebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-20 16:35:15.263069 nbsite-0.8.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-20 16:34:09.000000 nbsite-0.8.1a6/setup.py
```

### Comparing `nbsite-0.8.1a5/LICENSE.txt` & `nbsite-0.8.1a6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/PKG-INFO` & `nbsite-0.8.1a6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.1a5
+Version: 0.8.1a6
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
@@ -21,26 +21,26 @@
 Description-Content-Type: text/markdown
 Provides-Extra: refman
 Provides-Extra: gallery
 Provides-Extra: tests
 Provides-Extra: build
 License-File: LICENSE.txt
 
-<img src="https://github.com/pyviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
+<img src="https://github.com/holoviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
 
 # NBSite: Build a tested, sphinx-based website from notebooks
 
 |    |    |
 | --- | --- |
-| Build Status | [![Build Status](https://github.com/pyviz-dev/nbsite/workflows/tests/badge.svg)](https://github.com/pyviz-dev/nbsite/actions?query=workflow%3Atests)
-| Coverage | [![codecov](https://codecov.io/gh/pyviz-dev/nbsite/branch/main/graph/badge.svg)](https://codecov.io/gh/pyviz-dev/nbsite) |
-| Latest dev release | [![Github tag](https://img.shields.io/github/tag/pyviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/pyviz-dev/nbsite/tags) [![dev-site](https://img.shields.io/website-up-down-green-red/https/pyviz-dev.github.io/nbsite-dev.svg?label=dev%20website)](https://pyviz-dev.github.io/nbsite-dev/)|
-| Latest release | [![Github release](https://img.shields.io/github/release/pyviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/pyviz-dev/nbsite/releases) [![PyPI version](https://img.shields.io/pypi/v/nbsite.svg?colorB=cc77dd)](https://pypi.python.org/pypi/nbsite) [![nbsite version](https://img.shields.io/conda/v/pyviz/nbsite.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/nbsite) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/nbsite.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/nbsite) [![defaults version](https://img.shields.io/conda/v/anaconda/nbsite.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/nbsite) |
+| Build Status | [![Build Status](https://github.com/holoviz-dev/nbsite/workflows/tests/badge.svg)](https://github.com/holoviz-dev/nbsite/actions?query=workflow%3Atests)
+| Coverage | [![codecov](https://codecov.io/gh/holoviz-dev/nbsite/branch/main/graph/badge.svg)](https://codecov.io/gh/holoviz-dev/nbsite) |
+| Latest dev release | [![Github tag](https://img.shields.io/github/tag/holoviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz-dev/nbsite/tags) [![dev-site](https://img.shields.io/website-up-down-green-red/https/holoviz-dev.github.io/nbsite-dev.svg?label=dev%20website)](https://holoviz-dev.github.io/nbsite-dev/)|
+| Latest release | [![Github release](https://img.shields.io/github/release/holoviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz-dev/nbsite/releases) [![PyPI version](https://img.shields.io/pypi/v/nbsite.svg?colorB=cc77dd)](https://pypi.python.org/pypi/nbsite) [![nbsite version](https://img.shields.io/conda/v/pyviz/nbsite.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/nbsite) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/nbsite.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/nbsite) [![defaults version](https://img.shields.io/conda/v/anaconda/nbsite.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/nbsite) |
 | Docs | [![gh-pages](https://img.shields.io/github/last-commit/pyviz/nbsite/gh-pages.svg)](https://github.com/pyviz/nbsite/tree/gh-pages) [![site](https://img.shields.io/website-up-down-green-red/https/nbsite.pyviz.org.svg)](https://nbsite.pyviz.org) |
 
 ---
 
 **DISCLAIMER**
 
 NBSite is a tool supporting the developers of the [HoloViz](https://holoviz/org) project. As such it is tailored to their use case, workflow, and **breaking changes may occur at any time**. We suggest that before using NBSite you investigate alternatives such as [MyST-NB](https://myst-nb.readthedocs.io) or [nbsphinx](https://nbsphinx.readthedocs.io/). If you select NBSite anyway, we recommend that you pin its version.
```

### Comparing `nbsite-0.8.1a5/README.md` & `nbsite-0.8.1a6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-<img src="https://github.com/pyviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
+<img src="https://github.com/holoviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
 
 # NBSite: Build a tested, sphinx-based website from notebooks
 
 |    |    |
 | --- | --- |
-| Build Status | [![Build Status](https://github.com/pyviz-dev/nbsite/workflows/tests/badge.svg)](https://github.com/pyviz-dev/nbsite/actions?query=workflow%3Atests)
-| Coverage | [![codecov](https://codecov.io/gh/pyviz-dev/nbsite/branch/main/graph/badge.svg)](https://codecov.io/gh/pyviz-dev/nbsite) |
-| Latest dev release | [![Github tag](https://img.shields.io/github/tag/pyviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/pyviz-dev/nbsite/tags) [![dev-site](https://img.shields.io/website-up-down-green-red/https/pyviz-dev.github.io/nbsite-dev.svg?label=dev%20website)](https://pyviz-dev.github.io/nbsite-dev/)|
-| Latest release | [![Github release](https://img.shields.io/github/release/pyviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/pyviz-dev/nbsite/releases) [![PyPI version](https://img.shields.io/pypi/v/nbsite.svg?colorB=cc77dd)](https://pypi.python.org/pypi/nbsite) [![nbsite version](https://img.shields.io/conda/v/pyviz/nbsite.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/nbsite) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/nbsite.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/nbsite) [![defaults version](https://img.shields.io/conda/v/anaconda/nbsite.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/nbsite) |
+| Build Status | [![Build Status](https://github.com/holoviz-dev/nbsite/workflows/tests/badge.svg)](https://github.com/holoviz-dev/nbsite/actions?query=workflow%3Atests)
+| Coverage | [![codecov](https://codecov.io/gh/holoviz-dev/nbsite/branch/main/graph/badge.svg)](https://codecov.io/gh/holoviz-dev/nbsite) |
+| Latest dev release | [![Github tag](https://img.shields.io/github/tag/holoviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz-dev/nbsite/tags) [![dev-site](https://img.shields.io/website-up-down-green-red/https/holoviz-dev.github.io/nbsite-dev.svg?label=dev%20website)](https://holoviz-dev.github.io/nbsite-dev/)|
+| Latest release | [![Github release](https://img.shields.io/github/release/holoviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz-dev/nbsite/releases) [![PyPI version](https://img.shields.io/pypi/v/nbsite.svg?colorB=cc77dd)](https://pypi.python.org/pypi/nbsite) [![nbsite version](https://img.shields.io/conda/v/pyviz/nbsite.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/nbsite) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/nbsite.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/nbsite) [![defaults version](https://img.shields.io/conda/v/anaconda/nbsite.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/nbsite) |
 | Docs | [![gh-pages](https://img.shields.io/github/last-commit/pyviz/nbsite/gh-pages.svg)](https://github.com/pyviz/nbsite/tree/gh-pages) [![site](https://img.shields.io/website-up-down-green-red/https/nbsite.pyviz.org.svg)](https://nbsite.pyviz.org) |
 
 ---
 
 **DISCLAIMER**
 
 NBSite is a tool supporting the developers of the [HoloViz](https://holoviz/org) project. As such it is tailored to their use case, workflow, and **breaking changes may occur at any time**. We suggest that before using NBSite you investigate alternatives such as [MyST-NB](https://myst-nb.readthedocs.io) or [nbsphinx](https://nbsphinx.readthedocs.io/). If you select NBSite anyway, we recommend that you pin its version.
```

### Comparing `nbsite-0.8.1a5/nbsite/__main__.py` & `nbsite-0.8.1a6/nbsite/__main__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_static/alert.css` & `nbsite-0.8.1a6/nbsite/_shared_static/alert.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_static/dataframe.css` & `nbsite-0.8.1a6/nbsite/_shared_static/dataframe.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_static/holoviz-icon-white.svg` & `nbsite-0.8.1a6/nbsite/_shared_static/holoviz-icon-white.svg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_static/mystnb.css` & `nbsite-0.8.1a6/nbsite/_shared_static/mystnb.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_static/nbsite.css` & `nbsite-0.8.1a6/nbsite/_shared_static/nbsite.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_static/notebook.css` & `nbsite-0.8.1a6/nbsite/_shared_static/notebook.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_static/scroller.css` & `nbsite-0.8.1a6/nbsite/_shared_static/scroller.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_templates/copyright-last-updated.html` & `nbsite-0.8.1a6/nbsite/_shared_templates/copyright-last-updated.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/_shared_templates/layout.html` & `nbsite-0.8.1a6/nbsite/_shared_templates/layout.html`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/cmd.py` & `nbsite-0.8.1a6/nbsite/cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/gallery/gen.py` & `nbsite-0.8.1a6/nbsite/gallery/gen.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/gallery/thumbnailer.py` & `nbsite-0.8.1a6/nbsite/gallery/thumbnailer.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/nbbuild.py` & `nbsite-0.8.1a6/nbsite/nbbuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/paramdoc.py` & `nbsite-0.8.1a6/nbsite/paramdoc.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/pyodide/ServiceWorker.js` & `nbsite-0.8.1a6/nbsite/pyodide/ServiceWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/pyodide/WebWorker.js` & `nbsite-0.8.1a6/nbsite/pyodide/WebWorker.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/pyodide/WorkerHandler.js` & `nbsite-0.8.1a6/nbsite/pyodide/WorkerHandler.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/pyodide/__init__.py` & `nbsite-0.8.1a6/nbsite/pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/pyodide/_static/run_cell.js` & `nbsite-0.8.1a6/nbsite/pyodide/_static/run_cell.js`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/pyodide/_static/runbutton.css` & `nbsite-0.8.1a6/nbsite/pyodide/_static/runbutton.css`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/pyodide/site.webmanifest` & `nbsite-0.8.1a6/nbsite/pyodide/site.webmanifest`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/shared_conf.py` & `nbsite-0.8.1a6/nbsite/shared_conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/templates/basic/conf.py` & `nbsite-0.8.1a6/nbsite/templates/basic/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/templates/holoviz/conf.py` & `nbsite-0.8.1a6/nbsite/templates/holoviz/conf.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/tests/test_cmd.py` & `nbsite-0.8.1a6/nbsite/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/tests/test_util.py` & `nbsite-0.8.1a6/nbsite/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite/util.py` & `nbsite-0.8.1a6/nbsite/util.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/nbsite.egg-info/PKG-INFO` & `nbsite-0.8.1a6/nbsite.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbsite
-Version: 0.8.1a5
+Version: 0.8.1a6
 Summary: Build a tested, sphinx-based website from notebooks.
 Home-page: https://nbsite.holoviz.org
 Author: HoloViz developers
 Author-email: developers@holoviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-3
@@ -21,26 +21,26 @@
 Description-Content-Type: text/markdown
 Provides-Extra: refman
 Provides-Extra: gallery
 Provides-Extra: tests
 Provides-Extra: build
 License-File: LICENSE.txt
 
-<img src="https://github.com/pyviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
+<img src="https://github.com/holoviz-dev/nbsite/raw/main/site/doc/_static/nbsite-logo.png" height=150><br>
 
 -----------------
 
 # NBSite: Build a tested, sphinx-based website from notebooks
 
 |    |    |
 | --- | --- |
-| Build Status | [![Build Status](https://github.com/pyviz-dev/nbsite/workflows/tests/badge.svg)](https://github.com/pyviz-dev/nbsite/actions?query=workflow%3Atests)
-| Coverage | [![codecov](https://codecov.io/gh/pyviz-dev/nbsite/branch/main/graph/badge.svg)](https://codecov.io/gh/pyviz-dev/nbsite) |
-| Latest dev release | [![Github tag](https://img.shields.io/github/tag/pyviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/pyviz-dev/nbsite/tags) [![dev-site](https://img.shields.io/website-up-down-green-red/https/pyviz-dev.github.io/nbsite-dev.svg?label=dev%20website)](https://pyviz-dev.github.io/nbsite-dev/)|
-| Latest release | [![Github release](https://img.shields.io/github/release/pyviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/pyviz-dev/nbsite/releases) [![PyPI version](https://img.shields.io/pypi/v/nbsite.svg?colorB=cc77dd)](https://pypi.python.org/pypi/nbsite) [![nbsite version](https://img.shields.io/conda/v/pyviz/nbsite.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/nbsite) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/nbsite.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/nbsite) [![defaults version](https://img.shields.io/conda/v/anaconda/nbsite.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/nbsite) |
+| Build Status | [![Build Status](https://github.com/holoviz-dev/nbsite/workflows/tests/badge.svg)](https://github.com/holoviz-dev/nbsite/actions?query=workflow%3Atests)
+| Coverage | [![codecov](https://codecov.io/gh/holoviz-dev/nbsite/branch/main/graph/badge.svg)](https://codecov.io/gh/holoviz-dev/nbsite) |
+| Latest dev release | [![Github tag](https://img.shields.io/github/tag/holoviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz-dev/nbsite/tags) [![dev-site](https://img.shields.io/website-up-down-green-red/https/holoviz-dev.github.io/nbsite-dev.svg?label=dev%20website)](https://holoviz-dev.github.io/nbsite-dev/)|
+| Latest release | [![Github release](https://img.shields.io/github/release/holoviz-dev/nbsite.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz-dev/nbsite/releases) [![PyPI version](https://img.shields.io/pypi/v/nbsite.svg?colorB=cc77dd)](https://pypi.python.org/pypi/nbsite) [![nbsite version](https://img.shields.io/conda/v/pyviz/nbsite.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/nbsite) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/nbsite.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/nbsite) [![defaults version](https://img.shields.io/conda/v/anaconda/nbsite.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/nbsite) |
 | Docs | [![gh-pages](https://img.shields.io/github/last-commit/pyviz/nbsite/gh-pages.svg)](https://github.com/pyviz/nbsite/tree/gh-pages) [![site](https://img.shields.io/website-up-down-green-red/https/nbsite.pyviz.org.svg)](https://nbsite.pyviz.org) |
 
 ---
 
 **DISCLAIMER**
 
 NBSite is a tool supporting the developers of the [HoloViz](https://holoviz/org) project. As such it is tailored to their use case, workflow, and **breaking changes may occur at any time**. We suggest that before using NBSite you investigate alternatives such as [MyST-NB](https://myst-nb.readthedocs.io) or [nbsphinx](https://nbsphinx.readthedocs.io/). If you select NBSite anyway, we recommend that you pin its version.
```

### Comparing `nbsite-0.8.1a5/nbsite.egg-info/SOURCES.txt` & `nbsite-0.8.1a6/nbsite.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 nbsite/_shared_static/gallery.css
 nbsite/_shared_static/holoviz-icon-white.svg
 nbsite/_shared_static/mystnb.css
 nbsite/_shared_static/nbsite.css
 nbsite/_shared_static/notebook.css
 nbsite/_shared_static/scroller.css
 nbsite/_shared_templates/copyright-last-updated.html
+nbsite/_shared_templates/github-stars-button.html
 nbsite/_shared_templates/layout.html
 nbsite/_shared_templates/sidebar-nav-bs.html
 nbsite/gallery/__init__.py
 nbsite/gallery/gen.py
 nbsite/gallery/thumbnailer.py
 nbsite/pyodide/ServiceHandler.js
 nbsite/pyodide/ServiceWorker.js
```

### Comparing `nbsite-0.8.1a5/pyproject.toml` & `nbsite-0.8.1a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/scripts/nbsite_cleandisthtml.py` & `nbsite-0.8.1a6/scripts/nbsite_cleandisthtml.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/scripts/nbsite_fix_links.py` & `nbsite-0.8.1a6/scripts/nbsite_fix_links.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/scripts/nbsite_generate_modules.py` & `nbsite-0.8.1a6/scripts/nbsite_generate_modules.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/scripts/nbsite_nbpagebuild.py` & `nbsite-0.8.1a6/scripts/nbsite_nbpagebuild.py`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/setup.cfg` & `nbsite-0.8.1a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `nbsite-0.8.1a5/setup.py` & `nbsite-0.8.1a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         'beautifulsoup4',
         'jinja2',
         'pillow',
         'pydata-sphinx-theme >=0.13.3,<0.14',
         'myst-parser',
         'sphinx-copybutton',
         'sphinx-design',
+        'urllib3 <2.0.0',
     ],
     extras_require= {
         'refman':[
             'graphviz',
         ],
         'gallery':[
             'selenium',
```

