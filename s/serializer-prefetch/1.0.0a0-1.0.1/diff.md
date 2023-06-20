# Comparing `tmp/serializer_prefetch-1.0.0a0.tar.gz` & `tmp/serializer_prefetch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_prefetch-1.0.0a0.tar", last modified: Tue Jun 20 14:59:18 2023, max compression
+gzip compressed data, was "serializer_prefetch-1.0.1.tar", last modified: Tue Jun 20 15:04:40 2023, max compression
```

## Comparing `serializer_prefetch-1.0.0a0.tar` & `serializer_prefetch-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 14:59:18.379488 serializer_prefetch-1.0.0a0/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 serializer_prefetch-1.0.0a0/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)      207 2023-06-20 14:59:18.379488 serializer_prefetch-1.0.0a0/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     8750 2023-06-20 14:39:57.000000 serializer_prefetch-1.0.0a0/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 14:59:18.379488 serializer_prefetch-1.0.0a0/serializer_prefetch/
--rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 serializer_prefetch-1.0.0a0/serializer_prefetch/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    11814 2023-06-20 14:27:16.000000 serializer_prefetch-1.0.0a0/serializer_prefetch/base.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 14:59:18.379488 serializer_prefetch-1.0.0a0/serializer_prefetch.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)      207 2023-06-20 14:59:18.000000 serializer_prefetch-1.0.0a0/serializer_prefetch.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      300 2023-06-20 14:59:18.000000 serializer_prefetch-1.0.0a0/serializer_prefetch.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 14:59:18.000000 serializer_prefetch-1.0.0a0/serializer_prefetch.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 14:59:18.000000 serializer_prefetch-1.0.0a0/serializer_prefetch.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       20 2023-06-20 14:59:18.000000 serializer_prefetch-1.0.0a0/serializer_prefetch.egg-info/top_level.txt
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 14:59:18.379488 serializer_prefetch-1.0.0a0/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      395 2023-06-20 14:59:11.000000 serializer_prefetch-1.0.0a0/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/
+-rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 serializer_prefetch-1.0.1/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)     8996 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     8750 2023-06-20 14:39:57.000000 serializer_prefetch-1.0.1/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/serializer_prefetch/
+-rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 serializer_prefetch-1.0.1/serializer_prefetch/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11814 2023-06-20 14:27:16.000000 serializer_prefetch-1.0.1/serializer_prefetch/base.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)     8996 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      300 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      610 2023-06-20 15:04:14.000000 serializer_prefetch-1.0.1/setup.py
```

### Comparing `serializer_prefetch-1.0.0a0/LICENSE` & `serializer_prefetch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serializer_prefetch-1.0.0a0/README.md` & `serializer_prefetch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `serializer_prefetch-1.0.0a0/serializer_prefetch/base.py` & `serializer_prefetch-1.0.1/serializer_prefetch/base.py`

 * *Files identical despite different names*

