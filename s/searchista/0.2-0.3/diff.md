# Comparing `tmp/searchista-0.2.tar.gz` & `tmp/searchista-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchista-0.2.tar", last modified: Tue Jun 20 13:29:33 2023, max compression
+gzip compressed data, was "searchista-0.3.tar", last modified: Tue Jun 20 14:22:30 2023, max compression
```

## Comparing `searchista-0.2.tar` & `searchista-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 13:29:33.085214 searchista-0.2/
--rw-rw----   0 root         (0) everybody  (9997)       30 2023-06-20 13:28:34.000000 searchista-0.2/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      846 2023-06-20 13:29:33.077214 searchista-0.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      398 2023-06-20 13:18:01.000000 searchista-0.2/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-20 13:29:33.085214 searchista-0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      923 2023-06-20 13:27:29.000000 searchista-0.2/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 13:29:32.885214 searchista-0.2/src/
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 13:29:33.001214 searchista-0.2/src/searchista/
--rw-rw----   0 root         (0) everybody  (9997)       25 2023-06-20 13:27:21.000000 searchista-0.2/src/searchista/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      192 2023-06-20 13:14:48.000000 searchista-0.2/src/searchista/searchista.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 13:29:33.065214 searchista-0.2/src/searchista.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      846 2023-06-20 13:29:32.000000 searchista-0.2/src/searchista.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      238 2023-06-20 13:29:32.000000 searchista-0.2/src/searchista.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-20 13:29:32.000000 searchista-0.2/src/searchista.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-20 13:29:32.000000 searchista-0.2/src/searchista.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 14:22:30.493467 searchista-0.3/
+-rw-rw----   0 root         (0) everybody  (9997)       30 2023-06-20 13:28:34.000000 searchista-0.3/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      847 2023-06-20 14:22:30.481467 searchista-0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      399 2023-06-20 14:21:38.000000 searchista-0.3/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-20 14:22:30.493467 searchista-0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      923 2023-06-20 14:22:07.000000 searchista-0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 14:22:30.389467 searchista-0.3/src/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 14:22:30.425467 searchista-0.3/src/searchista/
+-rw-rw----   0 root         (0) everybody  (9997)       25 2023-06-20 13:27:21.000000 searchista-0.3/src/searchista/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      192 2023-06-20 13:14:48.000000 searchista-0.3/src/searchista/searchista.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 14:22:30.465467 searchista-0.3/src/searchista.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      847 2023-06-20 14:22:30.000000 searchista-0.3/src/searchista.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      238 2023-06-20 14:22:30.000000 searchista-0.3/src/searchista.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-20 14:22:30.000000 searchista-0.3/src/searchista.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-20 14:22:30.000000 searchista-0.3/src/searchista.egg-info/top_level.txt
```

### Comparing `searchista-0.2/PKG-INFO` & `searchista-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: searchista
-Version: 0.2
+Version: 0.3
 Summary: •search username in instagram
 Home-page: 
 Author: searchistax
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-<h1 align="center">HamodyToola</h1>
+<h1 align="center">search insta</h1>
 <p align="center">It's a Usefull Project for Developers ... search username in instagram with word</p>
 
 <p align="center"> • DevVlopered The Lib BY ALAA7X • </p>
 
 
 ## Installing :
 ```
```

### Comparing `searchista-0.2/setup.py` & `searchista-0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 f.write('instaloder\nuser_agent\nrequests')
 
 fr = open("requirements.txt",'r')
 requires = fr.read().split('\n')
     
 setuptools.setup(
     name="searchista",
-    version="0.2",
+    version="0.3",
     author="searchistax",
     author_email="",
     description="•search username in instagram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `searchista-0.2/src/searchista.egg-info/PKG-INFO` & `searchista-0.3/src/searchista.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: searchista
-Version: 0.2
+Version: 0.3
 Summary: •search username in instagram
 Home-page: 
 Author: searchistax
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-<h1 align="center">HamodyToola</h1>
+<h1 align="center">search insta</h1>
 <p align="center">It's a Usefull Project for Developers ... search username in instagram with word</p>
 
 <p align="center"> • DevVlopered The Lib BY ALAA7X • </p>
 
 
 ## Installing :
 ```
```

