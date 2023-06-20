# Comparing `tmp/serializer_prefetch-1.0.1.tar.gz` & `tmp/serializer_prefetch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_prefetch-1.0.1.tar", last modified: Tue Jun 20 15:04:40 2023, max compression
+gzip compressed data, was "serializer_prefetch-1.0.2.tar", last modified: Tue Jun 20 15:37:06 2023, max compression
```

## Comparing `serializer_prefetch-1.0.1.tar` & `serializer_prefetch-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 serializer_prefetch-1.0.1/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)     8996 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     8750 2023-06-20 14:39:57.000000 serializer_prefetch-1.0.1/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/serializer_prefetch/
--rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 serializer_prefetch-1.0.1/serializer_prefetch/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    11814 2023-06-20 14:27:16.000000 serializer_prefetch-1.0.1/serializer_prefetch/base.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)     8996 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      300 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       20 2023-06-20 15:04:40.000000 serializer_prefetch-1.0.1/serializer_prefetch.egg-info/top_level.txt
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 15:04:40.897017 serializer_prefetch-1.0.1/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      610 2023-06-20 15:04:14.000000 serializer_prefetch-1.0.1/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:37:06.337741 serializer_prefetch-1.0.2/
+-rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 serializer_prefetch-1.0.2/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)     8992 2023-06-20 15:37:06.337741 serializer_prefetch-1.0.2/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     8746 2023-06-20 15:36:55.000000 serializer_prefetch-1.0.2/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:37:06.337741 serializer_prefetch-1.0.2/serializer_prefetch/
+-rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 serializer_prefetch-1.0.2/serializer_prefetch/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11814 2023-06-20 14:27:16.000000 serializer_prefetch-1.0.2/serializer_prefetch/base.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:37:06.337741 serializer_prefetch-1.0.2/serializer_prefetch.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)     8992 2023-06-20 15:37:06.000000 serializer_prefetch-1.0.2/serializer_prefetch.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      300 2023-06-20 15:37:06.000000 serializer_prefetch-1.0.2/serializer_prefetch.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 15:37:06.000000 serializer_prefetch-1.0.2/serializer_prefetch.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 15:37:06.000000 serializer_prefetch-1.0.2/serializer_prefetch.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2023-06-20 15:37:06.000000 serializer_prefetch-1.0.2/serializer_prefetch.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 15:37:06.337741 serializer_prefetch-1.0.2/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      610 2023-06-20 15:37:04.000000 serializer_prefetch-1.0.2/setup.py
```

### Comparing `serializer_prefetch-1.0.1/LICENSE` & `serializer_prefetch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serializer_prefetch-1.0.1/PKG-INFO` & `serializer_prefetch-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: serializer_prefetch
-Version: 1.0.1
+Version: 1.0.2
 Summary: An automatic prefetcher for django-rest-framework.
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # drf-serializer-prefetch
 
 An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
 
 ## Installation
 
-To install, call `pip install drf-serializer-prefetch`.
+To install, call `pip install serializer-prefetch`.
 
 ## Usage
 
 In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
 
 ``` python
 from rest_framework import serializers
```

### Comparing `serializer_prefetch-1.0.1/README.md` & `serializer_prefetch-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # drf-serializer-prefetch
 
 An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
 
 ## Installation
 
-To install, call `pip install drf-serializer-prefetch`.
+To install, call `pip install serializer-prefetch`.
 
 ## Usage
 
 In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
 
 ``` python
 from rest_framework import serializers
```

### Comparing `serializer_prefetch-1.0.1/serializer_prefetch/base.py` & `serializer_prefetch-1.0.2/serializer_prefetch/base.py`

 * *Files identical despite different names*

### Comparing `serializer_prefetch-1.0.1/serializer_prefetch.egg-info/PKG-INFO` & `serializer_prefetch-1.0.2/serializer_prefetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: serializer-prefetch
-Version: 1.0.1
+Version: 1.0.2
 Summary: An automatic prefetcher for django-rest-framework.
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # drf-serializer-prefetch
 
 An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
 
 ## Installation
 
-To install, call `pip install drf-serializer-prefetch`.
+To install, call `pip install serializer-prefetch`.
 
 ## Usage
 
 In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
 
 ``` python
 from rest_framework import serializers
```

### Comparing `serializer_prefetch-1.0.1/setup.py` & `serializer_prefetch-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "An automatic prefetcher for django-rest-framework."
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 setup(
     name="serializer_prefetch",
     version=VERSION,
```

