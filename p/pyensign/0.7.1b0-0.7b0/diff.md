# Comparing `tmp/pyensign-0.7.1b0.tar.gz` & `tmp/pyensign-0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyensign-0.7.1b0.tar", last modified: Mon Jun 19 22:24:25 2023, max compression
+gzip compressed data, was "pyensign-0.7b0.tar", last modified: Wed May 31 20:40:58 2023, max compression
```

## Comparing `pyensign-0.7.1b0.tar` & `pyensign-0.7b0.tar`

### file list

```diff
@@ -1,57 +1,54 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.936118 pyensign-0.7.1b0/
--rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/CONTRIBUTING.md
--rw-r--r--   0 patrick    (501) staff       (20)     2360 2023-05-31 19:58:09.000000 pyensign-0.7.1b0/DESCRIPTION.md
--rw-r--r--   0 patrick    (501) staff       (20)      180 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)      394 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/Makefile
--rw-r--r--   0 patrick    (501) staff       (20)     3756 2023-06-19 22:24:25.936382 pyensign-0.7.1b0/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     4329 2023-05-31 19:58:28.000000 pyensign-0.7.1b0/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.925486 pyensign-0.7.1b0/pyensign/
--rw-r--r--   0 patrick    (501) staff       (20)      507 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.927995 pyensign-0.7.1b0/pyensign/api/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/api/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.930627 pyensign-0.7.1b0/pyensign/api/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/api/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7865 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/api/v1beta1/ensign_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)    19552 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
--rw-r--r--   0 patrick    (501) staff       (20)      809 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/api/v1beta1/event.py
--rw-r--r--   0 patrick    (501) staff       (20)     7539 2023-05-31 15:33:48.000000 pyensign-0.7.1b0/pyensign/api/v1beta1/event_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/api/v1beta1/groups_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     4416 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/api/v1beta1/topic_pb2.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.931762 pyensign-0.7.1b0/pyensign/auth/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/auth/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4664 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/auth/client.py
--rw-r--r--   0 patrick    (501) staff       (20)      347 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/auth/tokens.py
--rw-r--r--   0 patrick    (501) staff       (20)     8481 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/connection.py
--rw-r--r--   0 patrick    (501) staff       (20)    14465 2023-06-19 22:21:50.000000 pyensign-0.7.1b0/pyensign/ensign.py
--rw-r--r--   0 patrick    (501) staff       (20)     6362 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/events.py
--rw-r--r--   0 patrick    (501) staff       (20)     4340 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/exceptions.py
--rw-r--r--   0 patrick    (501) staff       (20)     4063 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/iterator.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.932175 pyensign-0.7.1b0/pyensign/mimetype/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/mimetype/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.932929 pyensign-0.7.1b0/pyensign/mimetype/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/mimetype/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     5383 2023-05-31 15:33:48.000000 pyensign-0.7.1b0/pyensign/mimetypes.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.933365 pyensign-0.7.1b0/pyensign/region/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/region/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.934002 pyensign-0.7.1b0/pyensign/region/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/region/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7945 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/region/v1beta1/region_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     8738 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/stream.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.935660 pyensign-0.7.1b0/pyensign/utils/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-31 18:56:39.000000 pyensign-0.7.1b0/pyensign/utils/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      983 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/pyensign/utils/cache.py
--rw-r--r--   0 patrick    (501) staff       (20)     1542 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyensign/utils/queue.py
--rw-r--r--   0 patrick    (501) staff       (20)     1089 2023-06-09 23:30:01.000000 pyensign-0.7.1b0/pyensign/utils/tasks.py
--rw-r--r--   0 patrick    (501) staff       (20)     1108 2023-06-19 22:24:15.000000 pyensign-0.7.1b0/pyensign/version.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-19 22:24:25.927496 pyensign-0.7.1b0/pyensign.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)     3756 2023-06-19 22:24:25.000000 pyensign-0.7.1b0/pyensign.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     1140 2023-06-19 22:24:25.000000 pyensign-0.7.1b0/pyensign.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-19 22:24:25.000000 pyensign-0.7.1b0/pyensign.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-19 22:24:25.000000 pyensign-0.7.1b0/pyensign.egg-info/not-zip-safe
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-19 22:24:25.000000 pyensign-0.7.1b0/pyensign.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        9 2023-06-19 22:24:25.000000 pyensign-0.7.1b0/pyensign.egg-info/top_level.txt
--rw-r--r--   0 patrick    (501) staff       (20)       47 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/pyproject.toml
--rw-r--r--   0 patrick    (501) staff       (20)       63 2023-06-19 21:58:15.000000 pyensign-0.7.1b0/requirements.txt
--rw-r--r--   0 patrick    (501) staff       (20)       38 2023-06-19 22:24:25.936988 pyensign-0.7.1b0/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-05-16 21:00:20.000000 pyensign-0.7.1b0/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854409 pyensign-0.7b0/
+-rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-05-16 21:00:20.000000 pyensign-0.7b0/CONTRIBUTING.md
+-rw-r--r--   0 patrick    (501) staff       (20)     2360 2023-05-31 19:58:09.000000 pyensign-0.7b0/DESCRIPTION.md
+-rw-r--r--   0 patrick    (501) staff       (20)      180 2023-05-16 21:00:20.000000 pyensign-0.7b0/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)      394 2023-05-16 21:00:20.000000 pyensign-0.7b0/Makefile
+-rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.854558 pyensign-0.7b0/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4329 2023-05-31 19:58:28.000000 pyensign-0.7b0/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.846230 pyensign-0.7b0/pyensign/
+-rw-r--r--   0 patrick    (501) staff       (20)      507 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.848027 pyensign-0.7b0/pyensign/api/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.850724 pyensign-0.7b0/pyensign/api/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7865 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19552 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
+-rw-r--r--   0 patrick    (501) staff       (20)      786 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/event.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7539 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/api/v1beta1/event_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4416 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.851841 pyensign-0.7b0/pyensign/auth/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3937 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/client.py
+-rw-r--r--   0 patrick    (501) staff       (20)      347 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/tokens.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11976 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/connection.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10517 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/ensign.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1905 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/events.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3601 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/exceptions.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852166 pyensign-0.7b0/pyensign/mimetype/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852581 pyensign-0.7b0/pyensign/mimetype/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5383 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/mimetypes.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852880 pyensign-0.7b0/pyensign/region/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.853269 pyensign-0.7b0/pyensign/region/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7945 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/region_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854128 pyensign-0.7b0/pyensign/utils/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/utils/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      983 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/utils/cache.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1089 2023-05-31 15:33:49.000000 pyensign-0.7b0/pyensign/utils/tasks.py
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-05-31 19:17:18.000000 pyensign-0.7b0/pyensign/version.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.847769 pyensign-0.7b0/pyensign.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     1076 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/not-zip-safe
+-rw-r--r--   0 patrick    (501) staff       (20)       89 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyproject.toml
+-rw-r--r--   0 patrick    (501) staff       (20)       88 2023-05-31 18:56:39.000000 pyensign-0.7b0/requirements.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-05-31 20:40:58.854916 pyensign-0.7b0/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-05-16 21:00:20.000000 pyensign-0.7b0/setup.py
```

### Comparing `pyensign-0.7.1b0/CONTRIBUTING.md` & `pyensign-0.7b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/DESCRIPTION.md` & `pyensign-0.7b0/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/PKG-INFO` & `pyensign-0.7b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.7.1b0
+Version: 0.7b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7.1b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
```

### Comparing `pyensign-0.7.1b0/README.md` & `pyensign-0.7b0/README.md`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/api/v1beta1/ensign_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/api/v1beta1/ensign_pb2_grpc.py` & `pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/api/v1beta1/event.py` & `pyensign-0.7b0/pyensign/api/v1beta1/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if not isinstance(event, event_pb2.Event):
         raise TypeError("event must be a protobuf event")
 
     if not isinstance(topic_id, ULID):
         raise TypeError("topic_id must be a ULID")
 
     return event_pb2.EventWrapper(
-        local_id=ULID().bytes, event=event.SerializeToString(), topic_id=topic_id.bytes
+        event=event.SerializeToString(), topic_id=topic_id.bytes
     )
 
 
 def unwrap(event_wrapper):
     """
     Unwrap an event from an EventWrapper.
     """
```

