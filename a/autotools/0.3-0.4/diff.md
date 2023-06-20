# Comparing `tmp/autotools-0.3.tar.gz` & `tmp/autotools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotools-0.3.tar", last modified: Tue Jun 20 17:11:44 2023, max compression
+gzip compressed data, was "autotools-0.4.tar", last modified: Tue Jun 20 17:16:22 2023, max compression
```

## Comparing `autotools-0.3.tar` & `autotools-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 17:11:44.357699 autotools-0.3/
--rw-rw-rw-   0        0        0      252 2023-06-20 17:11:44.355668 autotools-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 17:11:44.300441 autotools-0.3/autotools/
--rw-rw-rw-   0        0        0      637 2023-06-20 17:04:47.000000 autotools-0.3/autotools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:11:44.351670 autotools-0.3/autotools.egg-info/
--rw-rw-rw-   0        0        0      252 2023-06-20 17:11:43.000000 autotools-0.3/autotools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-20 17:11:44.000000 autotools-0.3/autotools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 17:11:43.000000 autotools-0.3/autotools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 17:11:43.000000 autotools-0.3/autotools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-20 17:11:43.000000 autotools-0.3/autotools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 17:11:44.358695 autotools-0.3/setup.cfg
--rw-rw-rw-   0        0        0      369 2023-06-20 17:07:53.000000 autotools-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:16:22.090422 autotools-0.4/
+-rw-rw-rw-   0        0        0      324 2023-06-20 17:16:22.074795 autotools-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 17:16:22.027457 autotools-0.4/autotools/
+-rw-rw-rw-   0        0        0      637 2023-06-20 17:04:47.000000 autotools-0.4/autotools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:16:22.074795 autotools-0.4/autotools.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-20 17:16:21.000000 autotools-0.4/autotools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 17:16:22.090422 autotools-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      467 2023-06-20 17:16:14.000000 autotools-0.4/setup.py
```

### Comparing `autotools-0.3/autotools/__init__.py` & `autotools-0.4/autotools/__init__.py`

 * *Files identical despite different names*

