# Comparing `tmp/dvg-randomizer-1.4.2.tar.gz` & `tmp/dvg-randomizer-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvg-randomizer-1.4.2.tar", last modified: Fri May 26 10:48:25 2023, max compression
+gzip compressed data, was "dvg-randomizer-1.4.3.tar", last modified: Tue Jun 20 11:24:10 2023, max compression
```

## Comparing `dvg-randomizer-1.4.2.tar` & `dvg-randomizer-1.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.680579 dvg-randomizer-1.4.2/
--rw-r--r--   0 jquelin   (5000) users      (100)    35149 2017-09-30 07:16:26.000000 dvg-randomizer-1.4.2/COPYING
--rw-r--r--   0 jquelin   (5000) users      (100)      716 2022-02-07 14:15:49.000000 dvg-randomizer-1.4.2/LICENSE
--rw-r--r--   0 jquelin   (5000) users      (100)      156 2023-05-26 10:32:26.000000 dvg-randomizer-1.4.2/MANIFEST.in
--rw-r--r--   0 jquelin   (5000) users      (100)     1970 2023-05-26 10:48:25.679579 dvg-randomizer-1.4.2/PKG-INFO
--rw-r--r--   0 jquelin   (5000) users      (100)     1386 2023-05-26 10:45:44.000000 dvg-randomizer-1.4.2/README.md
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.677579 dvg-randomizer-1.4.2/dvg_randomizer/
--rw-r--r--   0 jquelin   (5000) users      (100)      815 2022-12-10 14:56:14.000000 dvg-randomizer-1.4.2/dvg_randomizer/__main__.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1712 2023-05-25 12:50:05.000000 dvg-randomizer-1.4.2/dvg_randomizer/aircraft.py
--rw-r--r--   0 jquelin   (5000) users      (100)     6122 2023-05-25 11:06:48.000000 dvg-randomizer-1.4.2/dvg_randomizer/boardgame.py
--rw-r--r--   0 jquelin   (5000) users      (100)     3866 2023-05-26 08:56:42.000000 dvg-randomizer-1.4.2/dvg_randomizer/campaign.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1512 2022-12-10 12:58:30.000000 dvg-randomizer-1.4.2/dvg_randomizer/config.py
--rw-r--r--   0 jquelin   (5000) users      (100)     9179 2023-05-26 08:48:30.000000 dvg-randomizer-1.4.2/dvg_randomizer/data.py
--rw-r--r--   0 jquelin   (5000) users      (100)    45175 2023-05-26 09:01:35.000000 dvg-randomizer-1.4.2/dvg_randomizer/dvg.ods
--rwxr-xr-x   0 jquelin   (5000) users      (100)     6111 2022-12-12 17:02:41.000000 dvg-randomizer-1.4.2/dvg_randomizer/game.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.678578 dvg-randomizer-1.4.2/dvg_randomizer/gui/
--rw-r--r--   0 jquelin   (5000) users      (100)     5930 2022-12-10 13:12:48.000000 dvg-randomizer-1.4.2/dvg_randomizer/gui/composition.py
--rw-r--r--   0 jquelin   (5000) users      (100)    14179 2022-12-10 13:27:14.000000 dvg-randomizer-1.4.2/dvg_randomizer/gui/main.py
--rw-r--r--   0 jquelin   (5000) users      (100)     1203 2022-12-10 13:03:44.000000 dvg-randomizer-1.4.2/dvg_randomizer/logger.py
--rw-r--r--   0 jquelin   (5000) users      (100)    16460 2023-05-25 14:33:55.000000 dvg-randomizer-1.4.2/dvg_randomizer/logsheet.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.679579 dvg-randomizer-1.4.2/dvg_randomizer/misc/
--rw-r--r--   0 jquelin   (5000) users      (100)   755124 2021-12-07 18:53:06.000000 dvg-randomizer-1.4.2/dvg_randomizer/misc/DejaVuSansCondensed.ttf
--rw-r--r--   0 jquelin   (5000) users      (100)     2425 2023-05-26 08:45:33.000000 dvg-randomizer-1.4.2/dvg_randomizer/pilot.py
-drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-05-26 10:48:25.678578 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/
--rw-r--r--   0 jquelin   (5000) users      (100)     1970 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/PKG-INFO
--rw-r--r--   0 jquelin   (5000) users      (100)      666 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/SOURCES.txt
--rw-r--r--   0 jquelin   (5000) users      (100)        1 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/dependency_links.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       63 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/entry_points.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       34 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/requires.txt
--rw-r--r--   0 jquelin   (5000) users      (100)       15 2023-05-26 10:48:25.000000 dvg-randomizer-1.4.2/dvg_randomizer.egg-info/top_level.txt
--rw-r--r--   0 jquelin   (5000) users      (100)      784 2023-05-26 10:47:57.000000 dvg-randomizer-1.4.2/pyproject.toml
--rw-r--r--   0 jquelin   (5000) users      (100)       38 2023-05-26 10:48:25.680579 dvg-randomizer-1.4.2/setup.cfg
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-06-20 11:24:10.108477 dvg-randomizer-1.4.3/
+-rw-r--r--   0 jquelin   (5000) users      (100)    35149 2017-09-30 07:16:26.000000 dvg-randomizer-1.4.3/COPYING
+-rw-r--r--   0 jquelin   (5000) users      (100)      716 2022-02-07 14:15:49.000000 dvg-randomizer-1.4.3/LICENSE
+-rw-r--r--   0 jquelin   (5000) users      (100)      156 2023-05-26 10:32:26.000000 dvg-randomizer-1.4.3/MANIFEST.in
+-rw-r--r--   0 jquelin   (5000) users      (100)     1970 2023-06-20 11:24:10.108477 dvg-randomizer-1.4.3/PKG-INFO
+-rw-r--r--   0 jquelin   (5000) users      (100)     1386 2023-05-26 10:45:44.000000 dvg-randomizer-1.4.3/README.md
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-06-20 11:24:10.108477 dvg-randomizer-1.4.3/dvg_randomizer/
+-rw-r--r--   0 jquelin   (5000) users      (100)      815 2022-12-10 14:56:14.000000 dvg-randomizer-1.4.3/dvg_randomizer/__main__.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1712 2023-05-25 12:50:05.000000 dvg-randomizer-1.4.3/dvg_randomizer/aircraft.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     6122 2023-05-25 11:06:48.000000 dvg-randomizer-1.4.3/dvg_randomizer/boardgame.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     3866 2023-05-26 08:56:42.000000 dvg-randomizer-1.4.3/dvg_randomizer/campaign.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1512 2022-12-10 12:58:30.000000 dvg-randomizer-1.4.3/dvg_randomizer/config.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     9179 2023-05-26 08:48:30.000000 dvg-randomizer-1.4.3/dvg_randomizer/data.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    42228 2023-05-26 13:06:30.000000 dvg-randomizer-1.4.3/dvg_randomizer/dvg.ods
+-rwxr-xr-x   0 jquelin   (5000) users      (100)     6111 2022-12-12 17:02:41.000000 dvg-randomizer-1.4.3/dvg_randomizer/game.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-06-20 11:24:10.108477 dvg-randomizer-1.4.3/dvg_randomizer/gui/
+-rw-r--r--   0 jquelin   (5000) users      (100)     5930 2022-12-10 13:12:48.000000 dvg-randomizer-1.4.3/dvg_randomizer/gui/composition.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    14179 2022-12-10 13:27:14.000000 dvg-randomizer-1.4.3/dvg_randomizer/gui/main.py
+-rw-r--r--   0 jquelin   (5000) users      (100)     1203 2022-12-10 13:03:44.000000 dvg-randomizer-1.4.3/dvg_randomizer/logger.py
+-rw-r--r--   0 jquelin   (5000) users      (100)    16460 2023-05-25 14:33:55.000000 dvg-randomizer-1.4.3/dvg_randomizer/logsheet.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-06-20 11:24:10.108477 dvg-randomizer-1.4.3/dvg_randomizer/misc/
+-rw-r--r--   0 jquelin   (5000) users      (100)   755124 2021-12-07 18:53:06.000000 dvg-randomizer-1.4.3/dvg_randomizer/misc/DejaVuSansCondensed.ttf
+-rw-r--r--   0 jquelin   (5000) users      (100)     2425 2023-05-26 08:45:33.000000 dvg-randomizer-1.4.3/dvg_randomizer/pilot.py
+drwxr-xr-x   0 jquelin   (5000) users      (100)        0 2023-06-20 11:24:10.108477 dvg-randomizer-1.4.3/dvg_randomizer.egg-info/
+-rw-r--r--   0 jquelin   (5000) users      (100)     1970 2023-06-20 11:24:10.000000 dvg-randomizer-1.4.3/dvg_randomizer.egg-info/PKG-INFO
+-rw-r--r--   0 jquelin   (5000) users      (100)      666 2023-06-20 11:24:10.000000 dvg-randomizer-1.4.3/dvg_randomizer.egg-info/SOURCES.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)        1 2023-06-20 11:24:10.000000 dvg-randomizer-1.4.3/dvg_randomizer.egg-info/dependency_links.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       63 2023-06-20 11:24:10.000000 dvg-randomizer-1.4.3/dvg_randomizer.egg-info/entry_points.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       46 2023-06-20 11:24:10.000000 dvg-randomizer-1.4.3/dvg_randomizer.egg-info/requires.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)       15 2023-06-20 11:24:10.000000 dvg-randomizer-1.4.3/dvg_randomizer.egg-info/top_level.txt
+-rw-r--r--   0 jquelin   (5000) users      (100)      810 2023-06-20 11:20:29.000000 dvg-randomizer-1.4.3/pyproject.toml
+-rw-r--r--   0 jquelin   (5000) users      (100)       38 2023-06-20 11:24:10.108477 dvg-randomizer-1.4.3/setup.cfg
```

### Comparing `dvg-randomizer-1.4.2/COPYING` & `dvg-randomizer-1.4.3/COPYING`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/LICENSE` & `dvg-randomizer-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/PKG-INFO` & `dvg-randomizer-1.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvg-randomizer
-Version: 1.4.2
+Version: 1.4.3
 Summary: Randomizer app for DVG Leader boardgames
 Author-email: Jerome Quelin <jquelin@gmail.com>
 Project-URL: Homepage, https://github.com/jquelin/dvg-randomize
 Project-URL: Bug Tracker, https://github.com/jquelin/dvg-randomize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `dvg-randomizer-1.4.2/README.md` & `dvg-randomizer-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/__main__.py` & `dvg-randomizer-1.4.3/dvg_randomizer/__main__.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/aircraft.py` & `dvg-randomizer-1.4.3/dvg_randomizer/aircraft.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/boardgame.py` & `dvg-randomizer-1.4.3/dvg_randomizer/boardgame.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/campaign.py` & `dvg-randomizer-1.4.3/dvg_randomizer/campaign.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/config.py` & `dvg-randomizer-1.4.3/dvg_randomizer/config.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/data.py` & `dvg-randomizer-1.4.3/dvg_randomizer/data.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/game.py` & `dvg-randomizer-1.4.3/dvg_randomizer/game.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/gui/composition.py` & `dvg-randomizer-1.4.3/dvg_randomizer/gui/composition.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/gui/main.py` & `dvg-randomizer-1.4.3/dvg_randomizer/gui/main.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/logger.py` & `dvg-randomizer-1.4.3/dvg_randomizer/logger.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/logsheet.py` & `dvg-randomizer-1.4.3/dvg_randomizer/logsheet.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/misc/DejaVuSansCondensed.ttf` & `dvg-randomizer-1.4.3/dvg_randomizer/misc/DejaVuSansCondensed.ttf`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer/pilot.py` & `dvg-randomizer-1.4.3/dvg_randomizer/pilot.py`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer.egg-info/PKG-INFO` & `dvg-randomizer-1.4.3/dvg_randomizer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvg-randomizer
-Version: 1.4.2
+Version: 1.4.3
 Summary: Randomizer app for DVG Leader boardgames
 Author-email: Jerome Quelin <jquelin@gmail.com>
 Project-URL: Homepage, https://github.com/jquelin/dvg-randomize
 Project-URL: Bug Tracker, https://github.com/jquelin/dvg-randomize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `dvg-randomizer-1.4.2/dvg_randomizer.egg-info/SOURCES.txt` & `dvg-randomizer-1.4.3/dvg_randomizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvg-randomizer-1.4.2/pyproject.toml` & `dvg-randomizer-1.4.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dvg-randomizer"
-version = '1.4.2'
+version = '1.4.3'
 authors = [
   { name="Jerome Quelin", email="jquelin@gmail.com" },
 ]
 description = "Randomizer app for DVG Leader boardgames"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,14 +17,16 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "appdirs",
     "colorlog",
     "fpdf",
     "pyexcel_ods",
+    "pyyaml",
+    "cmd2",
 ]
 
 [project.scripts]
 dvg-randomizer = "dvg_randomizer.__main__:run"
 
 [project.urls]
 "Homepage" = "https://github.com/jquelin/dvg-randomize"
```

