# Comparing `tmp/boreal-0.8.2.tar.gz` & `tmp/boreal-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boreal-0.8.2.tar", last modified: Thu Mar 16 19:42:00 2023, max compression
+gzip compressed data, was "boreal-0.8.3.tar", last modified: Tue Jun 20 18:45:31 2023, max compression
```

## Comparing `boreal-0.8.2.tar` & `boreal-0.8.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-03-16 19:42:00.126737 boreal-0.8.2/
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      159 2023-02-09 23:09:12.000000 boreal-0.8.2/AUTHORS.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     3503 2023-02-09 23:09:12.000000 boreal-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)       89 2023-02-09 23:09:12.000000 boreal-0.8.2/HISTORY.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1076 2023-02-09 23:09:12.000000 boreal-0.8.2/LICENSE
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      262 2023-02-09 23:09:12.000000 boreal-0.8.2/MANIFEST.in
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     3324 2023-03-16 19:42:00.126830 boreal-0.8.2/PKG-INFO
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     2534 2023-02-09 23:09:12.000000 boreal-0.8.2/README.rst
-drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-03-16 19:42:00.121918 boreal-0.8.2/boreal/
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      183 2023-03-16 19:40:01.000000 boreal-0.8.2/boreal/__init__.py
-drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-03-16 19:42:00.123695 boreal-0.8.2/boreal/audio_widgets/
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      153 2023-02-09 23:09:12.000000 boreal-0.8.2/boreal/audio_widgets/__init__.py
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     6041 2023-02-12 05:01:55.000000 boreal-0.8.2/boreal/audio_widgets/audio.py
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     2628 2023-02-09 23:09:12.000000 boreal-0.8.2/boreal/audio_widgets/audio_processors.py
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)    10649 2023-02-26 18:21:31.000000 boreal-0.8.2/boreal/audio_widgets/audio_widgets.py
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      586 2023-02-09 23:09:12.000000 boreal-0.8.2/boreal/audio_widgets/description.html
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     8687 2023-02-26 19:40:29.000000 boreal-0.8.2/boreal/audio_widgets/main.py
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)  2646044 2023-02-09 23:09:12.000000 boreal-0.8.2/boreal/beatles.wav
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     4080 2023-02-26 18:25:52.000000 boreal-0.8.2/boreal/boreal.py
-drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-03-16 19:42:00.122916 boreal-0.8.2/boreal.egg-info/
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     3324 2023-03-16 19:41:59.000000 boreal-0.8.2/boreal.egg-info/PKG-INFO
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      832 2023-03-16 19:42:00.000000 boreal-0.8.2/boreal.egg-info/SOURCES.txt
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)        1 2023-03-16 19:41:59.000000 boreal-0.8.2/boreal.egg-info/dependency_links.txt
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)       43 2023-03-16 19:41:59.000000 boreal-0.8.2/boreal.egg-info/entry_points.txt
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)        1 2023-03-16 19:41:59.000000 boreal-0.8.2/boreal.egg-info/not-zip-safe
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      164 2023-03-16 19:41:59.000000 boreal-0.8.2/boreal.egg-info/requires.txt
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)        7 2023-03-16 19:41:59.000000 boreal-0.8.2/boreal.egg-info/top_level.txt
-drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-03-16 19:42:00.126295 boreal-0.8.2/docs/
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      607 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/Makefile
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)       28 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/authors.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      942 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/boreal.audio_widgets.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      372 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/boreal.rst
--rwxr-xr-x   0 george.tzanetakis   (502) staff       (20)     4847 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/conf.py
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)       33 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/contributing.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1658 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/history.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      303 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/index.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1094 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/installation.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      804 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/make.bat
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)       55 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/modules.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)       27 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/readme.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      391 2023-02-09 23:09:12.000000 boreal-0.8.2/docs/usage.rst
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      652 2023-03-16 19:42:00.127249 boreal-0.8.2/setup.cfg
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1408 2023-03-16 19:39:43.000000 boreal-0.8.2/setup.py
-drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-03-16 19:42:00.126596 boreal-0.8.2/tests/
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)       36 2023-02-09 23:09:12.000000 boreal-0.8.2/tests/__init__.py
--rw-r--r--   0 george.tzanetakis   (502) staff       (20)      382 2023-02-09 23:09:12.000000 boreal-0.8.2/tests/test_boreal.py
+drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-06-20 18:45:31.414827 boreal-0.8.3/
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      159 2023-02-09 23:09:12.000000 boreal-0.8.3/AUTHORS.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     3503 2023-02-09 23:09:12.000000 boreal-0.8.3/CONTRIBUTING.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)       89 2023-02-09 23:09:12.000000 boreal-0.8.3/HISTORY.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1076 2023-02-09 23:09:12.000000 boreal-0.8.3/LICENSE
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      262 2023-02-09 23:09:12.000000 boreal-0.8.3/MANIFEST.in
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     3324 2023-06-20 18:45:31.414918 boreal-0.8.3/PKG-INFO
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     2534 2023-02-09 23:09:12.000000 boreal-0.8.3/README.rst
+drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-06-20 18:45:31.409932 boreal-0.8.3/boreal/
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      183 2023-06-20 18:17:40.000000 boreal-0.8.3/boreal/__init__.py
+drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-06-20 18:45:31.411895 boreal-0.8.3/boreal/audio_widgets/
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      153 2023-02-09 23:09:12.000000 boreal-0.8.3/boreal/audio_widgets/__init__.py
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     6041 2023-05-23 22:30:18.000000 boreal-0.8.3/boreal/audio_widgets/audio.py
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     2628 2023-02-09 23:09:12.000000 boreal-0.8.3/boreal/audio_widgets/audio_processors.py
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)    10649 2023-03-25 18:14:15.000000 boreal-0.8.3/boreal/audio_widgets/audio_widgets.py
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      586 2023-02-09 23:09:12.000000 boreal-0.8.3/boreal/audio_widgets/description.html
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     8688 2023-05-23 18:04:45.000000 boreal-0.8.3/boreal/audio_widgets/main.py
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)  2646044 2023-02-09 23:09:12.000000 boreal-0.8.3/boreal/beatles.wav
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     9965 2023-06-20 18:41:20.000000 boreal-0.8.3/boreal/boreal.py
+drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-06-20 18:45:31.410963 boreal-0.8.3/boreal.egg-info/
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     3324 2023-06-20 18:45:31.000000 boreal-0.8.3/boreal.egg-info/PKG-INFO
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      832 2023-06-20 18:45:31.000000 boreal-0.8.3/boreal.egg-info/SOURCES.txt
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)        1 2023-06-20 18:45:31.000000 boreal-0.8.3/boreal.egg-info/dependency_links.txt
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)       43 2023-06-20 18:45:31.000000 boreal-0.8.3/boreal.egg-info/entry_points.txt
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)        1 2023-06-20 18:45:31.000000 boreal-0.8.3/boreal.egg-info/not-zip-safe
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      137 2023-06-20 18:45:31.000000 boreal-0.8.3/boreal.egg-info/requires.txt
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)        7 2023-06-20 18:45:31.000000 boreal-0.8.3/boreal.egg-info/top_level.txt
+drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-06-20 18:45:31.414414 boreal-0.8.3/docs/
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      607 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/Makefile
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)       28 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/authors.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      942 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/boreal.audio_widgets.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      372 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/boreal.rst
+-rwxr-xr-x   0 george.tzanetakis   (502) staff       (20)     4847 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/conf.py
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)       33 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/contributing.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1658 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/history.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      303 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/index.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1094 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/installation.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      804 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/make.bat
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)       55 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/modules.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)       27 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/readme.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      391 2023-02-09 23:09:12.000000 boreal-0.8.3/docs/usage.rst
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      623 2023-06-20 18:45:31.415316 boreal-0.8.3/setup.cfg
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)     1408 2023-06-20 18:17:18.000000 boreal-0.8.3/setup.py
+drwxr-xr-x   0 george.tzanetakis   (502) staff       (20)        0 2023-06-20 18:45:31.414715 boreal-0.8.3/tests/
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)       36 2023-02-09 23:09:12.000000 boreal-0.8.3/tests/__init__.py
+-rw-r--r--   0 george.tzanetakis   (502) staff       (20)      382 2023-02-09 23:09:12.000000 boreal-0.8.3/tests/test_boreal.py
```

### Comparing `boreal-0.8.2/CONTRIBUTING.rst` & `boreal-0.8.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/LICENSE` & `boreal-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/PKG-INFO` & `boreal-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boreal
-Version: 0.8.2
+Version: 0.8.3
 Summary: Bokeh Reactive Audio Library
 Home-page: https://github.com/gtzan/boreal
 Author: George Tzanetakis
 Author-email: gtzan@cs.uvic.ca
 License: MIT license
 Keywords: boreal
 Platform: UNKNOWN
