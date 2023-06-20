# Comparing `tmp/shapes_recognition-2.2.2.tar.gz` & `tmp/shapes_recognition-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.2.2.tar", last modified: Mon Jun 19 18:48:59 2023, max compression
+gzip compressed data, was "shapes_recognition-2.2.3.tar", last modified: Tue Jun 20 03:29:35 2023, max compression
```

## Comparing `shapes_recognition-2.2.2.tar` & `shapes_recognition-2.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-19 18:48:59.399436 shapes_recognition-2.2.2/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-19 18:48:59.399141 shapes_recognition-2.2.2/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.2.2/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-19 18:48:59.399518 shapes_recognition-2.2.2/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-19 17:36:28.000000 shapes_recognition-2.2.2/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-19 18:48:59.398727 shapes_recognition-2.2.2/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-19 18:48:59.000000 shapes_recognition-2.2.2/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-19 18:48:59.000000 shapes_recognition-2.2.2/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-19 18:48:59.000000 shapes_recognition-2.2.2/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-19 18:48:59.000000 shapes_recognition-2.2.2/shapes_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-20 03:29:35.663707 shapes_recognition-2.2.3/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1175 2023-06-20 03:29:35.663474 shapes_recognition-2.2.3/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.2.3/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-20 03:29:35.663783 shapes_recognition-2.2.3/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-20 03:24:23.000000 shapes_recognition-2.2.3/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-20 03:29:35.663126 shapes_recognition-2.2.3/shapes_recognition.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1175 2023-06-20 03:29:35.000000 shapes_recognition-2.2.3/shapes_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-20 03:29:35.000000 shapes_recognition-2.2.3/shapes_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-20 03:29:35.000000 shapes_recognition-2.2.3/shapes_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-20 03:29:35.000000 shapes_recognition-2.2.3/shapes_recognition.egg-info/top_level.txt
```

### Comparing `shapes_recognition-2.2.2/PKG-INFO` & `shapes_recognition-2.2.3/shapes_recognition.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: shapes_recognition
-Version: 2.2.2
+Name: shapes-recognition
+Version: 2.2.3
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
@@ -26,7 +27,9 @@
 
 <p align="center"><img src="https://boriskravtsov.com/pypi/shapes.png"/>
 
 To simulate such recognition capability, we introduce the **shapes_recognition** library.
 
 [Here](https://kravtsov-development.medium.com/amazing-ai-tables-44af52c993a2) 
 we show how to use it. 
+
+
```

### Comparing `shapes_recognition-2.2.2/README.md` & `shapes_recognition-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `shapes_recognition-2.2.2/setup.py` & `shapes_recognition-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="shapes_recognition",
-    version="2.2.2",
+    version="2.2.3",
     description="New Shape Matching Technology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
```

### Comparing `shapes_recognition-2.2.2/shapes_recognition.egg-info/PKG-INFO` & `shapes_recognition-2.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: shapes-recognition
-Version: 2.2.2
+Name: shapes_recognition
+Version: 2.2.3
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
@@ -26,7 +27,9 @@
 
 <p align="center"><img src="https://boriskravtsov.com/pypi/shapes.png"/>
 
 To simulate such recognition capability, we introduce the **shapes_recognition** library.
 
 [Here](https://kravtsov-development.medium.com/amazing-ai-tables-44af52c993a2) 
 we show how to use it. 
+
+
```

