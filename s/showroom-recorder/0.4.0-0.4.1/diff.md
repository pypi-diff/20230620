# Comparing `tmp/showroom-recorder-0.4.0.tar.gz` & `tmp/showroom-recorder-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.4.0.tar", last modified: Tue Jun 20 09:32:43 2023, max compression
+gzip compressed data, was "showroom-recorder-0.4.1.tar", last modified: Tue Jun 20 09:48:41 2023, max compression
```

## Comparing `showroom-recorder-0.4.0.tar` & `showroom-recorder-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:32:43.868577 showroom-recorder-0.4.0/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      288 2023-06-20 09:32:43.868577 showroom-recorder-0.4.0/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3216 2023-06-20 07:25:10.000000 showroom-recorder-0.4.0/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-20 09:32:43.868577 showroom-recorder-0.4.0/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1111 2023-06-20 09:32:42.000000 showroom-recorder-0.4.0/setup.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:32:43.864577 showroom-recorder-0.4.0/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:32:43.864577 showroom-recorder-0.4.0/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 08:29:21.000000 showroom-recorder-0.4.0/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 08:29:05.000000 showroom-recorder-0.4.0/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 08:29:01.000000 showroom-recorder-0.4.0/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:32:43.868577 showroom-recorder-0.4.0/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 08:25:23.000000 showroom-recorder-0.4.0/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 08:25:53.000000 showroom-recorder-0.4.0/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6333 2023-06-20 08:25:58.000000 showroom-recorder-0.4.0/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:32:43.868577 showroom-recorder-0.4.0/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 08:25:11.000000 showroom-recorder-0.4.0/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 06:57:18.000000 showroom-recorder-0.4.0/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 08:26:06.000000 showroom-recorder-0.4.0/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       69 2023-06-20 08:28:54.000000 showroom-recorder-0.4.0/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:32:43.868577 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      288 2023-06-20 09:32:43.000000 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      713 2023-06-20 09:32:43.000000 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:32:43.000000 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-20 09:32:43.000000 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       70 2023-06-20 09:32:43.000000 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-20 09:32:43.000000 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.4.0/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.619405 showroom-recorder-0.4.1/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:46:54.000000 showroom-recorder-0.4.1/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1675 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.4.1/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-20 09:48:41.619405 showroom-recorder-0.4.1/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1109 2023-06-20 09:48:20.000000 showroom-recorder-0.4.1/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      566 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6333 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       69 2023-06-20 09:48:31.000000 showroom-recorder-0.4.1/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1675 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      748 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       70 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/zip-safe
```

### Comparing `showroom-recorder-0.4.0/setup.py` & `showroom-recorder-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     name=proj_info['name'],
     version=VERSION,
     author=proj_info['author'],
     url=proj_info['url'],
     author_email=proj_info['author_email'],
     description=proj_info['description'],
     keywords=proj_info['keywords'],
-    # long_description=README,
+    long_description=README,
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     test_suite='tests',
     platforms='any',
     zip_safe=True,
     include_package_data=True,
     entry_points={'console_scripts': proj_info['console_scripts']},
```

### Comparing `showroom-recorder-0.4.0/src/showroom_recorder/common.py` & `showroom-recorder-0.4.1/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.0/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.4.1/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.0/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.4.1/src/showroom_recorder/processor/video.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.0/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.4.1/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.0/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.4.1/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.0/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.4.1/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+MANIFEST.in
 README.md
 setup.py
+showroom-recorder.json
 src/showroom_recorder/__init__.py
 src/showroom_recorder/__main__.py
 src/showroom_recorder/common.py
 src/showroom_recorder/version.py
 src/showroom_recorder.egg-info/PKG-INFO
 src/showroom_recorder.egg-info/SOURCES.txt
 src/showroom_recorder.egg-info/dependency_links.txt
```

