# Comparing `tmp/oexp-0.8.3.tar.gz` & `tmp/oexp-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.8.3.tar", last modified: Tue Jun 20 16:52:10 2023, max compression
+gzip compressed data, was "oexp-0.8.4.tar", last modified: Tue Jun 20 17:23:32 2023, max compression
```

## Comparing `oexp-0.8.3.tar` & `oexp-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.086848 oexp-0.8.3/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:52:10.086669 oexp-0.8.3/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.3/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.085370 oexp-0.8.3/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      189 2023-06-20 15:09:33.000000 oexp-0.8.3/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    81355 2023-06-20 16:51:46.000000 oexp-0.8.3/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 16:51:45.000000 oexp-0.8.3/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2042 2023-06-20 16:51:14.000000 oexp-0.8.3/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.086501 oexp-0.8.3/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.3/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.3/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.3/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.086092 oexp-0.8.3/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 16:52:05.000000 oexp-0.8.3/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 16:52:10.086942 oexp-0.8.3/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:23:32.561104 oexp-0.8.4/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 17:23:32.560929 oexp-0.8.4/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.4/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:23:32.559303 oexp-0.8.4/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      189 2023-06-20 15:09:33.000000 oexp-0.8.4/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    81355 2023-06-20 16:51:46.000000 oexp-0.8.4/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 16:51:45.000000 oexp-0.8.4/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2042 2023-06-20 17:22:52.000000 oexp-0.8.4/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:23:32.560627 oexp-0.8.4/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.4/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.4/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.4/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:23:32.560106 oexp-0.8.4/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 17:23:32.000000 oexp-0.8.4/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 17:23:32.000000 oexp-0.8.4/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 17:23:32.000000 oexp-0.8.4/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 17:23:32.000000 oexp-0.8.4/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 17:23:32.000000 oexp-0.8.4/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 17:23:27.000000 oexp-0.8.4/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 17:23:32.561152 oexp-0.8.4/setup.cfg
```

### Comparing `oexp-0.8.3/oexp/access.py` & `oexp-0.8.4/oexp/access.py`

 * *Files identical despite different names*

### Comparing `oexp-0.8.3/oexp/jbridge.py` & `oexp-0.8.4/oexp/jbridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import oexp.access as access
 from oexp.util import ops
 from oexp.util import vals
 
 import os
 
-print("invalidate version 1")
+print("invalidate version 2")
 
 _jar_process: Optional[subprocess.Popen] = None
 _java_sock: Optional[socket.socket] = None
 _java_exit_sock: Optional[socket.socket] = None
 _java_conn: Optional[socket.socket] = None
 _java_exit_conn: Optional[socket.socket] = None
```

### Comparing `oexp-0.8.3/oexp/util/ops.py` & `oexp-0.8.4/oexp/util/ops.py`

 * *Files identical despite different names*

### Comparing `oexp-0.8.3/oexp/util/vals.py` & `oexp-0.8.4/oexp/util/vals.py`

 * *Files identical despite different names*

