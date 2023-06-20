# Comparing `tmp/drf-serializer-prefetch-1.0.6.tar.gz` & `tmp/drf-serializer-prefetch-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-serializer-prefetch-1.0.6.tar", last modified: Tue Jun 20 17:29:00 2023, max compression
+gzip compressed data, was "drf-serializer-prefetch-1.0.7.tar", last modified: Tue Jun 20 19:55:30 2023, max compression
```

## Comparing `drf-serializer-prefetch-1.0.6.tar` & `drf-serializer-prefetch-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:29:00.446236 drf-serializer-prefetch-1.0.6/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.0.6/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)     9130 2023-06-20 17:29:00.446236 drf-serializer-prefetch-1.0.6/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     8815 2023-06-20 16:22:03.000000 drf-serializer-prefetch-1.0.6/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:29:00.446236 drf-serializer-prefetch-1.0.6/drf_serializer_prefetch.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)     9130 2023-06-20 17:29:00.000000 drf-serializer-prefetch-1.0.6/drf_serializer_prefetch.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      338 2023-06-20 17:29:00.000000 drf-serializer-prefetch-1.0.6/drf_serializer_prefetch.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 17:29:00.000000 drf-serializer-prefetch-1.0.6/drf_serializer_prefetch.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 17:29:00.000000 drf-serializer-prefetch-1.0.6/drf_serializer_prefetch.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       26 2023-06-20 17:29:00.000000 drf-serializer-prefetch-1.0.6/drf_serializer_prefetch.egg-info/top_level.txt
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:29:00.446236 drf-serializer-prefetch-1.0.6/serializer_prefetch/
--rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.0.6/serializer_prefetch/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    11767 2023-06-20 17:27:49.000000 drf-serializer-prefetch-1.0.6/serializer_prefetch/base.py
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 17:29:00.446236 drf-serializer-prefetch-1.0.6/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      679 2023-06-20 17:28:45.000000 drf-serializer-prefetch-1.0.6/setup.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:29:00.446236 drf-serializer-prefetch-1.0.6/tests/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-20 15:59:03.000000 drf-serializer-prefetch-1.0.6/tests/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 19:55:30.607313 drf-serializer-prefetch-1.0.7/
+-rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.0.7/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)     9130 2023-06-20 19:55:30.607313 drf-serializer-prefetch-1.0.7/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     8815 2023-06-20 16:22:03.000000 drf-serializer-prefetch-1.0.7/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 19:55:30.607313 drf-serializer-prefetch-1.0.7/drf_serializer_prefetch.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)     9130 2023-06-20 19:55:30.000000 drf-serializer-prefetch-1.0.7/drf_serializer_prefetch.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      398 2023-06-20 19:55:30.000000 drf-serializer-prefetch-1.0.7/drf_serializer_prefetch.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 19:55:30.000000 drf-serializer-prefetch-1.0.7/drf_serializer_prefetch.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 19:55:30.000000 drf-serializer-prefetch-1.0.7/drf_serializer_prefetch.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       26 2023-06-20 19:55:30.000000 drf-serializer-prefetch-1.0.7/drf_serializer_prefetch.egg-info/top_level.txt
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 19:55:30.607313 drf-serializer-prefetch-1.0.7/serializer_prefetch/
+-rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.0.7/serializer_prefetch/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11870 2023-06-20 19:49:26.000000 drf-serializer-prefetch-1.0.7/serializer_prefetch/base.py
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 19:55:30.607313 drf-serializer-prefetch-1.0.7/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      679 2023-06-20 19:55:24.000000 drf-serializer-prefetch-1.0.7/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 19:55:30.607313 drf-serializer-prefetch-1.0.7/tests/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-20 15:59:03.000000 drf-serializer-prefetch-1.0.7/tests/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      265 2023-06-20 19:01:15.000000 drf-serializer-prefetch-1.0.7/tests/models.py
+-rw-rw-r--   0 max       (1000) max       (1000)      381 2023-06-20 18:58:38.000000 drf-serializer-prefetch-1.0.7/tests/settings.py
+-rw-rw-r--   0 max       (1000) max       (1000)     6615 2023-06-20 19:53:22.000000 drf-serializer-prefetch-1.0.7/tests/test_serializers.py
```

### Comparing `drf-serializer-prefetch-1.0.6/LICENSE` & `drf-serializer-prefetch-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.6/PKG-INFO` & `drf-serializer-prefetch-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.6
+Version: 1.0.7
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drf-serializer-prefetch-1.0.6/README.md` & `drf-serializer-prefetch-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.6/drf_serializer_prefetch.egg-info/PKG-INFO` & `drf-serializer-prefetch-1.0.7/drf_serializer_prefetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.6
+Version: 1.0.7
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `drf-serializer-prefetch-1.0.6/serializer_prefetch/base.py` & `drf-serializer-prefetch-1.0.7/serializer_prefetch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,16 @@
         select_items = []
         prefetch_items = []
 
         for additional_serializer_data in additional_serializers:
             custom_current_relation = additional_serializer_data.get(
                 "relation_and_field", ""
             )
+            if custom_current_relation:
+                prefetch_items.append(custom_current_relation)
 
             if current_relation:
                 custom_current_relation = self._get_joined_prefetch(
                     current_relation, custom_current_relation
                 )
 
             additional_serializer = additional_serializer_data.get("serializer")
```

### Comparing `drf-serializer-prefetch-1.0.6/setup.py` & `drf-serializer-prefetch-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 DESCRIPTION = "An automatic prefetcher for django-rest-framework."
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 setup(
     name="drf-serializer-prefetch",
     version=VERSION,
```

