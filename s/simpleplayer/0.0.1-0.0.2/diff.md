# Comparing `tmp/simpleplayer-0.0.1.tar.gz` & `tmp/simpleplayer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleplayer-0.0.1.tar", last modified: Mon Jun 19 17:58:40 2023, max compression
+gzip compressed data, was "simpleplayer-0.0.2.tar", last modified: Tue Jun 20 16:57:25 2023, max compression
```

## Comparing `simpleplayer-0.0.1.tar` & `simpleplayer-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 17:58:40.011410 simpleplayer-0.0.1/
--rw-r--r--   0 thowie     (501) staff       (20)     1067 2023-06-19 07:04:08.000000 simpleplayer-0.0.1/LICENSE
--rw-r--r--   0 thowie     (501) staff       (20)     3856 2023-06-19 17:58:40.011281 simpleplayer-0.0.1/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)     3485 2023-06-19 17:02:11.000000 simpleplayer-0.0.1/README.md
--rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-19 17:58:40.011463 simpleplayer-0.0.1/setup.cfg
--rw-r--r--   0 thowie     (501) staff       (20)      895 2023-06-19 17:40:09.000000 simpleplayer-0.0.1/setup.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 17:58:40.010060 simpleplayer-0.0.1/simpleplayer/
--rw-r--r--   0 thowie     (501) staff       (20)       83 2023-06-19 17:58:09.000000 simpleplayer-0.0.1/simpleplayer/__init__.py
--rw-r--r--   0 thowie     (501) staff       (20)     3788 2023-06-19 17:57:52.000000 simpleplayer-0.0.1/simpleplayer/simpleplayer.py
--rw-r--r--   0 thowie     (501) staff       (20)     1433 2023-06-19 16:42:57.000000 simpleplayer-0.0.1/simpleplayer/voicegen.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 17:58:40.011072 simpleplayer-0.0.1/simpleplayer.egg-info/
--rw-r--r--   0 thowie     (501) staff       (20)     3856 2023-06-19 17:58:39.000000 simpleplayer-0.0.1/simpleplayer.egg-info/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)      323 2023-06-19 17:58:39.000000 simpleplayer-0.0.1/simpleplayer.egg-info/SOURCES.txt
--rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-19 17:58:39.000000 simpleplayer-0.0.1/simpleplayer.egg-info/dependency_links.txt
--rw-r--r--   0 thowie     (501) staff       (20)      102 2023-06-19 17:58:39.000000 simpleplayer-0.0.1/simpleplayer.egg-info/entry_points.txt
--rw-r--r--   0 thowie     (501) staff       (20)       33 2023-06-19 17:58:39.000000 simpleplayer-0.0.1/simpleplayer.egg-info/requires.txt
--rw-r--r--   0 thowie     (501) staff       (20)       13 2023-06-19 17:58:39.000000 simpleplayer-0.0.1/simpleplayer.egg-info/top_level.txt
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-20 16:57:25.238458 simpleplayer-0.0.2/
+-rw-r--r--   0 thowie     (501) staff       (20)     1067 2023-06-19 07:04:08.000000 simpleplayer-0.0.2/LICENSE
+-rw-r--r--   0 thowie     (501) staff       (20)     3864 2023-06-20 16:57:25.238320 simpleplayer-0.0.2/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)     3486 2023-06-20 16:41:36.000000 simpleplayer-0.0.2/README.md
+-rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-20 16:57:25.238504 simpleplayer-0.0.2/setup.cfg
+-rw-r--r--   0 thowie     (501) staff       (20)      900 2023-06-20 16:40:31.000000 simpleplayer-0.0.2/setup.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-20 16:57:25.237249 simpleplayer-0.0.2/simpleplayer/
+-rw-r--r--   0 thowie     (501) staff       (20)      101 2023-06-20 16:28:47.000000 simpleplayer-0.0.2/simpleplayer/__init__.py
+-rw-r--r--   0 thowie     (501) staff       (20)     3686 2023-06-20 16:45:28.000000 simpleplayer-0.0.2/simpleplayer/longplayer.py
+-rw-r--r--   0 thowie     (501) staff       (20)      538 2023-06-20 16:56:13.000000 simpleplayer-0.0.2/simpleplayer/playsong.py
+-rw-r--r--   0 thowie     (501) staff       (20)     3788 2023-06-19 17:57:52.000000 simpleplayer-0.0.2/simpleplayer/simpleplayer.py
+-rw-r--r--   0 thowie     (501) staff       (20)     1433 2023-06-19 16:42:57.000000 simpleplayer-0.0.2/simpleplayer/voicegen.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-20 16:57:25.238065 simpleplayer-0.0.2/simpleplayer.egg-info/
+-rw-r--r--   0 thowie     (501) staff       (20)     3864 2023-06-20 16:57:25.000000 simpleplayer-0.0.2/simpleplayer.egg-info/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)      375 2023-06-20 16:57:25.000000 simpleplayer-0.0.2/simpleplayer.egg-info/SOURCES.txt
+-rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-20 16:57:25.000000 simpleplayer-0.0.2/simpleplayer.egg-info/dependency_links.txt
+-rw-r--r--   0 thowie     (501) staff       (20)      100 2023-06-20 16:57:25.000000 simpleplayer-0.0.2/simpleplayer.egg-info/entry_points.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       33 2023-06-20 16:57:25.000000 simpleplayer-0.0.2/simpleplayer.egg-info/requires.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       13 2023-06-20 16:57:25.000000 simpleplayer-0.0.2/simpleplayer.egg-info/top_level.txt
```

### Comparing `simpleplayer-0.0.1/LICENSE` & `simpleplayer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleplayer-0.0.1/PKG-INFO` & `simpleplayer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: simpleplayer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
-Author: TOWDIO
+Author: Thowie Studio
 Author-email: thowiestudio@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simple Player
 
