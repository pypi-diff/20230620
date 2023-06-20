# Comparing `tmp/audiobook-tags-1.1.0.tar.gz` & `tmp/audiobook-tags-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-tags-1.1.0.tar", last modified: Mon Jun 19 04:41:04 2023, max compression
+gzip compressed data, was "audiobook-tags-1.1.1.tar", last modified: Tue Jun 20 04:22:59 2023, max compression
```

## Comparing `audiobook-tags-1.1.0.tar` & `audiobook-tags-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-19 04:40:52.000000 audiobook-tags-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 04:41:04.691847 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 04:41:04.000000 audiobook-tags-1.1.0/src/audiobook_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-20 04:22:48.000000 audiobook-tags-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:22:59.369826 audiobook-tags-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:22:59.373826 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:22:59.000000 audiobook-tags-1.1.1/src/audiobook_tags.egg-info/top_level.txt
```

### Comparing `audiobook-tags-1.1.0/LICENSE.txt` & `audiobook-tags-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiobook-tags-1.1.0/PKG-INFO` & `audiobook-tags-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-tags
-Version: 1.1.0
+Version: 1.1.1
 Summary: Fix mp3 tags to use in iTunes/iPhone audiobooks
 Home-page: https://andgineer.github.io/audiobook-tags/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: audiobook mp3-tags
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `audiobook-tags-1.1.0/README.md` & `audiobook-tags-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `audiobook-tags-1.1.0/setup.py` & `audiobook-tags-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `audiobook-tags-1.1.0/src/audiobook_tags.egg-info/PKG-INFO` & `audiobook-tags-1.1.1/src/audiobook_tags.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-tags
-Version: 1.1.0
+Version: 1.1.1
 Summary: Fix mp3 tags to use in iTunes/iPhone audiobooks
 Home-page: https://andgineer.github.io/audiobook-tags/
 Author: Andrey Sorokin
 Author-email: andrey@sorokin.engineer
 Keywords: audiobook mp3-tags
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

