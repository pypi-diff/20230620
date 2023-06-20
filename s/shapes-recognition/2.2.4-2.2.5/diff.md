# Comparing `tmp/shapes_recognition-2.2.4.tar.gz` & `tmp/shapes_recognition-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.2.4.tar", last modified: Tue Jun 20 05:07:29 2023, max compression
+gzip compressed data, was "shapes_recognition-2.2.5.tar", last modified: Tue Jun 20 05:56:11 2023, max compression
```

## Comparing `shapes_recognition-2.2.4.tar` & `shapes_recognition-2.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-20 05:07:29.367644 shapes_recognition-2.2.4/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-20 05:07:29.367352 shapes_recognition-2.2.4/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.2.4/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-20 05:07:29.367718 shapes_recognition-2.2.4/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-20 04:43:32.000000 shapes_recognition-2.2.4/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-20 05:07:29.366912 shapes_recognition-2.2.4/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-20 05:07:29.000000 shapes_recognition-2.2.4/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-20 05:07:29.000000 shapes_recognition-2.2.4/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-20 05:07:29.000000 shapes_recognition-2.2.4/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-20 05:07:29.000000 shapes_recognition-2.2.4/shapes_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-20 05:56:11.451637 shapes_recognition-2.2.5/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-20 05:56:11.451322 shapes_recognition-2.2.5/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.2.5/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-20 05:56:11.451724 shapes_recognition-2.2.5/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-20 05:51:42.000000 shapes_recognition-2.2.5/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-20 05:56:11.450817 shapes_recognition-2.2.5/shapes_recognition.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-20 05:56:11.000000 shapes_recognition-2.2.5/shapes_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-20 05:56:11.000000 shapes_recognition-2.2.5/shapes_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-20 05:56:11.000000 shapes_recognition-2.2.5/shapes_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-20 05:56:11.000000 shapes_recognition-2.2.5/shapes_recognition.egg-info/top_level.txt
```

### Comparing `shapes_recognition-2.2.4/PKG-INFO` & `shapes_recognition-2.2.5/shapes_recognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shapes_recognition
-Version: 2.2.4
+Name: shapes-recognition
+Version: 2.2.5
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shapes_recognition-2.2.4/README.md` & `shapes_recognition-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `shapes_recognition-2.2.4/setup.py` & `shapes_recognition-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="shapes_recognition",
-    version="2.2.4",
+    version="2.2.5",
     description="New Shape Matching Technology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
```

### Comparing `shapes_recognition-2.2.4/shapes_recognition.egg-info/PKG-INFO` & `shapes_recognition-2.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shapes-recognition
-Version: 2.2.4
+Name: shapes_recognition
+Version: 2.2.5
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

