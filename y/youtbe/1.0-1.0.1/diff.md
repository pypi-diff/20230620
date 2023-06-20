# Comparing `tmp/youtbe-1.0.tar.gz` & `tmp/youtbe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtbe-1.0.tar", last modified: Tue Jun 20 16:50:52 2023, max compression
+gzip compressed data, was "youtbe-1.0.1.tar", last modified: Tue Jun 20 18:43:23 2023, max compression
```

## Comparing `youtbe-1.0.tar` & `youtbe-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 16:50:52.778383 youtbe-1.0/
--rw-rw-rw-   0        0        0     1309 2023-06-20 16:50:52.777391 youtbe-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      779 2023-06-19 19:57:04.000000 youtbe-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 16:50:52.778383 youtbe-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-06-20 16:49:32.000000 youtbe-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:50:52.775385 youtbe-1.0/youtbe.egg-info/
--rw-rw-rw-   0        0        0     1309 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 18:43:23.371578 youtbe-1.0.1/
+-rw-rw-rw-   0        0        0     1285 2023-06-20 18:43:23.370578 youtbe-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2023-06-20 18:36:58.000000 youtbe-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 18:43:23.371578 youtbe-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-06-20 18:42:57.000000 youtbe-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:43:23.352602 youtbe-1.0.1/youtbe/
+-rw-rw-rw-   0        0        0       89 2023-06-20 18:37:24.000000 youtbe-1.0.1/youtbe/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-06-20 18:38:18.000000 youtbe-1.0.1/youtbe/base.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:43:23.368579 youtbe-1.0.1/youtbe.egg-info/
+-rw-rw-rw-   0        0        0     1285 2023-06-20 18:43:23.000000 youtbe-1.0.1/youtbe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-20 18:43:23.000000 youtbe-1.0.1/youtbe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 18:43:23.000000 youtbe-1.0.1/youtbe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-20 18:43:23.000000 youtbe-1.0.1/youtbe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 18:43:23.000000 youtbe-1.0.1/youtbe.egg-info/top_level.txt
```

### Comparing `youtbe-1.0/PKG-INFO` & `youtbe-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: youtbe
-Version: 1.0
-Summary: Scrap Any Youtube Stats
+Version: 1.0.1
+Summary: Package to Scrap Stats from Youtube Video
 Author: vardxg
 Author-email: <dev@vardxg.com>
 Keywords: python,video,stats,video stats
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -20,22 +20,23 @@
 
 ## Examples of How To Use (Alpha Version)
 
 How To Start
 
 ```python
 from youtbe import videoStats
-from zeus import banner # When u want Print The Banner, before response.
+from youtbe import banner
 from vardxg import Center, Colors, Write # For Color, Style etc
 
 # Supported link formats are: https://www.youtube.com/watch?v=kffacxfA7G4, and Mobile Links
 #Only links like this please! because my api automatically pulls the videoid from the link.
 
 odin = banner() # Define the Banner as logo
 
 Write.Print(Center.XCenter(odin), Colors.red, interval=0) # Prints the Banner Centered, cuz the Fuctions Provided
 
 result = videoStats(input("\n Link >>> "))
+
 print(result)
 
 ```
 if u have Questions, contact me on Telegram: https://t.me/Fhivo
```

### Comparing `youtbe-1.0/README.md` & `youtbe-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 
 ## Examples of How To Use (Alpha Version)
 
 How To Start
 
 ```python
 from youtbe import videoStats
-from zeus import banner # When u want Print The Banner, before response.
+from youtbe import banner
 from vardxg import Center, Colors, Write # For Color, Style etc
 
 # Supported link formats are: https://www.youtube.com/watch?v=kffacxfA7G4, and Mobile Links
 #Only links like this please! because my api automatically pulls the videoid from the link.
 
 odin = banner() # Define the Banner as logo
 
 Write.Print(Center.XCenter(odin), Colors.red, interval=0) # Prints the Banner Centered, cuz the Fuctions Provided
 
 result = videoStats(input("\n Link >>> "))
+
 print(result)
 
 ```
 if u have Questions, contact me on Telegram: https://t.me/Fhivo
```

### Comparing `youtbe-1.0/setup.py` & `youtbe-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0'
-DESCRIPTION = 'Scrap Any Youtube Stats'
+VERSION = '1.0.1'
+DESCRIPTION = 'Package to Scrap Stats from Youtube Video'
 LONG_DESCRIPTION = 'Simple Package to Scrap Basic Stats from any Youtube Video.'
 
 # Setting up
 setup(
     name="youtbe",
     version=VERSION,
     author="vardxg",
```

### Comparing `youtbe-1.0/youtbe.egg-info/PKG-INFO` & `youtbe-1.0.1/youtbe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: youtbe
-Version: 1.0
-Summary: Scrap Any Youtube Stats
+Version: 1.0.1
+Summary: Package to Scrap Stats from Youtube Video
 Author: vardxg
 Author-email: <dev@vardxg.com>
 Keywords: python,video,stats,video stats
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -20,22 +20,23 @@
 
 ## Examples of How To Use (Alpha Version)
 
 How To Start
 
 ```python
 from youtbe import videoStats
-from zeus import banner # When u want Print The Banner, before response.
+from youtbe import banner
 from vardxg import Center, Colors, Write # For Color, Style etc
 
 # Supported link formats are: https://www.youtube.com/watch?v=kffacxfA7G4, and Mobile Links
 #Only links like this please! because my api automatically pulls the videoid from the link.
 
 odin = banner() # Define the Banner as logo
 
 Write.Print(Center.XCenter(odin), Colors.red, interval=0) # Prints the Banner Centered, cuz the Fuctions Provided
 
 result = videoStats(input("\n Link >>> "))
+
 print(result)
 
 ```
 if u have Questions, contact me on Telegram: https://t.me/Fhivo
```

