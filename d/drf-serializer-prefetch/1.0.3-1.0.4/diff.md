# Comparing `tmp/drf-serializer-prefetch-1.0.3.tar.gz` & `tmp/drf-serializer-prefetch-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-serializer-prefetch-1.0.3.tar", last modified: Tue Jun 20 15:49:37 2023, max compression
+gzip compressed data, was "drf-serializer-prefetch-1.0.4.tar", last modified: Tue Jun 20 15:55:52 2023, max compression
```

## Comparing `drf-serializer-prefetch-1.0.3.tar` & `drf-serializer-prefetch-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:49:37.176715 drf-serializer-prefetch-1.0.3/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.0.3/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)     9000 2023-06-20 15:49:37.176715 drf-serializer-prefetch-1.0.3/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     8750 2023-06-20 15:49:10.000000 drf-serializer-prefetch-1.0.3/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:49:37.176715 drf-serializer-prefetch-1.0.3/drf_serializer_prefetch.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)     9000 2023-06-20 15:49:37.000000 drf-serializer-prefetch-1.0.3/drf_serializer_prefetch.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      320 2023-06-20 15:49:37.000000 drf-serializer-prefetch-1.0.3/drf_serializer_prefetch.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 15:49:37.000000 drf-serializer-prefetch-1.0.3/drf_serializer_prefetch.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 15:49:37.000000 drf-serializer-prefetch-1.0.3/drf_serializer_prefetch.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       20 2023-06-20 15:49:37.000000 drf-serializer-prefetch-1.0.3/drf_serializer_prefetch.egg-info/top_level.txt
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:49:37.176715 drf-serializer-prefetch-1.0.3/serializer_prefetch/
--rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.0.3/serializer_prefetch/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    11814 2023-06-20 14:27:16.000000 drf-serializer-prefetch-1.0.3/serializer_prefetch/base.py
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 15:49:37.176715 drf-serializer-prefetch-1.0.3/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      614 2023-06-20 15:48:58.000000 drf-serializer-prefetch-1.0.3/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/
+-rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.0.4/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)     9065 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     8750 2023-06-20 15:49:10.000000 drf-serializer-prefetch-1.0.4/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)     9065 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      320 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/top_level.txt
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/serializer_prefetch/
+-rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.0.4/serializer_prefetch/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11814 2023-06-20 14:27:16.000000 drf-serializer-prefetch-1.0.4/serializer_prefetch/base.py
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      679 2023-06-20 15:55:48.000000 drf-serializer-prefetch-1.0.4/setup.py
```

### Comparing `drf-serializer-prefetch-1.0.3/LICENSE` & `drf-serializer-prefetch-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.3/PKG-INFO` & `drf-serializer-prefetch-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.3
+Version: 1.0.4
 Summary: An automatic prefetcher for django-rest-framework.
+Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # drf-serializer-prefetch
```

### Comparing `drf-serializer-prefetch-1.0.3/README.md` & `drf-serializer-prefetch-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.3/drf_serializer_prefetch.egg-info/PKG-INFO` & `drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.3
+Version: 1.0.4
 Summary: An automatic prefetcher for django-rest-framework.
+Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # drf-serializer-prefetch
```

### Comparing `drf-serializer-prefetch-1.0.3/serializer_prefetch/base.py` & `drf-serializer-prefetch-1.0.4/serializer_prefetch/base.py`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.3/setup.py` & `drf-serializer-prefetch-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 DESCRIPTION = "An automatic prefetcher for django-rest-framework."
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 setup(
     name="drf-serializer-prefetch",
     version=VERSION,
     author="Maxime Toussaint",
     author_email="m.toussaint@mail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=("django>=3.2.0", "djangorestframework>=3.12"),
+    url="https://github.com/MaxDude132/drf-serializer-prefetch",
 )
```

