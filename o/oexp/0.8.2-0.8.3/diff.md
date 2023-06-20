# Comparing `tmp/oexp-0.8.2.tar.gz` & `tmp/oexp-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.8.2.tar", last modified: Tue Jun 20 16:39:34 2023, max compression
+gzip compressed data, was "oexp-0.8.3.tar", last modified: Tue Jun 20 16:52:10 2023, max compression
```

## Comparing `oexp-0.8.2.tar` & `oexp-0.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.741430 oexp-0.8.2/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:39:34.741265 oexp-0.8.2/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.2/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.740005 oexp-0.8.2/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      189 2023-06-20 15:09:33.000000 oexp-0.8.2/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    81355 2023-06-20 16:39:14.000000 oexp-0.8.2/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 16:39:07.000000 oexp-0.8.2/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.8.2/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.741096 oexp-0.8.2/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.2/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.2/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.2/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.740705 oexp-0.8.2/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 16:39:30.000000 oexp-0.8.2/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 16:39:34.741474 oexp-0.8.2/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.086848 oexp-0.8.3/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:52:10.086669 oexp-0.8.3/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.3/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.085370 oexp-0.8.3/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      189 2023-06-20 15:09:33.000000 oexp-0.8.3/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    81355 2023-06-20 16:51:46.000000 oexp-0.8.3/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 16:51:45.000000 oexp-0.8.3/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2042 2023-06-20 16:51:14.000000 oexp-0.8.3/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.086501 oexp-0.8.3/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.3/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.3/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.3/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:52:10.086092 oexp-0.8.3/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 16:52:10.000000 oexp-0.8.3/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 16:52:05.000000 oexp-0.8.3/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 16:52:10.086942 oexp-0.8.3/setup.cfg
```

### Comparing `oexp-0.8.2/oexp/access.py` & `oexp-0.8.3/oexp/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/556/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/557/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
```

### Comparing `oexp-0.8.2/oexp/jbridge.py` & `oexp-0.8.3/oexp/jbridge.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 import oexp.access as access
 from oexp.util import ops
 from oexp.util import vals
 
 import os
 
+print("invalidate version 1")
+
 _jar_process: Optional[subprocess.Popen] = None
 _java_sock: Optional[socket.socket] = None
 _java_exit_sock: Optional[socket.socket] = None
 _java_conn: Optional[socket.socket] = None
 _java_exit_conn: Optional[socket.socket] = None
```

### Comparing `oexp-0.8.2/oexp/util/ops.py` & `oexp-0.8.3/oexp/util/ops.py`

 * *Files identical despite different names*

### Comparing `oexp-0.8.2/oexp/util/vals.py` & `oexp-0.8.3/oexp/util/vals.py`

 * *Files identical despite different names*