### Comparing `pyensign-0.7.1b0/pyensign/api/v1beta1/event_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/api/v1beta1/groups_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/api/v1beta1/topic_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/connection.py` & `pyensign-0.7b0/pyensign/connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import grpc
 import asyncio
-from ulid import ULID
 from grpc import aio
-from datetime import timedelta
 
 from pyensign.api.v1beta1 import topic_pb2
 from pyensign.api.v1beta1 import ensign_pb2
 from pyensign.utils.tasks import WorkerPool
-from pyensign.stream import Publisher, Subscriber
 from pyensign.api.v1beta1 import ensign_pb2_grpc
 from pyensign.exceptions import catch_rpc_error
-from pyensign.exceptions import EnsignClientClosingError
+from pyensign.api.v1beta1.event import wrap, unwrap
+from pyensign.exceptions import EnsignError, EnsignTypeError
 
 
 class Connection:
     """
     Connection defines a gRPC connection to an Ensign server.
     """
 
@@ -51,119 +49,167 @@
                     credentials, call_credentials
                 )
             self.channel = aio.secure_channel(addrport, credentials)
 
 
 class Client:
     """
-    Client defines the actual gRPC client that makes requests to an Ensign server.
+    Client defines a high level client that makes requests to an Ensign server.
     """
 
