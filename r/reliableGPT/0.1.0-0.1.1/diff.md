# Comparing `tmp/reliableGPT-0.1.0.tar.gz` & `tmp/reliableGPT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/reliableGPT-0.1.0.tar", last modified: Tue Jun 20 01:49:39 2023, max compression
+gzip compressed data, was "dist/reliableGPT-0.1.1.tar", last modified: Tue Jun 20 02:01:14 2023, max compression
```

## Comparing `reliableGPT-0.1.0.tar` & `reliableGPT-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 01:49:39.159598 reliableGPT-0.1.0/
--rw-r--r--   0 daddyish   (501) staff       (20)     1065 2023-06-20 01:36:38.000000 reliableGPT-0.1.0/LICENSE
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 01:49:39.159298 reliableGPT-0.1.0/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)       13 2023-06-20 01:36:38.000000 reliableGPT-0.1.0/README.md
-drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 01:49:39.159105 reliableGPT-0.1.0/reliableGPT.egg-info/
--rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 01:49:39.000000 reliableGPT-0.1.0/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 daddyish   (501) staff       (20)      200 2023-06-20 01:49:39.000000 reliableGPT-0.1.0/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 daddyish   (501) staff       (20)        1 2023-06-20 01:49:39.000000 reliableGPT-0.1.0/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       17 2023-06-20 01:49:39.000000 reliableGPT-0.1.0/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       12 2023-06-20 01:49:39.000000 reliableGPT-0.1.0/reliableGPT.egg-info/top_level.txt
--rw-r--r--   0 daddyish   (501) staff       (20)       38 2023-06-20 01:49:39.159649 reliableGPT-0.1.0/setup.cfg
--rw-r--r--   0 daddyish   (501) staff       (20)      275 2023-06-20 01:45:00.000000 reliableGPT-0.1.0/setup.py
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.441614 reliableGPT-0.1.1/
+-rw-r--r--   0 daddyish   (501) staff       (20)     1065 2023-06-20 01:36:38.000000 reliableGPT-0.1.1/LICENSE
+-rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 02:01:14.441419 reliableGPT-0.1.1/PKG-INFO
+-rw-r--r--   0 daddyish   (501) staff       (20)       13 2023-06-20 01:36:38.000000 reliableGPT-0.1.1/README.md
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.440401 reliableGPT-0.1.1/reliableGPT.egg-info/
+-rw-r--r--   0 daddyish   (501) staff       (20)      154 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 daddyish   (501) staff       (20)      259 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)        1 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)       17 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 daddyish   (501) staff       (20)       12 2023-06-20 02:01:14.000000 reliableGPT-0.1.1/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.440831 reliableGPT-0.1.1/reliablegpt/
+-rw-r--r--   0 daddyish   (501) staff       (20)       87 2023-06-20 01:42:39.000000 reliableGPT-0.1.1/reliablegpt/__init__.py
+-rw-r--r--   0 daddyish   (501) staff       (20)     4035 2023-06-20 01:44:48.000000 reliableGPT-0.1.1/reliablegpt/main.py
+-rw-r--r--   0 daddyish   (501) staff       (20)       38 2023-06-20 02:01:14.441654 reliableGPT-0.1.1/setup.cfg
+-rw-r--r--   0 daddyish   (501) staff       (20)      275 2023-06-20 02:00:56.000000 reliableGPT-0.1.1/setup.py
+drwxr-xr-x   0 daddyish   (501) staff       (20)        0 2023-06-20 02:01:14.441141 reliableGPT-0.1.1/tests/
+-rw-r--r--   0 daddyish   (501) staff       (20)     1804 2023-06-20 01:26:23.000000 reliableGPT-0.1.1/tests/tests.py
```

### Comparing `reliableGPT-0.1.0/LICENSE` & `reliableGPT-0.1.1/LICENSE`

 * *Files identical despite different names*