@@ -38,15 +38,15 @@
 ```python
 from simpleplayer import simpleplayer
 ```
 
 Create an instance of the AudioPlayer class, providing the filename of the audio file as a parameter:
 
 ```python
-player = AudioPlayer('path/to/your/audio/file.wav')
+player = simpleplayer('path/to/your/audio/file.wav')
 ```
 
 Replace 'path/to/your/audio/file.wav' with the actual path to your audio file.
 
 <br>
 
 ## Play Audio
```

### Comparing `simpleplayer-0.0.1/README.md` & `simpleplayer-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```python
 from simpleplayer import simpleplayer
 ```
 
 Create an instance of the AudioPlayer class, providing the filename of the audio file as a parameter:
 
 ```python
-player = AudioPlayer('path/to/your/audio/file.wav')
+player = simpleplayer('path/to/your/audio/file.wav')
 ```
 
 Replace 'path/to/your/audio/file.wav' with the actual path to your audio file.
 
 <br>
 
 ## Play Audio
```

### Comparing `simpleplayer-0.0.1/setup.py` & `simpleplayer-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 # Read the contents of README.md file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='simpleplayer',
-    version='0.0.1',
+    version='0.0.2',
     description='Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author='TOWDIO',
+    author='Thowie Studio',
     author_email='thowiestudio@gmail.com',
     packages=['simpleplayer'],
     install_requires=[
         'soundfile',
         'sounddevice',
         'numpy',
         'gtts',
     ],
     entry_points={
         'console_scripts': [
-            'simpleplayer = simpleplayer.simpleplayer:main',
+            'simpleplayer = simpleplayer.longplayer:main',
             'voicegen = simpleplayer.voicegen:main',
         ],
     },
     license='MIT',
 )
```

### Comparing `simpleplayer-0.0.1/simpleplayer/simpleplayer.py` & `simpleplayer-0.0.2/simpleplayer/simpleplayer.py`

 * *Files identical despite different names*

### Comparing `simpleplayer-0.0.1/simpleplayer/voicegen.py` & `simpleplayer-0.0.2/simpleplayer/voicegen.py`

 * *Files identical despite different names*

### Comparing `simpleplayer-0.0.1/simpleplayer.egg-info/PKG-INFO` & `simpleplayer-0.0.2/simpleplayer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: simpleplayer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
-Author: TOWDIO
+Author: Thowie Studio
 Author-email: thowiestudio@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simple Player
 
@@ -38,15 +38,15 @@
 ```python
 from simpleplayer import simpleplayer
 ```
 
 Create an instance of the AudioPlayer class, providing the filename of the audio file as a parameter:
 
 ```python
-player = AudioPlayer('path/to/your/audio/file.wav')
+player = simpleplayer('path/to/your/audio/file.wav')
 ```
 
 Replace 'path/to/your/audio/file.wav' with the actual path to your audio file.
 
 <br>
 
 ## Play Audio
```