-    def __init__(
-        self,
-        connection,
-        client_id="",
-        topic_cache=None,
-        reconnect_tick=timedelta(milliseconds=750),
-        reconnect_timeout=timedelta(minutes=5),
-    ):
+    def __init__(self, connection):
         """
         Create a new client from an established connection.
 
         Parameters
         ----------
         connection : Connection
             The connection to the Ensign server
         """
 
         self.channel = connection.channel
         self.stub = ensign_pb2_grpc.EnsignStub(self.channel)
-        self.publishers = {}
-        self.subscribers = {}
+        self.publish_streams = {}
+        self.subscribe_streams = {}
         self.pool = WorkerPool(max_workers=10, max_queue_size=100)
-        self.topics = topic_cache
-        self.reconnect_tick = reconnect_tick
-        self.reconnect_timeout = reconnect_timeout
-        self.shutdown = asyncio.Event()
-
-        # Create client ID if not provided, which exists for the lifetime of the client
-        # and persists across reconnects
-        if client_id == "":
-            self.client_id = str(ULID())
-        else:
-            self.client_id = client_id
 
     @catch_rpc_error
-    async def publish(self, topic_id, events, on_ack=None, on_nack=None):
-        if self.shutdown.is_set():
-            raise EnsignClientClosingError("client is closing")
-
+    async def publish(
+        self, topic_id, events, ack_callback=None, nack_callback=None, client_id=""
+    ):
         # Create a hash of the topic ID
         topic_hash = str(topic_id)
 
         # Check if there is already an open stream for this topic
-        if topic_hash in self.publishers:
-            publisher = self.publishers[topic_hash]
+        if topic_hash in self.publish_streams:
+            stream = self.publish_streams[topic_hash]
         else:
-            # Create the publish stream for this topic
-            publisher = Publisher(
-                self,
-                topic_id,
-                on_ack=on_ack,
-                on_nack=on_nack,
-            )
-            self.publishers[topic_hash] = publisher
+            # Create the stream for this topic
+            stream = Stream()
+            self.publish_streams[topic_hash] = stream
+
+            async def next_request():
+                # First message must be an OpenStream request
+                # TODO: Should we send topics here?
+                yield ensign_pb2.PublisherRequest(
+                    open_stream=ensign_pb2.OpenStream(client_id=client_id)
+                )
 
-            # Connect to the publish stream
-            # TODO: Distinguish between authentication errors, topic errors, and connection errors
-            await publisher.connect()
+                # The rest of the messages should be wrapped events
+                while True:
+                    req = await stream.read_request()
+                    if req is None:
+                        break
+                    yield req
+
+            async def publish_stream():
+                async for rep in self.stub.Publish(next_request()):
+                    rep_type = rep.WhichOneof("embed")
+                    if not stream.ready.is_set() and rep_type != "ready":
+                        raise EnsignTypeError(
+                            "expected ready response, got {}".format(rep_type)
+                        )
+                    if rep_type == "ready":
+                        # TODO: Parse topic map from stream_ready response
+                        stream.ready.set()
+                    elif rep_type == "ack":
+                        if ack_callback:
+                            await ack_callback(rep.ack)
+                    elif rep_type == "nack":
+                        if nack_callback:
+                            await nack_callback(rep.nack)
+                    elif rep_type == "close_stream":
+                        await stream.close()
+                        break
+                    else:
+                        raise EnsignTypeError(f"unexpected response type: {rep_type}")
 
