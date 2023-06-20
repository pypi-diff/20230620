# Comparing `tmp/Lemmy.py-0.0.1.tar.gz` & `tmp/Lemmy.py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lemmy.py-0.0.1.tar", last modified: Tue Jun 20 21:15:51 2023, max compression
+gzip compressed data, was "Lemmy.py-0.0.2.tar", last modified: Tue Jun 20 21:29:11 2023, max compression
```

## Comparing `Lemmy.py-0.0.1.tar` & `Lemmy.py-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 gamarus   (1001) gamarus   (1001)        0 2023-06-20 21:15:51.622911 Lemmy.py-0.0.1/
-drwxrwxr-x   0 gamarus   (1001) gamarus   (1001)        0 2023-06-20 21:15:51.618911 Lemmy.py-0.0.1/Lemmy.py.egg-info/
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       52 2023-06-20 21:15:51.000000 Lemmy.py-0.0.1/Lemmy.py.egg-info/PKG-INFO
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      380 2023-06-20 21:15:51.000000 Lemmy.py-0.0.1/Lemmy.py.egg-info/SOURCES.txt
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)        1 2023-06-20 21:15:51.000000 Lemmy.py-0.0.1/Lemmy.py.egg-info/dependency_links.txt
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       44 2023-06-20 21:15:51.000000 Lemmy.py-0.0.1/Lemmy.py.egg-info/requires.txt
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)        6 2023-06-20 21:15:51.000000 Lemmy.py-0.0.1/Lemmy.py.egg-info/top_level.txt
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       52 2023-06-20 21:15:51.622911 Lemmy.py-0.0.1/PKG-INFO
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      697 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/README.md
-drwxrwxr-x   0 gamarus   (1001) gamarus   (1001)        0 2023-06-20 21:15:51.622911 Lemmy.py-0.0.1/lemmy/
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       30 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/__init__.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      892 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/admin.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      948 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/auth.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     2799 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/comment.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     3398 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/community.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     1883 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/lemmy.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      492 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/modlog.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     3810 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/post.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     1836 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/private_message.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      507 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/search.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      796 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/site.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     5434 2023-06-20 20:56:53.000000 Lemmy.py-0.0.1/lemmy/user.py
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      200 2023-06-20 21:15:02.000000 Lemmy.py-0.0.1/pyproject.toml
--rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       38 2023-06-20 21:15:51.622911 Lemmy.py-0.0.1/setup.cfg
+drwxrwxr-x   0 gamarus   (1001) gamarus   (1001)        0 2023-06-20 21:29:11.066720 Lemmy.py-0.0.2/
+drwxrwxr-x   0 gamarus   (1001) gamarus   (1001)        0 2023-06-20 21:29:11.062720 Lemmy.py-0.0.2/Lemmy.py.egg-info/
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      949 2023-06-20 21:29:11.000000 Lemmy.py-0.0.2/Lemmy.py.egg-info/PKG-INFO
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      380 2023-06-20 21:29:11.000000 Lemmy.py-0.0.2/Lemmy.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)        1 2023-06-20 21:29:11.000000 Lemmy.py-0.0.2/Lemmy.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       44 2023-06-20 21:29:11.000000 Lemmy.py-0.0.2/Lemmy.py.egg-info/requires.txt
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)        6 2023-06-20 21:29:11.000000 Lemmy.py-0.0.2/Lemmy.py.egg-info/top_level.txt
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      949 2023-06-20 21:29:11.062720 Lemmy.py-0.0.2/PKG-INFO
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      697 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/README.md
+drwxrwxr-x   0 gamarus   (1001) gamarus   (1001)        0 2023-06-20 21:29:11.062720 Lemmy.py-0.0.2/lemmy/
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       30 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/__init__.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      892 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/admin.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      948 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/auth.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     2799 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/comment.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     3398 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/community.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     1883 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/lemmy.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      492 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/modlog.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     3810 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/post.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     1836 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/private_message.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      507 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/search.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      796 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/site.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)     5434 2023-06-20 20:56:53.000000 Lemmy.py-0.0.2/lemmy/user.py
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)      438 2023-06-20 21:28:53.000000 Lemmy.py-0.0.2/pyproject.toml
+-rw-rw-r--   0 gamarus   (1001) gamarus   (1001)       38 2023-06-20 21:29:11.066720 Lemmy.py-0.0.2/setup.cfg
```

### Comparing `Lemmy.py-0.0.1/README.md` & `Lemmy.py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/admin.py` & `Lemmy.py-0.0.2/lemmy/admin.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/auth.py` & `Lemmy.py-0.0.2/lemmy/auth.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/comment.py` & `Lemmy.py-0.0.2/lemmy/comment.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/community.py` & `Lemmy.py-0.0.2/lemmy/community.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/lemmy.py` & `Lemmy.py-0.0.2/lemmy/lemmy.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/post.py` & `Lemmy.py-0.0.2/lemmy/post.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/private_message.py` & `Lemmy.py-0.0.2/lemmy/private_message.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/site.py` & `Lemmy.py-0.0.2/lemmy/site.py`

 * *Files identical despite different names*

### Comparing `Lemmy.py-0.0.1/lemmy/user.py` & `Lemmy.py-0.0.2/lemmy/user.py`

 * *Files identical despite different names*

