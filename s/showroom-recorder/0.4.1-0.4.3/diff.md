# Comparing `tmp/showroom-recorder-0.4.1.tar.gz` & `tmp/showroom-recorder-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.4.1.tar", last modified: Tue Jun 20 09:48:41 2023, max compression
+gzip compressed data, was "showroom-recorder-0.4.3.tar", last modified: Tue Jun 20 10:00:25 2023, max compression
```

## Comparing `showroom-recorder-0.4.1.tar` & `showroom-recorder-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.619405 showroom-recorder-0.4.1/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:46:54.000000 showroom-recorder-0.4.1/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1675 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.4.1/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-20 09:48:41.619405 showroom-recorder-0.4.1/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1109 2023-06-20 09:48:20.000000 showroom-recorder-0.4.1/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      566 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6333 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.4.1/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       69 2023-06-20 09:48:31.000000 showroom-recorder-0.4.1/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:48:41.615405 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1675 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      748 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       70 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-20 09:48:41.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.4.1/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 10:00:25.457572 showroom-recorder-0.4.3/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:46:54.000000 showroom-recorder-0.4.3/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1285 2023-06-20 10:00:25.457572 showroom-recorder-0.4.3/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.4.3/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-20 10:00:25.457572 showroom-recorder-0.4.3/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-20 09:59:51.000000 showroom-recorder-0.4.3/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      566 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 10:00:25.453572 showroom-recorder-0.4.3/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 10:00:25.457572 showroom-recorder-0.4.3/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 10:00:25.457572 showroom-recorder-0.4.3/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6333 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 10:00:25.457572 showroom-recorder-0.4.3/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.4.3/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       69 2023-06-20 10:00:23.000000 showroom-recorder-0.4.3/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 10:00:25.457572 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1285 2023-06-20 10:00:25.000000 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      748 2023-06-20 10:00:25.000000 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 10:00:25.000000 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-20 10:00:25.000000 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       70 2023-06-20 10:00:25.000000 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-20 10:00:25.000000 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.4.3/src/showroom_recorder.egg-info/zip-safe
```

### Comparing `showroom-recorder-0.4.1/PKG-INFO` & `showroom-recorder-0.4.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: showroom-recorder
-Version: 0.4.1
-Summary: Recording Showroom Streaming Video
-Home-page: https://github.com/vacabun/showroom-recorder
-Author: vacabun
-Author-email: maguotong66@gmail.com
-License: UNKNOWN
-Keywords: video download showroom
-Platform: any
-
 # showroom-recorder
 A Script for Recording Showroom Streaming Video
 
 [![zh_CN](https://img.shields.io/badge/language-zh__CN-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.zh_CN.md)
 [![en_US](https://img.shields.io/badge/language-en__US-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.en_US.md)
 [![ja_JP](https://img.shields.io/badge/language-ja__JP-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.ja_JP.md)
 
@@ -55,9 +44,7 @@
 ``` shell
 showroom-recorder
 ```
 
 The recorded video will be stored in the save folder.
 
 And the comments will be saved in the comments folder as subtitles.
-
-
```

### Comparing `showroom-recorder-0.4.1/README.md` & `showroom-recorder-0.4.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+Metadata-Version: 2.1
+Name: showroom-recorder
+Version: 0.4.3
+Summary: Recording Showroom Streaming Video
+Home-page: https://github.com/vacabun/showroom-recorder
+Author: vacabun
+Author-email: maguotong66@gmail.com
+License: UNKNOWN
+Keywords: video download showroom
+Platform: any
+Description-Content-Type: text/markdown
+
 # showroom-recorder
 A Script for Recording Showroom Streaming Video
 
-[![zh_CN](https://img.shields.io/badge/language-zh__CN-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.zh_CN.md)
-[![en_US](https://img.shields.io/badge/language-en__US-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.en_US.md)
-[![ja_JP](https://img.shields.io/badge/language-ja__JP-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.ja_JP.md)
-
 ## Installation
 
 1. Install the python3.
 
 2. Install requirements.
 
 ``` shell
@@ -44,7 +52,9 @@
 ``` shell
 showroom-recorder
 ```
 
 The recorded video will be stored in the save folder.
 
 And the comments will be saved in the comments folder as subtitles.
+
+
```

### Comparing `showroom-recorder-0.4.1/setup.py` & `showroom-recorder-0.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 PACKAGE_NAME = 'showroom_recorder'
 
 PROJ_METADATA = '%s.json' % PROJ_NAME
 
 here = os.path.abspath(os.path.dirname(__file__))
 proj_info = json.loads(open(os.path.join(here, PROJ_METADATA), encoding='utf-8').read())
 
-README = open(os.path.join(here, 'README.md'), encoding='utf-8').read()
+Description = open(os.path.join(here, 'description.md'), encoding='utf-8').read()
 
 VERSION = importlib.machinery.SourceFileLoader("version", os.path.join(here, 'src/%s/version.py' % PACKAGE_NAME)).load_module().__version__
 
 setuptools.setup(
     name=proj_info['name'],
     version=VERSION,
     author=proj_info['author'],
     url=proj_info['url'],
     author_email=proj_info['author_email'],
     description=proj_info['description'],
     keywords=proj_info['keywords'],
-    long_description=README,
+    long_description=Description,
+    long_description_content_type='text/markdown',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     test_suite='tests',
     platforms='any',
     zip_safe=True,
     include_package_data=True,
     entry_points={'console_scripts': proj_info['console_scripts']},
```

### Comparing `showroom-recorder-0.4.1/showroom-recorder.json` & `showroom-recorder-0.4.3/showroom-recorder.json`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.1/src/showroom_recorder/common.py` & `showroom-recorder-0.4.3/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.1/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.4.3/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.1/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.4.3/src/showroom_recorder/processor/video.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.1/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.4.3/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.1/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.4.3/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.1/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.4.3/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.4.1
+Version: 0.4.3
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
+Description-Content-Type: text/markdown
 
 # showroom-recorder
 A Script for Recording Showroom Streaming Video
 
-[![zh_CN](https://img.shields.io/badge/language-zh__CN-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.zh_CN.md)
-[![en_US](https://img.shields.io/badge/language-en__US-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.en_US.md)
-[![ja_JP](https://img.shields.io/badge/language-ja__JP-green.svg)](https://github.com/vacabun/showroom-recorder/blob/main/doc/README.ja_JP.md)
-
 ## Installation
 
 1. Install the python3.
 
 2. Install requirements.
 
 ``` shell
```

### Comparing `showroom-recorder-0.4.1/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.4.3/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