-            # Run the publisher as a concurrent task which handles reconnects
+            # Create a concurrent task to handle the stream
             await self.pool.schedule(
-                publisher.run(),
-                done_callback=lambda: self.publishers.pop(topic_hash, None),
+                publish_stream(),
+                done_callback=lambda: self.publish_streams.pop(topic_hash),
             )
 
+        async def queue_events():
+            for event in events:
+                req = ensign_pb2.PublisherRequest(event=wrap(event, topic_id))
+                await stream.write_request(req)
+
         # Create a concurrent task to queue the events from the user
-        await self.pool.schedule(publisher.queue_events(events))
+        await self.pool.schedule(queue_events())
 
     @catch_rpc_error
-    async def subscribe(self, topic_ids, on_event, query="", consumer_group=None):
-        if self.shutdown.is_set():
-            raise EnsignClientClosingError("client is closing")
-
+    async def subscribe(self, topic_ids, client_id="", query="", consumer_group=None):
         # Create a hash of the topic IDs
         topic_hash = frozenset([id for id in topic_ids])
 
         # Check if there is already an open stream for these topics
-        if topic_hash in self.subscribers:
-            subscriber = self.subscribers[topic_hash]
+        if topic_hash in self.subscribe_streams:
+            stream = self.subscribe_streams[topic_hash]
         else:
-            # Create the subscribe stream for these topics
-            subscriber = Subscriber(
-                self,
-                topic_ids,
-                on_event,
-                query=query,
-                consumer_group=consumer_group,
-            )
-            self.subscribers[topic_hash] = subscriber
+            # Create the stream for these topics
+            stream = Stream()
+            self.subscribe_streams[topic_hash] = stream
+
+            async def next_request():
+                # First message must be a Subscription request with the topic
+                sub = ensign_pb2.Subscription(
+                    client_id=client_id,
+                    topics=topic_ids,
+                    query=query,
+                    group=consumer_group,
+                )
+                yield ensign_pb2.SubscribeRequest(subscription=sub)
 
-            # Connect to the subscribe stream
-            # TODO: Distinguish between authentication errors, topic errors, and connection errors
-            await subscriber.connect()
+                # Return acks and nacks to the server
+                while True:
+                    yield await stream.read_request()
+
+            async def subscribe_stream():
+                async for rep in self.stub.Subscribe(next_request()):
+                    rep_type = rep.WhichOneof("embed")
+                    if not stream.ready.is_set() and rep_type != "ready":
+                        stream.write_response(
+                            EnsignTypeError(
+                                "expected ready response, got {}".format(rep_type)
+                            )
+                        )
+                        break
+                    if rep_type == "ready":
+                        stream.ready.set()
+                    elif rep_type == "event":
+                        await stream.write_response(rep.event)
+                    elif rep_type == "close_stream":
+                        await stream.close()
+                        break
+                    else:
+                        stream.write_response(
+                            EnsignTypeError(f"unexpected response type: {rep_type}")
+                        )
+                        break
 
-            # Run the subscriber as a concurrent task which handles reconnects
+            # Create a concurrent task to handle the stream
             await self.pool.schedule(
-                subscriber.run(),
-                done_callback=lambda: self.subscribers.pop(topic_hash, None),
+                subscribe_stream(),
+                done_callback=lambda: self.subscribe_streams.pop(topic_hash),
             )
 
-        # Consume the events as a concurrent task
-        await self.pool.schedule(subscriber.consume())
+        # Yield events from the stream
+        while True:
+            rep = await stream.read_response()
+            if rep is None:
+                break
+            elif isinstance(rep, EnsignError):
+                raise rep
+            else:
+                # Ack back to the stream
+                # TODO: Allow the user to ack or nack the event
+                await stream.write_request(ensign_pb2.SubscribeRequest(ack=ensign_pb2.Ack(id=rep.id)))
+
+                yield unwrap(rep)
 
     @catch_rpc_error
     async def list_topics(self, page_size=100, next_page_token=""):
         params = ensign_pb2.PageInfo(
             page_size=page_size, next_page_token=next_page_token
         )
         rep = await self.stub.ListTopics(params)