```

### Comparing `boreal-0.8.2/README.rst` & `boreal-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/boreal/audio_widgets/audio.py` & `boreal-0.8.3/boreal/audio_widgets/audio.py`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/boreal/audio_widgets/audio_processors.py` & `boreal-0.8.3/boreal/audio_widgets/audio_processors.py`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/boreal/audio_widgets/audio_widgets.py` & `boreal-0.8.3/boreal/audio_widgets/audio_widgets.py`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/boreal/audio_widgets/description.html` & `boreal-0.8.3/boreal/audio_widgets/description.html`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/boreal/audio_widgets/main.py` & `boreal-0.8.3/boreal/audio_widgets/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         ipd.display(ipd.Javascript(s1))
     audio_play.set()    
 
     
     if (visualize_callback_active_ is False):
         callback_id_ = curdoc().add_periodic_callback(update, 60)
     visualize_callback_active_ = True
-
+w
 
 def pause_handler():
     """
     Pause the audio playback
     """
     global audio_playing_
     audio_playing_ = False
```

### Comparing `boreal-0.8.2/boreal/beatles.wav` & `boreal-0.8.3/boreal/beatles.wav`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/boreal.egg-info/PKG-INFO` & `boreal-0.8.3/boreal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boreal
-Version: 0.8.2
+Version: 0.8.3
 Summary: Bokeh Reactive Audio Library
 Home-page: https://github.com/gtzan/boreal
 Author: George Tzanetakis
 Author-email: gtzan@cs.uvic.ca
 License: MIT license
 Keywords: boreal
 Platform: UNKNOWN
```

