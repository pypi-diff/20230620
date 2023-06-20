# Comparing `tmp/drf-serializer-prefetch-1.0.4.tar.gz` & `tmp/drf-serializer-prefetch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-serializer-prefetch-1.0.4.tar", last modified: Tue Jun 20 15:55:52 2023, max compression
+gzip compressed data, was "drf-serializer-prefetch-1.0.5.tar", last modified: Tue Jun 20 17:10:20 2023, max compression
```

## Comparing `drf-serializer-prefetch-1.0.4.tar` & `drf-serializer-prefetch-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.0.4/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)     9065 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     8750 2023-06-20 15:49:10.000000 drf-serializer-prefetch-1.0.4/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)     9065 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      320 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       20 2023-06-20 15:55:52.000000 drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/top_level.txt
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/serializer_prefetch/
--rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.0.4/serializer_prefetch/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    11814 2023-06-20 14:27:16.000000 drf-serializer-prefetch-1.0.4/serializer_prefetch/base.py
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 15:55:52.208086 drf-serializer-prefetch-1.0.4/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      679 2023-06-20 15:55:48.000000 drf-serializer-prefetch-1.0.4/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:10:20.837336 drf-serializer-prefetch-1.0.5/
+-rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.0.5/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)     9130 2023-06-20 17:10:20.837336 drf-serializer-prefetch-1.0.5/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     8815 2023-06-20 16:22:03.000000 drf-serializer-prefetch-1.0.5/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:10:20.833336 drf-serializer-prefetch-1.0.5/drf_serializer_prefetch.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)     9130 2023-06-20 17:10:20.000000 drf-serializer-prefetch-1.0.5/drf_serializer_prefetch.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      338 2023-06-20 17:10:20.000000 drf-serializer-prefetch-1.0.5/drf_serializer_prefetch.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-20 17:10:20.000000 drf-serializer-prefetch-1.0.5/drf_serializer_prefetch.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       40 2023-06-20 17:10:20.000000 drf-serializer-prefetch-1.0.5/drf_serializer_prefetch.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       26 2023-06-20 17:10:20.000000 drf-serializer-prefetch-1.0.5/drf_serializer_prefetch.egg-info/top_level.txt
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:10:20.833336 drf-serializer-prefetch-1.0.5/serializer_prefetch/
+-rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.0.5/serializer_prefetch/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11760 2023-06-20 17:09:35.000000 drf-serializer-prefetch-1.0.5/serializer_prefetch/base.py
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-20 17:10:20.837336 drf-serializer-prefetch-1.0.5/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      679 2023-06-20 17:10:19.000000 drf-serializer-prefetch-1.0.5/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-20 17:10:20.833336 drf-serializer-prefetch-1.0.5/tests/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-20 15:59:03.000000 drf-serializer-prefetch-1.0.5/tests/__init__.py
```

### Comparing `drf-serializer-prefetch-1.0.4/LICENSE` & `drf-serializer-prefetch-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-serializer-prefetch-1.0.4/PKG-INFO` & `drf-serializer-prefetch-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.4
+Version: 1.0.5
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -164,15 +164,15 @@
 
 ### Adding logic to the PrefetchingListSerializer
 
 If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
 
 ### Adding compatibility with django-zen-queries or other libraries
 
-The goal of this library is to make is easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer. For django-zen-queries, it looks something like this:
+The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
 
 ``` python
 from contextlib import nullcontext
 from django.conf import settings
 import serializer_prefetch
 from zen_queries import fetch, queries_disabled
```

### Comparing `drf-serializer-prefetch-1.0.4/README.md` & `drf-serializer-prefetch-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
 ### Adding logic to the PrefetchingListSerializer
 
 If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
 
 ### Adding compatibility with django-zen-queries or other libraries
 
-The goal of this library is to make is easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer. For django-zen-queries, it looks something like this:
+The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
 
 ``` python
 from contextlib import nullcontext
 from django.conf import settings
 import serializer_prefetch
 from zen_queries import fetch, queries_disabled
```

### Comparing `drf-serializer-prefetch-1.0.4/drf_serializer_prefetch.egg-info/PKG-INFO` & `drf-serializer-prefetch-1.0.5/drf_serializer_prefetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-serializer-prefetch
-Version: 1.0.4
+Version: 1.0.5
 Summary: An automatic prefetcher for django-rest-framework.
 Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
 Author: Maxime Toussaint
 Author-email: m.toussaint@mail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -164,15 +164,15 @@
 
 ### Adding logic to the PrefetchingListSerializer
 
 If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
 
 ### Adding compatibility with django-zen-queries or other libraries
 
-The goal of this library is to make is easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer. For django-zen-queries, it looks something like this:
+The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
 
 ``` python
 from contextlib import nullcontext
 from django.conf import settings
 import serializer_prefetch
 from zen_queries import fetch, queries_disabled
```

### Comparing `drf-serializer-prefetch-1.0.4/serializer_prefetch/base.py` & `drf-serializer-prefetch-1.0.5/serializer_prefetch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         if isinstance(instance, list):
             instance = List(instance)
 
         instance._braindate_prefetch_done = True
 
         self.call_other_prefetching_methods()
 
-        return self.call_to_representation(super().to_representation, instance)
+        return self.call_to_representation(instance)
 
 
 class Dict(dict):
     _braindate_prefetch_done = False
 
 
 class PrefetchingSerializerMixin(PrefetchingLogicMixin):
@@ -279,15 +279,15 @@
             if isinstance(instance, dict):
                 instance = Dict(instance)
             instance._braindate_prefetch_done = True
 
             self.call_other_prefetching_methods()
 
             if isinstance(instance, Model):
-                return self.call_to_representation(super().to_representation, instance)
+                return self.call_to_representation(instance)
 
         super().to_representation(instance)
 
     def __init__(self, instance=None, data=empty, **kwargs):
         self._auto_prefetch = kwargs.pop("auto_prefetch", True)
         super().__init__(instance, data, **kwargs)
```

### Comparing `drf-serializer-prefetch-1.0.4/setup.py` & `drf-serializer-prefetch-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 DESCRIPTION = "An automatic prefetcher for django-rest-framework."
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 setup(
     name="drf-serializer-prefetch",
     version=VERSION,
```

