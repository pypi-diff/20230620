# Comparing `tmp/reliableGPT-0.1.5.tar.gz` & `tmp/reliableGPT-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/reliableGPT-0.1.5.tar", last modified: Tue Jun 20 06:43:39 2023, max compression
+gzip compressed data, was "dist/reliableGPT-0.1.6.tar", last modified: Tue Jun 20 06:46:47 2023, max compression
```

## Comparing `reliableGPT-0.1.5.tar` & `reliableGPT-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:43:39.709760 reliableGPT-0.1.5/
--rw-r--r--   0 daddyish   (501) staff       (20)     1065 2023-06-20 01:36:38.000000 reliableGPT-0.1.5/LICENSE
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 06:43:39.709549 reliableGPT-0.1.5/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)       13 2023-06-20 01:36:38.000000 reliableGPT-0.1.5/README.md
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:43:39.708727 reliableGPT-0.1.5/reliableGPT.egg-info/
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 06:43:39.000000 reliableGPT-0.1.5/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)      265 2023-06-20 06:43:39.000000 reliableGPT-0.1.5/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 daddyish   (501) staff       (20)        1 2023-06-20 06:43:39.000000 reliableGPT-0.1.5/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       24 2023-06-20 06:43:39.000000 reliableGPT-0.1.5/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       12 2023-06-20 06:43:39.000000 reliableGPT-0.1.5/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:43:39.709277 reliableGPT-0.1.5/reliablegpt/
--rw-r--r--   0 daddyish   (501) staff       (20)       87 2023-06-20 01:42:39.000000 reliableGPT-0.1.5/reliablegpt/__init__.py
--rw-r--r--   0 daddyish   (501) staff       (20)     4095 2023-06-20 06:40:45.000000 reliableGPT-0.1.5/reliablegpt/main.py
--rw-r--r--   0 daddyish   (501) staff       (20)     2111 2023-06-20 06:41:07.000000 reliableGPT-0.1.5/reliablegpt/tests.py
--rw-r--r--   0 daddyish   (501) staff       (20)       38 2023-06-20 06:43:39.709804 reliableGPT-0.1.5/setup.cfg
--rw-r--r--   0 daddyish   (501) staff       (20)      293 2023-06-20 06:43:34.000000 reliableGPT-0.1.5/setup.py
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:46:47.705878 reliableGPT-0.1.6/
+-rw-r--r--   0 daddyish   (501) staff       (20)     1065 2023-06-20 01:36:38.000000 reliableGPT-0.1.6/LICENSE
+-rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 06:46:47.705685 reliableGPT-0.1.6/PKG-INFO
+-rw-r--r--   0 daddyish   (501) staff       (20)       13 2023-06-20 01:36:38.000000 reliableGPT-0.1.6/README.md
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:46:47.704638 reliableGPT-0.1.6/reliableGPT.egg-info/
+-rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 daddyish   (501) staff       (20)      265 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)        1 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)       24 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)       12 2023-06-20 06:46:47.000000 reliableGPT-0.1.6/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 06:46:47.705344 reliableGPT-0.1.6/reliablegpt/
+-rw-r--r--   0 daddyish   (501) staff       (20)       87 2023-06-20 01:42:39.000000 reliableGPT-0.1.6/reliablegpt/__init__.py
+-rw-r--r--   0 daddyish   (501) staff       (20)     4095 2023-06-20 06:40:45.000000 reliableGPT-0.1.6/reliablegpt/main.py
+-rw-r--r--   0 daddyish   (501) staff       (20)     2111 2023-06-20 06:41:07.000000 reliableGPT-0.1.6/reliablegpt/tests.py
+-rw-r--r--   0 daddyish   (501) staff       (20)       38 2023-06-20 06:46:47.705922 reliableGPT-0.1.6/setup.cfg
+-rw-r--r--   0 daddyish   (501) staff       (20)      293 2023-06-20 06:46:42.000000 reliableGPT-0.1.6/setup.py
```

### Comparing `reliableGPT-0.1.5/LICENSE` & `reliableGPT-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.1.5/reliablegpt/main.py` & `reliableGPT-0.1.6/reliablegpt/main.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.1.5/reliablegpt/tests.py` & `reliableGPT-0.1.6/reliablegpt/tests.py`

 * *Files identical despite different names*