@@ -222,24 +268,56 @@
         rep = await self.stub.Status(params)
         return rep.status, rep.version, rep.uptime, rep.not_before, rep.not_after
 
     async def close(self):
         """
         Close the connection to the server and all ongoing streams.
         """
+        await self.pool.release()
         await self.channel.close()
-        await self._close_streams()
 
-    async def _close_streams(self):
-        # Prevent new streams from being created
-        self.shutdown.set()
-
-        # Close all ongoing publishers and subscribers
-        while self.publishers:
-            _, publisher = self.publishers.popitem()
-            await publisher.close()
-
-        while self.subscribers:
-            _, subscriber = self.subscribers.popitem()
-            await subscriber.close()
 
-        await self.pool.release()
+class Stream:
+    """
+    Stream implements an in-memory bidirectional buffer for non-blocking communication
+    between coroutines. The stream has a ready state that can be used to signal when the
+    stream is ready to receive requests.
+    """
+
+    def __init__(self, max_queue_size=100):
+        self._request_queue = asyncio.Queue(maxsize=max_queue_size)
+        self._response_queue = asyncio.Queue(maxsize=max_queue_size)
+        self.ready = asyncio.Event()
+
+    async def write_request(self, message):
+        """
+        Write a request to the stream, blocks if the queue is full.
+        """
+        await self._request_queue.put(message)
+
+    async def read_request(self):
+        """
+        Read a request from the stream, blocks if the queue is empty.
+        """
+        return await self._request_queue.get()
+
+    async def write_response(self, message):
+        """
+        Write a response to the stream, blocks if the queue is full.
+        """
+        await self._response_queue.put(message)
+
+    async def read_response(self):
+        """
+        Read a response from the stream, blocks if the queue is empty.
+        """
+        return await self._response_queue.get()
+
+    async def close(self):
+        """
+        Close the stream by sending a message to both the request and response streams.
+        The main purpose of this is to unblock pending consumers. Otherwise, consumers
+        will block indefinitely on read_request() or read_response(). This means that
+        consumers should be prepared to handle None responses from reads.
+        """
+        await self._request_queue.put(None)
+        await self._response_queue.put(None)
```

### Comparing `pyensign-0.7.1b0/pyensign/mimetype/v1beta1/mimetype_pb2.py` & `pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/mimetypes.py` & `pyensign-0.7b0/pyensign/mimetypes.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/region/v1beta1/region_pb2.py` & `pyensign-0.7b0/pyensign/region/v1beta1/region_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/utils/cache.py` & `pyensign-0.7b0/pyensign/utils/cache.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign/utils/tasks.py` & `pyensign-0.7b0/pyensign/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.1b0/pyensign.egg-info/PKG-INFO` & `pyensign-0.7b0/pyensign.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.7.1b0
+Version: 0.7b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7.1b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
```

### Comparing `pyensign-0.7.1b0/pyensign.egg-info/SOURCES.txt` & `pyensign-0.7b0/pyensign.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 setup.cfg
 setup.py
 pyensign/__init__.py
 pyensign/connection.py
 pyensign/ensign.py
 pyensign/events.py
 pyensign/exceptions.py
-pyensign/iterator.py
 pyensign/mimetypes.py
-pyensign/stream.py
 pyensign/version.py
 pyensign.egg-info/PKG-INFO
 pyensign.egg-info/SOURCES.txt
 pyensign.egg-info/dependency_links.txt
 pyensign.egg-info/not-zip-safe
 pyensign.egg-info/requires.txt
 pyensign.egg-info/top_level.txt
@@ -37,9 +35,8 @@
 pyensign/mimetype/v1beta1/__init__.py
 pyensign/mimetype/v1beta1/mimetype_pb2.py
 pyensign/region/__init__.py
 pyensign/region/v1beta1/__init__.py
 pyensign/region/v1beta1/region_pb2.py
 pyensign/utils/__init__.py
 pyensign/utils/cache.py
-pyensign/utils/queue.py
 pyensign/utils/tasks.py
```

### Comparing `pyensign-0.7.1b0/setup.py` & `pyensign-0.7b0/setup.py`

 * *Files identical despite different names*