### Comparing `boreal-0.8.2/boreal.egg-info/SOURCES.txt` & `boreal-0.8.3/boreal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/docs/Makefile` & `boreal-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/docs/boreal.audio_widgets.rst` & `boreal-0.8.3/docs/boreal.audio_widgets.rst`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/docs/conf.py` & `boreal-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/docs/history.rst` & `boreal-0.8.3/docs/history.rst`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/docs/installation.rst` & `boreal-0.8.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/docs/make.bat` & `boreal-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `boreal-0.8.2/setup.cfg` & `boreal-0.8.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.2
+current_version = 0.8.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -21,18 +21,16 @@
 packages = find:
 include_package_data = True
 install_requires = 
 	bokeh>=2.3.3
 	ipykernel>=5.3.4
 	ipython>=7.9.0
 	notebook>=5.3.0
-	numpy>=1.21.5
 	pyaudio>=0.2.12
 	requests>=2.27.1
-	scipy>=1.7.3
 	setuptools>=61.2.0
 	SoundFile>=0.10.3.post1
 python_requires = >=3.7
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `boreal-0.8.2/setup.py` & `boreal-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     package_data={'': ['beatles.wav', 'audio_widgets/description.html']}, 
     keywords='boreal',
     name='boreal',
     packages=find_packages(include=['boreal', 'boreal.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/gtzan/boreal',
-    version='0.8.2',
+    version='0.8.3',
     zip_safe=False,
 )
```

