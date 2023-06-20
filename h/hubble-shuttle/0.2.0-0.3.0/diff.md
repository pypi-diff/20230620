# Comparing `tmp/hubble_shuttle-0.2.0.tar.gz` & `tmp/hubble_shuttle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hubble_shuttle-0.2.0.tar", last modified: Tue Dec  8 10:23:38 2020, max compression
+gzip compressed data, was "hubble_shuttle-0.3.0.tar", last modified: Tue Jun 20 11:31:29 2023, max compression
```

## Comparing `hubble_shuttle-0.2.0.tar` & `hubble_shuttle-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-08 10:23:38.871369 hubble_shuttle-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     9506 2020-12-08 10:23:38.862472 hubble_shuttle-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7409 2020-12-07 17:47:09.000000 hubble_shuttle-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-08 10:23:38.720072 hubble_shuttle-0.2.0/hubble_shuttle/
--rw-r--r--   0 root         (0) root         (0)       30 2020-12-07 17:47:09.000000 hubble_shuttle-0.2.0/hubble_shuttle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1320 2020-12-07 17:47:09.000000 hubble_shuttle-0.2.0/hubble_shuttle/api.py
--rw-r--r--   0 root         (0) root         (0)     1134 2020-12-08 10:18:27.000000 hubble_shuttle-0.2.0/hubble_shuttle/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5272 2020-12-07 17:47:09.000000 hubble_shuttle-0.2.0/hubble_shuttle/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-08 10:23:38.842325 hubble_shuttle-0.2.0/hubble_shuttle/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2020-12-07 17:47:09.000000 hubble_shuttle-0.2.0/hubble_shuttle/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1430 2020-12-07 17:47:09.000000 hubble_shuttle-0.2.0/hubble_shuttle/tests/tests_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1549 2020-12-07 17:47:09.000000 hubble_shuttle-0.2.0/hubble_shuttle/tests/tests_requests_transport.py
--rw-r--r--   0 root         (0) root         (0)    40444 2020-12-08 10:18:27.000000 hubble_shuttle-0.2.0/hubble_shuttle/tests/tests_shuttle_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-08 10:23:38.783376 hubble_shuttle-0.2.0/hubble_shuttle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9506 2020-12-08 10:23:38.000000 hubble_shuttle-0.2.0/hubble_shuttle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2020-12-08 10:23:38.000000 hubble_shuttle-0.2.0/hubble_shuttle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-08 10:23:38.000000 hubble_shuttle-0.2.0/hubble_shuttle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2020-12-08 10:23:38.000000 hubble_shuttle-0.2.0/hubble_shuttle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-12-08 10:23:38.874442 hubble_shuttle-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      670 2020-12-08 10:19:26.000000 hubble_shuttle-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:31:29.770752 hubble_shuttle-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7901 2023-06-20 11:31:29.767314 hubble_shuttle-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:31:29.643930 hubble_shuttle-0.3.0/hubble_shuttle/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/api.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:31:29.750668 hubble_shuttle-0.3.0/hubble_shuttle/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/tests/tests_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/tests/tests_requests_transport.py
+-rw-r--r--   0 root         (0) root         (0)    40444 2023-06-16 10:32:23.000000 hubble_shuttle-0.3.0/hubble_shuttle/tests/tests_shuttle_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:31:29.699590 hubble_shuttle-0.3.0/hubble_shuttle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7901 2023-06-20 11:31:29.000000 hubble_shuttle-0.3.0/hubble_shuttle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-20 11:31:29.000000 hubble_shuttle-0.3.0/hubble_shuttle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:31:29.000000 hubble_shuttle-0.3.0/hubble_shuttle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 11:31:29.000000 hubble_shuttle-0.3.0/hubble_shuttle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 11:31:29.772803 hubble_shuttle-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      670 2023-06-16 14:36:38.000000 hubble_shuttle-0.3.0/setup.py
```

### Comparing `hubble_shuttle-0.2.0/README.md` & `hubble_shuttle-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hubble_shuttle-0.2.0/hubble_shuttle/api.py` & `hubble_shuttle-0.3.0/hubble_shuttle/api.py`

 * *Files identical despite different names*

### Comparing `hubble_shuttle-0.2.0/hubble_shuttle/exceptions.py` & `hubble_shuttle-0.3.0/hubble_shuttle/exceptions.py`

 * *Files identical despite different names*

### Comparing `hubble_shuttle-0.2.0/hubble_shuttle/http.py` & `hubble_shuttle-0.3.0/hubble_shuttle/http.py`

 * *Files identical despite different names*

### Comparing `hubble_shuttle-0.2.0/hubble_shuttle/tests/tests_exceptions.py` & `hubble_shuttle-0.3.0/hubble_shuttle/tests/tests_exceptions.py`

 * *Files identical despite different names*

### Comparing `hubble_shuttle-0.2.0/hubble_shuttle/tests/tests_requests_transport.py` & `hubble_shuttle-0.3.0/hubble_shuttle/tests/tests_requests_transport.py`

 * *Files identical despite different names*

### Comparing `hubble_shuttle-0.2.0/hubble_shuttle/tests/tests_shuttle_api.py` & `hubble_shuttle-0.3.0/hubble_shuttle/tests/tests_shuttle_api.py`

 * *Files identical despite different names*

### Comparing `hubble_shuttle-0.2.0/setup.py` & `hubble_shuttle-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hubble_shuttle",
-    version="0.2.0",
+    version="0.3.0",
     author="HubbleHQ",
     author_email="dev@hubblehq.com",
     description="Hubble's Shuttle",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HubbleHQ/shuttle",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.5',
+    python_requires=">=3.7",
 )
```

